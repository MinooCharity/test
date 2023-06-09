<template>
    <NuxtLayout name="custom">
      <div class="max-w-7xl mx-auto py-16 px-4 sm:px-6 lg:px-8 bg-amber-100 rounded-xl">
        <h1 class="text-3xl font-extrabold tracking-tight text-gray-900">محصولات کسا</h1>
        <p class="mt-4 max-w-xl text-sm text-gray-700">امیدواریم با حمایت های شما تنوع بیشتری به محصولات بدهیم.</p>
      </div>
<!--      //next version-->
<!--      <CategoryFilter/>-->
      <ProductList/>
      <hr class="bg-white py-1 ">
      <CommerceUs/>
    </NuxtLayout>

</template>

<script>
import CategoryFilter from "../components/CategoryFilter";
import ProductList from "../components/ProductList";
import CommerceUs from "../components/CommerceUs";
export default {
  name: "shop",
  components: {CommerceUs, ProductList, CategoryFilter},
  jsonld() {
    return {
      '@context': 'https://schema.org',
      '@type': 'Corporation',
      mainEntityOfPage: {
        '@type': 'WebPage',
        '@id': 'https://iranimarket.com/shop'
      },
      headline: ' فروشگاه ایرانی مارکت ',
      description: 'خرید آنلاین شال و روسری و اکسسوری از ترکیه با کلی محصول نخی و ابریشمی خاص و جذاب و چهار فصل',
      image: 'https://iranimarket.com/_nuxt/scrf1.47fd393c.jpeg',
      author: {
        '@type': 'Person',
        name: 'فربد نصیری پرتوی'
      },
      datePublished: '7/18/2022',
      dateModified: '7/18/2022',
      publisher: {
        '@type': 'Organization',
        name: 'ایرانی مارکت کسا',
        logo: {
          '@type': 'ImageObject',
          url: 'https://nuxt.markazimarket.com/public/storage/product/11042345975840'
        }
      }
    };
  },
  head: {
    title: 'فروشگاه ایرانی مارکت',
    meta: [
      {name:"google-site-verification" ,content:"_Y9NTv1bukKVeHHLG0K71UFKgFTeH0dtwHoiR9bg0oI" },
      {
        hid: 'og:title',
        property: 'og:title',
        content: 'ایرانی مارکت'
      },
      {
        hid: 'og:description',
        property: 'og:description',
        content: 'فروشگاه آنلاین برای خرید شال و روسری خاص و مجلسی و ابریشمی و نخی  و طرح ساده و بته جقه  و شیک و جذاب  برای خاص بانوان خاص پسند '
      },
      {
        hid: 'og:type',
        property: 'og:type',
        content: 'website',
      },
      {
        hid: 'og:image',
        property: 'og:image',
        content: 'https://iranimarket.com/_nuxt/logo.d57cb96c.png'
      },
      {
        hid: 'og:url',
        property: 'og:url',
        content: 'https://iranimarket.com/shop'
      },
      {
        property: 'og:locale',
        content: 'de_DE'
      }
    ],
    link: [{ rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' }]
  }
}
</script>

<style scoped>

</style>