<template>
  <div class="feature">
    <img
      :style="[isOffered ? {} : { display: 'none' }]"
      src="../assets/shared/desktop/icon-check.svg"
      alt=""
    />
    <p :style="[isOffered ? {} : { opacity: '0.7'}]">
      {{ featureName }}
    </p>
  </div>
</template>

<style scoped>
.feature {
  margin-top: 5%;
  margin-bottom: 5%;
  display: flex;

}

p {
  text-align: left;
  margin-left: 10%;
}
img {
  margin-top: 5px;
  height: 15px;
  width: 15px;
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