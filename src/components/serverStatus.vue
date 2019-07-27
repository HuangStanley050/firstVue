<template>
  <div>
    <p>Server {{ id }} Status: {{ status }}</p>
    <hr />
    <button @click="changeStatus">Change Status</button>
  </div>
</template>

<script>
import { eventBus } from "../main";
export default {
  name: "ServerStatus",
  props: {
    id: {
      type: Number
    },
    status: { type: String }
  },
  created() {
    eventBus.$on("selectedServer", status => (this.status = status));
  },
  methods: {
    changeStatus() {
      this.status = "Normal";
    }
  }
};
</script>

<style></style>
