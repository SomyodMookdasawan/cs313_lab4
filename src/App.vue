<template>
 <div id="app" :style="{'background-image':'url(https://407261-1281864-raikfcquaxqncofqfm.stackpathdns.com/wp-content/uploads/2019/10/infant-pink-backdrop-416x395.jpg)'}">
    <HelloWorld msg="LIKE-LOVE-UNLIKE-RESET" /><hr><br>
    <div class="row">
      <div class="col-12">
        <img alt="Vue logo" src="./assets/1.jpg" width="490" /><br><br><hr>
        <h1>{{total}}</h1>
      </div>
      <div class="col-12">
        <CsButton @cc="sum" />
      </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue"
import CsButton from "./components/CsButton.vue"

export default {
  name: "App",
  components: {
    HelloWorld,
    CsButton,
  },
  data: function(){
    return {
      total: 0,
    };
  },

  methods: {
    sum(counterValue) {
      this.total = counterValue;
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
