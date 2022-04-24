<template>
  <ion-app>
    <ion-router-outlet />
    <LayoutMenu />
  </ion-app>
</template>

<script lang="ts">
import { IonApp, IonRouterOutlet } from '@ionic/vue';
import LayoutMenu from '@/components/LayoutMenu.vue'
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {
    IonApp,
    IonRouterOutlet,
    LayoutMenu
  }
});
</script>

<style scoped>
span{
  color: #111;
}
</style>