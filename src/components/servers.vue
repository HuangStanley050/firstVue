<template>
  <div class="row">
    <div class="col-xs-12 col-sm-6">
      <ul class="list-group">
        <li
          v-bind:key="server.id"
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
export default {
  name: "servers",
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
