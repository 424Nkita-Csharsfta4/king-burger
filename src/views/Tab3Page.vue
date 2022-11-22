<template>
    <ion-page>
      <ion-header>
    
    <h1>King-burger</h1>
  </ion-header>
  <ion-content ref="content" class="ion-padding">
    <ion-button expand="block" @click="scrollToBottom()">Прокрутить вниз</ion-button>
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
  <ion-card>
    <img alt="Silhouette of mountains" src="https://proprikol.ru/wp-content/uploads/2020/11/kartinki-piczcza-40.jpeg" />
    <ion-card-header>
      <ion-card-title>Пица равиоле</ion-card-title>
      <ion-card-subtitle>Пиперони</ion-card-subtitle>
    </ion-card-header>

    <ion-card-content>
     Делается пица в течении 20-35 мин.
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
  <ion-card>
    <img alt="Silhouette of mountains" src="https://s0.rbk.ru/v6_top_pics/media/img/9/28/756400984063289.jpg" />
    <ion-card-header>
      <ion-card-title>Картошка фри</ion-card-title>
      <ion-card-subtitle>Картошка</ion-card-subtitle>
    </ion-card-header>

    <ion-card-content>
     Делается Бургер в течении 10-15 мин.
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
  

    <ion-button expand="block" @click="scrollToTop()" >Прокруть вверх</ion-button>
  </ion-content>

      <ExploreContainer name="Tab 3 page" />
    </ion-page>
</template>

<script lang="ts">

import { defineComponent } from 'vue';
import {  IonContent,IonButton,IonCard,IonCardContent,IonCardTitle,IonHeader,IonPage  } from '@ionic/vue';
import ExploreContainer from '@/components/ExploreContainer.vue';


export default defineComponent({
  name: 'Tab3Page',
  components: { ExploreContainer,   IonContent, IonButton,IonCard,IonCardContent,IonCardTitle,IonHeader,IonPage  },
  
  methods: {
      scrollToBottom() {
        this.$refs.content.$el.scrollToBottom(500);
      },
      scrollToTop() {
        this.$refs.content.$el.scrollToTop(500);
      },
}
})

</script>
