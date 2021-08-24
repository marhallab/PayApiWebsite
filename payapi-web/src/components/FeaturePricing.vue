<template>
  <div class="feature">
    <img
      :style="[isOffered ? {} : { display: 'none' }]"
      src="../assets/shared/desktop/icon-check.svg"
      alt=""
    />
    <p :style="[isOffered ? {} : { opacity: '0.7', 'margin-left': '-65%' }]">
      {{ featureName }}
    </p>
  </div>
</template>

<style scoped>
.feature {
  margin-top: 5%;
  margin-bottom: 5%;
}

p {
  display: inline;
  margin-left: -70%;
}
img {
  float: left;
  margin-top: 1%;
  width: 5%;
}
</style>

<script>
export default {
  props: {
    isOffered: {
      type: Boolean,
      required: true,
    },
    featureName: {
      type: String,
      default: "Test",
    },
  },
};
</script>