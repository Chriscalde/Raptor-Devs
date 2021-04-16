<template>
  <div class="bg-gray-900 flex flex-wrap p-4 justify-between">
      <a href="" class="logo mr-auto"><img src="../assets/img/logo.png" alt="logo_img"></a>
      <button class="text-white cursor-pointer text-3xl border border-solid border-transparent rounded bg-transparent md:hidden" type="button" v-on:click="toggleNavbar()"><i class="bx bx-menu"></i></button>
      <div v-bind:class="{'hidden':!showMenu, 'flex':showMenu}" class="nav-menu md:flex justify-center items-center text-center">
          <ul>
              <li>
                  <a href="#hero" class="px-2 lg:px-5">Home</a>
              </li>
              <li>
                  <a href="#services" class="px-2 lg:px-5">Services</a>
              </li>
              <li>
                  <a href="#about-us" class="px-2 lg:px-5">About Us</a>
              </li>
              <li>
                  <a href="#contact" class="px-2 lg:px-5">Contact</a>
              </li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    data(){
        return  {
            showMenu: false
        }
    },
    methods: {
        toggleNavbar: function(){
            this.showMenu = !this.showMenu;
        }
    }
}
</script>

<style scoped>
.logo img{
    max-width: 200px;
}
.nav-menu{
    list-style: none;
}
.nav-menu li{
    color: #f0eeee;
    list-style: none;
    display: inline-block;
}
.nav-menu a{
    font-family: 'Roboto', sans-serif;
    font-size: 18px;
    @apply font-bold;
}
.nav-menu a:hover, .nav-menu li:hover{
    color: #EB6E15;
    transform: scale(1.15)
}

</style>