<template>
  <div>
    <TheNav />
    <div class="container">
      <MyItem v-for="item in myRentals" :key="item.id" :item="item" />
    </div>
  </div>
</template>

<script>
import { mapState } from "vuex";
export default {
  computed: {
    ...mapState(["myRentals"]),
  },
};
</script>

<style scoped>
</style>