<template>

<div class="px-4 xl:px-0">
<div class="w-full pt-4 pb-20 lg:py-6">
<div class="grid grid-cols-[repeat(auto-fill,minmax(250px,1fr))] gap-3">
 <article class="h-full transform overflow-hidden rounded border border-border-200 bg-white shadow-sm transition-all
 duration-200 hover:-translate-y-0.5 hover:shadow"
          v-for="product in products" :key="product">
                                <div
                                    class="relative flex h-48 w-auto cursor-pointer items-center justify-center sm:h-64">
                                    <span class="sr-only">Product Image</span><img alt="Razero Wolverine" class="object-contain object-cover"
                                        :src="product.image"
                                        style="position: absolute; height: 100%; width: 100%; inset: 0px; color: transparent;">
        
                                </div>
                                <header class="p-3 md:p-6">
                                    <div class="mb-2 flex items-center"><span
                                            class="text-sm font-semibold text-heading md:text-base">${{product.price}}</span><del
                                            class="text-xs text-muted ltr:ml-2 rtl:mr-2 md:text-sm">${{product.pre_price}}</del></div>
                                    <h3 class="mb-4 cursor-pointer truncate text-xs text-body md:text-sm">{{product.title}}</h3>
                                    <div><button
                                            class="group flex h-7 w-full items-center justify-between rounded bg-gray-100 
                                            text-xs text-body-dark transition-colors hover:border-accent hover:bg-emerald-600 hover:text-light 
                                            focus:border-accent focus:bg-emerald-600 focus:text-light focus:outline-0 md:h-9 md:text-sm"><span
                                                class="flex-1">Add</span>
                                                <span class="grid h-7 w-7 place-items-center bg-gray-200 transition-colors
                                                duration-200 group-hover:bg-emerald-600 group-focus:bg-emerald-600
                                                ltr:rounded-tr ltr:rounded-br rtl:rounded-tl rtl:rounded-bl md:h-9 md:w-9">
                                                <PlusIcon class="h-4 w-4 stroke-2"/>
                                                </span>
                                                </button>
                                                </div>
                                </header>
                            </article>
</div>
</div>
</div>

</template>


<script setup>
import {ref} from 'vue'
import {
  PlusIcon
} from '@heroicons/vue/24/outline';

import data from "../data/price.json"

const products = ref(data);
</script>