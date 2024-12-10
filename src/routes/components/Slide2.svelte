<script>
    export let goToPreviousSlide;
    export let goToNextSlide; 
    </script>
  
  <div class="slide active">

  
    <div style="
        font-family: Arial, sans-serif; 
        line-height: 1.6; 
        color: #eaeaea; 
        background: #1e1e1e; 
        padding: 20px; 
        border-radius: 8px; 
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5); 
        max-width: 800px; 
        margin: 20px auto;
    ">
      <h1 style="color: #FF3E00;">Histoire de Svelte</h1>
      <p>
        <strong style="color: #FF3E00;">Svelte</strong> est un framework JavaScript moderne créé par <strong>Rich Harris</strong> en <strong>2016</strong>. 
        Contrairement à d'autres frameworks comme React ou Vue, Svelte compile le code à l'avance en JavaScript pur, 
        offrant des applications très performantes.
      </p>
      <p>
        En <strong>2020</strong>, SvelteKit a été lancé pour offrir des outils avancés comme le rendu côté serveur (SSR) et 
        la génération de sites statiques (SSG). Aujourd'hui, Svelte est reconnu pour sa simplicité et ses performances exceptionnelles.
      </p>
      <p style="text-align: center;">✨ <strong style="color: #FF3E00;">Svelte</strong> : simplicité, modernité et performance. ✨</p>
    </div>
    <button class="btn" on:click={goToPreviousSlide}>précédente</button>
    <button class="btn" on:click={goToNextSlide}>avancer</button>
  </div>
  
  <style>
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
  