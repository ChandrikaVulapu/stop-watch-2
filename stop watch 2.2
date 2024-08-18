let board;
let currentPlayer;
let gameActive;
let vsAI = false;

const statusDisplay = document.getElementById('status');
const cells = document.querySelectorAll('.cell');
const winningConditions = [
    [0, 1, 2],
    [3, 4, 5],
    [6, 7, 8],
    [0, 3, 6],
    [1, 4, 7],
    [2, 5, 8],
    [0, 4, 8],
    [2, 4, 6]
];

function initializeGame() {
    board = ['', '', '', '', '', '', '', '', ''];
    currentPlayer = 'X';
    gameActive = true;
    statusDisplay.textContent = `${currentPlayer}'s turn`;
    cells.forEach(cell => {
        cell.textContent = '';
        cell.classList.remove('winning-cell');
    });
}

function handleCellClick(e) {
    const clickedCell = e.target;
    const clickedCellIndex = clickedCell.getAttribute('data-index');

    if (board[clickedCellIndex] !== '' || !gameActive) {
        return;
    }

    updateCell(clickedCell, clickedCellIndex);
    checkWinner();

    if (vsAI && gameActive) {
        aiMove();
    }
}

function updateCell(cell, index) {
    board[index] = currentPlayer;
    cell.textContent = currentPlayer;
}

function checkWinner() {
    let roundWon = false;

    for (let i = 0; i < winningConditions.length; i++) {
        const winCondition = winningConditions[i];
        let a = board[winCondition[0]];
        let b = board[winCondition[1]];
        let c = board[winCondition[2]];

        if (a === '' || b === '' || c === '') {
            continue;
        }

        if (a === b && b === c) {
            roundWon = true;
            cells[winCondition[0]].classList.add('winning-cell');
            cells[winCondition[1]].classList.add('winning-cell');
            cells[winCondition[2]].classList.add('winning-cell');
            break;
        }
    }

    if (roundWon) {
        statusDisplay.textContent = `${currentPlayer} wins!`;
        gameActive = false;
        return;
    }

    if (!board.includes('')) {
        statusDisplay.textContent = `Draw!`;
        gameActive = false;
        return;
    }

    currentPlayer = currentPlayer === 'X' ? 'O' : 'X';
    statusDisplay.textContent = `${currentPlayer}'s turn`;
}

function aiMove() {
    let availableCells = board.map((val, idx) => val === '' ? idx : null).filter(val => val !== null);
    let randomIndex = availableCells[Math.floor(Math.random() * availableCells.length)];
    let aiCell = document.querySelector(`.cell[data-index='${randomIndex}']`);

    updateCell(aiCell, randomIndex);
    checkWinner();
}

function handleRestartGame() {
    initializeGame();
}

function handleTwoPlayerMode() {
    vsAI = false;
    initializeGame();
}

function handleAIMode() {
    vsAI = true;
    initializeGame();
}

document.getElementById('twoPlayerBtn').addEventListener('click', handleTwoPlayerMode);
document.getElementById('aiBtn').addEventListener('click', handleAIMode);
cells.forEach(cell => cell.addEventListener('click', handleCellClick));
document.getElementById('restartBtn').addEventListener('click', handleRestartGame);

initializeGame();
