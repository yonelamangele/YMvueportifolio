<template lang="">
    <div>
      <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <div class="container-fluid">
    <div class="logo">
      <img :src="logoUrl" alt="ym" class="logo"/>
    </div>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#"> Home </a>
         </li>
          <li class="nav-item">
            <a class="nav-link" href="#"> About </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"> Resume </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"> Projects </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"> Testimonials </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#"> Contacts </a>
          </li>
        
      </ul>
    </div>
  </div>
</nav>
    </div>
</template>
<script>
export default {
    data(){
      return{
        logoUrl: 'Yonela-removebg-preview.png'
      };
    },
};
</script>
<style>
    li {
        list-style-type: none;
    }

    .navbar-nav {
        display: flex;
        align-items: flex-end;
        justify-content: space-between
    }
</style>