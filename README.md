<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>🎅 Prank de Noël</title>

<style>
    body {
        margin: 0;
        height: 100vh;
        background: #111;
        color: white;
        font-family: Arial, sans-serif;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        overflow: hidden;
    }

    h1 {
        color: red;
        text-align: center;
        font-size: 2em;
    }

    p {
        color: #ddd;
    }

    #btn {
        position: absolute;
        padding: 15px 25px;
        background: green;
        border: none;
        color: white;
        font-size: 18px;
        border-radius: 10px;
        cursor: pointer;
        transition: 0.1s;
    }
</style>
</head>

<body>

<h1>🎅 Tu n’as pas été sage cette année...</h1>
<p>Pour quitter cette page, clique sur : <b>ÊTRE SAGE</b></p>

<button id="btn">ÊTRE SAGE</button>

<script>
const btn = document.getElementById("btn");

function moveButton() {
    const x = Math.random() * (window.innerWidth - 120);
    const y = Math.random() * (window.innerHeight - 60);

    btn.style.left = x + "px";
    btn.style.top = y + "px";
}

// le bouton fuit quand tu approches
btn.addEventListener("mouseover", moveButton);
btn.addEventListener("touchstart", moveButton);

// petit démarrage
moveButton();
</script>

</body>
</html>
