<template>
  <section id="card">
      <ion-card>
          <router-link class="route" :to="to">
    <ion-card-header>
      <ion-card-subtitle>{{ name }}</ion-card-subtitle>
      <ion-card-title>{{ description }}</ion-card-title>
    </ion-card-header>

    <ion-card-content>
      Keep close to Nature's heart... and break clear away, once in awhile,
      and climb a mountain or spend a week in the woods. Wash your spirit clean.
    </ion-card-content>
          </router-link>
  </ion-card>
    <!-- <div class="container">
      <router-link class="route" :to="to">
        <div class="content">
          <div class="text-card">
            {{ name }}
            <span>({{description}})</span>
          </div>
        </div>
      </router-link>
    </div> -->
  </section>
</template>


<script>
import { defineComponent } from "vue";
import {IonCard, IonCardHeader,IonCardSubtitle,IonCardTitle, IonCardContent, } from '@ionic/vue'

export default defineComponent({
  name: "CardContent",
  props: {
    name: String,
    description: String,
    to: String
  },
  components:{
      IonCard, IonCardHeader,IonCardSubtitle,IonCardTitle, IonCardContent,
  }
});
</script>


<style scoped>
#card{
    padding: 24px;
}

.container {
  width: 200px;
  max-width: 200vh;
  height: 75px;
  background-color: #ffe600;
  border-radius: 5px;
  text-decoration: none;
}
.route{
    text-decoration: none;
}
.text-card{
    text-align: center;
    padding: 10px;
    display: flex;
    flex-direction: column;
}
.content {
  display: flex;
  height: 100%;
  justify-content: center;
  align-items: center;
  color: #111;
  font-size: 24px;
  font-weight: 800;
}
.content span{
    font-size: 8px;
    color: #111;
}

ion-card{
    background-color: #ffe600;
    color: #111;
    max-width: 100vw;
}

ion-card-title{
    color: #111;
    font-weight: 500;
}

ion-card-subtitle{
    color: #111;
    font-weight: 900;
}

ion-card-content{
    color:  #111;
}


</style>