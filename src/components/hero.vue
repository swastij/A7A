<template>
  <div class="hero-box">
    <div class="a7a">
      <img src="../assets/svg/A7A.svg" />
      <p>CREATE. INSPIRE.</p>
    </div>
    <div class="hero-image">
      <img src="" >
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
  font-style: normal;
  font-weight: normal;
  font-size: 44px;
  line-height: 55px;

  color: #dfdfdf;
}
.hero-image{
  background:grey;
  width:50%;
  height: 80%;
}
@media screen and (max-width: 786px) {
  .hero-box{
    height:auto;
    margin-top:75px;
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
    width: 100%;
    order: 1;
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
