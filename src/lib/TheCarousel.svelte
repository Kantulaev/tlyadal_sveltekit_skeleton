<script>
  import { Carousel } from "flowbite-svelte";
  export const images = [
    {
      id: 0,
      name: "Cosmic timetraveler",
      imgurl: "1.jpg",
      attribution: "cosmic-timetraveler-pYyOZ8q7AII-unsplash.com",
    },
    {
      id: 1,
      name: "Cosmic timetraveler",
      imgurl: "2.jpg",
      attribution: "cosmic-timetraveler-pYyOZ8q7AII-unsplash.com",
    },
  ];

  let showThumbs = false;
  let showCaptions = false;
  let showIndicators = true;
</script>

<div id="gallery" class="flex flex-col justify-center py-8">
  <h2 class="text-center py-4">Галлерея</h2>
  <div class="max-w-5xl">
    <Carousel {images} {showThumbs} {showCaptions} {showIndicators} divClass />
  </div>
</div>
