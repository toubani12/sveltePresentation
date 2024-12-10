<script>
    export let goToNextSlide; // Fonction pour aller à la slide suivante
  </script>
  
  <div class="slide active">
    <div class="animate__animated animate__zoomIn animate__delay-1s">
      <img src="/images/blob.png" alt="Svelte" />
    </div>
    <button class="btn" on:click={goToNextSlide}>Commencer</button>
  </div>
  
  <style>
    img {
      max-width: 100%;
      height: auto;
      border-radius: 8px;
    }
  
    .btn {
      margin-top: 20px;
      padding: 12px 24px;
      font-size: 16px;
      font-weight: bold;
      background-color: #FF3E00;
      color: #ffffff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: transform 0.2s, background-color 0.3s;
    }
  
    .btn:hover {
      background-color: #333;
      transform: scale(1.05);
    }
  </style>
  