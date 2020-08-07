<template>
  <div class="feature-box-container">
    <div class="feature-box">
      <div class="circle">
          <img src="../assets/svg/circle.svg" >
      </div>
      <p>Feature 1</p>
      <p>
       WE DESIGN AND DEVELOP WEBSITES, WEB SHOPS, MOBILE APPS, DIGITAL CAMPAIGNS, SYSTEM INTEGRATIONS AND CUSTOMIZED SOFTWARE OF THE HIGHEST LEVEL.
      </p>
      <div class="read-more">Read More</div>
    </div>
    <div class="feature-box">
      <div class="circle">
          <img src="../assets/svg/circle.svg" >
      </div>
      <p>Feature 2</p>
      <p>
       WE DESIGN AND DEVELOP WEBSITES, WEB SHOPS, MOBILE APPS, DIGITAL CAMPAIGNS, SYSTEM INTEGRATIONS AND CUSTOMIZED SOFTWARE OF THE HIGHEST LEVEL.
      </p>
      <div class="read-more">Read More</div>
    </div>
    <div class="feature-box">
      <div class="circle">
          <img src="../assets/svg/circle.svg" >
      </div>
      <p>Feature 3</p>
      <p>
        WE DESIGN AND DEVELOP WEBSITES, WEB SHOPS, MOBILE APPS, DIGITAL CAMPAIGNS, SYSTEM INTEGRATIONS AND CUSTOMIZED SOFTWARE OF THE HIGHEST LEVEL.
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
  line-height: 42px;
  margin:4% 0%;
  color: #dfdfdf;
}
.feature-box > p:nth-of-type(even) {
  font-style: normal;
  font-weight: normal;
  font-size: 28px;
  line-height: 33px;

  color: #dfdfdf;
}
.read-more{
    background: #222222;
border: 1px solid #333333;
box-sizing: border-box;
border-radius: 5px;
margin:4% 4% 4% 0%;
padding:2%;
font-style: normal;
font-weight: normal;
font-size: 18px;
line-height: 21px;
text-align: center;
color: #CDCDCD;
max-width:40%;
width:40%;
}
</style>
