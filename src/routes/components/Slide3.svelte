
<script>
    export let goToPreviousSlide;
 
    </script>
  
  <div class="slide active" style="
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
  
  
      <h1 style="color: #FF3E00;">Comment créer un projet Svelte</h1>
      <ol style="text-align: left;">
        <li>
          <strong>Installer Node.js :</strong><br />
          Téléchargez et installez <a href="https://nodejs.org" target="_blank" style="color: #FF3E00;">Node.js</a> pour votre système d'exploitation.
        </li>
        <li>
          <strong>Créer un nouveau projet :</strong><br />
          Exécutez la commande suivante dans le terminal :
          <pre style="
              background-color: #333; 
              color: #fff; 
              padding: 10px; 
              border-radius: 5px; 
              font-family: monospace;">
  npx degit sveltejs/template nom-du-projet
          </pre>
        </li>
        <li>
          <strong>Accéder au dossier du projet :</strong><br />
          Entrez dans le dossier créé :
          <pre style="
              background-color: #333; 
              color: #fff; 
              padding: 10px; 
              border-radius: 5px; 
              font-family: monospace;">
  cd nom-du-projet
          </pre>
        </li>
        <li>
          <strong>Installer les dépendances :</strong><br />
          Installez les paquets nécessaires avec :
          <pre style="
              background-color: #333; 
              color: #fff; 
              padding: 10px; 
              border-radius: 5px; 
              font-family: monospace;">
  npm install
          </pre>
        </li>
        <li>
          <strong>Lancer le serveur de développement :</strong><br />
          Pour démarrer votre projet :
          <pre style="
              background-color: #333; 
              color: #fff; 
              padding: 10px; 
              border-radius: 5px; 
              font-family: monospace;">
  npm run dev
          </pre>
          Accédez à votre projet à l'adresse suivante : <strong>http://localhost:5173</strong>.
        </li>
      </ol>
      <p style="text-align: center; color: #aaa;">
        🚀 Vous êtes prêt à coder avec <strong style="color: #FF3E00;">Svelte</strong> !
      </p>
      <button class="btn" on:click={goToPreviousSlide}>précédente</button>
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

  