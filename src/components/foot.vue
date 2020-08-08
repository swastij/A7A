<template>
  <div class="footer-container">
    <div class="footer-row">
    <div class="left-footer">
      <img src="../assets/svg/A7A.svg" />
      <p>
        Outa voluptate et optio. Eos quasi impedit sapiente aliquid eius
        eligendi at. Necessitatibus magni et sed quod quas minima.
      </p>
    </div>
    <div class="right-footer">
      <div class="right-footer-box">
        <h3>Company</h3>
        <p>About us</p>
        <p>Jobs</p>
        <p>Contact</p>
        <p>Media</p>
      </div>
      <div class="right-footer-box">
        <h3>Product</h3>
        <p>About us</p>
        <p>Jobs</p>
        <p>Contact</p>
        <p>Media</p>
      </div>
      <div class="right-footer-box">
        <h3>Support</h3>
        <p>About us</p>
        <p>Jobs</p>
        <p>Contact</p>
        <p>Media</p>
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
  max-width: 80%;
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
  width: 30%;
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

  color: rgba(223, 223, 223, 0.5);
}
</style>
