<template functional>
  <div class="card" @click="listeners.click">
    <div class="additional">
      <figure class="avatar">
        <img :src="props.user.avatar" :alt="props.user.name">
        <button @click.stop="listeners.contact">Contact me</button>
      </figure>
    </div>
    <div class="more-info">
      <h2>{{ props.user.name }}</h2>
      <h2>{{ props.user.role }}</h2>
      <!-- <h2>{{ slots() }}</h2> -->
      <h2>{{ children }}</h2>
      <p>{{ Object.keys(listeners) }}</p>
    </div>
  </div>
</template>
