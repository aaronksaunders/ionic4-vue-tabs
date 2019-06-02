    
<template>
  <ion-page
    class="ion-page">
    <ion-header>
      <ion-toolbar color="primary">
        <ion-buttons slot="start">
          <ion-back-button default-href="/"></ion-back-button>
        </ion-buttons>
        <ion-title>Ionic4 VueJS: Tab 1 Details</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content padding>
      <ion-label>This is the details page</ion-label>
    </ion-content>
  </ion-page>
</template>

<script>
export default {
  name: "tab1",
  methods: {
    nextPage() {
      this.$router.push("/geo-location-page");
    }
  },
  onCreate() {
    debugger;
  }
};
</script>

<style>
</style>
