    
<template>
  <ion-page
    class="ion-page">
    <ion-header>
      <ion-toolbar color="primary">
        <ion-title>Ionic4 VueJS: Tab 1</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content padding>
      <ion-label>hello</ion-label>
      <ion-button @click="nextPage()">Next Page</ion-button>
    </ion-content>
  </ion-page>
</template>

<script>
export default {
  name:"tab1",
  methods: {
    nextPage() {
      this.$router.push("/tab1/details");
    }
  },
  onCreate() {
    debugger;
  }
};
</script>

<style>
</style>
