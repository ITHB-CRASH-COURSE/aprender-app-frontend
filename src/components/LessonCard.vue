<template>
  <div id="lesson">
    <img :src="lesson.imgUrl" alt="Lesson Thumbnail" />
    <div id="body">
      <h1 id="title">{{ lesson.title }}</h1>
      <span id="author">{{ lesson.author }}</span>
      <span id="price">Rp. {{ lesson.price }}</span>
    </div>
  </div>
</template>

<script>
export default {
  props: ["lesson"]
};
</script>

<style>
#lesson {
  border-radius: 0.5rem;

  max-width: 15rem;
  margin: 1rem;
}
#body {
  margin-top: -0.5rem;
  display: flex;
  flex-direction: column;
}

#title {
  font-size: 1rem;
  font-weight: 600;
}
#author {
  font-size: 12px;
  font-weight: 400;
  color: #73726c;
  margin-bottom: 1rem;
}
#price {
  font-size: 1rem;
  font-weight: 700;
  color: #3c3b37;
  margin-top: -0.325rem;
}
</style>
