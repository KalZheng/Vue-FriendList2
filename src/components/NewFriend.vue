<template>
  <form>
    <div>
      <label for="name">Name: </label
      ><input v-model="friend.name" id="name" type="text" />
    </div>
    <div>
      <label for="phone">Phone: </label
      ><input v-model="friend.phone" id="phone" type="text" />
    </div>
    <div>
      <label for="email">Email: </label
      ><input v-model="friend.email" id="email" type="text" />
    </div>
    <button @click.prevent="addFriend">Add Friend</button>
  </form>
</template>

<script>
export default {
  emits: ["add-friend"],
  data() {
    return {
      friend: {
        name: "",
        phone: "",
        email: "",
      },
    };
  },
  methods: {
    addFriend() {
      const friendData = this.friend;
      this.$emit("add-friend", friendData);
    },
  },
};
</script>
