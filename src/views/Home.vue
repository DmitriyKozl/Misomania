<template>
  <div>
    <header>
      <div class="banner">
        <div class="banner_text"><h1>Misomania</h1></div>
        <div class="banner_paragraph"><p>the highest form of escapism</p></div>
      </div>
    </header>

    <div class="preview_container">
      <section
        v-for="image in bgImages"
        :key="image.id"
        @click="this.$router.push(image.name)"
      >
        <div
          :style="{
            'background-image': 'url(' + require('@/assets/' + image.src) + ')',
          }"
          class="preview_img"
        ></div>
        <div class="titleImage">
          <h2>{{ image.title }}</h2>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Misomania',
  components: {},
  data() {
    return {
      bgImages: [
        {
          id: 1,
          src: 'images/stras.jpg',
          title: 'Untitled Straßburg',
          name: 'Strasburg',
        },
        {
          id: 2,
          src: 'images/normandie_banner.jpg',
          title: 'La Normandie',
        },
        { id: 3, src: 'images/door.jpg', title: '4 века на 400 километров' },
        {
          id: 4,
          src: 'images/жирона-и-беда-синоптики.jpg',
          title: 'Жирона и беда синоптики',
        },
        {
          id: 5,
          src: 'images/южнин-и-пунктуальность-вещи-не-совмес.jpg',
          title: 'Южанин и пунктуальность,вещи не совместимые',
        },
        {
          id: 6,
          src: 'images/день-первый.jpg',
          title: 'День первый',
        },
        {
          id: 7,
          src: 'images/радость-слёзы-и-бюро-находок.jpeg',
          title: 'Радость, слёзы и бюро находок',
        },
        {
          id: 8,
          src: 'images/албуфейра-нам-запомнится-на-долго.jpg',
          title: 'Албуфейра нам запомнится на долго!',
        },
        { id: 9, src: 'images/внедрёж.jpg', title: 'Внедрёж' },
        {
          id: 10,
          src: 'images/по-ту-сторону-африки.jpg',
          title: 'По ту сторону Африки',
        },
        {
          id: 11,
          src: 'images/кордова-сковзь-окно-уборных.jpg',
          title: 'Кордова сковзь окна уборных…',
        },
        {
          id: 12,
          src: 'images/ронда-белый-городок-андалузии.jpg',
          title: 'Ронда, белый городок Андалузии',
        },
        {
          id: 13,
          src: 'images/путешествие-во-времени.jpg',
          title: 'Путешествие во времени',
        },
        { id: 14, src: 'images/моря.jpg', title: 'У синего моря…' },
        {
          id: 15,
          src: 'images/в-севильской-тени-курица-готова-через-10.jpg',
          title: 'В Севильской тени курица готова через 10 минут',
        },
        {
          id: 16,
          src: 'images/wp-1456965754253.jpg',
          title: 'День третий, лучезарный',
        },
        {
          id: 17,
          src: 'images/wp-1456767118842.jpg',
          title: 'Будапешт день целёхонько второй',
        },
      ],
    };
  },
};
</script>

<style></style>
