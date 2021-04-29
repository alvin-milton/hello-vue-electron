<template>
  <div>
    <div class="embeds" v-for="item in feeds" v-bind:key="item">
      <div class="twitter-embed">
        <a
          class="twitter-timeline"
          :href="item.path"
          data-width="300"
          data-height="300"></a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TwitterEmbed',
  data: function() {
    return {
      feeds: [
        {
          path: 'https://twitter.com/bbcafrica'
        },
        {
          path: 'https://twitter.com/ethereum'
        },
      ]
    }
  }
}
</script>

<style scoped>
  .embeds {
    display: inline-block;
  }
</style>
