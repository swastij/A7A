<template>
  <div class="navbar-box">
    <div class="left-item">
      <img src="../assets/svg/A7A.svg" />
      <p>CREATE.INSPIRE.</p>
    </div>
    <div class="right-item">
      <p>HOME</p>
      <p>ABOUT</p>
      <P>PRODUCTS</P>
      <P>CONTACT</P>
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
  left:0;
  width: 100%;
  height: 74px;
  display: flex;
  justify-content: space-between;
  background: rgba(10, 10, 10, 0.3);
box-shadow: inset 0px 4px 10px rgba(0, 0, 0, 0.25);
z-index: 10;
color: #DFDFDF;
}
.left-item {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
  width: 40%;
  height: 100%;
}
.left-item > img{
    height:50%;
}
.right-item {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
  width: 60%;
  height: 100%;
}
</style>
