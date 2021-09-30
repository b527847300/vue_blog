<template>
  <div class="container">
    <List />
    <Secondary />
  </div>
</template>

<script>
// @ is an alias to /src

import List from "@/components/List.vue";
import Secondary from "@/components/Secondary.vue";
export default {
  name: "Home",
  components: {
    List,
    Secondary,
  },
  methods: {
  
  },
  mounted: function () {
    
  },
};
</script>


<style>
.container {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: flex-start;
}
</style>