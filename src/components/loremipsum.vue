<template>
  <div class="li-container">
    <div class="li-container-relative">
      <img src="../assets/svg/loremipsum.svg" />
      <div class="li-arrow-text">
        <div class="left-circle-box">
          <div class="arrow-circle">
            <img src="../assets/svg/leftarrow.svg" />
          </div>
        </div>
        <div class="text">
          <p>Lorem ipsum</p>
          <p>Row Row Row your boat gently down the stream</p>
        </div>
        <div class="right-circle-box">
          <div class="arrow-circle">
            <img src="../assets/svg/rightarrow.svg" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.li-container {
  position: absolute;
  left: 0;
  text-align: center;
  margin-top: 505px;
  width: 100%;
  max-width: 100%;
}
.li-container-relative {
  position: relative;
  display: flex;
  align-items: center;
}
.li-container-relative > img {
  width: 100%;
  position: absolute;
  left: 0;
}
.li-arrow-text {
  width: 100%;
  max-width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  text-align: center;
  position: absolute;
}
.left-circle-box {
  width: 10%;
  max-width: 10%;
}
.right-circle-box {
  width: 10%;
  max-width: 10%;
  display: flex;
  justify-content: flex-end;
}
.arrow-circle {
  height: 80px;
  width: 80px;
  /* max-width: 10%; */
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50%;
  background: rgba(17, 17, 17, 0.8);
  filter: blur(0.5px);
  text-align: center;
}
.text {
  width: 70%;
  max-width: 70%;
  color: #dfdfdf;
}
.text > p:nth-child(1) {
  font-style: normal;
  font-weight: normal;
  font-size: 153px;
  line-height: 192px;
  text-align: center;
}
.text > p:nth-child(2) {
  font-style: normal;
  font-weight: bold;
  font-size: 35px;
  line-height: 44px;
  text-align: center;
}
@media screen and (max-width:786px) {
  .li-container{
    margin-top:300px;
  }
.text > p:nth-child(1) {
  font-size: 80px;
  line-height: 122px;
}
.text > p:nth-child(2) {
  font-size: 24px;
  line-height: 34px;
}
.left-circle-box {
  width: 10%;
  max-width: 10%;
}
.right-circle-box {
  width: 10%;
  max-width: 10%;
}
.arrow-circle{
  height: 60px;
  width: 60px;
}
}
@media screen and (max-width:576px) {
.text > p:nth-child(1) {
  font-size: 58px;
  line-height: 108px;
}
.text > p:nth-child(2) {
  font-size: 20px;
  line-height: 28px;
}
.arrow-circle{
  height: 40px;
  width: 40px;
}
}
</style>
