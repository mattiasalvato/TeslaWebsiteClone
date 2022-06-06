<template>

  <header class="fixed w-[100%]"  id="index">
    <a href="index">
      <img  src="../assets/images/tesla_logo.svg" alt=""  class="absolute w-[10rem] p-6 
                                                                lg:w-[10rem] lg:ml-4 ">
    </a>

    <ul class=" text-gray-900 hidden sm:hidden lg:flex justify-center text-center  mt-5 font-semibold mr-10 md:gap-6 xl:gap-10">
      <li class="cursor-pointer hover:bg-gray-300 p-[7px] rounded-2xl"><a href="">Model S</a></li>
      <li class="cursor-pointer hover:bg-gray-300 p-[7px] rounded-2xl"><a href="">Model 3</a></li>
      <li class="cursor-pointer hover:bg-gray-300 p-[7px] rounded-2xl"><a href="">Model X</a></li>
      <li class="cursor-pointer hover:bg-gray-300 p-[7px] rounded-2xl"><a href="">Model Y</a></li>
      <li class="cursor-pointer hover:bg-gray-300 p-[7px] rounded-2xl"><a href="">Solar Roof</a></li>
      <li class="cursor-pointer hover:bg-gray-300 p-[7px] rounded-2xl"><a href="">Solar Panels</a></li>
    </ul>

    <div class="flex justify-end mr-2"> 
      <span class="bg-gray-500 rounded-lg p-2 w-[64px] h-[32px] mt-[17px] opacity-25 mr-5 sm:mr-5
                  lg:opacity-0 "> 
  
      </span>
      <h4 class="absolute mt-2 mr-3 font-semibold hidden cursor-pointer 
                  lg:mr-40 lg:-mt-[30px] lg:block">Account</h4>

      <h4 class="absolute mt-2 mr-3 font-semibold hidden cursor-pointer 
                  lg:mr-[100px] lg:-mt-[30px] lg:block">Shop</h4>

      <h4 class="absolute mt-5 mr-3 font-semibold mr-[32px] w-[40px] cursor-pointer 
                  lg:mr-10 lg:-mt-[30px]"  @click="displayMenu">Menu</h4>
    </div>
  </header>


  <div class="absolute top-0 right-0 w-[85%] max-w-[35rem] h-[100%] bg-white overflow-y-scroll
              xl:w-[320px]"  v-show="menuActive" id="cont">
      <div @click="displayMenu">
          <svg class="absolute w-3 mt-10 right-10 opacity-75" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"><!--! Font Awesome Pro 6.1.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M376.6 427.5c11.31 13.58 9.484 33.75-4.094 45.06c-5.984 4.984-13.25 7.422-20.47 7.422c-9.172 0-18.27-3.922-24.59-11.52L192 305.1l-135.4 162.5c-6.328 7.594-15.42 11.52-24.59 11.52c-7.219 0-14.48-2.438-20.47-7.422c-13.58-11.31-15.41-31.48-4.094-45.06l142.9-171.5L7.422 84.5C-3.891 70.92-2.063 50.75 11.52 39.44c13.56-11.34 33.73-9.516 45.06 4.094L192 206l135.4-162.5c11.3-13.58 31.48-15.42 45.06-4.094c13.58 11.31 15.41 31.48 4.094 45.06l-142.9 171.5L376.6 427.5z"/></svg>
      </div>
      <ul class="grid gap-y-2 mt-[90px] mr-[80px] ml-10 font-semibold text-gray-600 text-[15px] mb-80 capitalize">
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="#Model3">Model 3</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="#ModelS">Model S</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="#ModelX">Model X</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="#ModelY">Model Y</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="#SolarRoof">Solar Roof</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="#SolarPanel">Solar Panels</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Existing Inventory</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Used Inventory</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Trade-In</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Test Drive</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Insurance</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Cybertruck</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Roadster</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Semi</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Chargin</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Powerwall</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Commercial Energy</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Utilities</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Find Us</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Support</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Investor Relations</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Shop</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">Account</a></li>
        <li class="hover:bg-gray-100 p-[7px] rounded-2xl"><a href="">More</a></li>
      </ul>
    </div>


  <div id="container">

  
    <div id="section">
      <div id="content" class="text-center pt-[100px]">
        <h1 id="Model3" class="text-4xl font-semibold md:text-5xl">Model 3</h1>
        <h2 class="mt-[5px] capitalize">Order Online for <a href="" class="underline">Touchless Delivery</a></h2>

          <div class="mt-[300px] w-[100%] flex flex-wrap justify-center sm:grid grid-cols-2 md:grid grid-cols-2 md:mt-[400px]">
            <a href="" class="basis-[80%] bg-zinc-700 text-white  font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:ml-[150px] lg:ml-[250px] xl:ml-[300px] 2xl:ml-[500px] 2xl:w-[30%]">CUSTOM ORDER</a>
                              


            <a href="" class="basis-[80%] bg-gray-200 text-zinc-600 font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:mr-[150px] lg:mr-[250px] xl:mr-[300px] 2xl:mr-[500px] 2xl:w-[30%]">EXISTING INVENTORY</a>
          </div>
      </div>
    </div>

    <div id="section">
      <div id="content" class="text-center pt-[100px]">
        <h1 id="ModelY" class="text-4xl font-semibold md:text-5xl">Model Y</h1>
        <h2 class="mt-[5px] capitalize">Order Online for <a href="" class="underline">Touchless Delivery</a></h2>

          <div class="mt-[300px] w-[100%] flex flex-wrap justify-center md:grid grid-cols-2 md:mt-[400px]">
            <a href="" class="basis-[80%] bg-zinc-700 text-white  font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:ml-[150px] lg:ml-[250px] xl:ml-[300px] 2xl:ml-[500px] 2xl:w-[30%]">CUSTOM ORDER</a>
                              


            <a href="" class="basis-[80%] bg-gray-200 text-zinc-600 font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:mr-[150px] lg:mr-[250px] xl:mr-[300px] 2xl:mr-[500px] 2xl:w-[30%]">EXISTING INVENTORY</a>
          </div>
      </div>
    </div>

 
    <div id="section"> 
      <div id="content" class="text-center pt-[100px]">
        <h1 id="ModelS" class="text-4xl font-semibold md:text-5xl">Model S</h1>
        <h2 class="mt-[5px] capitalize">Order Online for <a href="" class="underline">Touchless Delivery</a></h2>

        <div class="mt-[300px] w-[100%] flex flex-wrap justify-center md:grid grid-cols-2 md:mt-[400px]">
            <a href="" class="basis-[80%] bg-zinc-700 text-white  font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:ml-[150px] lg:ml-[250px] xl:ml-[300px] 2xl:ml-[500px] 2xl:w-[30%]">CUSTOM ORDER</a>

            <a href="" class="basis-[80%] bg-gray-300 text-zinc-600 font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:mr-[150px] lg:mr-[250px] xl:mr-[300px] 2xl:mr-[500px] 2xl:w-[30%]">EXISTING INVENTORY</a>
          </div>
      </div>
    </div>

    <div id="section">
      <div id="content"  class="text-center pt-[100px]">
        <h1 id="ModelX" class="text-4xl font-semibold">Model X</h1>
        <h2 class="mt-[5px] capitalize">Order Online for <a href="" class="underline">Touchless Delivery</a></h2>

        <div class="mt-[300px] w-[100%] flex flex-wrap justify-center md:grid grid-cols-2 md:mt-[400px]">
            <a href="" class="basis-[80%] bg-zinc-700 text-white  font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:ml-[150px] lg:ml-[250px] xl:ml-[300px] 2xl:ml-[500px] 2xl:w-[30%]">CUSTOM ORDER</a>

            <a href="" class="basis-[80%] bg-gray-300 text-zinc-600 font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:mr-[150px] lg:mr-[250px] xl:mr-[300px] 2xl:mr-[500px] 2xl:w-[30%]">EXISTING INVENTORY</a>
          </div>
      </div>
    </div>
    

    <div id="section">
      <div id="content" class="text-center pt-[100px]">
        <h1 id="SolarPanel" class="text-4xl font-semibold">Solar Panel</h1>
        <h2 class="mt-[5px] capitalize">Lowest Cost Solar Panels in America</h2>

        <div class="mt-[300px] w-[100%] flex flex-wrap justify-center md:grid grid-cols-2 md:mt-[400px]">
            <a href="" class="basis-[80%] bg-zinc-700 text-white  font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:ml-[150px] lg:ml-[250px] xl:ml-[300px] 2xl:ml-[500px] 2xl:w-[30%]">ORDER NOW</a>

            <a href="" class="basis-[80%] bg-gray-300 text-zinc-600 font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:mr-[150px] lg:mr-[250px] xl:mr-[300px] 2xl:mr-[500px] 2xl:w-[30%]">LEARN MORE</a>
          </div>
      </div>
    </div>

    <div id="section">
      <div id="content" class="text-center pt-[100px]">
        <h1 id="SolarRoof" class="text-4xl font-semibold">Solar Roof</h1>
        <h2 class="mt-[5px] capitalize">Produce Clean Energy From Your Roof</h2>

        <div class="mt-[300px] w-[100%] flex flex-wrap justify-center md:grid grid-cols-2 md:mt-[400px]">
            <a href="" class="basis-[80%] bg-zinc-700 text-white  font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:ml-[150px] lg:ml-[250px] xl:ml-[300px] 2xl:ml-[500px] 2xl:w-[30%]">ORDER NOW</a>
            <a href="" class="basis-[80%] bg-gray-300 text-zinc-600 font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[50%] md:m-auto md:mr-[150px] lg:mr-[250px] xl:mr-[300px] 2xl:mr-[500px] 2xl:w-[30%]">LEARN MORE</a>
          </div>
      </div>
    </div>

    <div id="section">
      <div id="content"  class="text-center pt-[100px]">
        <h1 id="Accessories" class="text-4xl font-semibold">Accessories</h1>

        <div class="mt-[375px] w-[100%] text-center flex flex-wrap justify-center md:grid grid-cols-1 md:mt-[420px]">
            <a href="" class="basis-[80%] bg-zinc-900 text-white  font-semibold text-sm m-2 p-[10px] rounded-full
                              sm:mt-[50px] md:w-[30%] md:m-auto md:mr-[350px] lg:mr-[425px] xl:mr-[520px] xl:w-[20%] 2xl:mr-[600px] 2xl:w-[20%]">SHOP NOW</a>
          </div>
      </div>
    </div>

    

  </div>

  
  
</template>

<script>

export default {
  name: 'HomePage',
  data(){

    return{
       
       menuActive: false
    }
  },

  methods:{
    displayMenu(){

      this.menuActive = !this.menuActive
      
    
    }
  }
}
</script>

<style>
#container{
  width: 100%;
  height: 100vh;
  overflow: auto;
  scroll-snap-type: y mandatory;
}

#container #section{
  width: 100%;
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  scroll-snap-align: start ;
}

#container #section:nth-child(1){
  background-image: url(../assets/images/image1.avif);
  background-size: cover;
}

#container #section:nth-child(2){
  background-image: url(../assets/images/image2.avif);
  background-size: cover;
}

#container #section:nth-child(3){
  background-image: url(../assets/images/image3.avif);
  background-size: cover;
}

#container #section:nth-child(4){
  background-image: url(../assets/images/image4.avif);
  background-size: cover;
}

#container #section:nth-child(5){
  background-image: url(../assets/images/image5.avif);
  background-size: cover;
}

#container #section:nth-child(6){
  background-image: url(../assets/images/image6.avif);
  background-size: cover;
}

#container #section:nth-child(7){
  background-image: url(../assets/images/image7.avif);
  background-size: cover;
}

</style>
