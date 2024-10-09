<!--Sarah Chalegra 3c- 09/10/2024-->
<!DOCTYPE html>
<html lang="pt-BR">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <link rel="stylesheet" href="style.css">
 <link rel="preconnect" href="https://fonts.googleapis.com">
   <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
   <link href=https://casa.abril.com.br/wp-content/uploads/2019/09/3-5-casas-usadas-em-filmes-de-terror-que-podem-ser-visitadas.png?quality=70&w=1024&crop=1 rel="stylesheet">
<title>O Homem em minha casa</title>
</head>
<body>
<main>
    <div class="passo ativo" id="passo-0">
        <p> Era por volta das 23:45, meu filho me chama e fala: "Mamãe, tem monstros embaixo da minha cama!"</p>
        <button class="btn-proximo" data-proximo="1">Olhar de baixo da cama.</button>
        <button class="btn-proximo" data-proximo="2">Consolar o filho e convencê-lo do contrário.</button>
    </div>
    <div class="passo" id="passo-1">
        <p>Você acaricia seu filho, mas escuta um barunho estranho vindo do guarda-roupas</p>
        <button class="btn-proximo" data-proximo="3">Olhar dentro do guarda-roupas.</button>
        <button class="btn-proximo" data-proximo="4">Esquecer e ir dormir.</button>
    </div>
    <div class="passo" id="passo-2">
        <p>Você olha debaixo da cama e encontra um sapato de pessoa adulta.</p>
        <button class="btn-proximo" data-proximo="5">Jogar o sapato fora.</button>
        <button class="btn-proximo" data-proximo="6">Procurar o dono do Sapato pela casa.</button>
    </div>
    <div class="passo" id="passo-3">
        <p>Você coloca seu filho para dormir e começa a andar pela casa tentando não fazer barulho. </p>
        <button class="btn-proximo" data-proximo="7">Ir em direção ao corredor da sala.</button>
</div>

<div class="passo" id="passo-4">
    <img src=https://img.freepik.com/fotos-gratis/imagem-de-foco-raso-de-uma-mulher-dormindo-em-sua-cama_181624-16042.jpg?t=st=1728486878~exp=1728490478~hmac=4e41ddd54ac43c0aa1fab808c1fdb3dd2bf0d97b502b16f801a8d15ea494253d&w=740>
        <p>Você se cansa de procurar e não achar nada e vai se deitar, se culpando por ter se rendido a um medo bobo e infantil.</p>
</div>

<div class="passo" id="passo-5">
        <p> Você vai até seu quarto e deita na sua cama.</p>
        <button class="btn-proximo" data-proximo="7" Ir até a rua </button>
</div>

<div class="passo" id="passo-6">
        <p>Você tenta pegar no sono, mas o barulho da porta abrindo te assusta.</p>
        <button class="btn-proximo" data-proximo="8">Olhar em direção a porta para tentar ver algo.</button>
</div>

<div class="passo" id="passo-7">
        <p>O vulto de um homem grande começa a se aproximar de você.</p>
        <button class="btn-proximo" data-proximo="9">Gritar e tentar correr para salvar seu filho.</button>
        <button class="btn-proximo" data-proximo="10">Se manter quieta e tentar ligar para a polícia.</button>
</div>

<div class="passo" id="passo-8">
        <p>O homem consegue chegar até você e tampar sua boca.</p>
        <button class="btn-proximo" data-proximo="7">Manter a calma.</button>
</div>

<div class="passo" id="passo-9">
        <p>Um soco certeiro pode te dar tempo para correr.</p>
        <button class="btn-proximo" data-proximo="11">Dar um soco.</button>
</div>

<div class="passo" id="passo-10">
        <p>Ficar obediete pode fazer ele te liberar sem muitos danos.</p>
        <button class="btn-proximo" data-proximo="12">Obedecer e cooperar.</button>
</div>

<div class="passo" id="passo-11">
        <p>Ele te mata com facadas na garganta, coração e pernas. 
            Seu filho acorda com os gritos e vai ao seu quarto, te encontra na cama toda ensanguentada e se assusta.</p>
</div>

<div class="passo" id="passo-12">
        <p>É seu fim, e seu filho foi morto logo em segida. </p>
        <p>"E pensar que tudo poderia ser evitado se eu não tivesse chigado ele naquela tarde chuvosa."</p>
        <button class="btn-proximo" data-proximo="11">Explorar o ovni</button>
</div>
    </main>
    <script src="script.js"></script>
</body>
</html>>
............................................................................................................................................

const avanca = document.querySelectorAll('.btn-proximo');
avanca.forEach(button => {
    button.addEventListener('click', function(){
        const atual = document.querySelector('.ativo');
        const proximoPasso = 'passo-' + this.getAttribute('data-proximo');
        atual.classList.remove('ativo');
        document.getElementById(proximoPasso).classList.add('ativo');
    })
})
..............................................................................................................................................
body {
    background-color: #1D4221;
    color: white;
    font-family: "Bai Jamjuree", sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 700px;
    margin: 0;
}
button {
    background-color: #64A712;
    color: white;
    font-family: "Bai Jamjuree", sans-serif;
}
.passo {
    display: none;
}
.passo.ativo {
    display:block;
}
main {
    text-align: center;
    max-width: 90%;
}
img {
    max-width: 90%;
}
..............................................................................................................................................
