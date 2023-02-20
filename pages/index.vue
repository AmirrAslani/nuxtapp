<template>
  <div class="mt-4">
    <div class="mb-4">
      <HeadTitle />
    </div>
    <div class="row justify-content-center m-auto">
      <nuxt-link class="links" v-for="obj in mobInfo" :key="obj" :to="'/info/' + obj.id">
        <Card class="p-2" :image="obj.image" :title="obj.title" />
      </nuxt-link>
    </div>
    <div>
      <Footer class="mb-4"/>
    </div>
  </div>
</template>

<script>
import 'assets/css/style.css'

export default {
  name: 'IndexPage',
  data() {
    return {
      mobInfo: [
        {
          id: '1', image: 'images/mobile1.jpg', title: 'گوشی موبایل اپل مدل iPhone 13 Pro ZA/A Active دو سیم کارت ظرفیت 256 گیگابایت - رم 6 گیگابایت',
        },
        {
          id: '2', image: 'images/mobile2.jpg', title: 'گوشی موبایل سامسونگ مدل Galaxy A33 5G SM-A336 دو سیم کارت ظرفیت 128 گیگابایت و رم 6 گیگابایت',
        },
        {
          id: '3', image: 'images/mobile3.jpg', title: 'گوشی موبایل سامسونگ مدل Galaxy A73 5G SM-A736B/DS دو سیم کارت ظرفیت 128 گیگابایت',
        },
        {
          id: '4', image: 'images/mobile4.jpg', title: 'گوشی موبایل رنسو مدل Nep N9 Pro 5G دو سیم کارت ظرفیت 256 گیگابایت و رم 12 گیگابایت',
        },
        {
          id: '5', image: 'images/mobile5.jpg', title: 'گوشی موبایل اپل مدل iPhone 13 Pro Max LLA تک سیم‌ کارت ظرفیت 128 گیگابایت و رم 6 گیگابایت',
        },
        {
          id: '6', image: 'images/mobile6.jpg', title: 'گوشی موبایل سامسونگ مدل Galaxy S23 Ultra ظرفیت 256 گیگابایت و رم 12 گیگابایت',
        },
        {
          id: '7', image: 'images/mobile7.jpg', title: 'گوشی موبایل شیائومی مدل Redmi Note 9 ظرفیت 256 گیگابایت رم 8 گیگابایت',
        },
        {
          id: '8', image: 'images/mobile8.jpg', title: 'گوشی موبایل شیائومی مدل 12T Pro دو سیم کارت ظرفیت 256 گیگابایت و رم 8 گیگابایت',
        },
        {
          id: '9', image: 'images/mobile9.jpg', title: 'گوشی موبایل اوپو مدل A55 دو سیم کارت ظرفیت 128 گیگابایت و رم 4 گیگابایت',
        },
        {
          id: '10', image: 'images/mobile10.jpg', title: 'گوشی موبایل نوکیا مدل G11 Plus دو سیم کارت ظرفیت 64 گیگابایت و رم 4 گیگابایت',
        },

      ]
    }
  },
}
</script>

<style>
body {
  background-color: rgb(237, 243, 242);
}
</style>
