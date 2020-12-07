<template>
  <div id="app">
    <UserCard :user="user"/>
  </div>
</template>

<script>
import UserCard from './components/user-card.vue'
export default {
  name: 'App',
  components: {
    UserCard,
  },
  data() {
    return {
      user: {
        name: "nos nart",
        role: "Developer",
        avatar: "https://randomuser.me/api/portraits/women/26.jpg",
        bio: "Hello world!"
      }
    }
  }
}
</script>

<style>
</style>
