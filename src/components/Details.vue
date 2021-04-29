<template>
  <div>
    <div class="links" v-for="item in links" v-bind:key="item">
      <a :href="item.path" target="_blank">{{ item.label }}</a>
    </div>
  </div>
</template>

<script>

export default {
  name: "Details",
  data: () => {
    return {
      links: [
        { path: 'https://github.com/alvin-milton', label: 'Github' },
        { path: 'https://www.linkedin.com/in/agdmmgda', label: 'LinkedIn' },
        { path: 'mailto:alvin.milton@gmail.com', label: 'Email me' },
        { path: 'http://127.0.0.1:5000', label: 'Resume' },
      ]
    }
  }
};
</script>

<style scoped>
  .links {
    display: inline-block;
  }
  .links a {
    padding: 0 30px;
  }
</style>
