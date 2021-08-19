<template>
  <div class="FooterEmail">
    <p><b>Ready to start?</b></p>

    <div class="input-btn">
      <input type="text" placeholder="Enter email address" />
      <primaryBtn :btnText="'Schedule a Demo'" />
    </div>
  </div>
</template>

<style scoped>
.FooterEmail {
  display: flex;
  justify-content: space-between;
  margin-top: 5%;
  margin-bottom: 4%;
  padding-left: 13%;
  padding-right: 13%;
}
.input-btn {
  display: flex;
  flex-direction: row;
  height: 50px;
  width: 60%;
  margin-top: 6%;
}

.input-btn input {
  width: 40%;
  margin-left: 13% ;
  margin-right: -7%;
  padding-left: 5%;
  padding-right: 15%;
  border: none;
  outline: none;
  border-radius: 25px;
  box-shadow: 0 3px 5px rgb(0 0 0 / 0.2);
}

p {
font-family: DM Serif Display;
font-style: normal;
font-weight: normal;
font-size: 50px;
letter-spacing: -0.369231px;
color: #36536B;
}
</style>


<script>
import primaryBtn from "./PrimaryBtnLight.vue";

export default {
  components: {
    primaryBtn,
  },
};
</script>