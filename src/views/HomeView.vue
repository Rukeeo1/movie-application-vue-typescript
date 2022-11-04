<template>
  <div class="home">
    <AppHeader />
    <div class="home__body">
      <AppInput placeholder="Search" label="Search" />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import AppHeader from '@/components/AppHeader.vue';
import AppInput from '@/components/AppInput.vue';

export default defineComponent({
  name: 'HomeView',
  components: {
    AppHeader,
    AppInput,
  },
});
</script>

<style scoped lang="scss">
.home {
  &__body {

  }
}
</style>
