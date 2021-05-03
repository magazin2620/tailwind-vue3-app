<template>
  <div class="text-center">
    <h2 class="text-2xl font-bold">{{ text }}</h2>
    <div class="text-xl mt-4 mb-8">
      {{ timestamp }}
    </div>
  </div>
</template>

<script>
import moment from "moment";

export default {
  name: "DataTitle",
  props: ["text", "dataDate"],
  computed: {
    timestamp: function () {
      return moment(this.dataDate).format("MMMM D YYYY, h:mm:ss a");
    },
  },
};
</script>