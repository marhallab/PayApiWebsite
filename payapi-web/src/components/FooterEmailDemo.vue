<template>
  <div class="FooterEmail">
    <p>Ready to start?</p>

    <form
      class="input-btn"
      action="mailto:rhallab.dev@gmail.com"
      id="form-nav"
      method="post"
      enctype="text/plain"
    >
      <input name="Email" type="email" placeholder="Enter email address" />
      <primaryBtn :form="'form-nav'" :btnText="'Schedule a Demo'" />
    </form>
  </div>
</template>

<style scoped>
.FooterEmail {
  display: flex;
  justify-content: space-between;
  margin-top: 5%;
  margin-bottom: 4%;
  padding-left: 3%;
  width: 100%;
}
.input-btn {
  display: flex;
  flex-direction: row;
  height: 50px;
  width: 100%;
  padding-right: 10%;
  margin-top: 1%;
}

.input-btn input {
  width: 60%;
  margin-left: 13%;
  margin-right: -10%;
  padding-left: 6%;
  padding-right: 15%;
  border: none;
  outline: none;
  border-radius: 25px;
  box-shadow: 0 3px 5px rgb(0 0 0 / 0.2);
}

p {
  font-family: DM Serif Display;
  font-style: normal;
  font-weight: bold;
  font-size: 45px;
  color: #36536b;
  width: 100%;
}

@media only screen and (max-width:1024px) {
  .FooterEmail {
    flex-direction: column;
    margin-bottom: 10%;
    margin-top: 7%;
  }

  .input-btn input {
  margin-left: 17%;
}
}
</style>


<script>
import primaryBtn from "./Buttons/PrimaryBtnLight.vue";

export default {
  components: {
    primaryBtn,
  },
};
</script>