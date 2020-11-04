<template>
  <div>
    <h1>Ceci est le menu</h1>
  </div>

</template>

<script>
export default {
  name: "Menu",
  props: {
    unreadMessages: Number,
  }
};
</script>

<style scoped>
h1 {
  border: solid black 2px;
}

</style>
