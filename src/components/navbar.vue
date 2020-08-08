<template>
  <div class="navbar-box">
    <div class="nav-row">
      <div class="left-item">
        <div
          style="display: flex; flex-direction: column; align-items: center; justify-content: center"
        >
          <img src="../assets/svg/A7A.svg" />
          <p>CREATE.INSPIRE.</p>
        </div>
      </div>
      <div class="right-item">
        <p>HOME</p>
        <p>ABOUT</p>
        <P>PRODUCTS</P>
        <P>CONTACT</P>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.navbar-box {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 74px;
  backdrop-filter: blur(10px) opacity(0.4);
  box-shadow: inset 0px 4px 10px rgba(0, 0, 0, 0.25);
  z-index: 10;
  color: #dfdfdf;
}
.nav-row {
  max-width: 85%;
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
.left-item > div > img {
  height: 25%;
}
.right-item {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
  width: 40%;
  height: 100%;
}
</style>
