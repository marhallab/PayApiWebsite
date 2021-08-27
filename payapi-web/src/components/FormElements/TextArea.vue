<template>
  <input :class="state" v-on:click="inputClicked" placeholder="Message" v-model="text"/>
</template>

<style scoped>
.normalState {
    border: none;
    border-bottom: 1px solid #36536B;
    background-color: transparent;
    resize: none;
    overflow: hidden;
    outline: none;
    opacity: 0.5;
}

.errorState{
    border: none;
    border-bottom: 1px solid red;
    background-color: transparent;
    resize: none;
    overflow: hidden;
    outline: none;
    opacity: 0.5;   
}

.errorState::placeholder{
    color: red;
}

input:focus{
    opacity: 1;
}
</style>

<script>
export default {
    props: {
    state: {
      type: String,
      default: 'normalState',
    },
    text: {
      type: String,
    },
  },
  methods: {
    inputClicked() {
      if(this.state == "errorState"){
          this.state = "normalState"
      }
    },
  },
}
</script>