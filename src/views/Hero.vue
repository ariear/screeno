<template>
<div class="container mx-auto">
  <div class="flex lg:justify-center xl:justify-between items-center pt-24 pb-16 md:pb-48">
      <div class="text-white w-[90vw] lg:w-[400px] xl:w-[470px] xl:mr-0 lg:mr-16 md:mx-auto lg:mx-0 lg:text-left md:text-center ml-5">
          <p class="font-monstand font-semibold text-5xl mb-5">Reach More People in real time</p>
          <p class="font-mules font-light mb-10">The Screeno ecosystem is designed to help you generate profit. Set up complete sales and marketing funnels with ease using the Screeno</p>
          <div class="font-mules">
              <button class="bg-[#006AFF] rounded-full py-3 px-7 font-light mr-8 md:mt-0 mt-4">Start Free Trail</button>
              <button class="border border-white rounded-full py-3 px-16 md:mt-0 mt-4">Login</button>
          </div>
      </div>
      <div class="lg:block hidden">
          <div class="relative">
              <img src="/img/wedok-gedi.png" data-aos="fade-left" data-aos-duration="1000" class="lg:w-[400px] xl:w-[593px]" alt="">
              <img src="/img/wedok.png" data-aos="fade-right" data-aos-delay="200" class="lg:w-[100px] xl:w-[161px] absolute -left-8 -bottom-8" alt="">
          </div>
      </div>
  </div>

  <div class="flex items-center justify-evenly pb-10 lg:pb-20 flex-wrap">
      <img v-for="(gambar, index) in platform" :key="index" :src="gambar.img" class="mx-3 lg:mx-0 mt-5 lg:mt-0" alt="" data-aos="fade-up" data-aos-anchor-placement="top-bottom" :data-aos-delay="index * 150">
  </div>
</div>
</template>

<script>
export default {
    setup(props) {
        const platform = [
            {
                img: '/img/aplle-tv.png'
            },
            {
                img: '/img/android-tv.png'
            },
            {
                img: '/img/apple-watch.png'
            },
            {
                img: '/img/iphone.png'
            },
            {
                img: '/img/android.png'
            }
        ]

        return { platform }
    }
}
</script>