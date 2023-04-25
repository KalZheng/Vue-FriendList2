<template>
  <li>
    <h2>{{ friend.name }}</h2>
    <button>Show Details</button>
    <ul><li>
        <strong>Phone: </strong> {{ friend.phone }}
        <strong>Email: </strong> {{ friend.email }}
    </li></ul>
  </li>
</template>

<script>
export default {
    data(){
        return {
            detailsAreVisible
        };
    },
};
</script>
