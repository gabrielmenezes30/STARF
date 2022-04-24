<template>
  <ion-page>
    <ion-tabs>
      <ion-router-outlet></ion-router-outlet>
      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="tab1" href="/tabs/tab1">
          <ion-icon :icon="bulb" />
          <ion-label>Pendentes</ion-label>
        </ion-tab-button> 
          
        <ion-tab-button tab="tab2" href="/tabs/tab2">
          <ion-icon :icon="ellipse" />
          <ion-label>Externo</ion-label>
        </ion-tab-button>
        
        <ion-tab-button layout="icon-bottom" tab="tab3" href="/tabs/tab3">
          <ion-icon :icon="warning" />
          <ion-label>Avisos e links</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>
<script lang="ts">
import { defineComponent } from 'vue';
import { IonTabBar, IonTabButton, IonTabs, IonLabel, IonIcon, IonPage, IonRouterOutlet } from '@ionic/vue';
import { ellipse, square, triangle, accessibility, warning, bulb} from 'ionicons/icons';

export default defineComponent({
  name: 'TabsPage',
  components: { IonLabel, IonTabs, IonTabBar, IonTabButton, IonIcon, IonPage, IonRouterOutlet },
  setup() {
    return {
      ellipse, 
      square, 
      triangle,
      accessibility,
      warning,
      bulb
      
    }
  }
});
</script>


<style>
.title{
  text-align: center;
}

ion-tab-button{
  --color-focused: #111;
}
</style>