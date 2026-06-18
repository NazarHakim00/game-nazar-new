<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NAZA - Pixel Game</title>

<style>
body{
    margin:0;
    background:#222;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    font-family:monospace;
}

#game{
    position:relative;
    width:400px;
    height:600px;
    background:#87CEEB;
    overflow:hidden;
    border:4px solid #000;
    image-rendering: pixelated;
}

#player{
    position:absolute;
    width:32px;
    height:32px;
    background:#0066ff;
    left:184px;
    top:540px;
    box-shadow:
        8px 0 #003399,
        -8px 0 #3399ff;
}

.enemy{
    position:absolute;
    width:32px;
    height:32px;
    background:#ff3333;
}

#score{
    position:absolute;
    top:10px;
    left:10px;
    font-size:22px;
    color:#000;
    font-weight:bold;
}

#title{
    position:absolute;
    top:10px;
    right:10px;
    font-size:22px;
    color:#000;
    font-weight:bold;
}

#gameOver{
    position:absolute;
    width:100%;
    top:50%;
    transform:translateY(-50%);
    text-align:center;
    font-size:32px;
    color:#fff;
    display:none;
    background:rgba(0,0,0,0.7);
    padding:20px 0;
}
</style>
</head>
<body>

<div id="game">
    <div id="score">0</div>
    <div id="title">NAZA</div>
    <div id="player"></div>
    <div id="gameOver">GAME OVER<br>Tekan F5</div>
</div>

<script>
const game = document.getElementById("game");
const player = document.getElementById("player");
const scoreText = document.getElementById("score");
const gameOverText = document.getElementById("gameOver");

let playerX = 184;
let score = 0;
let gameOver = false;

const keys = {};

document.addEventListener("keydown", e => {
    keys[e.key] = true;
});

document.addEventListener("keyup", e => {
    keys[e.key] = false;
});

function createEnemy(){
    if(gameOver) return;

    const enemy = document.createElement("div");
    enemy.classList.add("enemy");

    const x = Math.random() * 368;
    enemy.style.left = x + "px";
    enemy.style.top = "-32px";

    game.appendChild(enemy);

    let y = -32;

    const moveEnemy = setInterval(() => {
        if(gameOver){
            clearInterval(moveEnemy);
            return;
        }

        y += 5;
        enemy.style.top = y + "px";

        const enemyRect = enemy.getBoundingClientRect();
        const playerRect = player.getBoundingClientRect();

        if(
            enemyRect.left < playerRect.right &&
            enemyRect.right > playerRect.left &&
            enemyRect.top < playerRect.bottom &&
            enemyRect.bottom > playerRect.top
        ){
            gameOver = true;
            gameOverText.style.display = "block";
        }

        if(y > 600){
            score++;
            scoreText.textContent = score;
            enemy.remove();
            clearInterval(moveEnemy);
        }

    }, 20);
}

setInterval(createEnemy, 900);

function gameLoop(){
    if(gameOver) return;

    if(keys["ArrowLeft"] && playerX > 0){
        playerX -= 6;
    }

    if(keys["ArrowRight"] && playerX < 368){
        playerX += 6;
    }

    player.style.left = playerX + "px";

    requestAnimationFrame(gameLoop);
}

gameLoop();
</script>

</body>
</html>
