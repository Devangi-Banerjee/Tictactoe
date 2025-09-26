<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Tic Tac Toe — Responsive</title>
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --muted:#9aa7bf;
      --accent:#7dd3fc;
      --x-color:#f97316;
      --o-color:#60a5fa;
      --glass: rgba(255,255,255,0.03);
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:Inter,ui-sans-serif,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;
      background: linear-gradient(135deg, #ffecd2, #fcb69f); /* peach gradient */
      color: #1e293b;
      display:flex;
      align-items:center;
      justify-content:center;
      padding:24px;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    .container{
      width:100%;
      max-width:520px;
      background: rgba(255,255,255,0.6);
      border-radius:16px;
      box-shadow: 0 8px 30px rgba(0,0,0,0.2);
      padding:18px;
      display:flex;
      flex-direction:column;
      gap:14px;
      border:1px solid rgba(255,255,255,0.3);
    }

    header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
    }
    h1{font-size:18px;margin:0}
    .sub{font-size:12px;color:var(--muted)}

    .board-wrap{
      display:flex;
      gap:16px;
      flex-direction:column;
      align-items:center;
      justify-content:center;
    }

    .board{
      width:100%;
      aspect-ratio:1/1;
      max-width:420px;
      display:grid;
      grid-template-columns:repeat(3,1fr);
      grid-template-rows:repeat(3,1fr);
      gap:8px;
      padding:8px;
      background: rgba(255,255,255,0.5);
      border-radius:12px;
      border:1px solid rgba(255,255,255,0.3);
    }

    .cell{
      background:#fff;
      border-radius:8px;
      display:flex;
      align-items:center;
      justify-content:center;
      font-weight:700;
      font-size:clamp(28px, 8vw, 52px);
      user-select:none;
      cursor:pointer;
      transition:transform .08s ease, box-shadow .12s ease;
      box-shadow: inset 0 -4px 10px rgba(0,0,0,0.1);
      touch-action: manipulation;
    }
    .cell:active{transform:scale(.98)}

    .cell.x{color:var(--x-color)}
    .cell.o{color:var(--o-color)}

    .cell.winning{outline:3px solid rgba(0,0,0,0.1); box-shadow:0 6px 20px rgba(0,0,0,0.2);}

    .controls{
      display:flex;
      gap:8px;
      align-items:center;
      justify-content:space-between;
      width:100%;
      flex-wrap:wrap;
    }

    .left-controls{display:flex;gap:8px;align-items:center}

    .btn{
      appearance:none;
      border:0;
      background:var(--glass);
      color:#1e293b;
      padding:8px 12px;
      border-radius:10px;
      font-weight:600;
      font-size:13px;
      cursor:pointer;
      transition:transform .12s ease, background .12s ease;
    }
    .btn:active{transform:translateY(1px)}
    .btn.primary{background:linear-gradient(90deg,#fca5a5,#fdba74); color:#fff}

    .status{
      text-align:center;
      font-size:14px;
      color:#1e293b;
    }

    .scoreboard{
      display:flex;gap:8px;align-items:center;justify-content:center;
      padding:6px 8px;border-radius:10px;background:rgba(255,255,255,0.5);
      font-size:13px;color:#1e293b;
    }
    .score-item{display:flex;flex-direction:column;align-items:center;padding:6px 8px}
    .score-item .label{font-size:11px;color:#334155}
    .score-item .value{font-weight:700;font-size:15px}

    footer{display:flex;justify-content:space-between;align-items:center;font-size:12px;color:#334155}

    @media (max-width:420px){
      .container{padding:14px}
      .board{gap:6px;padding:6px}
    }

    .overlay{
      position:fixed;
      top:0;left:0;width:100%;height:100%;
      background:linear-gradient(135deg, #fcb69f, #ffecd2);
      display:flex;
      align-items:center;
      justify-content:center;
      flex-direction:column;
      gap:16px;
      color:#1e293b;
      font-size:22px;
      z-index:100;
      visibility:hidden;
      opacity:0;
      transition:opacity 0.3s ease;
    }
    .overlay.show{visibility:visible;opacity:1;}
    .overlay button{
      padding:10px 18px;
      border-radius:8px;
      border:0;
      background:linear-gradient(90deg,#fca5a5,#fdba74);
      color:#fff;
      font-weight:700;
      cursor:pointer;
      font-size:16px;
    }
  </style>
</head>
<body>
  <div class="container" role="application" aria-label="Tic Tac Toe game">
    <header>
      <div>
        <h1>Tic Tac Toe</h1>
        <div class="sub">Tap squares to play — mobile responsive</div>
      </div>
      <div class="scoreboard">
        <div class="score-item">
          <div class="label">X (You)</div>
          <div id="scoreX" class="value">0</div>
        </div>
        <div class="score-item">
          <div class="label">Draws</div>
          <div id="scoreD" class="value">0</div>
        </div>
        <div class="score-item">
          <div class="label">O</div>
          <div id="scoreO" class="value">0</div>
        </div>
      </div>
    </header>

    <div class="board-wrap">
      <div id="status" class="status">Turn: <strong id="turnLabel">X</strong></div>
      <div id="board" class="board" role="grid"></div>
    </div>

    <div class="controls">
      <div class="left-controls">
        <button id="restart" class="btn">Restart board</button>
        <button id="resetScore" class="btn">Reset score</button>
      </div>
      <div>
        <button id="newGame" class="btn primary">New Game</button>
      </div>
    </div>

    <footer>
      <div>Keyboard: press R to restart</div>
      <div style="opacity:.6">Built with ❤️</div>
    </footer>
  </div>

  <div id="overlay" class="overlay">
    <div id="overlayMessage">Winner: X</div>
    <button id="overlayBtn">New Game</button>
  </div>

  <script>
    (function(){
      const boardEl = document.getElementById('board');
      const turnLabel = document.getElementById('turnLabel');
      const status = document.getElementById('status');
      const restartBtn = document.getElementById('restart');
      const newGameBtn = document.getElementById('newGame');
      const resetScoreBtn = document.getElementById('resetScore');
      const scoreX = document.getElementById('scoreX');
      const scoreO = document.getElementById('scoreO');
      const scoreD = document.getElementById('scoreD');
      const overlay = document.getElementById('overlay');
      const overlayMessage = document.getElementById('overlayMessage');
      const overlayBtn = document.getElementById('overlayBtn');

      let cells = [];
      let board = Array(9).fill(null);
      let current = 'X';
      let running = true;

      const WIN = [
        [0,1,2],[3,4,5],[6,7,8],
        [0,3,6],[1,4,7],[2,5,8],
        [0,4,8],[2,4,6]
      ];

      let scoreboard = JSON.parse(localStorage.getItem('ttt_score') || '{"X":0,"O":0,"D":0}');
      updateScoreUI();

      function createBoard(){
        boardEl.innerHTML = '';
        cells = [];
        for(let i=0;i<9;i++){
          const cell = document.createElement('button');
          cell.className = 'cell';
          cell.setAttribute('role','gridcell');
          cell.dataset.index = i;
          cell.addEventListener('click', onCellClick);
          boardEl.appendChild(cell);
          cells.push(cell);
        }
      }

      function onCellClick(e){
        if(!running) return;
        const idx = Number(e.currentTarget.dataset.index);
        if(board[idx]) return;
        makeMove(idx, current);
      }

      function makeMove(i, player){
        board[i] = player;
        const el = cells[i];
        el.textContent = player;
        el.classList.add(player.toLowerCase());
        const winInfo = checkWin();
        if(winInfo){
          running = false;
          showOverlay(`Winner: ${winInfo.player}`);
          scoreboard[winInfo.player]++;
          saveScore();
          updateScoreUI();
          return;
        }
        if(board.every(Boolean)){
          running = false;
          showOverlay('Draw!');
          scoreboard['D']++;
          saveScore();
          updateScoreUI();
          return;
        }
        current = current === 'X' ? 'O' : 'X';
        turnLabel.textContent = current;
        status.textContent = `Turn:`;
      }

      function checkWin(){
        for(const combo of WIN){
          const [a,b,c] = combo;
          if(board[a] && board[a] === board[b] && board[a] === board[c]){
            return {player: board[a], combo};
          }
        }
        return null;
      }

      function resetBoard(starting='X'){
        board = Array(9).fill(null);
        running = true;
        current = starting;
        turnLabel.textContent = current;
        status.textContent = `Turn:`;
        createBoard();
      }

      function newMatch(){
        const start = (Math.random() > 0.5) ? 'X' : 'O';
        resetBoard(start);
      }

      function saveScore(){
        localStorage.setItem('ttt_score', JSON.stringify(scoreboard));
      }
      function updateScoreUI(){
        scoreX.textContent = scoreboard['X'];
        scoreO.textContent = scoreboard['O'];
        scoreD.textContent = scoreboard['D'];
      }

      function showOverlay(message){
        overlayMessage.textContent = message;
        overlay.classList.add('show');
      }
      function hideOverlay(){
        overlay.classList.remove('show');
        newMatch();
      }

      restartBtn.addEventListener('click', ()=> resetBoard(current));
      newGameBtn.addEventListener('click', newMatch);
      resetScoreBtn.addEventListener('click', ()=>{
        scoreboard = {X:0,O:0,D:0}; saveScore(); updateScoreUI();
      });
      overlayBtn.addEventListener('click', hideOverlay);

      window.addEventListener('keydown', (e)=>{
        if(e.key.toLowerCase() === 'r') resetBoard(current);
      });

      createBoard();
    })();
  </script>
</body>
</html>