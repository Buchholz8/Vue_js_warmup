<template>
  <div>
    <button class="background" @click="color_change">Click Me</button>
    <article >
      <p class="pink" @click="pink_back" v-for="(secret, i) in secrets" :key="i">{{ secret }}</p>
    </article>
  </div>
</template>

<script>
export default {
  methods: {
    color_change: function () {
      let background = document.querySelector(`.background`);
      background[`style`][`backgroundColor`] = `red`;
    },
    pink_back: function(){
let pink_back = document.querySelector(`.pink`);
pink_back[`style`][`backgroundColor`] = `pink`;
    },
  },
  data() {
    return {
      secrets: [[`thing 1`, `thing 2`],[`option 1`, `option 2`],

      ],
    };
  },
};
</script>

<style scoped>
</style>