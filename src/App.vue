<template>
  <!-- <nav>
    <router-link to="/"> Home </router-link> |
    <router-link to="/about"> About </router-link> |
    <router-link to="/resume"> Resume </router-link> |
    <router-link to="/projects"> Projects </router-link> |
    <router-link to="/testimonials"> Testimonials </router-link> |
    <router-link to="/contacts"> Contacts </router-link>
  </nav> -->
  
  <div class="stuff" style="height: 100vh">
    <Navbar-comp/>

    <div class="middle">
      <div class="pic">
        <img src="https://yonelamangele.github.io/Images/20240422_122539.jpg" alt="" class="photo">
      </div>
  
      <div class="par">
        <h4> Hello There. </h4>  
        <h1> <i> I am YONELA MANGELE. </i> </h1> 
        <h4> An aspiring web developer. </h4>
      </div>
    </div>

  </div>
  
  <router-view/>

</template>

<script>
import NavbarComp from './components/NavbarComp.vue';
export default {
        components:{
              NavbarComp
        }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}


.stuff {
  background: linear-gradient(#252533, #27263C, #2D2C66, #302E78, #2F2D73, #4542DD, #302E78, #302E78);
}
/* .middle{
  position: relative;
  animation-delay: 0s;
  animation-duration: 4s;
  animation-name: middle;
  animation-fill-mode: backwards;
}
@keyframes middle {
  from{left:0px;}
  to{left:100px;}
} */

@keyframes slide-in-left {
  from {
    transform: translateX(-300px);
  }
  to {
    transform: translateX(0);
  }
}

.pic {
  animation-name: slide-in-left;
  animation-duration: 6s;
}
/* animation: slide-in-left 1.5s forwards;
animation: slide-in-right 1s forwards; */
@keyframes slide-in-right {
  from {
    transform: translateX(300px);
  }
  100% {
    transform: translateX(0);
  }
}

.par {
  animation-name: slide-in-right;
  animation-duration: 6s;
}

.nav-link {
  color: white;
}


.pic {
  height: 400px;
  width: 300px
}
.photo {
  height: 400px;
  width: 300px;
  border-radius: 10px;
  
}

.par {
  height: 328px;
  color: white;
  margin-top: 70px;
}

.middle {
    margin: 15ch;
    height: 300px;
    display: flex;
    justify-content: space-evenly;
}

</style>

<!-- github link - https://github.com/yonelamangele -->

<!-- linkedin link - https://www.linkedin.com/in/yonela-mangele-125044316/ -->