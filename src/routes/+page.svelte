<script>
    import 'animate.css';


    let currentSlide = 1; 

    const goToNextSlide = () => {
        currentSlide = 2; 
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

  img {
    max-width: 100%;
    height: auto;
    border-radius: 8px;
  }

  .btn {
    margin-top: 20px;
    padding: 10px 20px;
    font-size: 18px;
    background-color: #f5f5f5;
    color: #121212;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s, color 0.3s;
  }

  .btn:hover {
    background-color: #333;
    color: #f5f5f5;
  }

 
  .slide {
    display: none; 
  }

  .slide.active {
    display: block; 
  }
</style>

<!-- Main Container -->
<div class="container">
    <div>
    </div>
    
    <div class="slide {currentSlide === 1 ? 'active' : ''}">
        <div class="animate__animated animate__zoomIn animate__delay-1s">
            <img src="/images/blob.png" alt="Svelte">
        </div>
        <button class="btn" style="background-color: rgb(255, 62, 0);color: rgb(255, 255, 255);" on:click={goToNextSlide}>Start</button>
    </div>

    
    <div class="slide {currentSlide === 2 ? 'active' : ''}" style="width: 100%;">
        <button class="btn" style="background-color: rgb(255, 62, 0);color: rgb(255, 255, 255);" on:click={()=>currentSlide = currentSlide - 1}>return</button>

        <h1>Qu'est-ce que Svelte ?</h1>
         <p>   Svelte est un framework moderne pour le développement d'interfaces utilisateur (UI). Contrairement à des frameworks comme React ou Vue, Svelte adopte une approche unique en éliminant la phase d'exécution dans le navigateur.</p>

    </div>
</div>
