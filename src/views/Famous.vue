<template>
  <div class="py-28">
      <p class="font-monstand font-bold text-5xl text-center mb-5 px-4">Famous live on our platform</p>
      <p class="font-mules font-normal text-center px-4 mb-16">At the end of the day have fun with celebrities</p>

    <div class="overflow-hidden">
        <div class="flex anjim">
            <img v-for="(image, index) in kekiri" :key="index" :src="image.img" class="mr-5" alt="">
        </div>
        <div class="flex rill mt-5">
            <img v-for="(image, index) in kekiri" :key="index" :src="image.img" class="mr-5" alt="">
        </div>
    </div>

  </div>
</template>

<script>
export default {
    setup(props) {
        const kekiri = [
            {
                img: '/img/pemes1.png'
            },
            {
                img: '/img/pemes2.png'
            },
            {
                img: '/img/pemes3.png'
            },
            {
                img: '/img/pemes4.png'
            },
            {
                img: '/img/pemes5.png'
            },
            {
                img: '/img/pemes6.png'
            },
            {
                img: '/img/pemes7.png'
            },
            {
                img: '/img/pemes8.png'
            },      
            {
                img: '/img/pemes2.png'
            },
            {
                img: '/img/pemes3.png'
            },
            {
                img: '/img/pemes4.png'
            },      
        ]

        return { kekiri }
    }
}
</script>

<style>
    .anjim {
        animation: marquee 15s infinite linear;
    }
    .rill{
        animation: marqueekanan 15s infinite linear;
    }

    @keyframes marquee {
        0%{
            transform: translateX(0);
        }
        100%{
            transform: translateX(-100%);
        }
    }
    @keyframes marqueekanan {
        0%{
            transform: translateX(-100%);
        }
        100%{
            transform: translateX(0);
        }       
    }
</style>