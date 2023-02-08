<script>
  import { Carousel } from "flowbite-svelte";
  const images = [
    {
      id: 0,
      imgurl: "/gallery/w5.jpg",
    },
    {
      id: 1,
      imgurl: "/gallery/w6.jpg",
    },
    {
      id: 2,
      imgurl: "/gallery/w3.jpg",
    },
    {
      id: 3,
      imgurl: "/gallery/w4.jpg",
    },
    {
      id: 4,
      imgurl: "/gallery/w1.jpg",
    },
    {
      id: 5,
      imgurl: "/gallery/w2.jpg",
    },
    {
      id: 6,
      imgurl: "/gallery/w7.jpg",
    },
    {
      id: 7,
      imgurl: "/gallery/w8.jpg",
    },
  ];

  let showThumbs = false;
  let showCaptions = false;
  let showIndicators = true;
</script>

<div id="gallery" class="flex flex-col items-center py-8">
  <h2 class="text-center py-8 font-bold ">Тлядал зимой</h2>
  <div class="max-w-4xl">
    <Carousel {images} {showThumbs} {showCaptions} {showIndicators} divClass />
  </div>
</div>
