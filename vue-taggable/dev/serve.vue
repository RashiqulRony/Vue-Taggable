<script>
import Vue from 'vue';
import VueTaggable from '@/vue-taggable.vue';

export default Vue.extend({
  name: 'ServeDev',
  components: {
    VueTaggable
  }
});
</script>

<template>
  <div id="app">
    <vue-taggable />
  </div>
</template>
