<template>
  <div>
    <h1>Home</h1>

    <div id="lessons-wrapper">
      <div v-for="lesson in lessons" :key="lesson.id">
        <LessonCard :lesson="lesson" />
      </div>
    </div>
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
      lessons: [
        {
          id: 1,
          imgUrl:
            "https://img-a.udemycdn.com/course/240x135/3533422_867d.jpg?Rl3s9gb0iy3zvJ5Ru4FPuuLJcBn-CKucZqqf82ZTx1qGjz5Bv6yqU6ECuyfN3uuWyNnR5Yf0irLr-qtqFgJlg-xyW_QOfXMPrUJ-tiuFi9MuTOJ9odoYVgHH5L26ag",
          title: "MERN eCommerce From Scratch",
          author: "Brad Traversy",
          price: "179000"
        },
        {
          id: 2,
          imgUrl:
            "https://img-a.udemycdn.com/course/240x135/2782800_0b85.jpg?mERIElLOl8s__viiID-HRlv8Lynrl3wvajkx3xAX2Ki3iWcc-U9NMJNoEZabjug-7dcojOFQKzjFvIsWWDvITGT6VgXiECweUs4ibs-wZ7-ZXpX4KbZuqoIEIzeMag",
          title: "20 Projects with Vanilla JS",
          author: "Hanjaya Suryalim",
          price: "179000"
        },
        {
          id: 3,
          imgUrl:
            "https://img-a.udemycdn.com/course/240x135/1409142_1879_8.jpg?2HY3sHU9-PVJ7YHfXfg_S_ukhjinU8ab5xBtPI3C-MJMZd93vH5kTyoQc_XRbdla6xDlWN4dvc4F0Bdv0LGWePGrEZlQALZBTW_gXuXhl-6ed4hyfbSqOgAS3gxxnIhz",
          title: "The Coding Interview Bootcamp",
          author: "Andreas Aditya",
          price: "179000"
        },
        {
          id: 4,
          imgUrl:
            "https://img-a.udemycdn.com/course/240x135/3533422_867d.jpg?Rl3s9gb0iy3zvJ5Ru4FPuuLJcBn-CKucZqqf82ZTx1qGjz5Bv6yqU6ECuyfN3uuWyNnR5Yf0irLr-qtqFgJlg-xyW_QOfXMPrUJ-tiuFi9MuTOJ9odoYVgHH5L26ag",
          title: "MERN eCommerce From Scratch",
          author: "Brad Traversy",
          price: "179000"
        },
        {
          id: 5,
          imgUrl:
            "https://img-a.udemycdn.com/course/240x135/2782800_0b85.jpg?mERIElLOl8s__viiID-HRlv8Lynrl3wvajkx3xAX2Ki3iWcc-U9NMJNoEZabjug-7dcojOFQKzjFvIsWWDvITGT6VgXiECweUs4ibs-wZ7-ZXpX4KbZuqoIEIzeMag",
          title: "20 Projects with Vanilla JS",
          author: "Hanjaya Suryalim",
          price: "179000"
        },
        {
          id: 6,
          imgUrl:
            "https://img-a.udemycdn.com/course/240x135/1409142_1879_8.jpg?2HY3sHU9-PVJ7YHfXfg_S_ukhjinU8ab5xBtPI3C-MJMZd93vH5kTyoQc_XRbdla6xDlWN4dvc4F0Bdv0LGWePGrEZlQALZBTW_gXuXhl-6ed4hyfbSqOgAS3gxxnIhz",
          title: "The Coding Interview Bootcamp",
          author: "Andreas Aditya",
          price: "179000"
        }
      ]
    };
  }
};
</script>

<style>
#lessons-wrapper {
  display: flex;
}
</style>
