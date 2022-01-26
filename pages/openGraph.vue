<template>
  <div>
    Hello, Open Graph.
  </div>
</template>

<script>
export default {
  name: "openGraph",
  head() {
    return {
      title: '오픈 그래프 테스트',
      meta: [
        {
          hid: 'og:title',
          property: 'og:title',
          content: '오픈 그래프 페이지'
        },
        {
          hid: 'og:description',
          property: 'og:description',
          content: '오픈 그래프 정보를 확인해보세요'
        },
        {
          hid: 'og:image',
          property: 'og:image',
          content: 'http://placeimg.com/640/480/fashion'
        },
      ]
    }
  }
}
</script>
