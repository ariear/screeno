<template>
  <nav class="text-white flex justify-between items-center py-9 px-6 lg:px-10 xl:px-24 font-mules bg-[#141516]">
      <div class="flex items-center">
      <img src="/img/screeno.png" class="w-[120px] mr-20" alt="">
      <ul class="lg:flex hidden items-center font-light">
          <li>Exemplet</li>
          <li class="lg:mx-10 xl:mx-24">Pricing</li>
          <li>About</li>
      </ul>
      </div>
      <div class="hidden md:block">
          <button class="font-normal py-3 mr-14">Login</button>
          <button class="font-normal bg-[#006AFF] rounded-full py-3 px-7">Start Free Trail</button>
      </div>
      <div class="block md:hidden">
          <img src="/img/white-menu.png" class="w-[35px]" @click="menu = !menu" alt="">
      </div>
  </nav>
  <div class="list-none absolute bg-white w-full left-0 font-monstand font-medium pl-5 block md:hidden overflow-hidden transition-all" :class="menu ? 'h-[200px] py-4 ' : 'h-0' ">
      <li>Exemplet</li>
      <li class="my-3">Pricing</li>
      <li>About</li>
      <li class="mt-4">
        <button class="font-normal py-3 border px-5 rounded-full mr-4">Login</button>
        <button class="font-normal bg-[#006AFF] rounded-full py-3 px-7 text-white">Start Free Trail</button>
      </li>
  </div>
</template>

<script>
import { ref } from '@vue/reactivity'
export default {
    setup() {
        const menu = ref(false)

        return { menu }
    }
}
</script>