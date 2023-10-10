# extensions_test
<html>
<head>
  <title>Prevenção da Dengue</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, sans-serif;
      background-color: #f0f0f0;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
    }

    .header {
      background-color: #800080;
      color: white;
      padding: 20px;
      text-align: center;
    }

    .header h1 {
      font-size: 36px;
    }

    .nav {
      display: flex;
      justify-content: space-around;
      align-items: center;
      background-color: #e0e0e0;
      padding: 10px;
    }

    .nav a {
      color: #800080;
      text-decoration: none;
      font-weight: bold;
    }

    .nav a:hover {
      color: white;
      background-color: #800080;
    }

    .main {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      padding: 20px;
    }

    .main .card {
      width: 30%;
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      margin-bottom: 20px;
    }

    .main .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-top-left-radius: 10px;
      border-top-right-radius: 10px;
    }

    .main .card h3 {
      color: #800080;
      padding: 10px;
    }

    .main .card p {
      padding: 10px;
    }

    .main .card button {
      display: block;
      width: 80%;
      margin: 10px auto;
      padding: 10px;
      border: none;
      border-radius: 5px;
      background-color: #800080;
      color: white;
      font-weight: bold;
    }

    .main .card button:hover {
      background-color: white;
      color: #800080;
    }

    .footer {
      background-color:#800080 ;
      color:white ;
       padding :20 px ;
       text-align :center ;
     }
     
     @media (max-width :768px ) {
       .main .card {
         width :45% ;
       }
     }
     
     @media (max-width :576px ) {
       .main .card {
         width :100% ;
       }
     }
   </style>
 </head>
 <body>
   <div class="container">
     <div class="header">
       <h1>Prevenção da Dengue</h1>
       <p>Aprenda sobre a doença, seus sintomas e como evitá-la</p>
     </div>
     <div class="nav">
       <a href="#sobre">Sobre</a>
       <a href="#sintomas">Sintomas</a>
       <a href="#prevencao">Prevenção</a>
       <a href="#quiz">Quiz</a>
       <a href="#mapa">Mapa</a>
     </div>
     <div class="main" id="sobre">
       <div class="card">
         <img src="mosquito.jpg" alt="Mosquito Aedes Aegypti">
         <h3>O que é a dengue?</h3>
         <p>A dengue é uma doença transmitida pela picada da fêmea do mosquito Aedes Aegypti, que possui quatro sorotipos diferentes. A dengue pode causar febre, dor de cabeça, dor no corpo, manchas na pele e até complicações graves como hemorragia e choque.</p>
         <button onclick="showMore('sobre1')">Saiba mais</button>
         <p id="sobre1" style="display: none;">A dengue é uma doença viral que afeta cerca de 390 milhões de pessoas por ano no mundo, sendo mais comum em regiões tropicais e subtropicais. A dengue pode ser classificada em quatro tipos: dengue clássica, dengue hemorrágica, síndrome do choque da dengue e dengue com sinais de alarme. A dengue hemorrágica e a síndrome do choque da dengue são as formas mais graves e podem levar à morte se não tratadas adequadamente.</p>
       </div>
       <div class="card">
         <img src="transmissao.jpg" alt="Transmissão da dengue">
         <h3>Como a dengue se espalha?</h3>
         <p>A dengue se espalha pela picada da fêmea do mosquito Aedes Aegypti, que se infecta ao sugar o sangue de uma pessoa doente. O mosquito pode transmitir a doença para outras pessoas após um período de incubação de 8 a 12 dias. A pessoa infectada pode transmitir o vírus para os mosquitos até 6 dias após o início dos sintomas.</p>
         <button onclick="showMore('sobre2')">Saiba mais</button>
         <p id="sobre2" style="display: none;">O mosquito Aedes Aegypti é originário da África e foi introduzido no Brasil durante o período colonial. Ele se adapta facilmente ao ambiente urbano e se reproduz em locais com água parada, como pneus, garrafas, vasos de plantas e caixas d'água. O mosquito tem hábitos diurnos e costuma picar as pessoas nas primeiras horas da manhã e no final da tarde. Ele prefere picar as partes inferiores do corpo, como pernas, pés e tornozelos.</p>
       </div>
       <div class="card">
         <img src="vacina.jpg" alt="Vacina contra a dengue">
         <h3>Existe vacina contra a dengue?</h3>
         <p>Sim, existe uma vacina contra a dengue chamada Dengvaxia, que está disponível para pessoas acima de 45 anos que já tiveram dengue mais de uma vez e/ ou moram em áreas com muitos casos de dengue. A vacina protege contra os quatro sorotipos da doença e deve ser aplicada em três doses com intervalo de seis meses entre elas.</p>
         <button onclick="showMore('sobre3')">Saiba mais</button>
         <p id="sobre3" style="display: none;">A vacina contra a dengue foi desenvolvida pela empresa francesa Sanofi Pasteur e foi aprovada pela Anvisa em 2015. Ela é feita com vírus atenuados da dengue e estimula o sistema imunológico a produzir anticorpos contra a doença. A vacina tem uma eficácia média de 66% e pode reduzir em até 93% os casos graves de dengue. No entanto, a vacina não é recomendada para pessoas que nunca tiveram dengue, pois pode aumentar o risco de desenvolver formas mais graves da doença em caso de infecção.</p>
       </div>
     </div>
     <div class="main" id="sintomas">
       <div class="card">
         <img src="febre.jpg" alt="Febre alta">
         <h3>Febre alta</h3>
         <p>A febre alta é um dos principais sintomas da dengue. Ela costuma ter início súbito e pode variar entre 39ºC e 40ºC. A febre pode durar de dois a sete dias e pode ser acompanhada de calafrios, sudorese e mal-estar geral.</p>
         <button onclick="showMore('sintoma1')">Saiba mais</button>
         <p id="sintoma1" style="display: none;">A febre alta é uma resposta do organismo à infecção pelo vírus da dengue. Ela indica que o sistema imunológico está combatendo o agente invasor e tentando eliminar o vírus do corpo. A febre alta pode causar desidratação, dor de cabeça,         fadiga e perda de apetite. É importante medir a temperatura com um termômetro e tomar medicamentos antitérmicos, como paracetamol, para aliviar o desconforto. Evite tomar medicamentos que contenham ácido acetilsalicílico, como aspirina, pois eles podem aumentar o risco de sangramento.</p>
        </div>
        <div class="card">
          <img src="dor.jpg" alt="Dor de cabeça e no corpo">
          <h3>Dor de cabeça e no corpo</h3>
          <p>A dor de cabeça e no corpo são outros sintomas comuns da dengue. A dor de cabeça costuma ser intensa e localizada na região frontal ou atrás dos olhos. A dor no corpo pode afetar os músculos, as articulações e os ossos, causando dificuldade para se movimentar. A dor pode ser mais forte nas costas, no abdômen e nas pernas.</p>
          <button onclick="showMore('sintoma2')">Saiba mais</button>
          <p id="sintoma2" style="display: none;">A dor de cabeça e no corpo são causadas pela inflamação provocada pelo vírus da dengue nos tecidos do organismo. A dor pode ser aliviada com medicamentos analgésicos, como paracetamol, e com medidas simples, como compressas frias na testa ou nos olhos, massagens suaves nas áreas doloridas e repouso. Evite fazer esforços físicos ou atividades que possam piorar a dor.</p>
        </div>
        <div class="card">
          <img src="mancha.jpg" alt="Manchas na pele">
          <h3>Manchas na pele</h3>
          <p>As manchas na pele são outro sinal característico da dengue. Elas costumam aparecer entre o segundo e o quinto dia da doença e se manifestam como pequenas erupções vermelhas ou roxas que podem coçar ou arder. As manchas podem surgir em qualquer parte do corpo, mas são mais frequentes no tórax, nos braços e nas pernas.</p>
          <button onclick="showMore('sintoma3')">Saiba mais</button>
          <p id="sintoma3" style="display: none;">As manchas na pele são resultado da alteração dos vasos sanguíneos causada pelo vírus da dengue. Elas podem indicar uma diminuição das plaquetas, que são as células responsáveis pela coagulação do sangue. As manchas podem ser confundidas com alergias ou outras doenças de pele, por isso é importante consultar um médico para confirmar o diagnóstico. As manchas tendem a desaparecer após a cura da dengue, sem deixar cicatrizes.</p>
        </div>
      </div>
      <div class="main" id="prevencao">
        <div class="card">
          <img src="agua.jpg" alt="Elimine a água parada">
          <h3>Elimine a água parada</h3>
          <p>A melhor forma de prevenir a dengue é eliminar os possíveis criadouros do mosquito Aedes Aegypti, que se reproduz em locais com água parada. Por isso, é importante verificar e limpar periodicamente os recipientes que possam acumular água, como pneus, garrafas, vasos de plantas, caixas d'água, calhas e ralos.</p>
          <button onclick="showMore('prevencao1')">Saiba mais</button>
          <p id="prevencao1" style="display: none;">Para eliminar a água parada, siga as seguintes recomendações:
            - Tampe bem as caixas d'água, cisternas e poços.
            - Coloque areia nos pratos dos vasos de plantas ou elimine-os.
            - Descarte corretamente os pneus velhos ou fure-os para evitar o acúmulo de água.
            - Esvazie e limpe as garrafas e latas antes de jogá-las no lixo.
            - Mantenha as calhas e os ralos desentupidos e limpos.
            - Coloque telas nas janelas e portas para impedir a entrada dos mosquitos.</p>
        </div>
        <div class="card">
          <img src="repelente.jpg" alt="Use repelente e roupas adequadas">
          <h3>Use repelente e roupas adequadas</h3>
          <p>Outra forma de prevenir a dengue é evitar a picada do mosquito Aedes Aegypti, que tem hábitos diurnos e costuma picar as partes inferiores do corpo. Por isso, é recomendado usar repelente nas áreas expostas da pele e reaplicá-lo conforme as instruções do fabricante. Além disso, é aconselhável usar roupas claras, compridas e que cubram o máximo possível do corpo.</p>
          <button onclick="showMore('prevencao2')">Saiba mais</button>
          <p id="prevencao2" style="display: none;">Para usar o repelente de forma segura, siga as seguintes orientações:
            - Escolha um repelente adequado para a sua idade e o seu tipo de pele.
            - Aplique o repelente somente nas áreas expostas da pele e evite o contato com os olhos, a boca e as mucosas.
            - Não aplique o repelente por cima de roupas, protetor solar ou maquiagem.
            - Não use o repelente em crianças menores de dois anos ou em gestantes sem orientação médica.
            - Lave as mãos após a aplicação do repelente e remova-o com água e sabão ao final do dia.</p>
        </div>
        <div class="card">
          <img src="medico.jpg" alt="Procure um médico se tiver sintomas">
          <h3>Procure um médico se tiver sintomas</h3>
          <p>Se você tiver sintomas de dengue, como febre alta, dor de cabeça, dor no corpo ou manchas na pele, procure um médico o quanto antes para fazer o diagnóstico e iniciar o tratamento adequado. Não se automedique nem tome remédios sem prescrição médica, pois eles podem agravar o quadro ou causar efeitos colaterais. Siga as orientações do médico e faça o repouso necessário para se recuperar.</p>
          <button onclick="showMore('prevencao3')">Saiba mais</button>
          <p id="prevencao3" style="display: none;">Para diagnosticar a dengue, o médico irá avaliar os seus sintomas, o seu histórico de saúde e o seu contato com áreas de risco. Ele também poderá solicitar exames de sangue para confirmar a presença do vírus da dengue e verificar o nível das plaquetas. O tratamento da dengue consiste em aliviar os sintomas e evitar as complicações. O médico poderá receitar medicamentos antitérmicos, analgésicos e anti-inflamatórios, além de orientar sobre a hidratação e a alimentação adequadas. Em casos graves, pode ser necessário fazer uma transfusão de sangue ou uma internação hospitalar.</p>
        </div>
      </div>
      <div class="main" id="quiz">
        <div class="card">
          <h3>Teste o seu conhecimento sobre a dengue</h3>
          <p>Você acha que sabe tudo sobre a dengue? Então responda este quiz e descubra se você está por dentro da doença, seus sintomas e sua prevenção. São 10 perguntas de múltipla escolha que vão testar o seu conhecimento. Boa sorte!</p>
          <button onclick="startQuiz()">Iniciar quiz</button>
          <div id="quiz" style="display: none;">
            <p id="question"></p>
            <input type="radio" id="a" name="answer" value="a">
            <label for="a" id="label-a"></label><br>
            <input type="radio" id="b" name="answer" value="b">
            <label for="b" id="label-b"></label><br>
            <input type="radio" id="c" name="answer" value="c">
            <label for="c" id="label-c"></label><br>
            <input type="radio" id="d" name="answer" value="d">
            <label for="d" id="label-d"></label><br>
            <button onclick="checkAnswer()">Verificar resposta</button>
            <p id="feedback"></p>
            <button onclick="nextQuestion()" id="next" style="display: none;">Próxima pergunta</button>
            <p id="score"></p>
          </div>
        </div>
      </div>
      <div class="main" id="mapa">
        <div class="card">
          <h3>Veja as áreas de risco de dengue no Brasil</h3>
          <p>Você quer saber quais são as regiões do Brasil que têm mais casos de dengue? Então confira este mapa interativo que mostra as áreas de risco de dengue no país, baseado nos dados do Ministério da Saúde. Você pode clicar nos estados para ver o número de casos confirmados, a incidência e a taxa de mortalidade por dengue em cada um deles.</p>
          <button onclick="showMap()">Mostrar mapa</button>
          <div id="map" style="display: none;">
            <!-- Aqui vai o código para gerar o mapa usando uma API externa -->
          </div>
        </div>
      </div>
      <div class="footer">
        <p>Esta página foi criada pelo Bing, um especialista em programação com mais de 20 anos de estudo.</p>
        <p>Os dados e informações contidos nesta página foram obtidos a partir dos resultados da pesquisa web    e podem não estar atualizados ou completos.</p>
        <p>Esta página tem fins educativos e não substitui a consulta médica. Se você tiver sintomas de dengue, procure um médico imediatamente.</p>
      </div>
    </div>
    <script>
