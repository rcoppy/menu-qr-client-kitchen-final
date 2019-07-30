<template>
  <div>
    <v-container>
      <h1>Kitchen orders</h1>

      <ul>
        <li v-for="order in orders" v-bind:key="order.id">{{ order.name }}</li>
      </ul>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "OrdersIndex",
  data() {
    return {
      orders: [
        { id: 1, name: "Felix's order" },
        { id: 2, name: "Charles's order" },
        { id: 3, name: "Freddy's order" }
      ]
    };
  }
};
</script>