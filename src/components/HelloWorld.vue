<template>
  <div class="space-y-4">
    <h1>{{ msg }}</h1>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla ac varius augue, sit amet mattis ante. Nulla
      malesuada, sem nec dignissim lacinia, felis sem rhoncus magna, in tincidunt risus augue vitae orci. Nunc
      pellentesque dui ac lorem facilisis dapibus. Integer ut nulla elit. Nunc non lacus nibh. Nulla nec ipsum magna.
      Morbi et aliquam libero. Morbi a convallis eros, vitae scelerisque velit. Maecenas neque dolor, convallis at
      tortor sed, convallis pharetra lacus. Sed dignissim sagittis metus, id varius nibh. Aliquam auctor nibh sed
      malesuada fermentum. Ut non pellentesque felis.</p>
    <button type="button" @click="state.count++" class="btn">
      count is: {{ state.count }}
    </button>
  </div>
</template>

<script setup>
import {defineProps, reactive} from 'vue'

defineProps({
  msg: String
})

const state = reactive({ count: 0 })
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
