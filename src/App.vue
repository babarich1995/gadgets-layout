<template>
<div class="flex min-h-screen flex-col bg-gray-100 transition-colors duration-150">
         <HeaderComponent />
        <div class="min-h-screen">
          <div class="flex flex-1 bg-gray-100">
            <Sidebar/>
            <main class="block w-full xl:overflow-hidden ltr:xl:pl-0 ltr:xl:pr-5 rtl:xl:pr-0 rtl:xl:pl-5 lg:pt-20 xl:mt-8 2xl:mt-6">
              <Banner/>
              <Main />
              <PriceCard/>
            </main>
          </div>

        </div>


        </div>





</template>
<script setup>
import HeaderComponent from './components/HeaderComponent.vue'
import Sidebar from './components/Sidebar.vue'
import Main from './components/Main.vue'
import Banner from './components/Banner.vue'
import PriceCard from './components/PriceCard.vue'


</script>
<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
    