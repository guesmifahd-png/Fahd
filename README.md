<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For My Amazing Girlfriend ❤️</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #f9c5d1 0%, #c2e9fb 100%);
            color: #333;
            min-height: 100vh;
            overflow-x: hidden;
            padding: 20px;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.95);
            border-radius: 25px;
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.15);
            overflow: hidden;
            padding: 30px;
        }
        
        .header {
            text-align: center;
            padding: 40px 20px 30px;
            background: linear-gradient(135deg, #ff758c 0%, #ff7eb3 100%);
            border-radius: 20px;
            margin-bottom: 30px;
            color: white;
            position: relative;
            overflow: hidden;
        }
        
        h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 3.8rem;
            margin-bottom: 10px;
            position: relative;
            z-index: 1;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
        }
        
        .subtitle {
            font-size: 1.3rem;
            opacity: 0.9;
            position: relative;
            z-index: 1;
        }
        
        .heart {
            color: #ff3055;
            animation: heartbeat 1.5s infinite;
            display: inline-block;
        }
        
        .section {
            margin-bottom: 40px;
            padding: 25px;
            background: #fff;
            border-radius: 20px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease;
        }
        
        .section:hover {
            transform: translateY(-5px);
        }
        
        .section-title {
            font-family: 'Dancing Script', cursive;
            color: #ff3055;
            font-size: 2.5rem;
            margin-bottom: 20px;
            text-align: center;
        }
        
        .love-letter {
            line-height: 1.8;
            font-size: 1.1rem;
        }
        
        .love-letter p {
            margin-bottom: 20px;
            text-align: justify;
        }
        
        .signature {
            text-align: right;
            font-family: 'Dancing Script', cursive;
            font-size: 2.2rem;
            color: #ff3055;
            margin-top: 20px;
        }
        
        /* I Love You Selima Section */
        .love-message-section {
            text-align: center;
            padding: 50px 20px;
            background: linear-gradient(135deg, #ff9a9e 0%, #fad0c4 100%);
            border-radius: 20px;
            margin: 30px 0;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        .love-message {
            font-family: 'Dancing Script', cursive;
            font-size: 5rem;
            color: white;
            text-shadow: 3px 3px 6px rgba(0, 0, 0, 0.2);
            animation: glow 2s ease-in-out infinite alternate;
            margin-bottom: 20px;
        }
        
        .love-message-small {
            font-family: 'Dancing Script', cursive;
            font-size: 2.5rem;
            color: #fff;
            opacity: 0.9;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
        }
        
        @keyframes glow {
            from { text-shadow: 0 0 10px #fff, 0 0 20px #fff, 0 0 30px #ff4d6d; }
            to { text-shadow: 0 0 20px #fff, 0 0 30px #ff4d6d, 0 0 40px #ff4d6d; }
        }
        
        /* FIXED MUSIC PLAYER */
        .music-player {
            display: flex;
            flex-direction: column;
            align-items: center;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 30px;
            border-radius: 20px;
            margin-top: 20px;
            color: white;
            box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
        }
        
        .music-header {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 25px;
            width: 100%;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }
        
        .play-btn {
            background: white;
            color: #ff3055;
            border: none;
            width: 80px;
            height: 80px;
            border-radius: 50%;
            font-size: 2rem;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.3);
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .play-btn:hover {
            background: #ff3055;
            color: white;
            transform: scale(1.1);
        }
        
        .play-btn.playing {
            background: #ff3055;
            color: white;
        }
        
        .music-text {
            text-align: center;
        }
        
        .song-title {
            font-weight: bold;
            font-size: 1.5rem;
            margin-bottom: 5px;
        }
        
        .song-artist {
            opacity: 0.9;
            font-size: 1.1rem;
        }
        
        .volume-control {
            display: flex;
            align-items: center;
            gap: 15px;
            width: 80%;
            margin-top: 20px;
        }
        
        .volume-slider {
            flex-grow: 1;
            height: 6px;
            -webkit-appearance: none;
            background: rgba(255, 255, 255, 0.3);
            border-radius: 10px;
            outline: none;
        }
        
        .volume-slider::-webkit-slider-thumb {
            -webkit-appearance: none;
            width: 20px;
            height: 20px;
            background: white;
            border-radius: 50%;
            cursor: pointer;
        }
        
        .music-status {
            margin-top: 15px;
            font-size: 0.9rem;
            opacity: 0.8;
            color: #fff;
        }
        
        .secret-container {
            text-align: center;
            padding: 30px;
            background: linear-gradient(135deg, #a8edea 0%, #fed6e3 100%);
            border-radius: 15px;
            margin-top: 20px;
        }
        
        .reveal-btn {
            background: #ff3055;
            color: white;
            border: none;
            padding: 15px 35px;
            border-radius: 50px;
            font-size: 1.1rem;
            cursor: pointer;
            transition: all 0.3s ease;
            font-family: 'Poppins', sans-serif;
            margin-top: 15px;
            box-shadow: 0 5px 15px rgba(255, 48, 85, 0.3);
        }
        
        .reveal-btn:hover {
            background: #e00034;
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(255, 48, 85, 0.4);
        }
        
        .secret-message {
            display: none;
            margin-top: 25px;
            font-family: 'Dancing Script', cursive;
            font-size: 2.5rem;
            color: #ff3055;
            animation: fadeIn 1.5s;
        }
        
        .footer {
            text-align: center;
            padding: 30px 20px;
            color: #666;
            font-size: 0.9rem;
            margin-top: 30px;
            border-top: 1px solid #eee;
        }
        
        .floating-hearts {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .heart-float {
            position: absolute;
            color: rgba(255, 48, 85, 0.4);
            font-size: 24px;
            animation: float 8s infinite linear;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @keyframes heartbeat {
            0% { transform: scale(1); }
            5% { transform: scale(1.1); }
            10% { transform: scale(1); }
            15% { transform: scale(1.2); }
            50% { transform: scale(1); }
            100% { transform: scale(1); }
        }
        
        @keyframes float {
            0% {
                top: 100%;
                transform: translateX(0) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                top: -50px;
                transform: translateX(100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        @media (max-width: 768px) {
            h1 { font-size: 2.8rem; }
            .section-title { font-size: 2rem; }
            .love-message { font-size: 3.5rem; }
            .love-message-small { font-size: 2rem; }
            .play-btn { width: 70px; height: 70px; font-size: 1.8rem; }
            .song-title { font-size: 1.3rem; }
        }
        
        @media (max-width: 480px) {
            .container { padding: 15px; }
            h1 { font-size: 2.2rem; }
            .subtitle { font-size: 1rem; }
            .love-message { font-size: 2.8rem; }
            .love-message-small { font-size: 1.5rem; }
            .secret-message { font-size: 2rem; }
            .music-header { gap: 15px; }
        }
    </style>
</head>
<body>
    <div class="floating-hearts" id="floatingHearts"></div>
    
    <div class="container">
        <div class="header">
            <h1>For My Beautiful Girlfriend <span class="heart">❤️</span></h1>
            <p class="subtitle">A special surprise just for you, my love</p>
        </div>
        
        <div class="section">
            <h2 class="section-title">My Love Letter to You</h2>
            <div class="love-letter">
                <p>My dearest Selima,</p>
                <p>From the moment you came into my life, everything changed for the better. Your smile brightens my darkest days, your laughter is my favorite melody, and your love has transformed my world in ways I never thought possible.</p>
                <p>I cherish every moment we spend together - whether we're laughing until our stomachs hurt, having deep conversations about everything and nothing, or simply enjoying the comfortable silence that only comes when you're with someone who truly understands you.</p>
                <p>You are my greatest adventure, my safest haven, and my most beautiful surprise. With you, I've discovered a love so deep and genuine that it sometimes takes my breath away. I want to build a lifetime of memories with you, facing whatever comes our way, hand in hand.</p>
                <p>Thank you for being you - kind, compassionate, funny, intelligent, and endlessly beautiful inside and out. I fall in love with you more every single day.</p>
                <div class="signature">Forever yours</div>
            </div>
        </div>
        
        <!-- I Love You Selima Section -->
        <div class="love-message-section">
            <div class="love-message">I Love You</div>
            <div class="love-message-small">Selima</div>
            <div style="margin-top: 30px;">
                <i class="fas fa-heart" style="color: white; font-size: 2rem; margin: 0 10px; animation: heartbeat 1.5s infinite;"></i>
                <i class="fas fa-heart" style="color: white; font-size: 3rem; margin: 0 10px; animation: heartbeat 1.5s infinite 0.3s;"></i>
                <i class="fas fa-heart" style="color: white; font-size: 2rem; margin: 0 10px; animation: heartbeat 1.5s infinite 0.6s;"></i>
            </div>
        </div>
        
        <!-- FIXED MUSIC PLAYER - NOW WORKING -->
        <div class="section">
            <h2 class="section-title">Our Special Song <span class="heart">❤️</span></h2>
            <div class="music-player">
                <div class="music-header">
                    <button class="play-btn" id="playBtn">
                        <i class="fas fa-play"></i>
                    </button>
                    <div class="music-text">
                        <div class="song-title">Perfect - Ed Sheeran</div>
                        <div class="song-artist">Our Romantic Song</div>
                    </div>
                </div>
                <div class="volume-control">
                    <i class="fas fa-volume-down" style="color: white;"></i>
                    <input type="range" class="volume-slider" id="volumeSlider" min="0" max="1" step="0.1" value="0.7">
                    <i class="fas fa-volume-up" style="color: white;"></i>
                </div>
                <div class="music-status" id="musicStatus">
                    <i class="fas fa-music"></i> Click play to start the music
                </div>
            </div>
        </div>
        
        <div class="section">
            <h2 class="section-title">A Secret Just For You</h2>
            <div class="secret-container">
                <p>I have a special message that's just for your eyes only...</p>
                <button class="reveal-btn" id="revealBtn">Click to Reveal My Secret</button>
                <div class="secret-message" id="secretMessage">
                    I'm planning a special surprise for our anniversary next month! Get ready for something amazing, my love!
                </div>
            </div>
        </div>
        
        <div class="footer">
            <p>Made with <span class="heart">❤️</span> for the most amazing woman in my life</p>
            <p>You mean everything to me, Selima</p>
            <p style="margin-top: 15px; font-size: 0.8rem;">© Your loving boyfriend - This moment and forever</p>
        </div>
    </div>

    <!-- FIXED AUDIO - NOW USING A RELIABLE SOURCE -->
    <audio id="romanticMusic" loop preload="auto">
        <!-- Multiple sources for compatibility -->
        <source src="https://www.youtube.com/watch?v=J1Ki-XkDCgU&list=RDJ1Ki-XkDCgU&start_radio=1" type="audio/mpeg">
        <source src="https://files.freemusicarchive.org/storage-freemusicarchive-org/music/Creative_Commons/Ketsa/RAKAS/Ketsa_-_01_-_Hearing_It_All.mp3" type="audio/mpeg">
    </audio>

    <script>
        function createFloatingHearts() {
            const heartsContainer = document.getElementById('floatingHearts');
            const heartCount = 25;
            
            for (let i = 0; i < heartCount; i++) {
                const heart = document.createElement('div');
                heart.classList.add('heart-float');
                heart.innerHTML = '❤️';
                
                const left = Math.random() * 100;
                const size = Math.random() * 25 + 15;
                const duration = Math.random() * 8 + 8;
                const delay = Math.random() * 5;
                
                heart.style.left = `${left}vw`;
                heart.style.fontSize = `${size}px`;
                heart.style.animationDuration = `${duration}s`;
                heart.style.animationDelay = `${delay}s`;
                
                heartsContainer.appendChild(heart);
            }
        }
        
        // FIXED MUSIC PLAYER FUNCTIONALITY
        const music = document.getElementById('romanticMusic');
        const playBtn = document.getElementById('playBtn');
        const volumeSlider = document.getElementById('volumeSlider');
        const musicStatus = document.getElementById('musicStatus');
        let isPlaying = false;
        
        // Set initial volume
        music.volume = volumeSlider.value;
        
        // Play button functionality
        playBtn.addEventListener('click', function() {
            if (isPlaying) {
                // Pause music
                music.pause();
                playBtn.innerHTML = '<i class="fas fa-play"></i>';
                playBtn.style.background = 'white';
                playBtn.style.color = '#ff3055';
                musicStatus.innerHTML = '<i class="fas fa-music"></i> Music paused - click play to resume';
            } else {
                // Play music with error handling
                music.play()
                    .then(() => {
                        playBtn.innerHTML = '<i class="fas fa-pause"></i>';
                        playBtn.style.background = '#ff3055';
                        playBtn.style.color = 'white';
                        musicStatus.innerHTML = '<i class="fas fa-music"></i> Now playing: Perfect - Ed Sheeran';
                    })
                    .catch(error => {
                        console.log("Playback failed:", error);
                        musicStatus.innerHTML = '<i class="fas fa-exclamation-circle"></i> Click play again to start music';
                        // Try alternate method
                        setTimeout(() => {
                            music.play().catch(e => {});
                        }, 100);
                    });
            }
            isPlaying = !isPlaying;
        });
        
        // Volume control
        volumeSlider.addEventListener('input', function() {
            music.volume = this.value;
        });
        
        // When music ends (if not looping)
        music.addEventListener('ended', function() {
            isPlaying = false;
            playBtn.innerHTML = '<i class="fas fa-play"></i>';
            playBtn.style.background = 'white';
            playBtn.style.color = '#ff3055';
            musicStatus.innerHTML = '<i class="fas fa-music"></i> Song ended - click play again';
        });
        
        // Secret message reveal
        const revealBtn = document.getElementById('revealBtn');
        const secretMessage = document.getElementById('secretMessage');
        
        revealBtn.addEventListener('click', function() {
            if (secretMessage.style.display === 'block') {
                secretMessage.style.display = 'none';
                revealBtn.textContent = 'Click to Reveal My Secret';
            } else {
                secretMessage.style.display = 'block';
                revealBtn.textContent = 'Hide Secret Message';
                
                if (!revealBtn.dataset.changed) {
                    setTimeout(() => {
                        secretMessage.innerHTML = "Actually, I have an even bigger secret... I love you more than you could ever imagine! You're my everything, Selima!";
                        secretMessage.style.color = "#ff3055";
                        revealBtn.dataset.changed = true;
                    }, 4000);
                }
            }
        });
        
        document.addEventListener('DOMContentLoaded', function() {
            createFloatingHearts();
            
            const sections = document.querySelectorAll('.section');
            sections.forEach((section, index) => {
                section.style.animation = `fadeIn 1s ease ${index * 0.2}s forwards`;
                section.style.opacity = '0';
            });
            
            // Preload music
            music.load();
            console.log("Music player initialized");
        });
    </script>
</body>
</html>
