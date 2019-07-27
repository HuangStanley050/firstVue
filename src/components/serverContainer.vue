<template>
  <div>
    <Servers />
    <ServerStatus />
  </div>
</template>

<script>
import Servers from "./servers.vue";
import ServerStatus from "./serverStatus.vue";
export default {
  name: "ServerContainer",
  components: {
    Servers,
    ServerStatus
  }
};
</script>
