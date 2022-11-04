<template>
  <div class="header" :style="image">
  <h1 class="header__title">Watch something incredible</h1>
  <div class="header__overlay"/>
  </div>
</template>
<script lang="ts">
export default {
  name: 'AppHeader',
  data() {
    return {
      image: {
        backgroundImage: `url(${require('@/assets/pexels-nathan-engel-header.jpg')})`,
        backgroundSize: 'cover',
        "background-repeat": "no-repeat",
      },
    };
  },
};
</script>
<style scoped lang="scss">
.header {
  display: flex;
  justify-content: space-between;
  height: 500px;
  display : flex;
  padding: 2.5rem;
  align-items: center;
  position  : relative;
  &__title {
    color: white;
    font-size: 4rem;
     width: 490px;
     z-index: 25;
  }

  &__overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #000;
    opacity: 0.5;

 }
}
</style>
