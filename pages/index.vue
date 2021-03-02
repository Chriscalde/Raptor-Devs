<template>
  <div class="">
    <Header/>
    <div class="" id="content">
      <section id="hero" class="bg-gray-900">
        <div class="grid lg:grid-cols-2 gap-8 p-10">
            <div class="left-hero justify-center items-center text-center mx-auto">
              <h1 class="text-6xl text-white font-bold">Need a website?</h1>
              <h1 class="text-6xl text-white font-extrabold">We got you</h1>
            </div>
            <div class="right-hero">
              <img src="../assets/img/mb.png" alt="" rel='preload'>
            </div>
        </div>
      </section>
      <section id="services">
        <div class="text-center">
          <h2 id="services-title" class="text-4xl font-bold">Services</h2>
        </div>
        <p id="services-subtitle" class="text-center text-2xl">Check out the <span class="font-bold">services</span> we offer</p>
        <div class="grid lg:grid-cols-3 gap-8 p-10">
          <div class="text-center flex flex-col justify-center mx-auto">
            <img src="../assets/icons/img_web.png" alt="" class="rounded-full mx-auto object-cover">
            <h1 class="text-2xl font-bold">Websites</h1>
            <p>Text 1</p>
          </div>
          <div class="text-center flex flex-col justify-center mx-auto">
            <img src="../assets/icons/img_mobile.png" alt="" class="rounded-full mx-auto object-cover">
            <h1 class="text-2xl font-bold">Mobile Applications</h1>
            <p>Text 2</p>
          </div>
          <div class="text-center flex flex-col justify-center mx-auto">
            <img src="../assets/icons/img_tech.png" alt="" class="rounded-full mx-auto object-cover">
            <h1 class="text-2xl font-bold">Tech Support</h1>
            <p>Text 3</p>
          </div>
        </div>
      </section>
      <section id="about-us" class="rounded-xl bg-gray-900 m-6">
        <div class=" m-6 text-center">
          <h2 class="text-4xl font-bold text-white">About Us</h2>
        </div>
      </section>
      <section id="contact">
        <div class="text-center">
          <h2 class="text-4xl font-bold">Contact</h2>
        </div>
      </section>
    </div>
    <Footer/>
  </div>
</template>

<script>
export default {}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital@1&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
*{
  box-sizing: border-box
}
#content{
  background: #ECE9E6;  /*fallback for old browsers*/
  background: -webkit-linear-gradient(to right, #FFFFFF, #ECE9E6); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(to right, #FFFFFF, #ECE9E6); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}
@keyframes fadeInLeft {
   from {
      opacity: 0;
      transform: translateX(-20px);
   }
   to {
      opacity: 1;
      transform: translateX(0);
   }
}
@keyframes fadeInDown {
  from{
    opacity: 0;
    transform: translateY(-20px);
  }
  to{
    opacity: 1;
    transform: translateY(0);
  }
}   
#hero {
  /* background: #ECE9E6;  fallback for old browsers */
  /* background: -webkit-linear-gradient(to right, #FFFFFF, #ECE9E6);  Chrome 10-25, Safari 5.1-6 */
  /* background: linear-gradient(to right, #FFFFFF, #ECE9E6); W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}
#hero h1{
  font-family: 'Poppins', sans-serif;
  animation-duration: 2s;
  animation-name: fadeInLeft;
}
#hero img{
  /* animation-name: fadeInDown; */
  /* animation-duration: 2s; */
}
.right-hero{
  background: url('../assets/img/mb.png');
  background-size:cover;
}

#services{
  background: #ECE9E6;  /*fallback for old browsers*/
  background: -webkit-linear-gradient(to right, #FFFFFF, #ECE9E6); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(to right, #FFFFFF, #ECE9E6); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}
#services-subtitle span{
  color:#EB6E15
}
#services i {
  color: #EB6E15;
}

#services img{
  width: 150px;
  height: 150px;
  border-color: #ffffff00;
  border-width: 8px;
  
}
#services img:hover {
  border-color: #e9772692;
  
}
</style>
