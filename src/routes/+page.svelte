<script>
    import bannerlogo from "$lib/img/banner.png";
    
    import { Gallery } from 'flowbite-svelte';
  
    const images = [
      { alt: 'shoes', src: 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-1.jpg' },
      { alt: 'small bag', src: 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-2.jpg' },
      { alt: 'plants', src: 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-3.jpg' },
      { alt: 'watch', src: 'https://flowbite.s3.amazonaws.com/docs/gallery/square/image-4.jpg' }
    ];
</script>

<img src={bannerlogo} class="border shadow-2xl my-2 border-black flex justify-center items-center mx-auto max-h-60" alt="Imeen Store Logo" />

<Gallery class="gap-2 grid-cols-2" items={images} />