<template>
  <div class="">
    <Header class="fixed top-0 w-full"></Header>
    <div class="" id="content">
      <section id="hero" class="bg-gray-900 mt-32">
        <div class="grid lg:grid-cols-2 gap-8 p-10 shadow-2xl">
            <div class="left-hero justify-center items-center text-center mx-auto">
              <h1 class="text-6xl text-white font-bold">Need a website?</h1>
              <h1 class="text-6xl text-white font-extrabold">We got you</h1>
            </div>
            <div class="right-hero">
              <img src="../assets/img/mb.png" alt="macbook_img" rel='preload'>
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
            <img src="../assets/icons/img_web.png" alt="website_img" class="rounded-full mx-auto object-cover">
            <h1 class="text-2xl font-bold">Websites</h1>
            <p>Custom user-friendly websites for your business.</p>
          </div>
          <div class="text-center flex flex-col justify-center mx-auto">
            <img src="../assets/icons/img_mobile.png" alt="mobile_img" class="rounded-full mx-auto object-cover">
            <h1 class="text-2xl font-bold">Mobile Applications</h1>
            <p>We can build the app you need.</p>
          </div>
          <div class="text-center flex flex-col justify-center mx-auto">
            <img src="../assets/icons/img_tech.png" alt="tech_img" class="rounded-full mx-auto object-cover">
            <h1 class="text-2xl font-bold">Tech Support</h1>
            <p>Technical support and software installation.</p>
          </div>
        </div>
      </section>
      <section id="about-us" class="rounded-xl bg-gray-900 m-6">
        <div class=" m-6 text-center">
          <h2 class="text-4xl font-bold text-white">About Us</h2>
          <div class="grid lg:grid-cols-2 gap-8 p-10">
            <div id="about-content" class="flex flex-col">
              <h2 class="text-2xl text-white mb-5">We are a web development company. Providing our clients with the best technological solutions.</h2>
              <a class="text-2xl text-white align-middle my-2"><i class="text-4xl bx bx-pencil align-middle mr-4"></i>Custom Made</a>
              <a class="text-2xl text-white align-middle my-2"><i class="text-4xl bx bx-user-check align-middle mr-4"></i>User Friendly</a>
              <a class="text-2xl text-white align-middle my-2"><i class="text-4xl bx bx-trending-up align-middle mr-4"></i>Marketing Solutions</a>
            </div>
            <div class="justify-center items-center mx-auto">
              <img src="../assets/img/iphone_mockup.png" alt="app_img" class="object-contain">
            </div>
          </div>
        </div>
      </section>
      <section id="contact">
        <div class="text-center">
          <h2 class="text-4xl font-bold">Contact</h2>
        </div>
        <div class="grid lg:grid-cols-2 gap-12 p-10">
          <div id="contact-mail" class="shadow-xl rounded-2xl flex flex-col justify-center items-center my-2 lg:my-5 lg:mx-auto lg:px-24 py-5 bg-white">
            <i class="bx bx-mail-send text-4xl"></i>
            <h3 class="text-2xl font-bold text-gray-500">Email</h3>
            <a href="mailto:contact@raptordevs.com">contact@raptordevs.com</a>
          </div>
          <div id="contact-phone" class="shadow-xl rounded-2xl flex flex-col justify-center items-center my-2 lg:my-5 lg:mx-auto lg:px-24 py-5 bg-white">
            <i class="bx bx-phone-call text-4xl"></i>
            <h3 class="text-2xl font-bold text-gray-500">Call Us</h3>
            <a href="tel:+13852349700">+1 (385) 234 97 00</a>
          </div>
        </div>
        <div class="bg-white shadow-2xl rounded-2xl m-12 p-8">
          <form @submit.prevent="sendMail">
            <label class="block">
              <span>Full name</span>
              <input v-model="name" name="name" type="text" class="mt-1 py-2 w-full bg-gray-200 rounded-md">
            </label>
            <label class="block">
              <span>Phone</span>
              <input v-model="phone" name="phone" type="text" class="mt-1 py-2 w-full bg-gray-200 rounded-md">
            </label>
            <label class="block">
              <span>Email</span>
              <input v-model="mail" name="mail" type="mail" class="mt-1 py-2 w-full bg-gray-200 rounded-md">
            </label>
            <label class="block">
              <span>What are you interested in?</span>
              <select v-model="type" name="type" class="mt-1 w-full bg-gray-200 rounded-md">
                <option>Website</option>
                <option>Application</option>
                <option>Web Design</option>
                <option>Tech Support</option>
                <option>Online Marketing</option>
              </select>
            </label>
            <label class="block">
              <span>Details</span>
              <textarea v-model="description" name="description" class="bg-gray-200 w-full rounded" rows="3"></textarea>
            </label>
            <input id="btnSend" type="submit" value="Send" class="mt-3 px-5 py-2 rounded-md text-2xl text-white">
          </form>
        </div>
      </section>
      <section id="footer-top">
        <div class="grid lg:grid-cols-2 gap-8 p-8">
          <div id="contact-top-left">
            <h3 class="text-4xl font-bold">Raptor <span>Devs</span></h3>
            <p>Riverton, Utah</p>
            <p>84065</p>
            <a href="tel:+13852349700">+1 (385) 234 97 00</a>
          </div>
          <div id="contact-top-right" class="flex flex-col justify-end  items-start">
            <h2 class="text-2xl font-bold">Check our social media</h2>
            <a class="text-xl"><i class="bx bxl-twitter mr-4"></i>Twitter</a>
            <a href="https://www.facebook.com/Raptordevs" target="_blank" class="text-xl" ><i class="bx bxl-facebook mr-4"></i>Facebook</a>
            <a href="https://www.instagram.com/raptordevs/" target="_blank" class="text-xl"><i class="bx bxl-instagram mr-4"></i>Instagram</a>
          </div>
        </div>
      </section>
    </div>
    <Footer/>
  </div>
</template>

<script>
import emailjs from 'emailjs-com'
export default {
  data(){
    return{
      name:'',
      mail: '',
      phone: '',
      type: '',
      description:''
    }
  },
  methods:{
    sendMail(e){
      try{
        emailjs.sendForm('service_oog6qul','template_riwb6hm',e.target,'user_yf8l6RazsRR1DqwdKclmB',{
          name: this.name,
          mail: this.mail,
          phone: this.phone,
          type: this.type,
          description: this.description
        })
      }catch(error){
        console.log(error)
      }
    }
  }
}
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
  background: -webkit-linear-gradient(to right, #FFFFFF, #D3d3d3); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(to right, #FFFFFF, #d3d3d3); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
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
  background: -webkit-linear-gradient(to right, #FFFFFF, #D3D3D3); /* Chrome 10-25, Safari 5.1-6 */
  background: linear-gradient(to right, #FFFFFF, #D3D3D3); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
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
#about-us img{
  width: 300px;
}
#about-content a:hover {
  transform: scale(1.15);
  cursor: default;
}
#contact-mail i{
  border-radius: 50%;
  padding: 8px;
  color: #EB6E15;
  border:2px solid #EB6E15;
}
#contact-phone i{
  border-radius: 50%;
  padding: 8px;
  color: #EB6E15;
  border:2px solid #EB6E15;
}
#btnSend {
  background-color: #EB6E15;
  border: 2px solid #ffffff;
}
#btnSend:hover{
  background-color: #9b4a10;
}
#contact-top-left h3{
  font-family: 'Roboto', sans-serif;
}
#contact-top-left span{
  font-family: 'Roboto', sans-serif;
  color: #EB6E15;
}
</style>
