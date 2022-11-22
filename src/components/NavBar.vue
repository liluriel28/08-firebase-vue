<template>
    <div>
        <nav>
    <div class="nav-wrapper green darken-4">
      <router-link to="/" class="brand-logo">Proyectos</router-link>
      
      <a href="#" data-target="mobile-demo" class="sidenav-trigger"><i class="material-icons">menu</i></a>
      <ul class="right hide-on-med-and-down">
        <li><router-link to="/home">Home</router-link></li>
        <li><router-link to="/about">About</router-link></li>
        <li><router-link to="/proyectos" class="waves-effect waves-light btn indigo">Proyectos</router-link></li>
      </ul>
    </div>
  </nav>

  <ul class="sidenav" id="mobile-demo">
    <li><router-link to="/home">Home</router-link></li>
    <li><router-link to="/about">About</router-link></li>
    <li><router-link to="/proyectos" >Proyectos</router-link></li>
 
     </ul>
    </div>

</template>
<script>
export default{
    mounted(){
        M.AutoInit();
    },
};
    
</script>