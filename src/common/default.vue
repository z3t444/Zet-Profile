<script setup>
  import Hero from "../content/Hero.vue"
  import Card from "../content/card.vue"
  import "../assets/css/default.css"
  import CardGrid from "../content/gridCard.vue"
  import Services from "../content/services.vue"
  import CardContent from "../content/cardContent.vue"
  import Contact from "../content/contact.vue"
  import Footer from "../content/footer.vue"
  // //css import file
  import "../assets/css/responsive.css"
</script>
<template>
  <div class="background-svg mx-auto rounded-3xl shadow-xl">
    <div class="Poppins p-10">
      <nav class="py-4 text-gray-900">
        <div class="mx-auto">
          <div class="flex justify-around justify-navbar items-center">
            <div class="flex items-center">
              <router-link to="/" class="text-2xl uppercase font-bold">Zeeta</router-link>
            </div>
            <div class="hidden md:flex text-sm font-semibold space-x-6">
              <a class="hover:scale-95 duration-100" href="#">Home</a>
              <a class="hover:scale-95 duration-100" href="#about">About</a>
              <a class="hover:scale-95 duration-100" href="#">Services</a>
              <a class="hover:scale-95 duration-100" href="#contact">Contact</a>
            </div>
            <div class="md:hidden">
              <button @click="isOpen = !isOpen" class="block focus:outline-none">
                <svg class="h-6 w-6 fill-current" :class="{ hidden: isOpen, block: !isOpen }" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M3 5a1 1 0 0 1 1-1h12a1 1 0 1 1 0 2H4a1 1 0 0 1-1-1zm16 4a1 1 0 1 1 0 2H4a1 1 0 0 1 0-2h15a1 1 0 0 1 0 2h-.01A1.999 1.999 0 0 1 20 11V9a1 1 0 0 1-1-1zM4 16a1 1 0 1 1 0-2h12a1 1 0 1 1 0 2H4z" />
                </svg>
                <svg class="h-6 w-6 fill-current" :class="{ hidden: !isOpen, block: isOpen }" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M13.293 6.293a1 1 0 0 1 1.414 1.414L11.414 11l3.293 3.293a1 1 0 1 1-1.414 1.414L10 12.414l-3.293 3.293a1 1 0 1 1-1.414-1.414L8.586 11 5.293 7.707a1 1 0 0 1 1.414-1.414L10 9.586l3.293-3.293z" />
                </svg>
              </button>
            </div>
          </div>
        </div>
        <div class="md:hidden mt-2" :class="{ block: isOpen, hidden: !isOpen }">
          <div class="px-2 pt-2 pb-4 flex flex-col font-medium text-sm">
            <a class="hover:scale-95 duration-100" href="#">Home</a>
            <a class="hover:scale-95 duration-100 mt-3" href="#about">About</a>
            <a class="hover:scale-95 duration-100 mt-3" href="#">Services</a>
            <a class="hover:scale-95 duration-100 mt-3" href="#contact">Contact</a>
          </div>
        </div>
      </nav>
      <section class="ClassName Hero-section mt-10">
        <div class="ClassName">
          <Hero></Hero>
        </div>
      </section>
      <section id="about" class="ClassName Card-section">
        <div class="ClassName">
          <Card></Card>
        </div>
      </section>
      <section class="ClassName mt-60">
        <div class="ClassName">
          <CardGrid></CardGrid>
        </div>
      </section>
      <section id="services">
        <div class="ClassName">
          <Services></Services>
        </div>
      </section>
      <section class="card-content mt-60">
        <div class="ClassName">
          <CardContent></CardContent>
        </div>
      </section>
      <section class="ClassName mt-40">
        <div class="ClassName">
          <Contact> </Contact>
        </div>
      </section>
      <section class="ClassName mt-40">
        <div class="ClassName">
          <Footer></Footer>
        </div>
      </section>
    </div>
  </div>
</template>


<script>
  export default {
    data() {
      return {
        isOpen: false,
      }
    },
  }
</script>
