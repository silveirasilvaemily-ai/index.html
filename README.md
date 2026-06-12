<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Agrinho 2026 - Agricultura Forte do Norte do Paraná</title>

<style>
/* Reset e fonte */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, Helvetica, sans-serif;
}

body {
    background: #fff5f5;
    color: #333;
}

/* Header */
header {
    background: linear-gradient(135deg,#8b0000,#c62828,#ff5252);
    color: white;
    text-align: center;
    padding: 60px 20px;
}

header h1 {
    font-size: 3rem;
}

header p {
    margin-top: 15px;
    font-size: 1.2rem;
}

/* Navegação */
nav {
    background: #7a0000;
    padding: 15px;
    text-align: center;
}

nav a {
    color: white;
    text-decoration: none;
    margin: 15px;
    font-weight: bold;
}

nav a:hover, nav a:focus {
    text-decoration: underline;
    outline: 3px dashed #ff5252;
    outline-offset: 4px;
}

/* Seções */
section {
    padding: 50px 10%;
}

.titulo {
    color: #a30000;
    margin-bottom: 20px;
    font-size: 2rem;
    text-align: center;
}

/* Imagens */
.hero-img {
    width: 100%;
    max-width: 900px;
    display: block;
    margin: 20px auto;
    border-radius: 20px;
    box-shadow: 0 0 20px rgba(0,0,0,0.3);
}

/* Cards */
.card {
    background: white;
    padding: 25px;
    border-radius: 15px;
    margin-top: 20px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

/* Emojis */
.emoji-area {
    text-align: center;
    margin-top: 30px;
}

.emoji {
    font-size: 3rem;
    cursor: pointer;
    transition: 0.3s;
    margin: 10px;
}

.emoji:hover, .emoji:focus {
    transform: scale(1.3);
    outline: none;
}

#resultado {
    margin-top: 20px;
    font-size: 1.4rem;
    color: #8b0000;
    font-weight: bold;
}

/* Botão */
.botao {
    background: #c62828;
    color: white;
    border: none;
    padding: 15px 25px;
    border-radius: 10px;
    cursor: pointer;
    font-size: 1rem;
    margin-top: 20px;
}

.botao:hover, .botao:focus {
    background: #8b0000;
    outline: none;
}

/* Fatos */
.fato {
    margin-top: 20px;
    font-size: 1.1rem;
    color: #6d0000;
    font-weight: bold;
}

/* Footer */
footer {
    background: #8b0000;
    color: white;
    text-align: center;
    padding: 25px;
}

.autoria {
    margin-top: 10px;
    font-size: 0.9rem;
    color: #500000;
    text-align: center;
}

/* Responsividade */
@media (max-width: 768px) {
    header h1 {
        font-size: 2.2rem;
    }

    header p {
        font-size: 1rem;
    }

    nav a {
        display: block;
        margin: 10px 0;
    }

    section {
        padding: 30px 5%;
    }

    .hero-img {
        width: 100%;
        margin: 15px auto;
    }
}
</style>
</head>

<body>

<header>
    <h1>🌱 AGRINHO 2026</h1>
    <p>Agricultura Forte do Norte do Paraná</p>
</header>

<nav>
    <a href="#pinhalao">Pinhalão</a>
    <a href="#cafe">Café</a>
    <a href="#vivencie">Vivencie</a>
</nav>

<section id="pinhalao">
    <h2 class="titulo">📍 Pinhalão - Terra do Café</h2>

    <img class="hero-img"
         src="https://images.unsplash.com/photo-1447933601403-0c6688de566e?q=80&w=1200"
         alt="Plantação de café em Pinhalão, Paraná">

    <div class="card">
        <p>
            Localizado no Norte Pioneiro do Paraná, Pinhalão se destaca pela
            produção agrícola, especialmente o café. O trabalho dedicado dos
            produtores locais fortalece a economia e preserva tradições.
        </p>
    </div>
</section>

<section id="cafe">
    <h2 class="titulo">☕ O Café que Move Nossa Região</h2>

    <div class="card">
        <p>
            O café é uma das principais riquezas do Norte do Paraná. O clima
            e o solo contribuem para a produção de cafés de alta qualidade,
            reconhecidos nacional e internacionalmente.
        </p>

        <button class="botao" onclick="mostrarFato()">Descobrir Curiosidade do Café</button>
        <div class="fato" id="fato"></div>
    </div>
</section>

<section id="vivencie">
    <h2 class="titulo">🚜 Vivencie a Agricultura</h2>

    <div class="card">
        <p>
            A agricultura influencia nossa alimentação, gera empregos e
            impulsiona o desenvolvimento da região. Valorizar o trabalho do
            campo é reconhecer sua importância para a sociedade.
        </p>

        <div class="emoji-area">
            <h3>O que você achou do tema?</h3>

            <span class="emoji" role="button" tabindex="0" onclick="votar('😍')" onkeypress="if(event.key==='Enter') votar('😍')">😍</span>
            <span class="emoji" role="button" tabindex="0" onclick="votar('☕')" onkeypress="if(event.key==='Enter') votar('☕')">☕</span>
            <span class="emoji" role="button" tabindex="0" onclick="votar('🌱')" onkeypress="if(event.key==='Enter') votar('🌱')">🌱</span>
            <span class="emoji" role="button" tabindex="0" onclick="votar('🚜')" onkeypress="if(event.key==='Enter') votar('🚜')">🚜</span>

            <div id="resultado"></div>
        </div>
    </div>
</section>

<footer>
    <p>
        Projeto Agrinho 2026 🌱☕<br>
        Agricultura Forte do Norte do Paraná
    </p>
    <p class="autoria">
        Feito por uma estudante do <strong>Colégio Estadual Leonardo Francisco Nogueira</strong>
    </p>
</footer>

<script>
/* Fatos sobre café e agricultura */
const fatos = [
    "☕ O Brasil é o maior produtor de café do mundo.",
    "🌱 O cafeeiro pode produzir por muitos anos quando bem cuidado.",
    "🚜 A agricultura gera milhares de empregos no Paraná.",
    "☕ O Norte Pioneiro é conhecido pela qualidade de seus cafés especiais.",
    "🌿 O café faz parte da história econômica do Paraná."
];

let fatosMostrados = [];

function mostrarFato() {
    if(fatosMostrados.length === fatos.length) {
        fatosMostrados = [];
    }
    let restante = fatos.filter(f => !fatosMostrados.includes(f));
    let sorteio = restante[Math.floor(Math.random() * restante.length)];
    fatosMostrados.push(sorteio);
    document.getElementById("fato").innerHTML = sorteio;
}

/* Contagem de votos por emoji */
let votos = {};

function votar(emoji) {
    votos[emoji] = (votos[emoji] || 0) + 1;
    let resultadoTexto = "Você escolheu: " + emoji + " | Total de votos deste emoji: " + votos[emoji];
    document.getElementById("resultado").innerHTML = resultadoTexto;
}
</script>

</body>
</html>
