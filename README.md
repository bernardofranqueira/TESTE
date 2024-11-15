# TESTE
<!DOCTYPE html>
<html lang="pt-BR">
<head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>NAMING</title>
   <style>
       * {
           margin: 0;
           padding: 0;
           box-sizing: border-box;
       }
       body {
           font-family: Arial, sans-serif;
           background-color: #f5f5f5;
           padding: 2rem;
       }
       .container {
           max-width: 800px;
           margin: 0 auto;
       }
       .header {
           text-align: center;
           margin-bottom: 2rem;
           padding: 2rem;
           background: white;
           border-radius: 8px;
           box-shadow: 0 2px 4px rgba(0,0,0,0.1);
       }
       .header h1 {
           font-size: 2.5rem;
           color: #1a1a1a;
           margin-bottom: 1rem;
       }
       .header p {
           color: #666;
           font-size: 1.1rem;
       }
       .category-section {
           margin-bottom: 3rem;
       }
       .category-title {
           font-size: 1.5rem;
           color: #1a1a1a;
           margin-bottom: 1rem;
           padding: 0.5rem 1rem;
           background: white;
           border-radius: 4px;
           box-shadow: 0 2px 4px rgba(0,0,0,0.1);
       }
       .card {
           background: white;
           border-radius: 8px;
           padding: 1.5rem;
           margin-bottom: 1rem;
           box-shadow: 0 2px 4px rgba(0,0,0,0.1);
       }
       .card:hover {
           box-shadow: 0 4px 8px rgba(0,0,0,0.15);
           transition: box-shadow 0.3s ease;
       }
       .card-header {
           display: flex;
           justify-content: space-between;
           align-items: start;
           margin-bottom: 1rem;
       }
       .name {
           font-size: 1.8rem;
           font-weight: bold;
           color: #1a1a1a;
       }
       .tagline {
           font-style: italic;
           color: #666;
           margin-top: 0.5rem;
       }
       .button {
           background: #1a1a1a;
           color: white;
           border: none;
           padding: 0.5rem 1rem;
           border-radius: 4px;
           cursor: pointer;
           transition: all 0.3s ease;
           min-width: 180px;
           text-align: center;
       }
       .button:hover {
           background: #333;
           transform: translateY(-1px);
       }
       .button.selected {
           background: #059669;
       }
       .button.selected:hover {
           background: #047857;
       }
       .description {
           color: #444;
           margin-bottom: 1rem;
           line-height: 1.6;
       }
       .key-points {
           background: #f8f8f8;
           padding: 1rem;
           border-radius: 4px;
       }
       .key-points h4 {
           color: #1a1a1a;
           margin-bottom: 0.5rem;
       }
       .key-points ul {
           padding-left: 1.5rem;
       }
       .key-points li {
           color: #444;
           margin-bottom: 0.5rem;
       }
       .notification {
           position: fixed;
           bottom: 1rem;
           right: 1rem;
           background: #059669;
           color: white;
           padding: 1rem;
           border-radius: 4px;
           box-shadow: 0 2px 4px rgba(0,0,0,0.1);
           display: none;
           z-index: 1000;
       }
       .votes-counter {
           background: #f0f0f0;
           border-radius: 4px;
           padding: 0.5rem;
           margin-top: 1rem;
           text-align: center;
           color: #666;
       }
   </style>
