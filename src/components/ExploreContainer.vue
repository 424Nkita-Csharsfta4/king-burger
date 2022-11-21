<template>
  <div id="container">
   
   
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'ExploreContainer',
  props: {
    name: String
  }
});
</script>

<style scoped>
#container {
  background-color: inherit;
  color: inherit;
  opacity: 1;
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
  color: inherit;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  color: inherit;
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
