<script setup lang="ts">
import Header from "../../organisms/Header.vue";
import SearchComponent from "../mainjob/search/index.vue";
import { useAuthStore } from "@/stores/auth";
defineProps<{}>();
const auth = useAuthStore();
</script>


<template>
  <Header />
  <div class="__default__ body-layout">
    <!-- <SearchComponent /> -->
    <slot class="body">
      
    </slot>
  </div>
</template>

<style lang="scss" scoped>
.body-layout {
  margin: 0 auto;
  width: 1300px;
  max-width: 100%;
  margin-top: 70px;
}
.bg {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: -1;
}
</style>
