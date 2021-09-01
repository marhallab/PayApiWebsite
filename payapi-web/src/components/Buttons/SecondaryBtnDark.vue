<template>
  <div>
    <input :form="form" type="submit" :disabled="isDisabled" :value="btnText" />
  </div>
</template>

<style scoped>
input {
  background: Transparent;
  border-radius: 25px;
  border: 1px solid #36536b;

  padding-left: 25px;
  padding-right: 25px;

  padding-top: 10px;
  padding-bottom: 10px;

  font-family: Public Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  color: #36536b;

  z-index: 3;
}

input:hover {
  background: #36536b;
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