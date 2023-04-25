<template>
  <section>
    <h2>My Friends</h2>
    <ul v-for="friend in friends" :key="friend.id">
      <li></li>
    </ul>
  </section>
</template>

<script>
export default {
  data() {
    return {
      friends: [
        {
          id: "manuel",
          name: "Manuel Test",
          phone: "1234565",
          email: "manuelTest@remail.com",
        },
        {
          id: "julie",
          name: "Julie Test",
          phone: "123124325325",
          email: "julieTest@remail.com",
        },
      ],
    };
  },
};
</script>
