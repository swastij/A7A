<template>
  <div class="aboutus-box">
    <div class="aboutus-text">
      <h3>About Us</h3>
      <p>
        We design and develop websites, web shops, mobile apps, digital
        campaigns, system integrations and customized software of the highest
        level.
      </p>
      <p />
      <br />
      <p>
        Designs that are meticulously thought out to the pixel and are of this
        time. Today's software, ready for tomorrow's technology.
      </p>
    </div>
    <div class="image">
      <img src="https://i.pinimg.com/originals/e8/4b/ab/e84babd42e49b0c879536315d30788ed.gif" >
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.aboutus-box {
  width: 100%;
  max-width: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin-top: 252px;
}
.aboutus-text {
  width: 50%;
}
.aboutus-text > h3 {
  font-style: normal;
  font-weight: normal;
  font-size: 89px;
  line-height: 112px;
  color: #bebebe;
}
.aboutus-text > p {
  font-style: normal;
  font-weight: normal;
  font-size: 36px;
  line-height: 45px;
  display: flex;
  align-items: center;

  color: #bebebe;
}
.image {
  width: 50%;
  display: flex;
  justify-content: flex-end;
}
.image > img{
    width:100%;
  }
@media screen and (max-width: 786px) {

  .aboutus-box{
    margin-top: 120px;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    flex-direction: row-reverse;
  }
  .aboutus-text{
    order:2;
  }
  .image{
    order:1;
    width: 100%;
    justify-content: center;
  }
  .image > img{
    width:80%;
  }
  .aboutus-text{
    width:100%;
  }
  
  .aboutus-text > h3 {
    font-size: 69px;
    text-align: center;
  }
  .aboutus-text > p {
    font-size: 24px;
    line-height: 35px;
  }

}
@media screen and (max-width: 576px) {
  .aboutus-box{
    margin-top: 90px;
  }
  
  .aboutus-text > h3 {
    font-size: 39px;
    text-align: center;

  }
  .aboutus-text > p {
    font-size: 14px;
    line-height: 25px;
  }
  .image > img{
    width:100%;
  }
}
</style>
