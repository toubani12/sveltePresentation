<script>
    import Footer from './components/footer.svelte';
    import Slide1 from './components/Slide1.svelte';
    import Slide2 from './components/Slide2.svelte';
  import Slide3 from './components/Slide3.svelte';
  
    let currentSlide = 1;
  
    const goToNextSlide = () => {
      currentSlide += 1;
    };
  
    const goToPreviousSlide = () => {
      currentSlide -= 1;
    };
  

  </script>
  
  <style lang="postcss">
    :global(html) {
      background-color: #121212;
      color: #f5f5f5;
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }
  
    .container {
      width: 90%;
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
      text-align: center;
    }
  
    .slide {
      display: none;
    }
  
    .slide.active {
      display: block;
      animation: fade-in 0.5s ease;
    }
  
    @keyframes fade-in {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }
  </style>
  
  <div class="container">
    {#if currentSlide === 1}
      <Slide1 {goToNextSlide} />
    {/if}
  
    {#if currentSlide === 2}
      <Slide2 {goToNextSlide} {goToPreviousSlide} />
    {/if}

    {#if currentSlide === 3}
    <Slide3 {goToNextSlide} {goToPreviousSlide} />
    {/if}

  </div>
  <Footer />
  