<template>
  <div>
    <h1>About page</h1>

    <LessonCard :lesson="lesson" />
  </div>
</template>

<script>
import LessonCard from "../components/LessonCard";

export default {
  components: {
    LessonCard
  },
  data: () => {
    return {
      lesson: {
        id: 1,
        imgUrl:
          "https://img-a.udemycdn.com/course/240x135/3533422_867d.jpg?Rl3s9gb0iy3zvJ5Ru4FPuuLJcBn-CKucZqqf82ZTx1qGjz5Bv6yqU6ECuyfN3uuWyNnR5Yf0irLr-qtqFgJlg-xyW_QOfXMPrUJ-tiuFi9MuTOJ9odoYVgHH5L26ag",
        title: "MERN eCommerce From Scratch",
        author: "Brad Traversy",
        price: "179000"
      }
    };
  }
};
</script>

<style></style>
