<template>
  <header>
    <img :src="img">
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      img: require('@/assets/apex.png')
    }
  }
}
</script>

<style scoped>
  .body-bg-pub-image img{
    display: none;
  }

  img {
    width: 300px;
  }

  @media(max-width: 700px) {
    img {
      display: block;
      margin: auto;
    }
  }
</style>
