<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For My Love Juliet</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            background: linear-gradient(135deg, #ffafbd 0%, #ffc3a0 100%);
            color: #8a2b5e;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px;
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 800px;
            width: 100%;
            background: rgba(255, 255, 255, 0.92);
            border-radius: 25px;
            padding: 40px;
            box-shadow: 0 20px 40px rgba(255, 105, 180, 0.3);
            position: relative;
            overflow: hidden;
            border: 8px solid #ff69b4;
            margin: 20px 0;
        }
        
        .container::before {
            content: "";
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,182,193,0.1) 1px, transparent 1px);
            background-size: 30px 30px;
            z-index: 0;
            animation: floatHearts 60s linear infinite;
        }
        
        @keyframes floatHearts {
            0% { transform: translate(0, 0) rotate(0deg); }
            100% { transform: translate(-30px, -30px) rotate(360deg); }
        }
        
        .header {
            text-align: center;
            margin-bottom: 30px;
            position: relative;
            z-index: 1;
        }
        
        .title {
            font-family: 'Dancing Script', cursive;
            font-size: 3.5rem;
            color: #ff1493;
            margin-bottom: 10px;
            text-shadow: 3px 3px 0px rgba(255, 20, 147, 0.2);
        }
        
        .name-container {
            background: linear-gradient(45deg, #ff1493, #ff69b4);
            padding: 15px 30px;
            border-radius: 50px;
            display: inline-block;
            margin: 20px 0;
            box-shadow: 0 10px 20px rgba(255, 20, 147, 0.3);
            transform: rotate(-2deg);
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { transform: rotate(-2deg) scale(1); }
            50% { transform: rotate(-2deg) scale(1.03); }
            100% { transform: rotate(-2deg) scale(1); }
        }
        
        .name-highlight {
            font-size: 2.5rem;
            color: white;
            font-weight: 700;
            letter-spacing: 1px;
        }
        
        .nickname {
            font-size: 1.8rem;
            color: #ff1493;
            font-family: 'Dancing Script', cursive;
            margin: 10px 0;
            font-weight: 700;
        }
        
        .my-name {
            text-align: center;
            font-size: 1.5rem;
            color: #db7093;
            margin-top: 10px;
            font-weight: 600;
        }
        
        .heart-banner {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 25px 0;
            flex-wrap: wrap;
        }
        
        .heart {
            font-size: 2.5rem;
            color: #ff69b4;
            animation: bounce 1.5s infinite;
        }
        
        .heart:nth-child(2) { animation-delay: 0.2s; color: #ff1493; }
        .heart:nth-child(3) { animation-delay: 0.4s; color: #db7093; }
        .heart:nth-child(4) { animation-delay: 0.6s; color: #ff69b4; }
        .heart:nth-child(5) { animation-delay: 0.8s; color: #ff1493; }
        
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-15px); }
        }
        
        .apology-card {
            background: linear-gradient(145deg, #fff5f7, #ffeef2);
            border-radius: 20px;
            padding: 30px;
            margin: 30px 0;
            border-left: 10px solid #ff69b4;
            box-shadow: 0 10px 25px rgba(255, 105, 180, 0.15);
            position: relative;
            z-index: 1;
        }
        
        .apology-card::after {
            content: "💖";
            position: absolute;
            top: -20px;
            right: -20px;
            font-size: 3rem;
            transform: rotate(15deg);
        }
        
        .apology-text {
            font-size: 1.2rem;
            line-height: 1.8;
            margin-bottom: 20px;
        }
        
        .apology-text p {
            margin-bottom: 15px;
        }
        
        .highlight {
            color: #ff1493;
            font-weight: 600;
        }
        
        .promise-section {
            background: linear-gradient(135deg, #ff69b4, #ff1493);
            color: white;
            padding: 25px;
            border-radius: 20px;
            text-align: center;
            margin: 30px 0;
            box-shadow: 0 15px 30px rgba(255, 20, 147, 0.3);
            position: relative;
            overflow: hidden;
        }
        
        .promise-section::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 5px;
            background: linear-gradient(90deg, #ffb6c1, #fff, #ffb6c1);
        }
        
        .promise-title {
            font-family: 'Dancing Script', cursive;
            font-size: 2.5rem;
            margin-bottom: 15px;
        }
        
        .promise-text {
            font-size: 1.5rem;
            font-weight: 600;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }
        
        .special-names {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 25px;
            margin: 30px 0;
            text-align: center;
            border: 3px dashed #ff69b4;
            position: relative;
            z-index: 1;
        }
        
        .special-title {
            font-family: 'Dancing Script', cursive;
            font-size: 2.5rem;
            color: #ff1493;
            margin-bottom: 20px;
        }
        
        .names-container {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
            margin: 20px 0;
        }
        
        .name-box {
            background: linear-gradient(135deg, #ffb6c1, #ff69b4);
            padding: 15px 25px;
            border-radius: 15px;
            min-width: 200px;
            box-shadow: 0 10px 20px rgba(255, 105, 180, 0.2);
        }
        
        .name-box h3 {
            color: white;
            font-size: 1.3rem;
            margin-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        .name-box p {
            color: white;
            font-size: 1.8rem;
            font-weight: 700;
        }
        
        .love-quote {
            font-style: italic;
            font-size: 1.3rem;
            color: #ff1493;
            margin-top: 20px;
            font-family: 'Dancing Script', cursive;
        }
        
        .juli-juli {
            font-size: 2.5rem;
            color: #ff1493;
            font-family: 'Dancing Script', cursive;
            text-align: center;
            margin: 20px 0;
            animation: glow 2s infinite alternate;
        }
        
        @keyframes glow {
            from { text-shadow: 0 0 10px #ff69b4; }
            to { text-shadow: 0 0 20px #ff1493, 0 0 30px #ff1493; }
        }
        
        .love-game {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 30px;
            margin: 30px 0;
            text-align: center;
            border: 3px dashed #ff69b4;
            position: relative;
            z-index: 1;
        }
        
        .game-title {
            font-family: 'Dancing Script', cursive;
            font-size: 2.5rem;
            color: #ff1493;
            margin-bottom: 20px;
        }
        
        .game-instruction {
            font-size: 1.1rem;
            margin-bottom: 25px;
            color: #8a2b5e;
        }
        
        .love-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 15px;
            margin-bottom: 25px;
        }
        
        .love-box {
            background: linear-gradient(135deg, #ffb6c1, #ff69b4);
            height: 80px;
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 8px 15px rgba(255, 105, 180, 0.2);
        }
        
        .love-box:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 20px rgba(255, 105, 180, 0.4);
        }
        
        .love-box.revealed {
            background: linear-gradient(135deg, #ff1493, #c71585);
            color: white;
            transform: scale(1.05);
        }
        
        .game-message {
            font-size: 1.4rem;
            color: #ff1493;
            min-height: 40px;
            margin-top: 20px;
            font-weight: 600;
            transition: all 0.5s ease;
        }
        
        .forgiveness-btn {
            background: linear-gradient(to right, #ff1493, #ff69b4);
            border: none;
            color: white;
            padding: 18px 50px;
            font-size: 1.5rem;
            border-radius: 50px;
            cursor: pointer;
            margin: 25px auto;
            display: block;
            font-weight: 600;
            letter-spacing: 1px;
            transition: all 0.3s ease;
            box-shadow: 0 10px 20px rgba(255, 20, 147, 0.4);
            font-family: 'Poppins', sans-serif;
            position: relative;
            overflow: hidden;
        }
        
        .forgiveness-btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 25px rgba(255, 20, 147, 0.6);
            background: linear-gradient(to right, #ff69b4, #ff1493);
        }
        
        .forgiveness-btn:active {
            transform: translateY(0);
        }
        
        .forgiveness-btn::after {
            content: "💝";
            position: absolute;
            right: 20px;
            top: 50%;
            transform: translateY(-50%);
        }
        
        .signature {
            text-align: center;
            margin-top: 30px;
            padding-top: 20px;
            border-top: 2px dotted #ffb6c1;
            color: #8a2b5e;
            font-style: italic;
            position: relative;
            z-index: 1;
        }
        
        .footer {
            text-align: center;
            margin-top: 30px;
            color: #8a2b5e;
            font-size: 0.9rem;
            opacity: 0.8;
        }
        
        .pink-flower {
            position: absolute;
            font-size: 2rem;
            opacity: 0.7;
            z-index: 0;
        }
        
        .flower1 { top: 10%; left: 5%; transform: rotate(45deg); }
        .flower2 { top: 15%; right: 5%; transform: rotate(-20deg); }
        .flower3 { bottom: 20%; left: 8%; transform: rotate(10deg); }
        .flower4 { bottom: 15%; right: 10%; transform: rotate(-45deg); }
        
        @media (max-width: 768px) {
            .container { padding: 25px; }
            .title { font-size: 2.8rem; }
            .name-highlight { font-size: 2.2rem; }
            .love-grid { grid-template-columns: repeat(3, 1fr); }
            .love-box { height: 70px; font-size: 1.8rem; }
            .apology-text { font-size: 1.1rem; }
            .names-container { flex-direction: column; align-items: center; }
        }
        
        @media (max-width: 480px) {
            .container { padding: 20px; }
            .title { font-size: 2.2rem; }
            .name-highlight { font-size: 1.8rem; }
            .love-grid { grid-template-columns: repeat(2, 1fr); }
            .love-box { height: 75px; }
            .forgiveness-btn { padding: 15px 30px; font-size: 1.3rem; }
        }
    </style>
</head>
<body>
    <div class="pink-flower flower1">🌸</div>
    <div class="pink-flower flower2">🌺</div>
    <div class="pink-flower flower3">💮</div>
    <div class="pink-flower flower4">🏵️</div>
    
    <div class="container">
        <div class="header">
            <h1 class="title">To My Dearest Juliet</h1>
            
            <div class="heart-banner">
                <div class="heart">❤️</div>
                <div class="heart">💖</div>
                <div class="heart">💗</div>
                <div class="heart">💕</div>
                <div class="heart">💞</div>
            </div>
            
            <div class="name-container">
                <h2 class="name-highlight">For Mapenzi Miyano Juliet</h2>
            </div>
            
            <div class="nickname">My Mbumbu Wangu 💖</div>
            <div class="juli-juli">juli juli 💘</div>
            
            <div class="my-name">From Lifasi Malumo Lucky</div>
        </div>
        
        <div class="apology-card">
            <div class="apology-text">
                <p>My dearest <span class="highlight">Mapenzi Miyano Juliet</span>,</p>
                <p>I'm writing this with a heart full of regret and love. <span class="highlight">I'm sorry my love for what I did</span>. I know I've hurt you, and I can't express how much I regret my actions.</p>
                <p>Every moment with you is special, and I realize now how much I've taken that for granted. Your smile lights up my world, your laughter is my favorite melody, and your presence makes everything better.</p>
                <p><span class="highlight">I'll not do it again</span>, I promise you that. I've learned my lesson, and I understand now how much you mean to me. You are my everything, my <span class="highlight">mbumbu wangu</span>.</p>
                <p>Please know that <span class="highlight">I love you</span> more than words can express. You are the most important person in my life, and I can't imagine my world without you in it.</p>
            </div>
        </div>
        
        <div class="promise-section">
            <h3 class="promise-title">My Solemn Promise</h3>
            <p class="promise-text">I will never hurt you again, my Juli juli 💝</p>
        </div>
        
        <div class="special-names">
            <h3 class="special-title">Our Special Names</h3>
            <div class="names-container">
                <div class="name-box">
                    <h3>My Queen</h3>
                    <p>Mapenzi Miyano Juliet</p>
                </div>
                <div class="name-box">
                    <h3>My Love</h3>
                    <p>Juli juli 💘</p>
                </div>
                <div class="name-box">
                    <h3>My Mbumbu</h3>
                    <p>My Everything</p>
                </div>
            </div>
            <div class="love-quote">
                "You are the love of my life, today, tomorrow, and forever"
            </div>
        </div>
        
        <div class="love-game">
            <h3 class="game-title">Find My Love Messages</h3>
            <p class="game-instruction">Click on the hearts to reveal hidden messages for you!</p>
            
            <div class="love-grid" id="loveGrid">
                <!-- Hearts will be generated by JavaScript -->
            </div>
            
            <div class="game-message" id="gameMessage">Click a heart to reveal a message, my love!</div>
        </div>
        
        <button class="forgiveness-btn" id="forgivenessBtn">Will You Forgive Me, My Mbumbu?</button>
        
        <div class="signature">
            <p>With all my love, deepest apologies, and a promise to be better,</p>
            <p style="font-size: 1.3rem; font-weight: 600; color: #ff1493;">Your Lifasi Malumo Lucky</p>
            <p style="font-size: 1.1rem; color: #ff69b4; margin-top: 5px;">Forever yours 💖</p>
        </div>
    </div>
    
    <div class="footer">
        <p>Made with endless love for the most amazing woman in my life 💘</p>
    </div>

    <script>
        // Love Game
        const loveGrid = document.getElementById('loveGrid');
        const gameMessage = document.getElementById('gameMessage');
        
        const loveMessages = [
            "I love you Juliet 💖",
            "You're my everything 🌹",
            "My heart is yours ❤️",
            "Forgive me? 🙏",
            "You're my queen 👑",
            "I miss your smile 😊",
            "Mbumbu wangu 💘",
            "Always yours 💕",
            "Juli juli 💞",
            "You complete me 💑",
            "My love for you is endless 💝",
            "You're my dream come true 💭"
        ];
        
        // Create heart boxes
        for (let i = 0; i < 12; i++) {
            const box = document.createElement('div');
            box.className = 'love-box';
            box.innerHTML = '💖';
            box.dataset.message = loveMessages[i];
            
            box.addEventListener('click', function() {
                if (!this.classList.contains('revealed')) {
                    this.classList.add('revealed');
                    this.innerHTML = this.dataset.message;
                    
                    // Update game message
                    const messages = [
                        "That's how I feel! 💖",
                        "You found my true feelings! 🌹",
                        "My heart speaks! ❤️",
                        "Another truth revealed! 💕",
                        "Exactly how I feel about you! 💘",
                        "Keep going, my love! 💞"
                    ];
                    const randomMessage = messages[Math.floor(Math.random() * messages.length)];
                    gameMessage.textContent = randomMessage;
                    
                    // Check if all boxes are revealed
                    const allBoxes = document.querySelectorAll('.love-box');
                    const revealedBoxes = document.querySelectorAll('.love-box.revealed');
                    
                    if (allBoxes.length === revealedBoxes.length) {
                        gameMessage.textContent = "You found all my love messages! I'm forever yours, Juliet! 💘";
                        gameMessage.style.color = "#ff1493";
                        gameMessage.style.fontSize = "1.6rem";
                    }
                }
            });
            
            loveGrid.appendChild(box);
        }
        
        // Forgiveness Button
        const forgivenessBtn = document.getElementById('forgivenessBtn');
        let clickCount = 0;
        
        forgivenessBtn.addEventListener('click', function() {
            clickCount++;
            
            if (clickCount === 1) {
                this.innerHTML = 'Please forgive me, Juli juli? 💖';
                this.style.transform = 'scale(1.05)';
                gameMessage.textContent = "I'm really sorry my love, please give me another chance!";
                
                // Create floating hearts
                createFloatingHearts(5);
                
                // Animate the "juli juli" text
                const juliText = document.querySelector('.juli-juli');
                juliText.style.animation = 'glow 0.5s infinite alternate';
                setTimeout(() => {
                    juliText.style.animation = 'glow 2s infinite alternate';
                }, 1000);
            } 
            else if (clickCount === 2) {
                this.innerHTML = 'I promise to be better, Mbumbu wangu! 💝';
                this.style.background = 'linear-gradient(to right, #ff69b4, #ff1493)';
                gameMessage.textContent = "I'll make it up to you, I promise! You are my everything!";
                
                // Create more floating hearts
                createFloatingHearts(8);
                
                // Add special effect to nickname
                const nickname = document.querySelector('.nickname');
                nickname.style.color = '#ff1493';
                nickname.style.textShadow = '0 0 10px #ff69b4';
            }
            else if (clickCount === 3) {
                this.innerHTML = 'Thank you, my love! I adore you! 💘';
                this.style.background = 'linear-gradient(to right, #4CAF50, #45a049)';
                gameMessage.textContent = "Thank you for forgiving me! I love you so much, Mapenzi Miyano Juliet! 💖";
                
                // Create celebration hearts
                createFloatingHearts(15);
                
                // Change all heart boxes to green
                const allBoxes = document.querySelectorAll('.love-box');
                allBoxes.forEach(box => {
                    box.style.background = 'linear-gradient(135deg, #4CAF50, #45a049)';
                });
                
                // Play celebration animation
                celebrationAnimation();
            }
            
            // Reset transform after animation
            setTimeout(() => {
                this.style.transform = '';
            }, 300);
        });
        
        function createFloatingHearts(count) {
            for (let i = 0; i < count; i++) {
                const heart = document.createElement('div');
                heart.innerHTML = '💖';
                heart.style.position = 'fixed';
                heart.style.fontSize = Math.random() * 20 + 20 + 'px';
                heart.style.left = Math.random() * 100 + 'vw';
                heart.style.top = '100vh';
                heart.style.zIndex = '9999';
                heart.style.pointerEvents = 'none';
                heart.style.opacity = '0.9';
                
                document.body.appendChild(heart);
                
                // Animate heart floating up
                const animation = heart.animate([
                    { transform: 'translateY(0) rotate(0deg)', opacity: 1 },
                    { transform: `translateY(-${window.innerHeight + 100}px) rotate(${Math.random() * 360}deg)`, opacity: 0 }
                ], {
                    duration: Math.random() * 3000 + 2000,
                    easing: 'cubic-bezier(0.215, 0.610, 0.355, 1)'
                });
                
                // Remove heart after animation completes
                animation.onfinish = () => {
                    document.body.removeChild(heart);
                };
            }
        }
        
        function celebrationAnimation() {
            // Add celebration message to the page
            const celebration = document.createElement('div');
            celebration.innerHTML = `
                <div style="position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%); 
                           background: rgba(255, 255, 255, 0.95); padding: 30px; border-radius: 20px; 
                           text-align: center; z-index: 10000; box-shadow: 0 20px 40px rgba(0,0,0,0.2);
                           border: 5px solid #ff69b4; max-width: 80%;">
                    <h2 style="color: #ff1493; font-family: 'Dancing Script', cursive; font-size: 3rem; margin-bottom: 20px;">
                        Thank You My Love! 💖
                    </h2>
                    <p style="font-size: 1.5rem; color: #8a2b5e;">
                        Thank you for forgiving me, my Juliet!<br>
                        I love you more than words can express!
                    </p>
                    <p style="font-size: 1.8rem; color: #ff1493; font-family: 'Dancing Script', cursive; margin: 15px 0;">
                        You are my Mbumbu Wangu forever! 💘
                    </p>
                    <button id="closeCelebration" style="margin-top: 20px; padding: 10px 30px; 
                           background: #ff69b4; color: white; border: none; border-radius: 50px; 
                           font-size: 1.2rem; cursor: pointer;">
                        Close
                    </button>
                </div>
            `;
            
            document.body.appendChild(celebration);
            
            // Close button functionality
            document.getElementById('closeCelebration').addEventListener('click', function() {
                document.body.removeChild(celebration);
            });
        }
        
        // Initialize with some floating hearts
        window.addEventListener('load', function() {
            setTimeout(() => {
                createFloatingHearts(3);
                
                // Add initial animation to "juli juli"
                const juliText = document.querySelector('.juli-juli');
                juliText.style.transform = 'scale(1.1)';
                setTimeout(() => {
                    juliText.style.transform = 'scale(1)';
                }, 500);
            }, 1000);
        });
    </script>
</body>
</html># Juliet-
