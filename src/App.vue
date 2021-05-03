<template>
  <Header />
  <div class="container mx-auto px-2">
    <router-view />
  </div>
</template>

<script>
import Header from "@/components/Header";
export default {
  components: {
    Header,
  },
};
</script>