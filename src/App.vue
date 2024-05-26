<template>
  <div id="app">
    <Navbar />
    <Carousel />
    <div class="container mt-5">
      <div class="row">
        <Card
          title="Glamour Party"
          description="Glamour Party adalah parfum dengan aroma jeruk mandarin, lada merah, bergamot sebagai top note, aroma jasmine, anggur, peach, geranium sebagai middle note, dan aroma nilam, musk, amber, vanilla sebagai base note.
"
          imgUrl="https://images.tokopedia.net/img/cache/900/VqbcmM/2023/5/28/18a25e13-c21c-4e60-9b3a-da12848d7e02.png"
        />
        <Card
          title="Aventa"
          description="Aventa adalah parfum dengan aroma nanas, bergamot, anggur dan apel sebagai top note, aroma birch, nilam, moroccan jasmine dan bunga mawar sebagai middle note, serta aroma musk, oak muss, ambergis dan vanilla sebagai base note."
          imgUrl="https://images.tokopedia.net/img/cache/900/VqbcmM/2023/6/3/946db829-f5e1-4bc2-9c47-3fc96530608d.png"
        />
        <Card
          title="Vanilla Ice"
          description="Vanilla Ice adalah parfum dengan paduan aroma susu, vanilla, sweet notes dan water notes.  "
          imgUrl="https://images.tokopedia.net/img/cache/900/VqbcmM/2023/3/11/22f4e315-0790-4419-a2ba-79cc532fee58.jpg"
        />
      </div>
      <h2 class="text-center my-4">Additional Information</h2>
      <div class="row">
        <InfoCard
          title="Outlet"
          description="Outlet Uchi Parfume Daerah mu"
          imgUrl="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQNDWHSipQwioixh7a7HS_Aydp-TqDPlfbRh1cBcU-iuA&s" 
        />
        <InfoCard
          title="We are Uchi Parfume"
          description="Kami ada dimana-mana"
          imgUrl="https://pict-b.sindonews.net/dyn/850/pena/news/2024/01/27/186/1308499/uchi-parfume-fokus-pada-kualitas-edukasi-dan-inovasi-digital-tgb.jpeg" 
        />
        <InfoCard
          title="Variant Parfume"
          description="Ada 1000+ Local & International Variants."
          imgUrl="https://images.samsung.com/id/galaxy-tab-s9/feature/galaxy-tab-s9-visual-pc.jpg" 
        />
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Carousel from './components/Carousel.vue';
import Card from './components/Card.vue';
import InfoCard from './components/InfoCard.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Carousel,
    Card,
    InfoCard,
    Footer
  }
}
</script>

<style>
body {
  display: flex;
  font-family: 'Arial', sans-serif;
  background-color: #e4f2ff;
  color: #E42427;
}

h2 {
  color: #FBEC22;
}

.container {
  padding: 0 15px;
}

.text-center {
  text-align: center;
}

.mb-4 {
  margin-bottom: 1.5rem;
}

.mt-5 {
  margin-top: 3rem;
}

.mt-4 {
  margin-top: 1.5rem;
}

.my-4 {
  margin-top: 1.5rem;
  margin-bottom: 1.5rem;
}

.row {
  display: flex;
  flex-wrap: wrap;
}

.card,
.info-card {
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover,
.info-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
}

hr {
  border: none;
  border-top: 2px solid #ddd;
}

.tittle {
  font-style: bold;
}
</style>