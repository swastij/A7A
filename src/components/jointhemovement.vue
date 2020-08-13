<template>
  <div class="jtm-container">
    <div class="left">
      <p>Join The Movement</p>
      <p>
        Get first month free for commercial use. Forever free for open source
        products.
      </p>
    </div>
    <div class="right">
      <input type="text" placeholder="Email Address" />
      <div>
        <p>Get Started</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.jtm-container {
  width: 100%;
  max-width: 100%;
  background: #1c1c1c;
  border-radius: 20px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin-top: 145px;
  box-sizing: border-box;
  padding: 2% 0%;
}
.left {
  width: 40%;
  max-width: 40%;
}
.left > p:nth-child(1) {
  font-style: normal;
  font-weight: normal;
  font-size: 49px;
  line-height: 61px;
  color: #dfdfdf;
}
.left > p:nth-child(2) {
  font-style: normal;
  font-weight: normal;
  font-size: 30px;
  line-height: 40px;
  color: rgba(223, 223, 223, 0.5);
}
.right {
  width: 40%;
  max-width: 40%;
  height: 48px;
  display: flex;
}
.right > input {
  width: 70%;
  height: 100%;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 20px;
  border: none;
  color: #dfdfdf;
  background: #383838;
  border-radius: 10px 0px 0px 10px;
  box-sizing: border-box;
  padding: 0% 2%;
}
.right > div {
  height: 100%;
  width: 30%;
  max-width: 30%;
  font-family: Muli;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 20px;
  text-align: center;
  color: #dfdfdf;
  background: #5c4ccc;
  border-radius: 0px 10px 10px 0px;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
}
@media screen and (max-width: 786px) {
  .jtm-container {
    margin-top: 598px;
    flex-wrap: wrap;
  }
  .left {
    width: 100%;
    max-width: 100%;
    margin: 2%;
  }
  .right {
    width: 100%;
    max-width: 100%;
    margin: 2%;
  }
  .left > p:nth-child(1) {
    font-size: 39px;
    line-height: 51px;
  }
  .left > p:nth-child(2) {
    font-size: 20px;
    line-height: 30px;
  }
}
@media screen and (max-width: 576px) {
.left > p:nth-child(1) {
    font-size: 28px;
    line-height: 41px;
  }
  .left > p:nth-child(2) {
    font-size: 14px;
    line-height: 20px;
  }
}
</style>
