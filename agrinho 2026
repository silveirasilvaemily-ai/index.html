<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Agro Forte Sustentável - Pinhalão Paraná</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<style>
/* Reset e fonte */
* {margin:0; padding:0; box-sizing:border-box; font-family:'Poppins',sans-serif;}
html {scroll-behavior:smooth;}
body {background:#fff5f5; color:#333; overflow-x:hidden;}

/* Header com gradiente animado */
@keyframes gradientBG {
    0% {background-position:0% 50%;}
    50% {background-position:100% 50%;}
    100% {background-position:0% 50%;}
}
header {
    min-height:70vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    color:white;
    background: linear-gradient(-45deg, #8b0000, #ff5252, #228b22, #32cd32);
    background-size: 400% 400%;
    animation: gradientBG 15s ease infinite;
}
header h1 {font-size:4rem; margin-bottom:10px; text-shadow:2px 2px 15px rgba(0,0,0,.5);}
header p {font-size:1.5rem; text-shadow:1px 1px 10px rgba(0,0,0,.4);}

/* Navegação */
nav {
    background: rgba(139,0,0,0.9);
    text-align:center;
    padding:15px;
    position:sticky;
    top:0;
    z-index:999;
}
nav a {
    color:white;
    text-decoration:none;
    margin:0 15px;
    font-weight:600;
    transition:.3s;
}
nav a:hover, nav a:focus {color:#32cd32; outline:2px dashed #32cd32; outline-offset:4px;}

/* Seções */
section {padding:60px 10%;}
.titulo {text-align:center; font-size:2.8rem; margin-bottom:40px; color:#8b0000;}

/* Cards com efeito 3D */
.card {
    background:rgba(255,255,255,0.9);
    border-radius:25px;
    padding:30px;
    margin-bottom:30px;
    box-shadow:0 15px 30px rgba(0,0,0,.15);
    transition:.5s;
    transform-style: preserve-3d;
}
.card:hover {
    transform: rotateX(2deg) rotateY(2deg) scale(1.03);
    box-shadow:0 25px 40px rgba(0,0,0,.25);
}

/* Imagem */
.hero-img {
    width:100%;
    max-width:900px;
    display:block;
    margin:20px auto;
    border-radius:20px;
    box-shadow:0 20px 40px rgba(0,0,0,.25);
}

/* Emojis interativos */
.emoji-area {text-align:center; margin-top:30px;}
.emoji {
    font-size:3.2rem;
    cursor:pointer;
    margin:15px;
    transition:.3s;
    display:inline-block;
}
.emoji:hover {transform:scale(1.5);}
@keyframes bounce {
    0%,100% {transform: translateY(0);}
    50% {transform: translateY(-15px);}
}
.bounce {animation:bounce 0.5s;}

/* Botão com gradiente animado */
.botao {
    background: linear-gradient(135deg,#8b0000,#ff5252,#32cd32,#228b22);
    background-size:400% 400%;
    color:white;
    border:none;
    padding:15px 35px;
    border-radius:50px;
    cursor:pointer;
    margin-top:20px;
    font-size:1rem;
    font-weight:600;
    transition:.3s;
    animation: gradientBG 10s ease infinite;
}
.botao:hover {transform:scale(1.1);}

/* Resultado e curiosidade */
#resultado, #fato {
    margin-top:20px; 
    font-size:1.2rem; 
    font-weight:bold; 
    color:#8b0000;
}

/* Footer */
footer {
    background:#8b0000;
    color:white;
    text-align:center;
    padding:35px 10%;
}
.autoria {margin-top:10px; font-size:0.9rem; opacity:.8;}

/* Responsivo */
@media(max-width:768px){
    header h1 {font-size:2.5rem;}
    header p {font-size:1rem;}
    section {padding:40px 5%;}
    nav a {display:block; margin:10px 0;}
}
</style>
</head>

<body>

<header>
    <h1>🌱 Agro Forte Sustentável</h1>
    <p>Pinhalão - Paraná, Terra do Café</p>
</header>

<nav>
    <a href="#pinhalao">Pinhalão</a>
    <a href="#cafe">Café</a>
    <a href="#interacao">Interação</a>
</nav>

<section id="pinhalao">
    <h2 class="titulo">📍 Pinhalão - Terra do Café</h2>
    <img class="hero-img" src="https://images.unsplash.com/photo-1509042239860-f550ce710b93?q=80&w=1200" alt="Plantação de café em Pinhalão">
    <div class="card">
        <p>Pinhalão é conhecida por sua agricultura forte e sustentável, especialmente a produção de café de alta qualidade. Produtores locais combinam tradição e inovação, cuidando do solo e do meio ambiente.</p>
    </div>
</section>

<section id="cafe">
    <h2 class="titulo">☕ Café que Move a Região</h2>
    <div class="card">
        <p>O café produzido em Pinhalão é reconhecido nacional e internacionalmente. O clima, solo fértil e técnicas agrícolas modernas garantem sabor e sustentabilidade.</p>
        <button class="botao" onclick="mostrarFato()">Descobrir Curiosidade do Café</button>
        <div id="fato"></div>
    </div>
</section>

<section id="interacao">
    <h2 class="titulo">💬 Interaja Conosco</h2>
    <div class="card">
        <p>O que você achou do tema Agro Forte Sustentável?</p>
        <div class="emoji-area">
            <span class="emoji" onclick="votar(this,'😍')">😍</span>
            <span class="emoji" onclick="votar(this,'☕')">☕</span>
            <span class="emoji" onclick="votar(this,'🌱')">🌱</span>
            <span class="emoji" onclick="votar(this,'🚜')">🚜</span>
        </div>
        <div id="resultado"></div>
    </div>
</section>

<footer>
    <p>Projeto feito por uma aluna do <strong>Colégio Leonardo Francisco Nogueira</strong></p>
    <p class="autoria">🌱 Agro Forte Sustentável - Pinhalão, Paraná</p>
</footer>

<script>
// Curiosidades do café
const fatos = [
    "☕ O Brasil é o maior produtor de café do mundo.",
    "🌱 O cafeeiro pode produzir por muitos anos quando bem cuidado.",
    "🚜 A agricultura gera empregos e fortalece a região.",
    "☕ O Norte do Paraná é conhecido pela qualidade dos cafés especiais."
];
let fatosMostrados = [];
function mostrarFato(){
    if(fatosMostrados.length===fatos.length) fatosMostrados=[];
    let restante = fatos.filter(f=>!fatosMostrados.includes(f));
    let sorteio = restante[Math.floor(Math.random()*restante.length)];
    fatosMostrados.push(sorteio);
    document.getElementById("fato").innerHTML = sorteio;
}

// Emojis interativos com efeito bounce
let votos = {};
function votar(elemento, emoji){
    votos[emoji] = (votos[emoji]||0)+1;
    elemento.classList.add('bounce');
    setTimeout(()=>elemento.classList.remove('bounce'),500);
    document.getElementById("resultado").innerHTML = `Você escolheu: ${emoji} | Total de votos deste emoji: ${votos[emoji]}`;
}
</script>

</body>
</html>
