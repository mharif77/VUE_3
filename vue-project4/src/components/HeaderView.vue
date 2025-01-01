<template>
     <div class="jumbotron text-center" style="margin-bottom:0">
  <h1>My First Bootstrap 4 Page</h1>
  <p>Resize this responsive page to see the effect!</p> 
</div>
<nav class="navbar navbar-expand-sm bg-dark navbar-dark">
  <Router-link class="navbar-brand" to="#">Navbar</Router-link>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#collapsibleNavbar">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="collapsibleNavbar">
    <ul class="navbar-nav">
      <li class="nav-item">
        <Router-link class="nav-link" to="/">Home</Router-link>
      </li>
      <li class="nav-item">
        <Router-link class="nav-link" to="/about">About</Router-link>
      </li>
      <li class="nav-item">
        <Router-link class="nav-link" to="/contact">Contact</Router-link>
      </li>   
       <li class="nav-item">
        <Router-link class="nav-link" to="/http">http</Router-link>
      </li> 

       <li class="nav-item">
        <Router-link class="nav-link" to="/json">Json</Router-link>
      </li>

      <li class="nav-item">
        <Router-link class="nav-link" to="/axios">Axios</Router-link>
      </li>
    </ul>
  </div>  
</nav>
</template>