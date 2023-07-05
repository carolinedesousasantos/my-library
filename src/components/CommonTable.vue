<template>
  <div class="q-pa-md">
    <q-table title="Treats" :rows="rows" :columns="columns" row-key="name" />
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "CommonTable",
  props: {
    columns: {
      type: Array,
      required: true,
    },

    rows: {
      type: Array,
      required: true,
    },
  },
});
</script>
