<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tic Tac Toe</title>
    <link rel="icon" type="image/png" href="favicon.png">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container" id="loginForm">
        <h2>Login</h2>
        <div id="loginError" class="error"></div>
        <input type="text" id="loginUsername" placeholder="Username">
        <input type="password" id="loginPassword" placeholder="Password">
        <input type="button" value="Login" onclick="login(document.getElementById('loginUsername').value,document.getElementById('loginPassword').value)">
        <p>Don't have an account? <a href="#" onclick="showRegisterForm()">Register</a></p>
    </div>
    <div class="container" id="registerForm" style="display: none;">
        <h2>Register</h2>
        <div id="registerError" class="error"></div>
        <input type="text" id="registerUsername" placeholder="Username">
        <input type="password" id="registerPassword" placeholder="Password">
        <input type="button" value="Register" onclick="register()">
        <p>Already have an account? <a href="#" onclick="showLoginForm()">Login</a></p>
    </div>

    <div id="ticTacToe" class="container" style="display: none;">
        <button id="logoutBtn" onclick="logout()">Logout</button>
        <button id="deleteUserBtn" onclick="showDeleteUserForm()">Delete User</button>
        <div id="deleteUserForm">
            <h3>Confirm Deletion</h3>
            <input type="password" id="deletePassword" placeholder="Password">
            <input type="button" value="Confirm" onclick="deleteUser()">
            <input type="button" value="Cancel" onclick="hideDeleteUserForm()">
            <div id="deleteError" class="error"></div>
        </div>
        <h2>Tic Tac Toe</h2>
        <div id="board">
            <div class="cell" onclick="cellClicked(0)"></div>
            <div class="cell" onclick="cellClicked(1)"></div>
            <div class="cell" onclick="cellClicked(2)"></div>
            <div class="cell" onclick="cellClicked(3)"></div>
            <div class="cell" onclick="cellClicked(4)"></div>
            <div class="cell" onclick="cellClicked(5)"></div>
            <div class="cell" onclick="cellClicked(6)"></div>
            <div class="cell" onclick="cellClicked(7)"></div>
            <div class="cell" onclick="cellClicked(8)"></div>
        </div>
        <div id="leaderboard">
            <h2>Leaderboard</h2>
            <table>
                <thead>
                    <tr>
                        <th>Rank</th>
                        <th>Username</th>
                        <th>Wins</th>
                        <th>Losses</th>
                    </tr>
                </thead>
                <tbody id="leaderboardBody">
                </tbody>
            </table>
        </div>
        <div id="whowon">
            <br>
            <a id="winner"></a>
            <br>
            <br>
            <button onclick="resetGame();" id="resetBtn" hidden>Play again?</button>
        </div>
    </div>

    <button id="themeChangerBtn" onclick="changeTheme()">Change Theme</button>
    <script>
    let currentTheme = 0;
    const themes = [
        {
            background: "linear-gradient(to right, #000000, #8B0000)",
            buttonColor: "#8B0000",
            textColor: "#FFFFFF"
        },
        {
            background: "linear-gradient(to right, #000000, #8A2BE2)",
            buttonColor: "#8A2BE2",
            textColor: "#FFFFFF"
        },
        {
            background: "linear-gradient(to right, #000000, #006400)",
            buttonColor: "#006400",
            textColor: "#FFFFFF"
        },
        {
            background: "linear-gradient(to right, #FFFFFF, #FFA07A)",
            buttonColor: "#FFA07A",
            textColor: "#000000"
        },
        {
            background: "linear-gradient(to right, #FFFFFF, #E6E6FA)",
            buttonColor: "#E6E6FA",
            textColor: "#000000"
        },
        {
            background: "linear-gradient(to right, #FFFFFF, #90EE90)",
            buttonColor: "#90EE90",
            textColor: "#000000"
        },
        {
            background: "linear-gradient(to right, #007bff, #28a745)",
            buttonColor: "#28a745",
            textColor: "#FFFFFF"
        },
        {
            background: "linear-gradient(to right, #ff0000, #ffff00)",
            buttonColor: "#ffff00",
            textColor: "#000000"
        },
        {
            background: "linear-gradient(to right, #800080, #ff69b4)",
            buttonColor: "#ff69b4",
            textColor: "#000000"
        },
        {
            background: "linear-gradient(to right, #008080, #00ffff)",
            buttonColor: "#00ffff",
            textColor: "#000000"
        },
        {
            background: "linear-gradient(to right, #ff8c00, #ffff00)",
            buttonColor: "#ffff00",
            textColor: "#000000"
        },
        {
            background: "linear-gradient(to right, #1E90FF, #FF4500)",
            buttonColor: "#FF4500",
            textColor: "#FFFFFF"
        },
        {
            background: "linear-gradient(to right, #4B0082, #FFD700)",
            buttonColor: "#FFD700",
            textColor: "#4B0082"
        },
        {
            background: "linear-gradient(to right, #00CED1, #FF6347)",
            buttonColor: "#FF6347",
            textColor: "#FFFFFF"
        },
        {
            background: "linear-gradient(to right, #483D8B, #32CD32)",
            buttonColor: "#32CD32",
            textColor: "#FFFFFF"
        },
    {
        background: "linear-gradient(to right, #9400D3, #FF1493)",
        buttonColor: "#FF1493",
        textColor: "#FFFFFF"
    }
    ];

    function changeTheme() {
        currentTheme = (currentTheme + 1) % themes.length;
        applyTheme(themes[currentTheme]);
    }

    function applyTheme(theme) {
        document.body.style.background = theme.background;
        document.querySelectorAll('.container').forEach(container => {
            container.style.color = theme.textColor;
        });
        document.querySelectorAll('input[type="button"]').forEach(button => {
            button.style.backgroundColor = theme.buttonColor;
        });
        document.querySelectorAll('button[id=resetBtn]').forEach(button => {
            button.style.backgroundColor = theme.buttonColor;
        });
        document.querySelectorAll('#leaderboard th').forEach(button => {
            button.style.backgroundColor = theme.buttonColor;
        });
    }

    applyTheme(themes[currentTheme]);
    function getUsers() {
            const users = localStorage.getItem('users');
            return users ? JSON.parse(users) : [];
        }
        

        function setUsers(users) {
            localStorage.setItem('users', JSON.stringify(users));
        }


        function showRegisterForm() {
            document.getElementById("loginForm").style.display = "none";
            document.getElementById("registerForm").style.display = "block";
        }

        function showLoginForm() {
            document.getElementById("loginForm").style.display = "block";
            document.getElementById("registerForm").style.display = "none";
        }

        function register() {
            let username = document.getElementById("registerUsername").value;
            let password = document.getElementById("registerPassword").value;

            if (!username || !password) {
                document.getElementById("registerError").innerHTML = "Please enter username and password.";
                return;
            }
            
            let users = getUsers();

            if (users.some(user => user.username === username)) {
                document.getElementById("registerError").innerHTML = "Username already exists.";
                return;
            }

            users.push({ username, password, wins: 0, losses: 0 });
            setUsers(users);
            document.getElementById("registerError").innerHTML = "";
            document.getElementById("registerUsername").value = "";
            document.getElementById("registerPassword").value = "";
            showTicTacToe();
            logout();
            login(username, password);
        }

        function login(username, password) {
            if (!username || !password) {
                document.getElementById("loginError").innerHTML = "Please enter username and password.";
                return;
            }
            
            let users = getUsers();

            let user = users.find(user => user.username === username && user.password === password);

            if (!user) {
                document.getElementById("loginError").innerHTML = "Invalid username or password.";
                return;
            }
            
            currentUser = user;

            document.getElementById("loginError").innerHTML = "";
            document.getElementById("loginUsername").value = "";
            document.getElementById("loginPassword").value = "";
            showTicTacToe();
        }

        function showTicTacToe() {
            document.getElementById("loginForm").style.display = "none";
            document.getElementById("registerForm").style.display = "none";
            document.getElementById("ticTacToe").style.display = "block";
            updateLeaderboard();
        }

        function cellClicked(index) {
            if (gameBoard[index] === '') {
                gameBoard[index] = currentPlayer;
                document.getElementsByClassName('cell')[index].innerHTML = currentPlayer;
                if (checkWinner(currentPlayer)) {
                    document.getElementById("winner").innerHTML = currentPlayer + " wins!";
                    if (currentPlayer === 'X') {
                        updateStats('win');
                    } else {
                        updateStats('loss');
                    }
                    document.getElementById("resetBtn").hidden = false;
                } else if (gameBoard.every(cell => cell !== '')) {
                    document.getElementById("winner").innerHTML = "It's a draw!";
                    document.getElementById("resetBtn").hidden = false;
                } else {
                    currentPlayer = currentPlayer === 'X' ? 'O' : 'X';
                    if (currentPlayer === 'O') {
                        aiMove();
                    }
                }
            }
        }
         function aiMove() {
            let emptyCells = gameBoard.map((cell, index) => cell === '' ? index : null).filter(index => index !== null);
            for (let i of emptyCells) {
                gameBoard[i] = 'O';
                if (checkWinner('O')) {
                    document.getElementsByClassName('cell')[i].innerHTML = 'O';
                    currentPlayer = 'X';
                    document.getElementById("winner").innerHTML = "O wins!";
                    updateStats('loss');
                    document.getElementById("resetBtn").hidden = false;
                    return;
                }
                gameBoard[i] = '';
            }
            for (let i of emptyCells) {
                gameBoard[i] = 'X';
                if (checkWinner('X')) {
                    gameBoard[i] = 'O';
                    document.getElementsByClassName('cell')[i].innerHTML = 'O';
                    currentPlayer = 'X';
                    return;
                }
                gameBoard[i] = '';
            }

            let move = emptyCells[Math.floor(Math.random() * emptyCells.length)];
            gameBoard[move] = 'O';
            document.getElementsByClassName('cell')[move].innerHTML = 'O';
            currentPlayer = 'X';
        }

        function checkWinner(player) {
            for (let i = 0; i < 3; i++) {
                if (gameBoard[i * 3] === player && gameBoard[i * 3 + 1] === player && gameBoard[i * 3 + 2] === player) {
                    return true;
                }
            }
            for (let i = 0; i < 3; i++) {
                if (gameBoard[i] === player && gameBoard[i + 3] === player && gameBoard[i + 6] === player) {
                    return true;
                }
            }
            if ((gameBoard[0] === player && gameBoard[4] === player && gameBoard[8] === player) ||
                (gameBoard[2] === player && gameBoard[4] === player && gameBoard[6] === player)) {
                return true;
            }
            return false;
        }

        function resetGame() {
            document.getElementById("winner").innerHTML = "";
            document.getElementById("resetBtn").hidden = true;
            gameBoard = ['', '', '', '', '', '', '', '', ''];
            currentPlayer = 'X';
            Array.from(document.getElementsByClassName('cell')).forEach(cell => cell.innerHTML = '');
        }

        function logout() {
            document.getElementById("loginForm").style.display = "block";
            document.getElementById("registerForm").style.display = "none";
            document.getElementById("ticTacToe").style.display = "none";
            currentUser = null;
        }
        function showDeleteUserForm() {
            document.getElementById('deleteUserForm').style.display = 'block';
        }

        function hideDeleteUserForm() {
            document.getElementById('deleteUserForm').style.display = 'none';
            document.getElementById('deletePassword').value = '';
            document.getElementById('deleteError').innerHTML = '';
        }

        function deleteUser() {
            let password = document.getElementById('deletePassword').value;
            if (password !== currentUser.password) {
                document.getElementById('deleteError').innerHTML = 'Incorrect password.';
                return;
            }

            let users = getUsers();
            users = users.filter(user => user.username !== currentUser.username);
            setUsers(users);
            hideDeleteUserForm();
            logout();
        }

        function updateStats(result) {
            let users = getUsers();
            let userIndex = users.findIndex(user => user.username === currentUser.username);
            if (userIndex > -1) {
                if (result === 'win') {
                    users[userIndex].wins += 1;
                } else if (result === 'loss') {
                    users[userIndex].losses += 1;
                }
                setUsers(users);
                updateLeaderboard();
            }
        }

        function updateLeaderboard() {
            let users = getUsers();
            users.sort((a, b) => (b.wins - b.losses) - (a.wins - a.losses));
            let leaderboardBody = document.getElementById('leaderboardBody');
            leaderboardBody.innerHTML = '';
            users.forEach((user, index) => {
                let row = document.createElement('tr');
                let rank = index === 0 ? "🥇" : index === 1 ? "🥈" : index === 2 ? "🥉" : index + 1;
                console.log(rank);
                row.innerHTML = `
                    <td>${rank}</td>
                    <td>${user.username}</td>
                    <td>${user.wins}</td>
                    <td>${user.losses}</td>
                `;
                leaderboardBody.appendChild(row);
            });
        }

        let currentUser = null;
        let currentPlayer = 'X';
        let gameBoard = ['', '', '', '', '', '', '', '', ''];
    </script>
</body>
</html>
