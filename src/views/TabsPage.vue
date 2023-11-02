<template>
  <ion-page>
    <ion-tabs>
      <ion-router-outlet></ion-router-outlet>
      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="tab1" href="/tabs/Camera">
          <ion-icon aria-hidden="true" :icon="triangle" />
          <ion-label>Camera</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="tab2" href="/tabs/Library">
          <ion-icon aria-hidden="true" :icon="ellipse" />
          <ion-label>Library</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>

<script setup lang="ts">
import { IonTabBar, IonTabButton, IonTabs, IonLabel, IonIcon, IonPage, IonRouterOutlet } from '@ionic/vue';
import { ellipse, square, triangle } from 'ionicons/icons';
</script>
