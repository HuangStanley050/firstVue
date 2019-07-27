<template>
  <div>
    <Servers @selectedServer="status = $event" />
    <ServerStatus :id="id" :status="status" />
  </div>
</template>

<script>
import Servers from "./servers.vue";
import ServerStatus from "./serverStatus.vue";
export default {
  data: function() {
    return {
      id: null,
      status: null
    };
  },
  name: "ServerContainer",
  components: {
    Servers,
    ServerStatus
  }
};
</script>
