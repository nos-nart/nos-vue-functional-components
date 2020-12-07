<template>
  <div class="card">
    <div class="additional">
      <figure class="avatar">
        <img :src="user.avatar" :alt="user.name">
      </figure>
    </div>
    <div class="more-info">
      <h2>{{ user.name }}</h2>
      <h2>{{ user.role }}</h2>
      <h2>{{ user.bio }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    user: Object
  }
}
</script>

<style scoped>
.card {
  padding: 1rem;
  border-radius: 10px;
  border: 1px solid #f2f2f2;
  display: flex;
}
</style>