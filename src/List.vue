<template>
  <div>
    <div class="col-xs-12 col-sm-8 col-sm-offset-2 col-md-6 col-md-offset-3">
      <h1>Filters & Mixins</h1>
      <input type="text" v-model="filterText" />
      <ul>
        <li v-for="fruit in filteredFruits">{{ fruit }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
import { fruitMixin } from "./fruitMixin";
export default {
  mixins: [fruitMixin],
  created(){
      console.log('inside component created')
  }
};
</script>

<style></style>
