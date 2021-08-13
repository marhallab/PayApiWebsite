<template>
  <button :disabled="isDisabled">{{ btnText }}</button>
</template>

<style scoped>
button {
  background: #fbfcfe;
  border-radius: 25px;
  border: 0 solid #36536B;

  padding-left: 25px;
  padding-right: 25px;

  font-family: Public Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  color: #36536B;

  z-index: 3;
}

button:hover {
  background: #36536B;
  color: #fbfcfe;
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