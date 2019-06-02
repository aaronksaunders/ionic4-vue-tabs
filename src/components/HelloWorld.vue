<template>
  <div>
    <ion-tabs>
      <ion-tab tab="/tab1">
        <ion-vue-router name="tab1"></ion-vue-router>
      </ion-tab>

      <ion-tab tab="/tab2">
        <ion-vue-router name="tab2"></ion-vue-router>
      </ion-tab>

      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="/tab1">
          <ion-icon name="contacts"/>
          <ion-label>Tab 1</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="/tab2">
          <ion-icon name="contacts"/>
          <ion-label>Tab 2</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </div>
</template>