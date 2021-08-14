<template>
  <button :disabled="isDisabled">{{ btnText }}</button>
</template>

<style scoped>
button {
  background: #1b262f;
  border-radius: 25px;
  border: solid #fbfcfe;

  padding-left: 25px;
  padding-right: 25px;

  font-family: Public Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  color: #fbfcfe;

  z-index: 3;
}

button:hover {
  background: #fbfcfe;
  color: #1b262f;
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

  computed: {},

  methods: {
    test() {
      alert("YES");
    },
  },
};
</script>