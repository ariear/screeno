<template>
  <div class="text-center font-monstand pt-32">
      <p class="font-semibold text-5xl mb-4" data-aos="fade-up" data-aos-duration="900">All-in-one platform</p>
      <p class="font-normal mb-8 w-[80vw] md:w-[457px] mx-auto" data-aos="fade-up" data-aos-duration="1200">You take care of the video quality and we take care of everything else</p>
      <div>
          <button class="bg-[#006AFF] rounded-full py-3 px-7 text-white font-normal mr-8">Start Free Trail</button>
          <button class="border border-black rounded-full py-3 px-16 font-normal md:mt-0 mt-3">Login</button>
      </div>
  </div>
  <div class="container mt-28 pb-24 mx-auto md:grid-cols-2 grid lg:grid-cols-3 justify-items-center gap-y-16">
      <div v-for="(featue, index) in features" :key="index" class="w-[228px]" data-aos="fade-up" data-aos-anchor-placement="top-bottom" :data-aos-delay="index * 100">
      <div class="flex items-center mb-2">
          <img :src="featue.icon" alt="">
          <p v-text="featue.title" class="font-monstand font-semibold text-lg ml-3"></p>
      </div>
      <p class="font-mules font-normal" v-text="featue.detail"></p>
      </div>
  </div>
</template>

<script>
export default {
    setup(props) {
        const features = [
            {
                icon: '/img/upload.png',
                title: 'Upload & Organize',
                detail: 'Upload in bulk, organize content in categories, add custom filters & upload extras.'
            },
            {
                icon: '/img/icon-record.png',
                title : 'Stream On-Demand',
                detail : 'Showcase your content in a beautiful on-demand video catalog.'
            },
            {
                icon: '/img/icon-net.png',
                title: 'Stream Live',
                detail: 'Schedule events in advance & build excitement with a countdown overlay.'
            },
            {
                icon: '/img/icon-dollar.png',
                title: 'Monetization',
                detail: 'Offer subscriptions or one-time purchases. Accept credit cards & PayPal.'
            },
            {
                icon: '/img/jaringan.png',
                title: 'Analytics',
                detail: 'Know what your audience likes & how your content is performing.'
            },
            {
                icon: '/img/icon-pc.png',
                title: 'For all devices',
                detail: 'Get organized on all devices'
            }
        ]

        return { features }
    }
}
</script>