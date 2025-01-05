<template>
    <div>
<br>
<h1>Registration Form</h1>
<div ref="infoShow" v-show="abc" id="display">..</div>
<hr>


<div>{{ fullname }}</div>
<div>{{ gender }}</div>
<div>{{ district }}</div>
<div>{{ language }}</div>
<div>{{ address }}</div>
    <div>
        <form @submit.prevent="FormSubmit" action="">
            name: <br> <input type="text" v-model="fullname" name="fullname"><br>
            Gender: <br>
            Male: <input type="radio" v-model="gender" name="gender" value="male">
            Female: <input type="radio" name="gender" value="female"><br>
            District <br>
            <select name="district" id="" v-model="district">
                <option disabled select>select one</option>
                <option>Dhaka</option>
                <option>Rangpur</option>
                <option>khulna</option>
                <option>sylhet</option>
            </select><br>
            Interest Language: <br>
            <input type="checkbox" name="PHP" v-model="language" value="PHP">PHP
            <input type="checkbox" name="JavaScript" v-model="language" value="JavaScript">JavaScript
            <input type="checkbox" name="vue" v-model="language" value="vue">vue
            <br>
            <textarea name="" id="" v-model="address">address</textarea><br>
            <input type="submit" name="submit" value="SUBMIT">
            

        </form>
    </div>
</div>
</template>

<script>
    export default {
        data() {
            return {
                fullname: '',
                gender: '',
                district: '',
                language:[],
                address: '',
                info: '',
                abc: false
            }
        },
        methods: {
            FormSubmit(){   
                this.info += "<br>Full Name : " + this.fullname;
                this.info += "<br> Gender : " + this.gender;
                this.info += "<br>District : " + this.district;
                this.info += "<br>Language : " + this.language;
                this.info += "<br>address : " + this.address;

                this.$refs.infoShow.innerHTML = this.info;

            }
        },
    }
</script>

<style scoped>

#display{
background-color: hotpink;
}
</style>

