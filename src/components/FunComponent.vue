<template>
  <div>
    <button class="background" @click="color_change">Click Me</button>
    <article v-for="(secret, i) in secrets" :key="i">
      <p class="pink" @click="pink_back">{{ secret[`string1`]}}</p>
      <p class="pink_2" @click="pink_back_2">{{ secret[`string2`]}}</p>
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
        pink_back_2: function(){
let pink_back_2 = document.querySelector(`.pink_2`);
pink_back_2[`style`][`backgroundColor`] = `pink`;
    }
  },
  data() {
    return {
      secrets: [
        {
          string1: [`thing 1`, `thing 2`],
          string2: [`option 1`, `option 2`],
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>