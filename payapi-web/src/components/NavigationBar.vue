<template>
  <div class="nav">
    <div class="nav-bar">
      <div id="nav-links">
        <router-link to="/home"
          ><img src="../assets/shared/desktop/logo.svg" alt=""
        /></router-link>

        <div class="router-links">
          <router-link to="/pricing">Pricing</router-link>
          <router-link to="/about">About</router-link>
          <router-link to="/contact">Contact</router-link>
        </div>
      </div>

      <div class="sidebar">
        <b-button v-b-toggle.sidebar-right variant="transparent">
          <img src="../assets/shared/mobile/menu.svg" alt="" />
        </b-button>

        <b-sidebar
          id="sidebar-right"
          bg-variant="dark"
          text-variant="light"
          right
          no-header
        >
          <template #default="{ toggle }">

            <b-button
              v-b-toggle.sidebar-right
              variant="transparent"
              @click="toggle"
              class="closeSidebarBtn"
            >
              <img src="../assets/shared/mobile/close.svg" alt="" />
            </b-button>

            <hr width="80%" />

            <div class="px-3 py-3">

              <div class="router-links-sidebar">
                <router-link to="/pricing">Pricing</router-link>
                <router-link to="/about">About</router-link>
                <router-link to="/contact">Contact</router-link>
              </div>

              <form id="form-nav-sidebar" action="./contact">
                <primaryBtn
                  :form="'form-nav-sidebar'"
                  :isDisabled="false"
                  :btnText="'Schedule a Demo'"
                />
              </form>

            </div>
          </template>
        </b-sidebar>
      </div>

      <form id="form-nav" action="./contact">
        <primaryBtn
          :form="'form-nav'"
          :isDisabled="false"
          :btnText="'Schedule a Demo'"
        />
      </form>
    </div>
  </div>
</template>

<style scoped>
.nav {
  z-index: 3;
  padding-top: 4%;
  padding-left: 10%;
  padding-right: 10%;
}

.nav-bar {
  display: flex;
  justify-content: space-between;
  width: 100%;
  z-index: 3;
}

.sidebar {
  display: none;
}

#nav-links {
  display: flex;
  width: 500px;
}

.router-links {
  margin: auto;
  margin-top: 10px;
  display: flex;
  justify-content: space-evenly;
  width: 50%;
}

.router-links a {
  font-family: Public Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  line-height: 18px;
  color: #36536b;
  mix-blend-mode: normal;
  opacity: 0.7;
}

.router-links a:hover {
  opacity: 1;
}

@media only screen and (max-width: 500px) {
  .sidebar {
    display: block;
  }

  .router-links {
    display: none;
  }

  #form-nav {
    display: none;
  }

  .closeSidebarBtn {
    padding-top: 7%;
    margin-left: 50%;
  }

  hr {
    margin: auto;
    margin-top: 5%;
  }

  .router-links-sidebar {
    margin: auto;
    margin-top: 10px;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    width: 50%;
    height: 200px;
  }

  .router-links-sidebar a {
    font-family: Public Sans;
    font-style: normal;
    font-weight: bold;
    font-size: 20px;
    line-height: 18px;
    color: #fbfcfe;
    mix-blend-mode: normal;
    opacity: 0.7;
  }

  .router-links-sidebar a:hover {
    opacity: 1;
  }

  #sidebar-right{
    
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
