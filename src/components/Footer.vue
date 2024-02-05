<template>
  <nav class="visible fixed bottom-0 z-10 flex h-12 w-full justify-between bg-white
   py-1.5 px-2 shadow-400 ltr:left-0 rtl:right-0 md:h-14 lg:hidden">
    <button class="flex h-full items-center justify-center p-2 focus:text-accent focus:outline-0"
            tabindex="0">
      <span class="sr-only">Burger Menu</span>
    <BackspaceIcon  class="w-5 h-5"/>
    </button>
    <button class="flex h-full items-center justify-center p-2 focus:text-accent focus:outline-0"
        tabindex="0">
      <span class="sr-only">Search</span>
    <MagnifyingGlassCircleIcon class="h-5 w-5"/>
    </button>
    <button class="flex h-full items-center justify-center p-2 focus:text-accent focus:outline-0"
     tabindex="0"><span class="sr-only">Home</span>
    <HomeIcon  class="w-5 h-5"/>
    </button>
    <button class="product-cart relative flex h-full items-center justify-center p-2 focus:text-accent
    focus:outline-0" tabindex="0"><span class="sr-only">Cart</span>
      <ShoppingCartIcon class="w-5 h-5" />
    </button>
    <button class="flex h-full items-center justify-center p-2 focus:text-accent focus:outline-0"
            tabindex="0">
      <span class="sr-only">User</span>
     <UserIcon  class="w-5 h-5"/>
    </button>
  </nav>
</template>

<script setup>
import {UserIcon,ShoppingCartIcon,HomeIcon,MagnifyingGlassCircleIcon,BackspaceIcon} from "@heroicons/vue/24/outline"

</script>

<style scoped>

</style>