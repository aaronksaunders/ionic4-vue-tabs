<template>
  <div class="ion-page">
    <ion-tabs>
      <ion-tab tab="tab1" :routes="['tab1', 'tab1-details']" :to="{name:'tab1'}">
        <ion-vue-router name="tab1Route"></ion-vue-router>
      </ion-tab>

      <ion-tab tab="tab2">
        <ion-vue-router name="tab2Route"></ion-vue-router>
      </ion-tab>

      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="tab1">
          <ion-icon name="contacts" />
          <ion-label>Tab 1</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="tab2" :to="{name:'tab2'}"> 
          <ion-icon name="map" />
          <ion-label>Tab 2</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </div>
</template>

<script>
import { contacts, map } from "ionicons/icons";
import { addIcons } from "ionicons";
// import Tab1 from "./Tab1";
// import Tab2 from "./Tab2";
addIcons({
  "ios-contacts": contacts.ios,
  "md-contacts": contacts.md,
  "ios-map": map.ios,
  "md-map": map.md
});
export default {
  name: "TabRoot",
  props: {}
};
</script>