<template>
  <input
    :form="form"
    type="text"
    :name="placeHolder"
    :class="state"
    v-on:click="inputClicked"
    :placeholder="placeHolder"
    v-bind:value="value"
    v-on:input="$emit('input', $event.target.value)"
  />
</template>

<style scoped>
input {
  margin-bottom: 10%;
}

.normalState {
  border: none;
  border-bottom: 1px solid #36536b;
  background-color: transparent;
  resize: none;
  overflow: hidden;
  outline: none;
  opacity: 0.7;
}

.errorState {
  border: none;
  border-bottom: 1px solid red;
  background-color: transparent;
  resize: none;
  overflow: hidden;
  outline: none;
  opacity: 0.5;
}

.errorState::placeholder {
  color: red;
}

input:focus {
  opacity: 1;
}
</style>

<script>
export default {
  props: {
    state: {
      type: String,
      default: "normalState",
    },
    value: {
      type: String,
    },
    placeHolder: {
      type: String,
    },
    form: {
      type: String,
    },
  },

  methods: {
    inputClicked() {
      var currentState = this.state;
      if (currentState == "errorState") {
        currentState = "normalState";
      }
      this.$emit("update-state", currentState);
    },
  },
};
</script>