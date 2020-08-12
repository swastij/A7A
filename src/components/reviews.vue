<template>
  <div class="review-container">
    <div ref="reviewRow" class="review-row">
      <div class="review-item" v-for="(review, key) in reviews" :key="key">
        <div>
          {{ key }}
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
</style>
