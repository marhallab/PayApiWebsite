<template>
  <textarea
    :name="name"
    :form="form"
    :class="state"
    v-on:click="textAreaClicked"
    rows="4"
    cols="50"
    :placeholder="placeHolder"
    v-bind:value="value"
    v-on:input="$emit('input', $event.target.value)"
  />
</template>

<style scoped>
textarea {
  margin-bottom: 10%;
}

.normalState {
  border: none;
  border-bottom: 1px solid #36536b;
  background-color: transparent;
  resize: none;
  outline: none;
  opacity: 0.5;
}

.errorState {
  border: none;
  border-bottom: 1px solid red;
  background-color: transparent;
  resize: none;
  outline: none;
  opacity: 0.7;
}

.errorState::placeholder {
  color: red;
}

textarea:focus {
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
    form: {
      type: String,
    },
    placeHolder: {
      type: String,
    },
    name: {
      type: String,
    },
  },

  methods: {
    textAreaClicked() {
      var currentState = this.state;
      if (currentState == "errorState") {
        currentState = "normalState";
      }
      this.$emit("update-state", currentState);
    },
  },
};
</script>