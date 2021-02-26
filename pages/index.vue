<template>
  <div class="mx-0 bg-gray-900">
    <Header/>
    <div class="h-screen">
      <section id="hero">
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
      <section id="services" class="max-h-full">
        <div class="grid lg:grid-cols-3 gap-8 p-10">
          <div class="text-center flex flex-col justify-center mx-auto">
            <img src="../assets/img/orange_bg.png" alt="" class="rounded-full mx-auto">
            <h1>Header 1</h1>
            <p>Text 1</p>
          </div>
          <div class="text-center flex flex-col justify-center mx-auto">
            <img src="../assets/img/orange_bg.png" alt="" class="rounded-full mx-auto">
            <h1>Header 2</h1>
            <p>Text 2</p>
          </div>
          <div class="text-center flex flex-col justify-center mx-auto">
            <img src="../assets/img/orange_bg.png" alt="" class="rounded-full mx-auto">
            <h1>Header 3</h1>
            <p>Text 3</p>
          </div>
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
#services i {
  color: #EB6E15;
}
#services img{
  width: 70px;
  height: 70px;
  border-color: #ffffff00;
  border-width: 3px;
  
}
#services img:hover {
  border-color: #e9772692;
  
}
</style>
