<template>
  <div class="take-action">
    <p>take action now</p>
    <p>your search for finding products are over</p>
  </div>
</template>

<script>
export default {};
</script>

<style>
.take-action {
  margin-top: 430px;
}
.take-action > p:nth-child(1) {
  font-style: normal;
  font-weight: normal;
  font-size: 71px;
  line-height: 89px;
  text-align: center;
  text-transform: capitalize;
  color: #dfdfdf;
}
.take-action > p:nth-child(2) {
  font-style: normal;
  font-weight: normal;
  font-size: 25px;
  line-height: 31px;
  text-align: center;
  text-transform: uppercase;
  color: #dfdfdf;
}
@media screen and (max-width: 786px) {
  .take-action{
    margin-top: 180px ;
  }
  .take-action > p:nth-child(1) {
    font-size: 51px;
  line-height: 69px;
  }
  .take-action > p:nth-child(2) {
    font-size: 18px;
    line-height: 35px;
  text-transform: capitalize;

  }

}
@media screen and (max-width: 576px) {
  .aboutus-box{
    margin-top: 130px;
  }
  .take-action > p:nth-child(1) {
    font-size: 41px;
  line-height: 49px;
  }
  .take-action > p:nth-child(2) {
    font-size: 14px;
    line-height: 25px;
  }
}
</style>
