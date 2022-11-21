<template>
  <ion-page>
    <ion-card>
    <img alt="Silhouette of mountains" src="https://world.openfoodfacts.org/images/products/505/478/112/8878/front_en.3.full.jpg" />
    <ion-card-header>
      <ion-card-title>Mega Burger</ion-card-title>
      <ion-card-subtitle>Мясо:Гавядина</ion-card-subtitle>
    </ion-card-header>

    <ion-card-content>
     Делается бургкр в течении 10-15 мин.
     Доставка по всему Тирасполю
    </ion-card-content>
    <ion-button>Заказать</ion-button>
  </ion-card>

  <ion-card color="success">
    <ion-card-header>
      <ion-card-title>Оплата</ion-card-title>
      <ion-card-subtitle>Наличными или карта</ion-card-subtitle>
    </ion-card-header>

    <ion-button>Оплатить</ion-button>
  </ion-card>
      <ExploreContainer name="Tab 1 page" />
   
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle,IonButton  } from '@ionic/vue';
import ExploreContainer from '@/components/ExploreContainer.vue';


export default  defineComponent({
  name: 'Tab1Page',
  components: { ExploreContainer,  IonPage,IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle,IonButton  }
});
</script>
<style scoped>
  /* iOS places the subtitle above the title */
  ion-card-header.ios {
    display: flex;
    flex-flow: column-reverse;
  }
 
</style>