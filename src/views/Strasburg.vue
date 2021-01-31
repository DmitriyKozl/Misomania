<template>
  <div class="Strasburg">
    <div class="banner">
      <video
        src="@\assets\images\banner.mp4"
        type="video/mp4"
        controls
        autoplay
      ></video>
      <div class="title">
        <h1>{{ title }}</h1>
        <span>{{ date }}</span>
        <div class="title__line"></div>
      </div>
    </div>
    <main>
      <p>{{ text }}</p>
      <div class="image">
        <img :src="image" alt="" />
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'Strasburg',
  data() {
    return {
      title: 'Untitled Strasburg',
      content: [
        {
          text:
            'Тучи, гонимые ветряными мельницами, темнели. Звук пролетающих мимо фонарей терялся в порывах предштормового вихря. Последний отблеск солнца исчез за горизонтом, но на тысячную секунды небо озарилось вновь. Гроза.',
          image: '',
        },
      ],
    };
  },
};
</script>

<style></style>
