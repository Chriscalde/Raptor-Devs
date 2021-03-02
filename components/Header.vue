<template>
  <div class="bg-gray-900 flex p-4 justify-between">
      <a href="" class="logo mr-auto"><img src="../assets/img/logo.png" alt=""></a>
      <nav class="nav-menu justify-center items-center text-center">
          <ul>
              <li>
                  <a href="" class="px-5">Home</a>
              </li>
              <li>
                  <a href="" class="px-5">Services</a>
              </li>
              <li>
                  <a href="" class="px-5">About Us</a>
              </li>
              <li>
                  <a href="" class="px-5 orange_app">Contact</a>
              </li>
          </ul>
      </nav>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.logo img{
    max-width: 200px;
}
.nav-menu{
    display: flex;
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
.nav-menu a:hover{
    color: #EB6E15
}

</style>