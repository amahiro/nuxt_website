<script setup>

const SITE_TITLE = "AMANO HIROKI portfolio"
useHead({
  titleTemplate: (titleChunk) => {
    return titleChunk ? `${titleChunk} | ${SITE_TITLE}` : SITE_TITLE;
  },
  // meta: [
  //       { name: 'description', content: 'My amazing site.'}
  //   ],
    meta: [
    {
      hid: 'description',
      name: 'description',
      content: 'ホームページの説明文です。',
    },
    {
      hid: 'og:title',
      property: 'og:title',
      content: 'ホームページのog:titleテスト',
    },
    {
      hid: 'og:description',
      property: 'og:description',
      content: 'ホームページのog:og:descriptionテスト',
    },
    {
      hid: 'og:image',
      property: 'og:image',
      content: 'http://illustrain.com/img/work/2016/illustrain04-kaisya01.png',
    },
  ],
  // link: [
  //   // GoogleFonts設定
  //   {
  //     rel: "stylesheet",
  //     href: "https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@400;500;700&display=swap",
  //   },
  // ],
});
</script>

<template>
  <div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<style lang="scss" scoped></style>