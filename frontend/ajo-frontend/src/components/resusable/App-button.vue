<template>
  <div>
    <v-btn
        elevation="0"
        :loading="loading"
           :width="width"
           :height="height"
           :disabled="disabled"
           @click="$emit('click')"
           color="#03a84e"
    >{{text}} </v-btn>
  </div>

</template>

<script>
export default {
  name: "App-button",
  props: {
    width: {
      type: String,
      default: "100%"
    },
    height: {
      type: String,
      default: "48px"
    },
    loading: Boolean,
    disabled: [Boolean],
    text: String


  }
}
</script>

<style scoped>

</style>