<template >
  <section>
    <div v-on:click="open()" id="menu">
      <button>
        <ion-icon :icon="menu" />
      </button>
    </div>
    <div v-show="toggle" class="sidemenu">
      <div class="menuOpen">
        <button v-on:click="closeMenu()">
          <ion-icon :icon="close" />
        </button>
      </div>
      <div class="list-menu">
          <a href="https://suap.ifsertao-pe.edu.br/" target="_blank">
        <ion-item color="danger" button @click="buttonClick()">
            <ion-icon :icon="person" />
          <ion-label>
            SUAP
          </ion-label>
        </ion-item>
        </a>
        <a href="https://suap.ifsertao-pe.edu.br/" target="_blank">
        <ion-item color="danger" button @click="buttonClick()">
            <ion-icon :icon="person" />
          <ion-label>
            SUAP
          </ion-label>
        </ion-item>
        </a>
        <a href="https://suap.ifsertao-pe.edu.br/" target="_blank">
        <ion-item color="danger" button @click="buttonClick()">
            <ion-icon :icon="person" />
          <ion-label>
            SUAP
          </ion-label>
        </ion-item>
        </a>
      </div>
    </div>
  </section>
</template>


<script lang="ts">
import { menu, close, person } from "ionicons/icons";

export default {
  name: "LayoutMenu",
  components: {},
  data() {
    return {
      toggle: false,
      count: 0,
    };
  },
  methods: {
    open() {
      this.toggle = !this.toggle;
    },
    closeMenu() {
      this.toggle = !this.toggle;
    },
    teste() {
      if (this.toggle === true) {
        this.toggle = !this.toggle;
      }
    },
  },
  setup() {
    return {
      menu,
      close,
      person
    };
  },
};
</script>


<style scoped>
section {
  height: 100vh;
  width: 100%;
}
#menu button {
  position: relative;
  left: 15px;
  top: 15px;
  font-size: 30px;
  font-weight: bold;
  color: #7001df;
  cursor: pointer;
  background-color: transparent;
}
.sidemenu {
  height: 100vh;
  width: 200px;
  background-color: #7001df;
  position: absolute;
  top: 0;
  transition: 0.5 ease all;
}
.menuOpen button {
  color: #ffee00;
  font-size: 30px;
  font-weight: bold;
  position: relative;
  left: 15px;
  top: 15px;
  background-color: transparent;
}
.list-menu{
    margin-top: 20px;
}
a{
    text-decoration: none;
    
}
ion-item{
    margin-top: 4px;
}
ion-label{
    margin-left: 4px;
}
</style>

