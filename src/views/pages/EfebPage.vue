<template>
  <ion-page>
    <ion-router-outlet></ion-router-outlet>
    <ion-content>
      <div class="container">
        <div class="content">
          <div>
            <p class="title">{{ name }}</p>
          </div>
          <div>
            <ion-item>
              <ion-label> Item 1 </ion-label>
            
            </ion-item>
            <ion-item>
              <ion-label> Item 2 </ion-label>
       
            </ion-item>,
            
          </div>
        </div>
      </div>
    </ion-content>
  </ion-page>
</template>

<script>
import { defineComponent } from "vue";
import { IonPage, IonContent, IonRouterOutlet, IonItem, IonLabel } from "@ionic/vue";

export default defineComponent({
  name: "EfebPage",
  components: {
    IonPage,
    IonContent,
    IonRouterOutlet,
     IonItem, 
     IonLabel
  },
  data() {
    return {
      name: "EFEB",
    };
  },
});
</script>


<style scoped>
div {
  color: #111;
}

.title {
  font-weight: 900;
  font-size: 40px;
}

ion-item{
    background-color: red !important;
}
</style>
