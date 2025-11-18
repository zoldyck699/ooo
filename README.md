
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Para ti, pequeña</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
    body {
        margin: 0;
        background: #fdf6f0;
        font-family: 'Poppins', sans-serif;
        overflow-x: hidden;
    }

    /* Fondo decorado estilo Snoopy */
    body::before {
        content: "";
        position: fixed;
        inset: 0;
        background: url('https://i.imgur.com/OzFzn2h.png') repeat;
        opacity: 0.13;
        z-index: -1;
    }

    /* CORAZONES CAYENDO */
    .corazon {
        position: fixed;
        top: -20px;
        color: #ff87b4;
        font-size: 18px;
        animation: caer 6s linear infinite;
        opacity: 0.8;
        z-index: 9999;
        pointer-events: none;
    }

    @keyframes caer {
        0% { transform: translateY(-20px) translateX(0); opacity: 1; }
        100% { transform: translateY(110vh) translateX(20px); opacity: 0; }
    }

    .carta {
        max-width: 900px;
        margin: 40px auto;
        background: white;
        padding: 35px;
        border-radius: 20px;
        box-shadow: 0 0 18px rgba(0,0,0,0.15);
        border: 4px dashed #ff9ecb;
        animation: abrirCarta 1.2s ease forwards;
        opacity: 0;
    }

    @keyframes abrirCarta {
        0% { transform: scale(0.75) rotate(-4deg); opacity: 0; }
        100% { transform: scale(1) rotate(0); opacity: 1; }
    }

    .titulo {
        font-size: 2.5rem;
        font-weight: bold;
        text-align: center;
        color: #ff5f8f;
        margin-bottom: 20px;
    }

    .texto {
        font-size: 1.3rem;
        line-height: 1.8;
        text-align: center;
        margin-top: 15px;
    }

    .btn-triste, .btn-secreto {
        margin-top: 30px;
        display: inline-block;
        padding: 15px 28px;
        background: #ff88b8;
        color: white;
        font-size: 1.2rem;
        border-radius: 16px;
        cursor: pointer;
        transition: 0.3s;
        font-weight: bold;
        border: none;
    }

    .btn-triste:hover,
    .btn-secreto:hover {
        background: #ff6aa6;
        transform: scale(1.07);
    }

    #pagina-secreta, #pagina-super-secreta {
        display: none;
        animation: fadeIn 1.1s forwards;
    }

    @keyframes fadeIn {
        from { opacity: 0; }
        to { opacity: 1; }
    }

    .snoopy-center {
        width: 230px;
        display: block;
        margin: 20px auto;
    }

    .audio-box {
        margin-top: 25px;
        text-align: center;
    }

    .imagenes-secretas {
        display: flex;
        justify-content: center;
        gap: 20px;
        flex-wrap: wrap;
        margin-top: 25px;
    }

    .imagenes-secretas img {
        width: 200px;
        border-radius: 14px;
        box-shadow: 0 0 12px rgba(0,0,0,0.15);
    }

</style>

</head>

<body>

<!-- CORAZONES CAYENDO -->
<script>
for (let i = 0; i < 18; i++) {
    let c = document.createElement("div");
    c.classList.add("corazon");
    c.innerHTML = "❤";
    c.style.left = Math.random() * 100 + "vw";
    c.style.animationDuration = 5 + Math.random() * 4 + "s";
    c.style.fontSize = 14 + Math.random() * 20 + "px";
    document.body.appendChild(c);
}
</script>



<!-- PRIMERA PARTE – CARTA PRINCIPAL -->
<div id="pagina-principal" class="carta">

    <h1 class="titulo">Esta página es para ti, pequeña ❤️</h1>

    <p class="texto">
        La hice pensando en esos días en los que te sientes triste, cansada o renegando.  
        Esta página es para recordarte lo increíble que eres, incluso cuando tú misma lo dudas.  
        No quiero que olvides que tienes un corazón hermoso, fuerte y muy especial.
    </p>

    <img src="https://files.catbox.moe/zqwcy9.jfif" class="snoopy-center">

    <p class="texto">
        Eres una persona trabajadora, dedicada, tierna, con un carácter fuerte y un corazón noble.  
        Y aunque a veces te sientas sola en tu cabeza… en mi mundo jamás lo estás, pequeña.
        <br><br>
        Y cuando estés triste… ven aquí.
    </p>

    <div style="text-align:center;">
        <button class="btn-triste" onclick="abrirSecreto()">Presióname si estás triste 💗</button>
    </div>

