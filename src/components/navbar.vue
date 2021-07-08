<template>
  <div class="navbar-box">
    <div v-if="isDrawerVisible" class="nav-drawer">
      <p>HOME</p>
      <p>ABOUT</p>
      <P>PRODUCTS</P>
      <P>CONTACT</P>
    </div>
    <div class="nav-row">
      <div class="left-item">
        <img src="../assets/svg/A7A.svg" />
        <!-- <p>CREATE.INSPIRE.</p> -->
      </div>
      <div class="right-item">
        <p>HOME</p>
        <p>ABOUT</p>
        <P>PRODUCTS</P>
        <P>CONTACT</P>
      </div>
      <div class="mobile">
        <div @click="toggleNavdrawer">
          <div ref="hamOne"></div>
          <div ref="hamTwo"></div>
          <div ref="hamThree"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isDrawerVisible: false,
    };
  },
  methods: {
    toggleNavdrawer() {
      this.isDrawerVisible = !this.isDrawerVisible;
      if (this.isDrawerVisible) {
        this.$refs.hamTwo.style.display = "none";
        this.$refs.hamOne.style.transform = "rotateZ(45deg)";
        this.$refs.hamThree.style.transform = "rotateZ(-45deg)";
        this.$refs.hamOne.style.transformOrigin = '50% -100%'
        this.$refs.hamThree.style.transformOrigin = '10% 10%'

      } else {
        this.$refs.hamTwo.style.display = "block";
        this.$refs.hamOne.style.transform = "rotateZ(0deg)";
        this.$refs.hamThree.style.transform = "rotateZ(0deg)";
      }
    },
  },
};
</script>

<style>
.navbar-box {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 74px;
  backdrop-filter: blur(6px);
  background-color: rgba(0, 0, 0, 0.6);
  box-shadow: inset 0px 4px 10px rgba(0, 0, 0, 0.25);
  z-index: 10;
  color: #dfdfdf;
}
.nav-drawer {
  height: 100vh;
  width: 100%;
  background-color: #040404;
  margin-top: 75px;
  position: fixed;
  left: 0;
  display:flex;
  text-align: center;
  flex-direction: column;
  justify-content: center;
  align-item: center;
}
.nav-drawer >p {
  font-size: 44px;
  margin-bottom: 5%;
}
.nav-row {
  max-width: 87%;
  display: flex;
  justify-content: space-between;
  margin: auto;
  height: 100%;
}
.left-item {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: flex-start;
  width: 60%;
  height: 100%;
}
.left-item > img {
  height: 60%;
}
.right-item {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  width: 40%;
  height: 100%;
  transition: 0.4s;
}
.mobile {
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  width: 40%;
  height: 100%;
  transition: 0.4s;
  display: none;
}
.mobile > div{
  cursor: pointer;
}

.mobile > div > div {
  height: 2px;
  width: 30px;
  background-color: azure;
  margin-top: 5px;
  margin-bottom: 5px;
  transition: .4s;
}

/* .ham-three {
  transform: rotateZ(-45deg);
}

.ham-one {
  transform: rotateZ(-45deg);
} */

@media screen and (max-width: 890px) {
  .left-item {
    width: 30%;
  }
  .right-item {
    width: 70%;
  }
}

@media screen and (max-width: 700px) {
  .right-item {
    display: none !important;
  }

  .mobile {
    display: flex !important;
  }
  .nav-row {
    max-width: 90%;
  }
  .nav-drawer >p {
  font-size: 24px;
  margin-bottom:15%;
}
}
</style>
