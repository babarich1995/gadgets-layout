<template>

  <div class="sticky z-20 flex h-14 items-center justify-between border-t border-b border-border-200 bg-white py-3 px-5 md:h-16 lg:px-6
  xl:hidden top-[58px] lg:top-[84px]">
    <button class="flex h-8 items-center rounded border border-border-200 bg-gray-100 bg-opacity-90 py-1 px-3 text-sm font-semibold
    text-heading transition-colors duration-200 hover:border-accent-hover hover:bg-accent hover:text-light focus:border-accent-hover
    focus:bg-accent focus:text-light focus:outline-0 md:h-10 md:py-1.5 md:px-4 md:text-base">
     <AdjustmentsHorizontalIcon class="h-5 w-5"/> Filter</button>
    <div class="relative inline-block ltr:text-left rtl:text-right">

      <Menu as="div" class="relative inline-block text-left">
        <div>
          <MenuButton
              class="flex h-8 items-center rounded border border-border-200 bg-gray-100 bg-opacity-90 py-1 px-3 text-sm font-semibold
    text-heading transition-colors duration-200 hover:border-accent-hover hover:bg-accent hover:text-light focus:border-accent-hover
    focus:bg-accent focus:text-light focus:outline-0 md:h-10 md:py-1.5 md:px-4 md:text-base"
          >
             <span class="flex h-5 w-5 items-center justify-center ltr:mr-2 rtl:ml-2">
     <WrenchScrewdriverIcon />
      </span>
            <span class="whitespace-nowrap">Gadget</span>
            <ChevronDownIcon
                class="-mr-1 ml-2 h-5 w-5 text-violet-200 hover:text-violet-100"
                aria-hidden="true"
            />
          </MenuButton>
        </div>

        <transition
            enter-active-class="transition duration-100 ease-out"
            enter-from-class="transform scale-95 opacity-0"
            enter-to-class="transform scale-100 opacity-100"
            leave-active-class="transition duration-75 ease-in"
            leave-from-class="transform scale-100 opacity-100"
            leave-to-class="transform scale-95 opacity-0"
        >
          <MenuItems
              class="absolute right-0 mt-2 w-56 origin-top-right divide-y divide-gray-100 rounded-md bg-white shadow-lg ring-1 ring-black/5 focus:outline-none"
          >
            <div class="px-1 py-1">
              <MenuItem v-slot="{ active }">
                <button
                    :class="[
                  active ? 'bg-violet-500 text-white' : 'text-gray-900',
                  'group flex w-full items-center rounded-md px-2 py-2 text-sm',
                ]"
                >

                  Grocery
                </button>
              </MenuItem>
              <MenuItem v-slot="{ active }">
                <button
                    :class="[
                  active ? 'bg-violet-500 text-white' : 'text-gray-900',
                  'group flex w-full items-center rounded-md px-2 py-2 text-sm',
                ]"
                >
                  Make up
                </button>
              </MenuItem>
            </div>
            <div class="px-1 py-1">
              <MenuItem v-slot="{ active }">
                <button
                    :class="[
                  active ? 'bg-violet-500 text-white' : 'text-gray-900',
                  'group flex w-full items-center rounded-md px-2 py-2 text-sm',
                ]"
                >

                  Bakery
                </button>
              </MenuItem>
              <MenuItem v-slot="{ active }">
                <button
                    :class="[
                  active ? 'bg-violet-500 text-white' : 'text-gray-900',
                  'group flex w-full items-center rounded-md px-2 py-2 text-sm',
                ]"
                >

                  Medicine
                </button>
              </MenuItem>
            </div>

            <div class="px-1 py-1">
              <MenuItem v-slot="{ active }">
                <button
                    :class="[
                  active ? 'bg-violet-500 text-white' : 'text-gray-900',
                  'group flex w-full items-center rounded-md px-2 py-2 text-sm',
                ]"
                >

                  Clothes & Shoes
                </button>
              </MenuItem>
            </div>
          </MenuItems>
        </transition>
      </Menu>

    </div>
  </div>

</template>


<script setup>
import { Menu, MenuButton, MenuItems, MenuItem } from '@headlessui/vue'
import {WrenchScrewdriverIcon, AdjustmentsHorizontalIcon,ChevronDownIcon} from '@heroicons/vue/24/outline'
</script>