<template>
  <nav class="nav">
  <h1 class="nav__app-name">OMBDI</h1>
  <div>
    <!-- <router-link to="/about">About</router-link> -->
  </div>
  </nav>
</template>
<script lang="ts">
export default {};
</script>
<style lang="scss">
.nav {
    height: 30px;
    display: flex;
    background: #292929;
    align-items: center;
    padding: 0.5rem 1rem;

  &__app-name {
      color: white;
      border: 0.5px solid white;
      padding: 2px 10px;
      border-radius: 3px;
      font-size: 16px;
      font-weight: bold;
    }
}

</style>
