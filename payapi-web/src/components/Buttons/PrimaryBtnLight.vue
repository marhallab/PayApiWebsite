<template>
  <div>
    <input :form="form" type="submit" :disabled="isDisabled" :value="btnText" />
  </div>
</template>

<style scoped>
input {
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

input:hover {
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
    form: {
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