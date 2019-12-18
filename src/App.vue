<template>
  <div id="app">
    <main>
      <div class="section">
        <Carousel :cards="cards" />
      </div>
    </main>
  </div>
</template>

<script>
import Carousel from "./components/Carousel";
export default {
  name: "app",
  components: { Carousel },

  data() {
    return {
      headline:
        "Here You Learn Everything about building Progressive Vue Apps!",
      sections: [
        { headline: "What does a Service Worker do?" },
        {
          headline: "How does a Service Worker exactly work?"
        }
      ],

      cards: [
        {
          headline: "Makes App available Offline",
          text:
            "By using the CachingAPI all static elements on an app can be pre-cached",
          imgName: "img-1.png"
        },
        {
          headline: "Use background sync to defer actions",
          text:
            "User inputs entered when offline are sent in the background once they get connectivity.",
          imgName: "img-2.png"
        },
        {
          headline: "Send Push Notifications",
          text:
            "The Notifications API lets us send push notifications to re-engage users.",
          imgName: "img-3.png"
        }
      ]
    };
  }
};
</script>

<style src="assets/styles/App.css"/>


