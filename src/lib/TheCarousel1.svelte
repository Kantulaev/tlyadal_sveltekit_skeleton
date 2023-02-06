<script>
  import { Carousel } from "flowbite-svelte";
  const images = [
    {
      id: 0,
      imgurl: "/gallery/s3.jpg",
    },
    {
      id: 1,
      imgurl: "/gallery/s4.jpg",
    },
    {
      id: 2,
      imgurl: "/gallery/s1.jpg",
    },
    {
      id: 3,
      imgurl: "/gallery/s2.jpg",
    },
    {
      id: 4,
      imgurl: "/gallery/s6.jpg",
    },
    {
      id: 5,
      imgurl: "/gallery/s7.jpg",
    },
  ];

  let showThumbs = false;
  let showCaptions = false;
  let showIndicators = true;
</script>

<div id="gallery" class="flex flex-col items-center py-8 ">
  <h2 class="text-center py-8 font-bold ">Тлядал Летом</h2>
  <div class="max-w-6xl ">
    <Carousel {images} {showThumbs} {showCaptions} {showIndicators} />
  </div>
</div>
