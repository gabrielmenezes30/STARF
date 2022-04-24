<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title class="title title-tab1">COMPUTAÇÃO 2022.1</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content  :fullscreen="true">
      <ion-header>
        <ion-toolbar>
          <ion-title size="medium">Atividades pendentes: <span>{{  }}</span></ion-title>
        </ion-toolbar>
      </ion-header>
    + 
      <!-- <ExploreContainer
       name="Bem vindo"
        /> -->
      <div class="content">
        
      <CardContent 
      name="EFEB" 
      description="Ensinamentos fundamentais da educação básica"
      to = "/efeb"
      />

      <CardContent 
      name="CI" 
      description="Ciência e inovação"
      to = "tab3"
      />

       <CardContent 
      name="FFE" 
      description="Fundamentos filosóficos da educação"
      to = "tab3"
      />

       <CardContent 
      name="IaC" 
      description="Introdução à computação"
      to = "tab3"
      />

       <CardContent 
      name="IaC" 
      description="Introdução à computação"
      to = "tab3"
      />

       <CardContent 
      name="IaC" 
      description="Introdução à computação"
      to = "tab3"
      />

       <CardContent 
      name="IaC" 
      description="Introdução à computação"
      to = "tab3"
      />
      


      


      
      
      </div>
      
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import CardContent from '@/components/CardContent.vue';


export default  defineComponent({
  name: 'Tab1Page',
  components: { CardContent, IonHeader, IonToolbar, IonTitle, IonContent, IonPage }
});
</script>


<style scoped>
.title-tab1{
  color: #ffee00;
  font-weight: bold;
}
.content{
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}
</style>