 <template>
  <div>Product Page</div>
  <span> Looking for Product: {{ this.$route.params.id }} </span>
  <div>
    <a href="#" @click="goTo('home')">Home</a>
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