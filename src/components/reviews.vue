<template>
  <div class="review-container">
    <div ref="reviewRow" class="review-row">
      <div class="review-item-container">
        <div class="review-item" v-for="(review, key) in reviews" :key="key">
          <div class="inverted-comma">
            "
          </div>
          <div class="review-text">
            {{ review.review }}
            <div>
              <div class="review-pic">
                <img :src=review.pic />
              </div>
              <div class="review-name">{{ review.name }}</div>
              <div class="review-about">{{ review.about }}</div>
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
          pic: "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcScwmUDUqzIvcDJGbL4bGaXPxYuBd8qrET1hA&usqp=CAU",
        },
        {
          name: "Test",
          review: "review",
          about: "about",
          pic: "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcScwmUDUqzIvcDJGbL4bGaXPxYuBd8qrET1hA&usqp=CAU",
        },
        {
          name: "Test",
          review: "review",
          about: "about",
          pic: "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcScwmUDUqzIvcDJGbL4bGaXPxYuBd8qrET1hA&usqp=CAU",
        },
        {
          name: "Test",
          review: "review",
          about: "about",
          pic: "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcScwmUDUqzIvcDJGbL4bGaXPxYuBd8qrET1hA&usqp=CAU",
        },
      ],
      activeReview: 0,
      prevReview: 0,
    };
  },
  methods: {
    scroll(key) {
      if ((this.activeReview == 0 && key == 0) || this.activeReview == key) {
        return;
      }
      if (key == 0) {
        this.$refs.reviewRow.scrollLeft -= this.reviews.length + 1 * 680;
      }
      if (key == this.reviews.length) {
        this.$refs.reviewRow.scrollLeft += this.reviews.length * 680;
      }
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
  display: none !important;
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
.review-item-container {
}
.inverted-comma {
  font-family: Muli;
  font-style: italic;
  font-weight: normal;
  font-size: 46px;
  line-height: 108px;
  color: #dfdfdf;
  width: 100%;
}

.review-text {
  ont-family: Muli;
  font-style: italic;
  font-weight: normal;
  font-size: 18px;
  line-height: 23px;
  width: 100%;
  height: 20%;
  color: #dfdfdf;
}
.review-pic {
  border: 1px solid rgba(223, 223, 223, 0.5);
  box-sizing: border-box;
    border-radius: 50%;

  height: 40px;
  width: 40px;
}

.review-pic > img{
  height: 100%;
  width: 100%;
  border-radius: 50%;
}
.review-name {
  ont-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 15px;

  color: #dfdfdf;
}
.review-about {
  font-family: Muli;
  font-style: normal;
  font-weight: normal;
  font-size: 11px;
  line-height: 14px;

  color: rgba(223, 223, 223, 0.5);
}
@media screen and (max-width: 786px) {
  .review-container {
    display: flex;
    flex-wrap: wrap;
    margin-top: 340px !important;
  }
  .review-row {
    margin-top: 370px !important;
  }
  .review-item {
    width: 100%;
  }
}
@media screen and (max-width: 576px) {
}
</style>
