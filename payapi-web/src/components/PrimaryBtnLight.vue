<template>
  <button :disabled="isDisabled">{{ btnText }}</button>
</template>

<style scoped>
button {
  background: #ba4270;
  border-radius: 25px;
  border: 0 solid;

  padding-left: 25px;
  padding-right: 25px;
  padding-top: 15px;
  padding-bottom: 15px;

  font-family: Public Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  color: #fbfcfe;

  z-index: 3;
}

button:hover {
  opacity: 0.7;
}
</style>

<script>
export default {
  props: {
    isDisabled: {
      type: Boolean,
      default: false,
    },
    btnText: {
      type: String,
    },
  },

  methods: {
    test() {
      alert("YES");
    },
  },
};
</script>