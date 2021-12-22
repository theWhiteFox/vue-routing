<template>
  <div class="profile">
    <h1>This is my profile page</h1>
  </div>
  <span>
    {{ this.$route.params.username }}
  </span>
  <div>
    <a href="#" @click="goTo('/')">Home</a>
    <a href="#" @click="goTo('about')">About</a>
  </div>
</template>

<script>
export default {
  name: "Product",
  methods: {
    goTo(route) {
      this.$router.push(route);
    },
  },
};
</script>

<style scoped>
a {
  padding: 16px;
}
</style>


