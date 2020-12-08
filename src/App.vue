<template>
  <div id="app">
    <UserCard :user="user"
      @click="alertName(user.name)"
      @contact="contactUser(user.name)">
      {{ user.bio }}
    </UserCard>
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
  },
  methods: {
    alertName(name) {
      alert(`Hello ${name}`);
    },
    contactUser(name) {
      alert(`Connect to ${name}`)
    }
  }
}
</script>

<style>
</style>
