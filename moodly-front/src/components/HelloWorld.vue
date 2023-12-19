<template>
  <div>
    <swiper class="swiper">
      <swiper-slide v-for="(emotion, index) in emotions" :key="index">
        <div class="emotion-card" :style="{ backgroundColor: emotion.color }">
          <p>{{ emotion.name }}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import 'swiper/css';
import { Swiper, SwiperSlide } from 'vue-awesome-swiper';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      emotions: [
        { name: 'Heureux', color: '#F8D65B' },
        { name: 'Fatigué', color: '#FF800A' },
        { name: 'Triste', color: '#9187FF' },
        { name: 'Perdu', color: '#4F9EC3' },
        { name: 'Déprimé', color: '#949599' },
        { name: 'Irritable', color: '#F57E20' },
        { name: 'Distrait', color: '#538BA4' },
        { name: 'Culpabilité', color: '#949599' },
        { name: 'Energique', color: '#F9D55B' },
        { name: 'Enjoué', color: '#F9D55B' },
        { name: 'Angoissé', color: '#949599' },
        { name: 'Manque énergétique', color: '#86B24F' },
        { name: 'Calme', color: '#4F9EC3' },
        { name: 'Je ne sais pas', color: '#D9D9D9' },
        // ... Ajoute les autres émotions avec leurs couleurs
      ],
      swiperOptions: {
        // Options du carrousel (voir la documentation de vue-awesome-swiper)
      },
    };
  },
};
</script>

<style scoped>
.emotion-card {
  width: 100%;
  height: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 24px;
  color: white;
}
</style>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
