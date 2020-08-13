<template>
  <div class="review-container">
    <div ref="reviewRow" class="review-row">
      <div class="review-item-container">
      <div class="review-item" v-for="(review, key) in reviews" :key="key">
        <div>
          {{ key }}
        </div>
        
        <div class="inverted-comma">
          "
        </div>
        <div class="review-text"> {{review.review}}
        <div>
          <div class="review-pic">
           <img src={review.pic}>
          </div>
          <div class="review-name">{{review.name}}</div>
          <div class="review-about">{{review.about}}</div>
          </div>
        </div>
      </div>
    </div>
    </div>
    <div class="review-dots-container">
      <div
        @click="scroll(key)"
        :class="activeReview == key ? 'review-dot-active' : 'review-dot'"
        v-for="(review, key) in reviews"
        :key="key"
      ></div>
    </div>
  </div>
 
</template>

<script>
export default {
  data() {
    return {
      reviews: [
        {
          name: "Test",
          review: "review",
          about: "about",
          pic: "../assets/svg/reviewpic.svg"
        },
        {
          name: "Test",
          review: "review",
          about: "about",
          pic: "pic",
        },
        {
          name: "Test",
          review: "review",
          about: "about",
          pic: "pic",
        },
        {
          name: "Test",
          review: "review",
          about: "about",
          pic: "pic",
        },
      ],
      activeReview: 0,
      prevReview: 0,
    };
  },
  methods: {
    scroll(key) {
      this.activeReview = key;
      if (this.activeReview == this.prevReview) {
        this.$refs.reviewRow.scrollLeft += 666;
        this.prevReview = this.activeReview;
      } else if (this.activeReview > this.prevReview) {
        this.$refs.reviewRow.scrollLeft += 666;
        this.prevReview = this.activeReview;
      } else {
        this.$refs.reviewRow.scrollLeft -= 666;
        this.prevReview = this.activeReview;
      }
    },
  },
};
</script>

<style scoped>
.review-container {
  width: 100%;
  margin-top: 1000px;
}
.review-row {
  width: 100%;
  overflow-x: auto;
  white-space: nowrap;
  scroll-behavior: smooth;
}

.review-row::-webkit-scrollbar {
  width: 5px;
  display: none;
}
.review-row::-webkit-scrollbar-track {
  background: #1c1c1c;
}
.review-row::-webkit-scrollbar-thumb {
  background-color: #585757;
  border-radius: 10px;
}

.review-item {
  background: #1c1c1c;
  border-radius: 10px;
  width: 40%;
  min-width: 300px;
  height: 200px;
  display: inline-block;
  margin-right: 20px;
  color: #fff;
}

.review-dots-container {
  display: flex;
  justify-content: center;
  width: 100%;
  margin-top: 20px;
}

.review-dot {
  height: 8px;
  width: 8px;
  background: rgba(223, 223, 223, 0.5);
  border-radius: 50%;
  margin-left: 2px;
  margin-right: 2px;
  transition: 0.4s;
  cursor: pointer;
}

.review-dot-active {
  height: 8px;
  width: 16px;
  background: rgba(223, 223, 223, 0.5);
  border-radius: 20px;
  margin-left: 2px;
  margin-right: 2px;
  transition: 0.4s;
}
.review-item-container{
  display:flex;
  justify-content: center;
  align-items: flex-start;
}
.inverted-comma{
  font-family: Muli;
font-style: italic;
font-weight: normal;
font-size: 46px;
line-height: 108px;
color: #DFDFDF;
width: 100%;
}

.review-text{
  ont-family: Muli;
font-style: italic;
font-weight: normal;
font-size: 18px;
line-height: 23px;
width: 100%;
height:20%;
color: #DFDFDF;
}
.review-pic{
border: 1px solid rgba(223, 223, 223, 0.5);
box-sizing: border-box;

}
.review-name{
ont-style: normal;
font-weight: normal;
font-size: 12px;
line-height: 15px;

color: #DFDFDF;

}
.review-about{
font-family: Muli;
font-style: normal;
font-weight: normal;
font-size: 11px;
line-height: 14px;

color: rgba(223, 223, 223, 0.5);

}
@media screen and (max-width:786px){
  .review-container{
    display:flex;
    flex-wrap: wrap;
  }
  .review-item{
    width:100%;
  }
}
@media screen and (max-width: 576px){
  
}
</style>
