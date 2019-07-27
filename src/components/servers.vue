<template>
  <div class="row">
    <div class="col-xs-12 col-sm-6">
      <ul class="list-group">
        <li
          :key="server.id"
          :id="server.id"
          :status="server.status"
          @click="sendDetail()"
          class="list-group-item"
          v-for="server in servers"
        >
          Server #{{ server.id }}
        </li>
      </ul>
    </div>
    <div class="col-xs-12 col-sm-6">
      <p>Server Details are currently not updated</p>
    </div>
  </div>
</template>

<script>
import { eventBus } from "../main";
export default {
  name: "servers",
  methods: {
    sendDetail() {
      //console.log("sending");
      console.log(this.status, this.id);
      eventBus.$emit("selectedServer", "test");
    }
  },

  data: function() {
    return {
      servers: [
        {
          id: 1,
          status: "Normal"
        },
        { id: 2, status: "Critical" },
        { id: 3, status: "Unknown" },
        { id: 4, status: "Normal" }
      ]
    };
  }
};
</script>
<style>
li {
  cursor: pointer;
}
</style>
