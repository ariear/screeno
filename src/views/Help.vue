<template>
  <div class="container mx-auto pt-20 pb-10">
      <p class="font-monstand text-white text-center text-5xl font-bold">We help you grow</p>

      <div class="text-white flex lg:justify-center xl:justify-between items-center pt-28 lg:pb-28">
          <div class="w-[90vw] md:w-[441px] xl:mr-0 lg:mr-16 mx-auto lg:mx-0">
              <p class="font-monstand font-semibold text-4xl mb-6">Monetize your way</p>
              <p class="font-mules font-normal mb-5" v-text="helpdetail[0]"></p>
              <p class="font-monstand font-medium flex items-center">Get Started <span class="ml-3"><img src="/img/arrow-right-blue.png" alt=""></span></p>
          </div>
          <div class="relative lg:block hidden">
              <img src="/img/orang-main-terompet.png" data-aos="fade-left" data-aos-duration="1000" class="lg:w-[400px] xl:w-[555px]" alt="">
              <img src="/img/content-donate.png" data-aos="fade-right" data-aos-duration="500" class="lg:w-[200px] xl:w-[262px] absolute -top-10 -left-10" alt="">
          </div>
      </div>

      <div class="text-white flex lg:justify-center xl:justify-between items-center py-28">
          <div class="relative xl:mr-0 lg:mr-16 lg:block hidden">
              <img src="/img/bapack-bapack.png" data-aos="fade-right" data-aos-duration="1000" class="lg:w-[400px] xl:w-[555px]" alt="">
              <img src="/img/message-pop.png" data-aos="fade-left" data-aos-duration="400" class="absolute -top-6 -right-6" alt="">
          </div>
          <div class="w-[90vw] md:w-[441px] mx-auto lg:mx-0">
              <p class="font-monstand font-semibold text-4xl mb-6">Optimized for growth</p>
              <p class="font-mules font-normal mb-5" v-text="helpdetail[1]"></p>
              <p class="font-monstand font-medium flex items-center">Get Started <span class="ml-3"><img src="/img/arrow-right-blue.png" alt=""></span></p>
          </div>
      </div>
      
      <div class="font-monstand text-white text-center pt-10">
          <p class="font-bold text-4xl md:text-5xl mb-4 md:px-5 lg:px-0">Start your own business today</p>
          <p class="font-light mb-9">Start your own business today</p>
          <div>
              <button class="py-3 px-7 bg-white rounded-full text-black mr-8">Get Started</button>
              <button class="py-3 px-14 border border-white rounded-full">Login</button>
          </div>
      </div>

      <div class="mx-auto w-max relative pt-24 pb-16">
          <img src="/img/orang-masak-gedi.png" data-aos="fade-up" data-aos-duration="2000" class="w-[90vw] md:w-[600px] lg:w-[792px]" alt="">
          <img src="/img/orang-masak-cilik.png" data-aos="fade-up" data-aos-duration="2300" class="w-[100px] md:w-[200px] lg:w-[231px] absolute bottom-0 md:-left-10" alt="">
      </div>
  </div>
</template>

<script>
export default {
    setup(props) {
        const helpdetail = ['Set up subscriptions, rentals, or one-time buys for access to your VOD and live streams. Create exclusive experiences for your subscribers with coupons and promotions. One predictable fee, transparent pricing, and same-day setup.','The Screeno ecosystem is designed to help you generate profit. Set up complete sales and marketing funnels with ease using the Screeno built-in marketing tools and integrations. Generate leads and convert your audience into paying subscribers, at no extra cost.']

        return { helpdetail }
    }
}
</script>