<template>
  <button :disabled="isDisabled"> <router-link to="/about"> {{ btnText }}</router-link></button>
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

  z-index: 3;
}

a{
   color: #fbfcfe;
}

button:hover {
  background: #fbfcfe;
}

button:hover a{
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

  methods: {
    test() {
      alert("YES");
    },
  },
};
</script>