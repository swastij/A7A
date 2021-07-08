<template>
  <div class="feature-box-container">
    <div class="feature-box">
      <div class="circle">
        <div class="icon">
          A
        </div>
      </div>
      <p>Mobile Development</p>
      <p>
        Delivering mobile apps to help bring your organization's ideas to
        reality across all types of iOS and Android devices.
      </p>
      <div class="read-more">Read More</div>
    </div>
    <div class="feature-box">
      <div class="circle">
        <div class="icon">
          7
        </div>
      </div>
      <p>Maintenance and support</p>
      <p>
        Focus on growing your business and let the experts keep your tools up
        and running.
      </p>
      <div class="read-more">Read More</div>
    </div>
    <div class="feature-box">
      <div class="circle">
        <div class="icon">
          A
        </div>
      </div>
      <p>Infrastructure management</p>
      <p>
        Secure and reliable IT infrastructures give businesses the ability to
        achieve continuous growth and sustainability.
      </p>
      <div class="read-more">Read More</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.feature-box-container {
  width: 100%;
  max-width: 100%;
  margin-top: 99px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.feature-box {
  box-sizing: border-box;
  max-width: 30%;
  width: 30%;
  height: 600px;
  background: rgba(16, 16, 16, 0.32);
  border: 1px solid #181818;
  backdrop-filter: blur(20px);
  border-radius: 24px;
  padding: 4%;
}
.feature-box > p:nth-of-type(odd) {
  font-style: normal;
  font-weight: normal;
  font-size: 36px;
  line-height: 36px;
  margin-top: 44px;
  color: #dfdfdf;
}
.feature-box > p:nth-of-type(even) {
  font-style: normal;
  font-weight: normal;
  font-size: 20px;
  line-height: 30px;
  margin-top: 24px;
  text-transform: capitalize;
  color: #dfdfdf;
}
.circle {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 84px 0;
}
.icon {
  width: 120px;
  height: 120px;
  background-color: #fff;
  border-radius: 50%;
  color: black;
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 56px;
}
.read-more {
  background: #222222;
  border: 1px solid #333333;
  box-sizing: border-box;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 5px;
  margin: 40px 40px 40px 0;
  height: 40px;
  padding: 2%;
  font-style: normal;
  font-weight: normal;
  font-size: 18px;
  line-height: 21px;
  text-align: center;
  color: #cdcdcd;
  max-width: 60%;
  cursor: pointer;
}
@media screen and (max-width: 900px) {
  
}
@media screen and (max-width: 1096px) {
  .feature-box-container {
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
  }
  .feature-box {
    width: 100%;
    max-width: 100%;
    margin-top: 24px;
    height: 500px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 20px;
  }
  .feature-box > p:nth-of-type(odd) {
    font-size: 28px;
    line-height: 36px;
  }
  .feature-box > p:nth-of-type(even) {
    font-size: 20px;
    line-height: 28px;
    text-transform: capitalize;
  }
  .read-more {
    max-width: 80%;
  }
}
@media screen and (max-width: 576px) {
  .feature-box > p:nth-of-type(odd) {
    font-size: 20px;
    line-height: 28px;
  }
  .feature-box > p:nth-of-type(even) {
    font-size: 14px;
    line-height: 20px;
  }
  .read-more {
    max-width: 50%;
  }
}
</style>
