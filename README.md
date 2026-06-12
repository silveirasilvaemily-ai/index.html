<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Agrinho 2026 - Agricultura Forte do Norte do Paraná</title>

<!-- Fonte moderna -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
/* Reset e fonte */
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;}
html{scroll-behavior:smooth;}
body{background:linear-gradient(180deg,#f8fff8,#eef8ee);color:#333;}

/* Header Hero */
header{
    min-height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    color:white;
    background:
    linear-gradient(rgba(0,0,0,.45),rgba(0,0,0,.45)),
    url("https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1600");
    background-size:cover;
    background-position:center;
}
header h1{font-size:4rem;margin-bottom:15px;text-shadow:2px 2px 10px rgba(0,0,0,.4);}
header p{font-size:1.4rem;}

/* Navegação */
nav{
    position:sticky;
    top:0;
    z-index:999;
    background:rgba(0,0,0,.8);
    backdrop-filter:blur(12px);
    padding:18px;
    text-align:center;
}
nav a{
    color:white;
    text-decoration:none;
    margin:0 20px;
    font-weight:600;
    transition:.3s;
}
nav a:hover, nav a:focus{
    color:#7cff7c;
    outline:3px dashed #7cff7c;
    outline-offset:4px;
}

/* Seções */
section{padding:80px 10%;}
.titulo{text-align:center;font-size:2.5rem;margin-bottom:40px;color:#146b14;}
.card{
    background:rgba(255,255,255,.7);
    backdrop-filter:blur(15px);
    border:1px solid rgba(255,255,255,.4);
    border-radius:25px;
    padding:35px;
    box-shadow:0 15px 30px rgba(0,0,0,.08);
    transition:.4s;
}
.card:hover{transform:translateY(-8px);}

/* Imagens */
.hero-img{
    width:100%;
    border-radius:25px;
    margin-top:25px;
    box-shadow:0 20px 40px rgba(0,0,0,.15);
}

/* Grid de números */
.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
    margin-top:40px;
}
.info-box{
    background:white;
    border-radius:20px;
    padding:30px;
    text-align:center;
    box-shadow:0 10px 20px rgba(0,0,0,.08);
    transition:.3s;
}
.info-box:hover{transform:scale(1.05);}
.info-box h3{font-size:3rem;}
.info-box h4{margin-top:10px;color:#146b14;}
.info-box p{margin-top:5px;color:#555;}

/* Botão moderno */
.botao{
    background:linear-gradient(135deg,#0e8d0e,#3ac93a);
    color:white;
    border:none;
    padding:15px 30px;
    border-radius:50px;
    cursor:pointer;
    margin-top:20px;
    font-size:1rem;
    font-weight:600;
    transition:.3s;
}
.botao:hover{transform:scale(1.05);}

/* Emojis */
.emoji{
    font-size:3.5rem;
    cursor:pointer;
    margin:15px;
    transition:.3s;
}
.emoji:hover{transform:translateY(-10px) scale(1.2);}
#resultado,.fato{margin-top:20px;font-size:1.2rem;color:#146b14;font-weight:600;}

/* Footer */
footer{
    background:#0b3f0b;
    color:white;
    text-align:center;
    padding:40px;
}
.autoria{margin-top:10px;opacity:.8;}

/* Responsivo */
@media(max-width:768px){
    header h1{font-size:2.5rem;}
    header p{font-size:1rem;}
    section{padding:60px 5%;}
    nav a{display:block;margin:10px 0;}
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
    <img class="hero-img" src="https://images.unsplash.com/photo-1447933601403-0c6688de566e?q=80&w=1200" alt="Plantação de café em Pinhalão, Paraná">
    <div class="card">
        <p>Localizado no Norte Pioneiro do Paraná, Pinhalão se destaca pela produção agrícola, especialmente o café. O trabalho dedicado dos produtores locais fortalece a economia e preserva tradições.</p>
    </div>
</section>

<section id="cafe">
    <h2 class="titulo">☕ O Café que Move Nossa Região</h2>
    <div class="card">
        <p>O café é uma das principais riquezas do Norte do Paraná. O clima e o solo contribuem para a produção de cafés de alta qualidade, reconhecidos nacional e internacionalmente.</p>
        <button class="botao" onclick="mostrarFato()">Descobrir Curiosidade do Café</button>
        <div class="fato" id="fato"></div>
    </div>
</section>

<section>
<h2 class="titulo">📊 Agricultura em Números</h2>
<div class="grid">
<div class="info-box">
<h3>☕</h3>
<h4>Café Especial</h4>
<p>Reconhecido internacionalmente.</p>
</div>
<div class="info-box">
<h3>🚜</h3>
<h4>Tecnologia</h4>
<p>Máquinas modernas ajudam a produção.</p>
</div>
<div class="info-box">
<h3>🌱</h3>
<h4>Sustentabilidade</h4>
<p>Produção com responsabilidade ambiental.</p>
</div>
</div>
</section>

<section id="vivencie">
    <h2 class="titulo">🚜 Vivencie a Agricultura</h2>
    <div class="card">
        <p>A agricultura influencia nossa alimentação, gera empregos e impulsiona o desenvolvimento da região. Valorizar o trabalho do campo é reconhecer sua importância para a sociedade.</p>
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
    <p>Projeto Agrinho 2026 🌱☕<br>Agricultura Forte do Norte do Paraná</p>
    <p class="autoria">Feito por uma estudante do <strong>Colégio Estadual Leonardo Francisco Nogueira</strong></p>
</footer>

<script>
const fatos=[
"☕ O Brasil é o maior produtor de café do mundo.",
"🌱 O cafeeiro pode produzir por muitos anos quando bem cuidado.",
"🚜 A agricultura gera milhares de empregos no Paraná.",
"☕ O Norte Pione
