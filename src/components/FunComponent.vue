<template>
    <div>
<button class="background" @click="color_change"> Click Me</button>
    </div>
</template>

<script>
    export default {
        methods: {
            color_change: function () {
let background = document.querySelector(`.background`)
background[`style`][`backgroundColor`] = `red`
            }
        }
    }
</script>

<style scoped>

</style>