<template>
  <div class="footer-container">
    <div class="footer-row">
      <div class="left-footer">
        <img src="../assets/svg/A7A.svg" />
      </div>
      <div class="right-footer">
        <div class="right-footer-box">
          <h3>Contact</h3>
          <p>Email: a7aent@gmail.com</p>
          <p>Phone: +917015100483</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.footer-container {
  position: absolute;
  left: 0;
  margin-top: 273px;
  padding: 1.5%;
  box-sizing: border-box;
  width: 100%;
  max-width: 100%;
  background: #1c1c1c;
}
.footer-row {
  display: flex;
  justify-content: space-around;
  align-items: center;
  max-width: 85%;
  margin: auto;
}
.left-footer {
  width: 40%;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 32px;
  color: #dfdfdf;
}
.left-footer > img {
  width: 50%;
  margin-bottom: 5%;
}
.right-footer {
  width: 55%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}
.right-footer-box {
  width: 100%;
}
.right-footer-box > h3 {
  font-style: normal;
  font-weight: normal;
  font-size: 33px;
  line-height: 41px;
  text-align: center;
  color: #dfdfdf;
}
.right-footer-box > p {
  font-style: normal;
  font-weight: normal;
  font-size: 26px;
  line-height: 33px;
  text-align: center;
  cursor: pointer;
  color: rgba(223, 223, 223, 0.5);
}
@media screen and (max-width: 996px) {
  .left-footer {
    display: none;
    width: 0;
  }
  .right-footer {
    width: 100%;
    flex-wrap: wrap;
    justify-content: center;
  }
  .right-footer-box {
    width: 50%;
    align-items: flex-start !important;
    text-align: left !important;
  }
  .right-footer-box > h3 {
    font-size: 24px;
    line-height: 31px;
    text-align: left !important;
  }
  .right-footer-box > p {
    font-size: 20px;
    line-height: 30px;
    text-align: left !important;
  }
  .bottom {
    width: 100% !important;
    margin-top: 16px;
  }
  .footer-container {
    margin-top: 140px;
  }
}
@media screen and (max-width: 576px) {
  .right-footer-box > h3 {
    font-size: 20px;
    line-height: 28px;
  }
  .right-footer-box > p {
    font-size: 14px;
    line-height: 28px;
  }
}
</style>
