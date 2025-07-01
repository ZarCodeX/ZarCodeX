<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="icon" type="image/x-icon" href="img/icons/ZarCodeX - Round.png">

    <!-- Page Title -->
    <title>404 - Page Not Found | ZarCodeX</title>

    <!-- Primary Meta Tags -->
    <meta name="description" content="Oops! The page you're looking for doesn't exist. Return to ZarCodeX's portfolio or explore available projects." />
    <meta name="keywords" content="404, page not found, ZarCodeX, error page, portfolio" />
    <meta name="author" content="Muhammad Abuzar (ZarCodeX)" />
    <meta name="robots" content="noindex, follow" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1" />

    <!-- Favicon and Icons -->
    <link rel="icon" href="img/icons/ZarCodeX - Round.png" sizes="any" />
    <link rel="icon" href="img/icons/ZarCodeX - Round.png" type="image/svg+xml" />
    <link rel="apple-touch-icon" href="img/icons/ZarCodeX - Round.png" />

    <!-- Theme Color -->
    <meta name="theme-color" media="(prefers-color-scheme: light)" content="#dcdce7" />
    <meta name="theme-color" media="(prefers-color-scheme: dark)" content="#111111" />
    <meta name="msapplication-navbutton-color" content="#111111" />
    <meta name="apple-mobile-web-app-capable" content="yes" />
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />

    <!-- Open Graph (Social Media Preview) -->
    <meta property="og:type" content="website" />
    <meta property="og:title" content="404 - Page Not Found | ZarCodeX" />
    <meta property="og:description" content="Oops! The page you're looking for doesn't exist. Return to ZarCodeX's portfolio or explore available projects." />
    <meta property="og:url" content="https://zarcodex.github.io/portfolio/404.html" />
    <meta property="og:site_name" content="ZarCodeX Portfolio" />
    <meta property="og:image" content="https://raw.githubusercontent.com/ZarCodeX/zarcodex.github.io/refs/heads/main/img/icons/ZarCodeX - Round.png" />
    <meta property="og:image:secure_url" content="https://raw.githubusercontent.com/ZarCodeX/zarcodex.github.io/refs/heads/main/img/icons/ZarCodeX - Round.png" />
    <meta property="og:image:type" content="image/png" />
    <meta property="og:image:width" content="1200" />
    <meta property="og:image:height" content="1200" />

    <!-- Twitter Card -->
    <meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:title" content="404 - Page Not Found | ZarCodeX" />
    <meta name="twitter:description" content="Page not found. Head back to ZarCodeX's portfolio to discover more projects and content." />
    <meta name="twitter:image" content="https://raw.githubusercontent.com/ZarCodeX/zarcodex.github.io/refs/heads/main/img/icons/ZarCodeX - Round.png" />
    <meta name="twitter:site" content="@ZarCodeX" />

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #001f1a, #003a32);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            color: white;
            padding: 20px;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            width: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 30px;
        }
        
        .header {
            text-align: center;
            padding: 20px;
            animation: fadeIn 1s ease-out;
        }
        
        .header h1 {
            font-size: 8rem;
            font-weight: 800;
            color: #00fff5;
            text-shadow: 0 0 15px rgba(0, 255, 245, 0.5);
            margin-bottom: 10px;
        }
        
        .header h2 {
            font-size: 2.5rem;
            font-weight: 600;
            margin-bottom: 15px;
        }
        
        .header p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto;
            opacity: 0.8;
            line-height: 1.6;
        }
        
        .game-container {
            position: relative;
            background: rgba(0, 0, 0, 0.3);
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            max-width: 500px;
            width: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;
            border: 2px solid #00fff5;
        }
        
        .game-header {
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 10px;
        }
        
        .score-container {
            display: flex;
            gap: 20px;
        }
        
        .score-box {
            background: rgba(0, 255, 245, 0.1);
            padding: 8px 15px;
            border-radius: 8px;
            border: 1px solid #00fff5;
        }
        
        .game-canvas {
            background: rgba(0, 0, 0, 0.5);
            border-radius: 8px;
            display: block;
            width: 100%;
            max-width: 400px;
            height: 300px;
            border: 1px solid #00fff5;
        }
        
        .controls {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
            margin-top: 10px;
        }
        
        .control-btn {
            background: rgba(0, 255, 245, 0.15);
            color: white;
            border: 1px solid #00fff5;
            padding: 8px 15px;
            border-radius: 6px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 500;
        }
        
        .control-btn:hover {
            background: rgba(0, 255, 245, 0.3);
            transform: translateY(-2px);
        }
        
        .home-button {
            background: linear-gradient(45deg, #00a69c, #00fff5);
            color: #003a32;
            border: none;
            padding: 14px 40px;
            font-size: 1.2rem;
            font-weight: 600;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 255, 245, 0.3);
            margin-top: 20px;
            text-decoration: none;
            display: inline-block;
        }
        
        .home-button:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 255, 245, 0.5);
        }
        
        .game-instructions {
            background: rgba(0, 0, 0, 0.2);
            padding: 15px;
            border-radius: 10px;
            margin-top: 10px;
            font-size: 0.9rem;
            text-align: center;
            border: 1px solid rgba(0, 255, 245, 0.3);
            max-width: 400px;
        }
        
        .snake-decoration {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
            z-index: -1;
            overflow: hidden;
        }
        
        .snake-path {
            position: absolute;
            width: 100%;
            height: 100%;
            stroke: rgba(0, 255, 245, 0.1);
            stroke-width: 2;
            fill: none;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        @media (max-width: 600px) {
            .header h1 {
                font-size: 5rem;
            }
            
            .header h2 {
                font-size: 1.8rem;
            }
            
            .game-canvas {
                height: 250px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>404</h1>
            <h2>Page Not Found</h2>
            <p>Oops! It seems the page you're looking for has slithered away. While you're here, enjoy a game of snake!</p>
        </div>
        
        <div class="game-container">
            <div class="snake-decoration">
                <svg viewBox="0 0 500 400" xmlns="http://www.w3.org/2000/svg">
                    <path class="snake-path" d="M10,50 C100,10 150,100 200,80 C250,60 300,120 350,100 C400,80 450,150 490,130" />
                    <path class="snake-path" d="M10,200 C80,180 120,250 180,220 C240,190 300,280 350,250 C400,220 450,300 490,280" />
                </svg>
            </div>
            
            <div class="game-header">
                <h3>SNAKE GAME</h3>
                <div class="score-container">
                    <div class="score-box">SCORE: <span id="score">0</span></div>
                    <div class="score-box">HIGH: <span id="high-score">0</span></div>
                </div>
            </div>
            
            <canvas id="gameCanvas" class="game-canvas"></canvas>
            
            <div class="controls">
                <button class="control-btn" id="startBtn">Start Game</button>
                <button class="control-btn" id="pauseBtn">Pause</button>
                <button class="control-btn" id="resetBtn">Reset</button>
            </div>
            
            <div class="game-instructions">
                <p>Use <strong>ARROW KEYS</strong> to control the snake. Collect food to grow and earn points!</p>
            </div>
        </div>
        
        <a href="/" class="home-button">Back to Homepage</a>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const canvas = document.getElementById('gameCanvas');
            const ctx = canvas.getContext('2d');
            const scoreElement = document.getElementById('score');
            const highScoreElement = document.getElementById('high-score');
            const startBtn = document.getElementById('startBtn');
            const pauseBtn = document.getElementById('pauseBtn');
            const resetBtn = document.getElementById('resetBtn');
            
            // Set canvas dimensions
            canvas.width = canvas.offsetWidth;
            canvas.height = canvas.offsetHeight;
            
            // Game variables
            const gridSize = 20;
            const gridWidth = Math.floor(canvas.width / gridSize);
            const gridHeight = Math.floor(canvas.height / gridSize);
            let snake = [];
            let food = {};
            let direction = 'right';
            let nextDirection = 'right';
            let gameInterval;
            let score = 0;
            let highScore = localStorage.getItem('snakeHighScore') || 0;
            let gameRunning = false;
            let gamePaused = false;
            
            // Set high score
            highScoreElement.textContent = highScore;
            
            // Initialize game
            function initGame() {
                // Initial snake position (center of canvas)
                snake = [
                    {x: Math.floor(gridWidth / 2), y: Math.floor(gridHeight / 2)},
                    {x: Math.floor(gridWidth / 2) - 1, y: Math.floor(gridHeight / 2)},
                    {x: Math.floor(gridWidth / 2) - 2, y: Math.floor(gridHeight / 2)}
                ];
                
                // Place first food
                placeFood();
                
                // Reset direction and score
                direction = 'right';
                nextDirection = 'right';
                score = 0;
                scoreElement.textContent = score;
                
                // Draw initial state
                draw();
            }
            
            // Place food at random position
            function placeFood() {
                food = {
                    x: Math.floor(Math.random() * gridWidth),
                    y: Math.floor(Math.random() * gridHeight)
                };
                
                // Make sure food doesn't appear on snake
                for (let segment of snake) {
                    if (segment.x === food.x && segment.y === food.y) {
                        return placeFood();
                    }
                }
            }
            
            // Draw game state
            function draw() {
                // Clear canvas
                ctx.clearRect(0, 0, canvas.width, canvas.height);
                
                // Draw background grid
                ctx.fillStyle = 'rgba(0, 60, 50, 0.3)';
                for (let x = 0; x < gridWidth; x++) {
                    for (let y = 0; y < gridHeight; y++) {
                        if ((x + y) % 2 === 0) {
                            ctx.fillRect(x * gridSize, y * gridSize, gridSize, gridSize);
                        }
                    }
                }
                
                // Draw snake
                snake.forEach((segment, index) => {
                    if (index === 0) {
                        // Snake head
                        ctx.fillStyle = '#00fff5';
                    } else {
                        // Snake body
                        const gradient = ctx.createLinearGradient(
                            segment.x * gridSize, 
                            segment.y * gridSize, 
                            segment.x * gridSize + gridSize, 
                            segment.y * gridSize + gridSize
                        );
                        gradient.addColorStop(0, '#00a69c');
                        gradient.addColorStop(1, '#00857c');
                        ctx.fillStyle = gradient;
                    }
                    
                    ctx.fillRect(segment.x * gridSize, segment.y * gridSize, gridSize, gridSize);
                    
                    // Add rounded corners
                    ctx.strokeStyle = '#003a32';
                    ctx.lineWidth = 2;
                    ctx.strokeRect(segment.x * gridSize, segment.y * gridSize, gridSize, gridSize);
                });
                
                // Draw food
                ctx.fillStyle = '#ff4757';
                ctx.beginPath();
                ctx.arc(
                    food.x * gridSize + gridSize/2,
                    food.y * gridSize + gridSize/2,
                    gridSize/2 - 2,
                    0,
                    Math.PI * 2
                );
                ctx.fill();
                
                // Draw food shine
                ctx.fillStyle = 'rgba(255, 255, 255, 0.6)';
                ctx.beginPath();
                ctx.arc(
                    food.x * gridSize + gridSize/3,
                    food.y * gridSize + gridSize/3,
                    gridSize/6,
                    0,
                    Math.PI * 2
                );
                ctx.fill();
            }
            
            // Update game state
            function update() {
                if (gamePaused) return;
                
                // Update direction
                direction = nextDirection;
                
                // Calculate new head position
                const head = {x: snake[0].x, y: snake[0].y};
                
                switch (direction) {
                    case 'up': head.y--; break;
                    case 'down': head.y++; break;
                    case 'left': head.x--; break;
                    case 'right': head.x++; break;
                }
                
                // Check collision with walls
                if (head.x < 0 || head.x >= gridWidth || head.y < 0 || head.y >= gridHeight) {
                    gameOver();
                    return;
                }
                
                // Check collision with self
                for (let i = 0; i < snake.length; i++) {
                    if (head.x === snake[i].x && head.y === snake[i].y) {
                        gameOver();
                        return;
                    }
                }
                
                // Add new head
                snake.unshift(head);
                
                // Check if food is eaten
                if (head.x === food.x && head.y === food.y) {
                    // Increase score
                    score += 10;
                    scoreElement.textContent = score;
                    
                    // Update high score if needed
                    if (score > highScore) {
                        highScore = score;
                        highScoreElement.textContent = highScore;
                        localStorage.setItem('snakeHighScore', highScore);
                    }
                    
                    // Place new food
                    placeFood();
                } else {
                    // Remove tail if no food eaten
                    snake.pop();
                }
                
                // Draw updated state
                draw();
            }
            
            // Game over
            function gameOver() {
                clearInterval(gameInterval);
                gameRunning = false;
                
                // Show game over message
                ctx.fillStyle = 'rgba(0, 0, 0, 0.7)';
                ctx.fillRect(0, 0, canvas.width, canvas.height);
                
                ctx.fillStyle = '#ff4757';
                ctx.font = 'bold 30px Arial';
                ctx.textAlign = 'center';
                ctx.fillText('GAME OVER', canvas.width / 2, canvas.height / 2 - 20);
                
                ctx.fillStyle = 'white';
                ctx.font = '20px Arial';
                ctx.fillText(`Score: ${score}`, canvas.width / 2, canvas.height / 2 + 20);
            }
            
            // Start game
            function startGame() {
                if (gameRunning) return;
                
                if (!gamePaused) {
                    initGame();
                }
                
                gameRunning = true;
                gamePaused = false;
                
                clearInterval(gameInterval);
                gameInterval = setInterval(update, 150);
            }
            
            // Pause game
            function pauseGame() {
                if (!gameRunning) return;
                
                gamePaused = !gamePaused;
                
                if (gamePaused) {
                    pauseBtn.textContent = 'Resume';
                    
                    // Show pause message
                    ctx.fillStyle = 'rgba(0, 0, 0, 0.7)';
                    ctx.fillRect(0, 0, canvas.width, canvas.height);
                    
                    ctx.fillStyle = '#00fff5';
                    ctx.font = 'bold 30px Arial';
                    ctx.textAlign = 'center';
                    ctx.fillText('PAUSED', canvas.width / 2, canvas.height / 2);
                } else {
                    pauseBtn.textContent = 'Pause';
                }
            }
            
            // Reset game
            function resetGame() {
                clearInterval(gameInterval);
                gameRunning = false;
                gamePaused = false;
                pauseBtn.textContent = 'Pause';
                initGame();
            }
            
            // Handle keyboard input
            function handleKeydown(e) {
                switch (e.key) {
                    case 'ArrowUp':
                        if (direction !== 'down') nextDirection = 'up';
                        e.preventDefault();
                        break;
                    case 'ArrowDown':
                        if (direction !== 'up') nextDirection = 'down';
                        e.preventDefault();
                        break;
                    case 'ArrowLeft':
                        if (direction !== 'right') nextDirection = 'left';
                        e.preventDefault();
                        break;
                    case 'ArrowRight':
                        if (direction !== 'left') nextDirection = 'right';
                        e.preventDefault();
                        break;
                    case ' ':
                        if (gameRunning) {
                            pauseGame();
                        } else {
                            startGame();
                        }
                        e.preventDefault();
                        break;
                }
            }
            
            // Event listeners
            startBtn.addEventListener('click', startGame);
            pauseBtn.addEventListener('click', pauseGame);
            resetBtn.addEventListener('click', resetGame);
            document.addEventListener('keydown', handleKeydown);
            
            // Initialize on load
            initGame();
            
            // Responsive canvas
            window.addEventListener('resize', () => {
                canvas.width = canvas.offsetWidth;
                canvas.height = canvas.offsetHeight;
                initGame();
            });
        });
    </script>
</body>
</html>