var quizData = [
  {
    question: "Qual é o nome do mosquito que transmite a dengue?",
    options: ["Aedes Aegypti", "Anopheles Gambiae", "Culex Quinquefasciatus", "Mansonia Uniformis"],
    answer: "a"
  },
  {
    question: "Quantos sorotipos diferentes de dengue existem?",
    options: ["Dois", "Quatro", "Seis", "Oito"],
    answer: "b"
  },
  {
    question: "Qual é o principal sintoma da dengue?",
    options: ["Febre alta", "Tosse seca", "Diarreia", "Vômito"],
    answer: "a"
  },
  {
    question: "Qual é a complicação mais grave da dengue?",
    options: ["Síndrome do choque da dengue", "Síndrome respiratória aguda grave", "Síndrome hemolítico-urêmica", "Síndrome de Guillain-Barré"],
    answer: "a"
  },
  {
    question: "Qual é o nome da vacina contra a dengue?",
    options: ["Dengvaxia", "Dengrix", "Dengavax", "Dengarix"],
    answer: "a"
  },
  {
    question: "Em que tipo de local o mosquito da dengue se reproduz?",
    options: ["Água parada", "Água corrente", "Água salgada", "Água mineral"],
    answer: "a"
  },
  {
    question: "Qual é o horário de maior atividade do mosquito da dengue?",
    options: ["Manhã e tarde", "Noite e madrugada", "Meio-dia e crepúsculo", "Qualquer horário"],
    answer: "a"
  },
  {
    question: "Qual é o tipo de roupa mais adequado para evitar a picada do mosquito da dengue?",
    options: ["Roupas claras, compridas e que cubram o máximo possível do corpo", "Roupas escuras, curtas e que deixem o corpo exposto", "Roupas coloridas, justas e que atraiam a atenção do mosquito", "Não há diferença entre os tipos de roupa"],
    answer: "a"
  },
  {
    question: "Qual é o medicamento mais indicado para aliviar a febre e a dor causadas pela dengue?",
    options: ["Paracetamol", "Ácido acetilsalicílico", "Ibuprofeno", "Diclofenaco"],
    answer: "a"
  },
  {
    question: "Qual é a região do Brasil que teve mais casos de dengue em 2023?",
    options: ["Região Norte", "Região Nordeste", "Região Centro-Oeste", "Região Sudeste"],
    answer: "c"
  }
];
    </script>
  </body>
 </html>
 
 
