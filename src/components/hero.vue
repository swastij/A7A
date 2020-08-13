<template>
  <div class="hero-box">
    <div class="a7a">
      <img src="../assets/svg/A7A.svg" />
      <p>CREATE. INSPIRE.</p>
    </div>
    <div class="hero-image">
      <img src="https://64.media.tumblr.com/d106208fa90288473bdd3e68d2d0672c/tumblr_opmbvl4qwR1tjryj4o1_540.gifv" >
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.hero-box {
  width: 100%;
  max-width: 100%;
  height: 90vh;
  display: flex;
  align-items: center;
}
.a7a {
  width: 50%;
  max-width: 50%;
  font-style: normal;
  font-weight: normal;
  font-size: 44px;
  line-height: 55px;

  color: #dfdfdf;
}
.hero-image{
  display: flex;
  justify-content: flex-end;
  width:50%;
}
.hero-image > img{
 width:80%;
  /* height: 60%; */
}
/* @media screen and (max-width:1072px){
  .hero-box{
    width:50%;
  } */
/* } */
@media screen and (max-width: 786px) {
  .hero-box{
    height:auto;
    margin-top:65px;
    flex-wrap:wrap;
    align-items: center;
    justify-content: space-around;
  }
  .a7a{
    width: 100%;
    text-align: center;
    order: 2;
  }
  .hero-image{
    justify-content: center;
    width: 100%;
    order: 1;
    margin-bottom: 5%;
  }
  .hero-image > img{
    width:50%;
  }
    .a7a>img{
         width:50%; 
    }
    .a7a>p{
        font-size:36px;
    }
}
@media screen and (max-width: 576px) {
  .a7a>img{
         width:40%; 
    }
    .a7a>p{
        font-size:24px;
    }
}
</style>
