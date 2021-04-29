<template>
  <div class="hello">
    <div class="qr-codes" v-for="item in qr" v-bind:key="item">
      <img :src="item.code" :alt="item.label" width="100" height="100">
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data: function() {
    return {
      qr: [
        { code: "http://images.wealthy.af/greenfire/qr-code-name.png",
          label: "name"
        },
        { code: "http://images.wealthy.af/greenfire/qr-code-tezos.png",
          label: "tezos"
        },
        { code: "http://images.wealthy.af/greenfire/qr-code-burst.png",
          label: "burst"
        },
        { code: "http://images.wealthy.af/greenfire/qr-code-algo.png",
          label: "algo"
        },
      ]
    };
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .qr-codes {
    padding: 10px 30px;
    display: inline-block;
  }
</style>
