<template>
  <section class="hero pre-leader-board leader-board">
    <div class="container w-75">
      <div class="hero-section-content text-center">
        <img :src="pageData.image" :alt="pageData.subtitle" class="img-fluid">
        <h2 class="title text-uppercase mt-3">
          Kay<span class="primary-text">-So</span>
        </h2>
        <h3>
          {{ pageData.subtitle }}
        </h3>
        <p class="text">
          {{ pageData.description }}
        </p>

        <div class="kay-so-podcast">
          <div class="kay-so-podcast-episode">
        <h5>Episode One - Your listening pleasures</h5>
          <audio controls>
            <source src="/audio/kay-so-one.mp3" type="audio/mpeg">
            Your browser does not support the audio tag.
          </audio>
        </div>

        <div class="kay-so-podcast-episode">
        <h5>Episode Two - Nevermore</h5>
          <audio controls>
            <source src="/audio/kay-so-two-nevermore.mp3" type="audio/mpeg">
            Your browser does not support the audio tag.
          </audio>
        </div>
        </div>
        <!-- <p>
          <a href="#what">More Info...</a>
        </p> -->
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const pageData = ref(
  {
    title: 'Kay-So',
    subtitle: 'For your listening pleasures...',
    description: 'The Kay-So Podcast is a collection of audio flotsam and jetsam from the interwebs filtered through the mind of Kay-So.  If you are interested in listening differently this podcast may be for you. I like to think of it as a podcast palate cleanse.',
    image: '/images/kay-so-280.webp',
    imageAlt: 'Kay-So',
  }
)

</script>

<style scoped>
.hero {
  background-image: linear-gradient(45deg,
    hsl(0deg 0% 5%) 0%,
    hsl(344deg 0% 4%) 10%,
    hsl(344deg 0% 3%) 20%,
    hsl(344deg 0% 2%) 30%,
    hsl(344deg 0% 1%) 40%,
    hsl(0deg 0% 0%) 50%,
    hsl(344deg 0% 1%) 60%,
    hsl(344deg 0% 3%) 70%,
    hsl(344deg 0% 4%) 80%,
    hsl(344deg 0% 5%) 90%,
    hsl(0deg 0% 6%) 100%);
}

.download-button {
  margin: .3rem 0 3rem 0;
}

.kay-so-podcast{
  display: flex;
  flex-direction: column;
  align-items: center;
}

.kay-so-podcast-episode {
  margin: 1.5rem 0;
  padding: 1rem;
  background-color: rgba(12, 12, 12, .3);
  min-width: 640px;
  border-radius: .33rem;
  border: 5px solid rgba(0, 0, 0, .3);
}

audio::-webkit-media-controls-enclosure {
  border-radius: 1rem;
  background-color: #000;
}

audio::-webkit-media-controls-panel {
  background-color: #000;
  border: 1px solid #000;
}

audio::-webkit-media-controls-mute-button {
  background-color: #0c0c0c;
  border-radius: 50%;

}

audio::-webkit-media-controls-play-button {
  background-color: #0c0c0c;
  border-radius: 50%;
}

audio::-webkit-media-controls-play-button:hover {
  background-color: #1cb752;
}

audio::-webkit-media-controls-current-time-display {
  color: #1cb752;
}

audio::-webkit-media-controls-time-remaining-display {
  color: #BDD684;
}

audio::-webkit-media-controls-timeline {
  background-color: #0c0c0c;
  border-radius: 25px;
  margin-left: 10px;
  margin-right: 10px;
}

audio::-webkit-media-controls-volume-slider {
  background-color: #1f2428;
  border-radius: 25px;
  padding-left: 8px;
  padding-right: 8px;
}
</style>