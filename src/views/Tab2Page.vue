<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Поиск бургера </ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-item>
    <ion-label position="floating">Поиск</ion-label>
    <ion-input placeholder="Enter text"></ion-input>
  </ion-item>
  <ion-card>
    <ion-card-header>
      <ion-card-title>Список</ion-card-title>
      <ion-card-subtitle>Наших бургеров</ion-card-subtitle>
    </ion-card-header>
    <ion-card-content>
      <ion-list>
        <ion-item>
          <ion-thumbnail slot="start">
            <img alt="Silhouette of mountains" src="https://images3.alphacoders.com/942/thumb-1920-942653.jpg" />
          </ion-thumbnail>
          <ion-label>Сендвич</ion-label>
        </ion-item>

        <ion-item>
          <ion-thumbnail slot="start">
            <img alt="Silhouette of mountains" src="http://www.operatorchan.org/arch/src/138322037264.jpg" />
          </ion-thumbnail>
          <ion-label>Гамбургер</ion-label>
        </ion-item>

        <ion-item>
          <ion-thumbnail slot="start">
            <img alt="Silhouette of mountains" src="https://pbs.twimg.com/media/CewH0V0XIAAlOMW.jpg" />
          </ion-thumbnail>
          <ion-label>Дабл бургер</ion-label>
        </ion-item>

        <ion-item lines="none">
          <ion-thumbnail slot="start">
            <img alt="Silhouette of mountains" src="https://medboli.ru/wp-content/uploads/6/d/9/6d98178bbddea79b51292888adb1af05.jpeg" />
          </ion-thumbnail>
          <ion-label>Мега острый</ion-label>
        </ion-item>
      </ion-list>
    </ion-card-content>
  </ion-card>
      <ExploreContainer name="Tab 2 page" />
   
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonPage, IonToolbar, IonTitle,  IonInput, IonItem, IonLabel,IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle} from '@ionic/vue';
import ExploreContainer from '@/components/ExploreContainer.vue';

export default defineComponent({
  name: 'Tab2Page',
  components: { ExploreContainer,  IonToolbar, IonTitle,  IonPage, IonInput, IonItem, IonLabel,IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle}
});
</script>
<style> 
  img{
    border-radius: 7px;
  }
 
  
</style>
