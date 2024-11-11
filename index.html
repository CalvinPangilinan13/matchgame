<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Predator Memory Match</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: #101010;
            font-family: 'Courier New', Courier, monospace;
            color: #fff;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            text-align: center;
            background-image: url('https://www.transparenttextures.com/patterns/dark-wood.png');
            background-size: cover;
        }

        #game-container {
            width: 100%;
            max-width: 600px; /* Max width for larger screens */
            margin: 20px;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.7);
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(0, 255, 0, 0.5);
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: #00ff00;
            text-shadow: 0 0 10px #00ff00, 0 0 20px #00ff00;
        }

        #memory-board {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 10px;
            margin-bottom: 20px;
        }

        .card {
            width: 100%;
            height: 100px;
            background-color: #333;
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-size: 2rem;
            color: #fff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);
            transition: transform 0.3s;
        }

        .card.flipped {
            background-color: #444;
            color: #00ff00;
            transform: scale(1.1);
        }

        .card:active {
            transform: scale(0.95);
        }

        #status {
            margin-bottom: 20px;
            font-size: 1.5rem;
            color: #00ff00;
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            background-color: #ff0000;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            text-transform: uppercase;
            letter-spacing: 1px;
            width: 100%;
            margin-top: 10px;
        }

        button:hover {
            background-color: #ff4444;
        }

        button:active {
            background-color: #cc0000;
        }

        /* Responsive design */
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem; /* Smaller title on mobile */
            }

            .card {
                height: 80px; /* Smaller card on mobile */
                font-size: 1.5rem; /* Adjust font size */
            }

            #memory-board {
                grid-template-columns: repeat(4, 1fr); /* Keep grid responsive */
                width: 100%;
            }
        }

        @media (max-width: 480px) {
            h1 {
                font-size: 1.8rem; /* Further reduce title size */
            }

            .card {
                height: 70px;
                font-size: 1.3rem; /* Smaller font size */
            }

            #memory-board {
                grid-template-columns: repeat(3, 1fr); /* Adjust to 3 columns for smaller screens */
            }

            button {
                font-size: 14px;
                width: 100%;
            }
        }

    </style>
</head>

<body>
    <div id="game-container">
        <h1>Calvin Memory Match</h1>
        <div id="memory-board"></div>
        <div id="status">
            <span>Matches: </span><span id="matches">0</span>
        </div>
        <button id="restart-button" onclick="startGame()">Restart Game</button>
    </div>

    <script>
        const images = [
            { src: '👹', alt: 'predator-mask' },
            { src: '🔥', alt: 'fire' },
            { src: '💀', alt: 'skull' },
            { src: '⚔️', alt: 'sword' },
            { src: '💣', alt: 'bomb' },
            { src: '🔫', alt: 'gun' },
            { src: '👁️', alt: 'eye' },
            { src: '🌕', alt: 'moon' },
        ];

        let cardArray = [...images, ...images];
        let flippedCards = [];
        let matches = 0;

        const gameBoard = document.getElementById('memory-board');
        const status = document.getElementById('matches');
        const restartButton = document.getElementById('restart-button');

        function shuffle(array) {
            for (let i = array.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [array[i], array[j]] = [array[j], array[i]];
            }
        }

        function createCards() {
            gameBoard.innerHTML = '';
            cardArray.forEach((card, index) => {
                const cardElement = document.createElement('div');
                cardElement.classList.add('card');
                cardElement.setAttribute('data-index', index);
                cardElement.addEventListener('click', flipCard);
                gameBoard.appendChild(cardElement);
            });
        }

        function flipCard() {
            if (flippedCards.length === 2) return;

            const clickedCard = this;
            const cardIndex = clickedCard.getAttribute('data-index');

            if (clickedCard.classList.contains('flipped')) return;

            clickedCard.textContent = cardArray[cardIndex].src;
            clickedCard.classList.add('flipped');
            flippedCards.push(clickedCard);

            if (flippedCards.length === 2) {
                checkMatch();
            }
        }

        function checkMatch() {
            const [card1, card2] = flippedCards;
            const index1 = card1.getAttribute('data-index');
            const index2 = card2.getAttribute('data-index');

            if (cardArray[index1].src === cardArray[index2].src) {
                matches++;
                status.textContent = matches;
                flippedCards = [];
                if (matches === images.length) {
                    setTimeout(() => {
                        alert('Congratulations! You matched all the pairs!');
                        startGame();
                    }, 500);
                }
            } else {
                setTimeout(() => {
                    card1.classList.remove('flipped');
                    card2.classList.remove('flipped');
                    card1.textContent = '';
                    card2.textContent = '';
                    flippedCards = [];
                }, 1000);
            }
        }

        function startGame() {
            flippedCards = [];
            matches = 0;
            status.textContent = matches;
            cardArray = [...images, ...images];
            shuffle(cardArray);
            createCards();
        }

        startGame();
    </script>
</body>

</html>