</head>
<body>
   <div class="container">
       <div class="header">
           <h1>NAMING</h1>
           <p>Selecione sua opção preferida para a nova marca de diamantes lab grown</p>
           <div id="total-votes" class="votes-counter">Total de votos: 0</div>
       </div>

       <!-- Nome Atual -->
       <section class="category-section">
           <h2 class="category-title">Nome Atual</h2>
           <div class="card">
               <div class="card-header">
                   <div>
                       <div class="name">ADEAN</div>
                       <div class="tagline">Sofisticação e Tecnologia</div>
                   </div>
                   <button class="button" onclick="toggleSelection('ADEAN', this)" data-name="ADEAN">
                       Selecionar (0 votos)
                   </button>
               </div>
               <p class="description">Nome atual da marca, representa America's Diamond Eco-friendly Alliance Network. Carrega consigo a história inicial do projeto e seus valores fundamentais.</p>
               <div class="key-points">
                   <h4>Pontos-chave:</h4>
                   <ul>
                       <li>Mantém a identidade original</li>
                       <li>Já possui reconhecimento no mercado</li>
                       <li>Comunica tecnologia e sustentabilidade</li>
                       <li>Conexão com mercado americano</li>
                   </ul>
               </div>
           </div>
       </section>

       <!-- Tecnologia -->
       <section class="category-section">
           <h2 class="category-title">Tecnologia</h2>
           
           <!-- AEVA -->
           <div class="card">
               <div class="card-header">
                   <div>
                       <div class="name">AEVA</div>
                       <div class="tagline">Evolução em Forma de Diamante</div>
                   </div>
                   <button class="button" onclick="toggleSelection('AEVA', this)" data-name="AEVA">
                       Selecionar (0 votos)
                   </button>
               </div>
               <p class="description">Evoca evolução e elevação, trazendo consigo a ideia de avanço tecnológico e sofisticação.</p>
               <div class="key-points">
                   <h4>Pontos-chave:</h4>
                   <ul>
                       <li>Som premium e tecnológico</li>
                       <li>Remete à evolução e elevação</li>
                       <li>Curto e memorável</li>
                       <li>Feminino e sofisticado</li>
                   </ul>
               </div>
           </div>

           <!-- LYRA -->
           <div class="card">
               <div class="card-header">
                   <div>
                       <div class="name">LYRA</div>
                       <div class="tagline">Precisão e Luz</div>
                   </div>
                   <button class="button" onclick="toggleSelection('LYRA', this)" data-name="LYRA">
                       Selecionar (0 votos)
                   </button>
               </div>
               <p class="description">Referência à constelação, une precisão tecnológica com a beleza da luz estelar.</p>
               <div class="key-points">
                   <h4>Pontos-chave:</h4>
                   <ul>
                       <li>Conexão com luz e precisão</li>
                       <li>Som elegante e distintivo</li>
                       <li>Apelo internacional</li>
                       <li>Fácil pronúncia</li>
                   </ul>
               </div>
           </div>

           <!-- LUMEX -->
           <div class="card">
               <div class="card-header">
                   <div>
                       <div class="name">LUMEX</div>
                       <div class="tagline">A Luz da Inovação</div>
                   </div>
                   <button class="button" onclick="toggleSelection('LUMEX', this)" data-name="LUMEX">
                       Selecionar (0 votos)
                   </button>
               </div>
               <p class="description">Combina 'lumen' (luz) com tecnologia, representando a união perfeita entre ciência e beleza.</p>
               <div class="key-points">
                   <h4>Pontos-chave:</h4>
                   <ul>
                       <li>Som tecnológico e premium</li>
                       <li>Conexão direta com luz</li>
                       <li>Distintivo no mercado</li>
                       <li>Memorável e único</li>
                   </ul>
               </div>
           </div>
       </section>

       <!-- Sustentabilidade -->
       <section class="category-section">
           <h2 class="category-title">Sustentabilidade</h2>
           
           <!-- AEON -->
           <div class="card">
               <div class="card-header">
                   <div>
                       <div class="name">AEON</div>
                       <div class="tagline">Eternamente Sustentável</div>
                   </div>
                   <button class="button" onclick="toggleSelection('AEON', this)" data-name="AEON">
                       Selecionar (0 votos)
                   </button>
               </div>
               <p class="description">Representa eternidade e atemporalidade, com forte conexão com sustentabilidade.</p>
               <div class="key-points">
                   <h4>Pontos-chave:</h4>
                   <ul>
                       <li>Posição alfabética inicial</li>
                       <li>Som premium e atemporal</li>
                       <li>Significado profundo</li>
                       <li>Fácil pronúncia global</li>
                   </ul>
               </div>
           </div>

           <!-- ALBA -->
           <div class="card">
               <div class="card-header">
                   <div>
                       <div class="name">ALBA</div>
                       <div class="tagline">O Amanhecer de Uma Nova Era</div>
                   </div>
                   <button class="button" onclick="toggleSelection('ALBA', this)" data-name="ALBA">
                       Selecionar (0 votos)
                   </button>
               </div>
               <p class="description">Significa 'amanhecer' em latim, representando o início de uma nova era sustentável.</p>
               <div class="key-points">
                   <h4>Pontos-chave:</h4>
                   <ul>
                       <li>Representa novo começo</li>
                       <li>Elegante e feminino</li>
                       <li>Som suave e sofisticado</li>
                       <li>Significado universal</li>
                   </ul>
               </div>
           </div>

           <!-- NOVA -->
           <div class="card">
               <div class="card-header">
                   <div>
                       <div class="name">NOVA</div>
                       <div class="tagline">O Novo Luxo Sustentável</div>
                   </div>
                   <button class="button" onclick="toggleSelection('NOVA', this)" data-name="NOVA">
                       Selecionar (0 votos)
                   </button>
               </div>
               <p class="description">Sugere inovação e novo começo, representando uma revolução no mercado de diamantes.</p>
               <div class="key-points">
                   <h4>Pontos-chave:</h4>
                   <ul>
                       <li>Direto e impactante</li>
                       <li>Fácil pronúncia global</li>
                       <li>Significado universal</li>
                       <li>Moderno e dinâmico</li>
                   </ul>
               </div>
           </div>
       </section>

       <!-- Origem -->
       <section class="category-section">
           <h2 class="category-title">Origem</h2>

           <!-- SEMA -->
           <div class="card">
               <div class="card-header">
                   <div>
                       <div class="name">SEMA</div>
                       <div class="tagline">Cultivando Preciosidades</div>
                   </div>
                   <button class="button" onclick="toggleSelection('SEMA', this)" data-name="SEMA">
                       Selecionar (0 votos)
                   </button>
               </div>
               <p class="description">Derivado do grego 'sema' (semente), representa o início, o cultivo e a transformação.</p>
               <div class="key-points">
                   <h4>Pontos-chave:</h4>
                   <ul>
                       <li>Conexão com origem</li>
                       <li>Som sofisticado</li>
                       <li>Nome curto e memorável</li>
                       <li>Fácil pronúncia</li>
                   </ul>
               </div>
           </div>

           <!-- PRIMA -->
           <div class="card">
               <div class="card-header">
                   <div>
                       <div class="name">PRIMA</div>
                       <div class="tagline">A Primeira em Inovação</div>
                   </div>
                   <button class="button" onclick="toggleSelection('PRIMA', this)" data-name="PRIMA">
                       Selecionar (0 votos)
                   </button>
               </div>
               <p class="description">Do latim 'primeira', sugere origem, pioneirismo e excelência.</p>
               <div class="key-points">
                   <h4>Pontos-chave:</h4>
                   <ul>
                       <li>Premium e sofisticado</li>
                       <li>Significado em vários idiomas</li>
                       <li>Forte apelo visual</li>
                       <li>Som elegante</li>
                   </ul>
               </div>
           </div>

           <!-- NEXUS -->
           <div class="card">
               <div class="card-header">
                   <div>
                       <div class="name">NEXUS</div>
                       <div class="tagline">O Elo entre Futuro e Tradição</div>
                   </div>
                   <button class="button" onclick="toggleSelection('NEXUS', this)" data-name="NEXUS">
                       Selecionar (0 votos)
                   </button>
               </div>
               <p class="description">Representa conexão e origem, unindo tradição e inovação.</p>
               <div class="key-points">
                   <h4>Pontos-chave:</h4>
                   <ul>
                       <li>Som tecnológico</li>
                       <li>Significa conexão/origem</li>
                       <li>Moderno e distintivo</li>
                       <li>Internacional
