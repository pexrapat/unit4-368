<template>
  <div class="htmlClass">
    <h1>{{ title }}</h1>
    <form>
      <input type="text" id="firstName" v-model="firstName" />
      <input type="text" id="secondName" v-model="secondName" />
      <input type="text" id="Nickname" v-model="Nickname" />
      <input type="text" id="StudentCode" v-model="StudentCode" />
      <button @click="submitForm()" class="submitForm">Submit</button>
  </form>
  </div>
</template>

<script>
export default {
  name: 'InputPage',
  data() {
    return {
      title: 'Vue is awesome.',
      firstName: 'Peerapat',
      secondName: 'Khodkaew',
      Nickname: 'Bas',
      StudentCode: '6604101368',
    }
  },
  methods: {
    submitForm() {
      this.$emit('submit form')
    },
  }
}
</script>

<style scoped></style>