</div>



<!-- SEGUNDA PARTE – PÁGINA SECRETA -->
<div id="pagina-secreta" class="carta">

    <h1 class="titulo">Ven aquí, pequeña… ❤️</h1>

    <img src="https://files.catbox.moe/g380lr.jfif" class="snoopy-center">

    <p class="texto">
    Si llegaste aquí es porque hoy no tuviste un buen día…  
    Algo te cansó, te fastidió, te dolió o simplemente te puso en un ánimo que tú misma quisieras quitarte.  
    Y está bien, pequeña. No tienes que esconderlo aquí.
    <br><br>

    Quiero que sepas algo antes de seguir leyendo:  
    <strong>tú eres muchísimo más fuerte de lo que piensas</strong>, incluso cuando tu mente te diga lo contrario.  
    No te das cuenta, pero siempre sacas adelante cosas que otras personas ni siquiera intentarían.  

    <br><br>

    Y sí, también eres tierna, intensa, decidida, con un carácter precioso que te hace única.  
    No importa si hoy te salió algo mal, o si dijiste algo que no querías,  
    o si sientes que el mundo te quedó grande…  
    <strong>tú sigues siendo tú, y eso ya vale bastante.</strong>
    <br><br>

    Recuerda esto también:  
    No eres un problema.  
    No eres una carga.  
    No eres “demasiado”.  
    Eres una persona real, con emociones reales, y mereces que alguien te trate con cariño incluso cuando no estás en tu mejor versión.
    <br><br>

    Pequeña, ojalá pudieras ver lo que yo veo cuando te miro de verdad:  
    una chica que sigue adelante incluso cuando está cansada,  
    una chica que lucha por lo suyo,  
    una chica que sin darse cuenta hace los días de los demás un poquito más suaves.
    <br><br>

    Y si hoy no te sientes suficiente…  
    está bien, aquí tienes un espacio donde sí lo eres.
    <br><br>

    Y si nada de esto te ayudó…  
    si sigues sintiendo ese peso en el pecho o ese vacío raro que no se explica…  
    quiero que por lo menos te lleves esto:
    <br><br>

    No tienes que poder con todo.  
    No tienes que tener siempre respuestas.  
    No tienes que fingir que estás bien.
    <br><br>

    Aquí puedes soltar.  
    Aquí puedes fallar.  
    Aquí puedes descansar sin que nadie te juzgue.
    <br><br>

    Porque aunque tu día haya sido feo, aunque tú misma dudes de ti o te sientas chiquita por dentro…  
    <strong>yo no dejo de creer en ti.</strong>  
    Ni hoy, ni mañana, ni en esos días en los que tú misma no sabes qué sentir.

    </p>

    <div class="audio-box">
        <h3>La cancion que te vuelve tu misma 🎧</h3>
        <audio controls autoplay>
            <source src="https://files.catbox.moe/123rae.mp3" type="audio/mpeg">
        </audio>
    </div>

    <div style="text-align:center;">
        <button class="btn-secreto" onclick="abrirSuperSecreto()">Una última cosa… 💞</button>
    </div>

</div>




<!-- TERCERA PARTE – PÁGINA SUPER SECRETA -->
<div id="pagina-super-secreta" class="carta">

    <h1 class="titulo">Si llegaste hasta aquí… 💗</h1>

    <p class="texto">
        Si llegaste aquí quiero que recuerdes que  
        <strong>te quiero mucho, pequeña.</strong>
        <br><br>
        No importa qué tan mal haya sido tu día,  
        yo estoy contigo… aunque sea en una página secreta.
    </p>

    <div class="imagenes-secretas">
        <img src="https://files.catbox.moe/qhfgl1.jpeg">
        <img src="https://files.catbox.moe/qwdn0a.jpeg">
        <img src="https://files.catbox.moe/4joqut.jpeg">
        
    </div>

    <div style="text-align:center; margin-top:30px;">
        <button class="btn-secreto" onclick="volver()">Volver</button>
    </div>

</div>




<script>
function abrirSecreto() {
    document.getElementById("pagina-principal").style.display = "none";
    document.getElementById("pagina-secreta").style.display = "block";
}

function abrirSuperSecreto() {
    document.getElementById("pagina-secreta").style.display = "none";
    document.getElementById("pagina-super-secreta").style.display = "block";
}

function volver() {
    document.getElementById("pagina-super-secreta").style.display = "none";
    document.getElementById("pagina-secreta").style.display = "block";
}
</script>

</body>
</html>


