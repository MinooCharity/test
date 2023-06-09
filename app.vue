<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>
<script>
export default {
  jsonld() {
    return {
      '@context': 'https://schema.org',
      '@type': 'Corporation',
      mainEntityOfPage: {
        '@type': 'WebPage',
        '@id': 'https://iranimarket.com/store'
      },
      headline: 'ایرانی مارکت',
      description: 'خرید آنلاین شال و روسری و اکسسوری  و گوشواره و گل سر های متنوع در جنس های خاص مثل نخ و ابریشمی و چهار فصل وارداتی ترکیه',
      image: 'https://iranimarket.com/_nuxt/scrf1.47fd393c.jpeg',
      author: {
        '@type': 'Person',
        name: 'فربد نصیری پرتوی'
      },
      datePublished: '7/17/2022',
      dateModified: '7/17/2022',
      publisher: {
        '@type': 'Organization',
        name: 'ایرانی مارکت کسا',
        logo: {
          '@type': 'ImageObject',
          url: 'httpS://nuxt.markazimarket.com/public/storage/product/11042345975840'
        }
      }
    };
  },
  head: {
    title: 'ایرانی مارکت',
    script: [
      {
        src: "https://www.googletagmanager.com/gtag/js?id=G-7BFYDEC3DP",
      },
    ],
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
        content: 'content="هر آنچه که میخوای با کمترین هزینه از ایرانی مارکت بخرید! جدیدترین انواع شال و روسری و اکسسوری و... با امکان تعویضی راحت | ✓ ارسال رايگان ✓ پرداخت - برای خرید کلیک کنید!"'
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
        content: 'https://iranimarket.com/'
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