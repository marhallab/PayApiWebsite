<template>
  <div class="contact">
    <section class="section1">
      <img
        class="img-circle-section1"
        src="../assets/shared/desktop/bg-pattern-circle.svg"
        alt=""
      />

      <p class="title-section1">
        Submit a help request and we’ll get in touch shortly.
      </p>
    </section>
  </div>
</template>

<style scoped>
.contact {
  width: 100%;
  height: 100%;
}

p {
  text-align: start;
  margin: 10px;
  line-height: 175%;
}

.title-text {
  display: flex;
  width: 100%;
  margin-top: 5%;
}

/*Section 1*/
.section1 {
  padding-left: 10%;
  padding-right: 10%;
  padding-top: 5%;
}

.title-section1 {
  font-family: DM Serif Display;
  font-style: normal;
  font-weight: bold;
  font-size: 56px;
  line-height: 56px;
  color: #36536b;
  width: 80%;
}

.img-circle-section1 {
  position: absolute;
  top: -600px;
  right: -200px;
}
</style>