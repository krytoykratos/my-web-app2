<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Veya Web App</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            background-color: #f4f8fb;
        }

        .container {
            background: #fff;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
            text-align: center;
            width: 100%;
            max-width: 800px;
            height: 100%;
            display: flex;
            flex-direction: column;
            justify-content: flex-start;
        }

        h1 {
            font-size: 26px;
            color: #007bff;
            margin-bottom: 20px;
        }

        .profile-section, .friends-section, .activities-section, .games-section {
            width: 100%;
            display: none;
            flex-direction: column;
            align-items: center;
            padding: 20px;
            margin-bottom: 20px;
            background-color: #fff;
            border-radius: 15px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
        }

        .profile-header {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
            width: 100%;
        }

        .avatar {
            width: 90px;
            height: 90px;
            border-radius: 50%;
            margin-right: 20px;
        }

        .profile-info {
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            flex-grow: 1;
        }

        .profile-info p {
            font-size: 16px;
            margin: 5px 0;
            color: #333;
        }

        .balance-container {
            background-color: #007bff;
            color: white;
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 20px;
            width: 100%;
            text-align: center;
        }

        .balance-container .tokens {
            font-size: 36px;
            font-weight: bold;
        }

        .balance-container .price {
            font-size: 14px;
            margin-top: 10px;
        }

        .button-container {
            display: flex;
            justify-content: space-between;
            width: 100%;
            padding: 10px;
            background-color: #fff;
            border-top: 1px solid #ddd;
        }

        .button-container .button {
            flex-grow: 1;
            font-size: 12px;
            padding: 6px;
            border-radius: 8px;
            border: none;
            background-color: #007bff;
            color: white;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .button-container .button:hover {
            background-color: #0056b3;
        }

        /* Секционные стили */
        .section h2 {
            font-size: 18px;
            color: #007bff;
        }

        .section p {
            font-size: 14px;
        }

        /* Стили для Home */
        .home-container {
            text-align: center;
            margin-top: 20px;
        }

        .home-info {
            margin-top: 20px;
        }

        .home-info p {
            font-size: 16px;
            color: #333;
        }

        /* Стили для Footer */
        .footer {
            font-size: 10px;
            color: #777;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Veya Web App</h1>

        <!-- Home Section -->
        <div class="home-container" id="homeSection">
            <div class="balance-container">
                <div class="tokens" id="tokenAmount">100 токенов</div>
                <div class="price" id="tokenPrice">$5.00</div>
            </div>

            <div class="home-info">
                <p><strong>Ранг:</strong> #30</p>
                <p><strong>Уровень:</strong> 10</p>
                <p><strong>Примерная стоимость:</strong> $5.00</p>
            </div>
        </div>

        <!-- Profile Section -->
        <div class="profile-section" id="profileSection">
            <div class="profile-header">
                <img src="https://www.gravatar.com/avatar/4b5c2b9992b1f61da7e8b7a2822d1bfc?s=80" alt="Avatar" class="avatar"> 
                <div class="profile-info">
                    <h2>Мой профиль</h2>
                    <p><strong>Ранг:</strong> #10</p>
                    <p><strong>Привязан кошелек:</strong> 1234...5678</p>
                    <p><strong>Статус подписки:</strong> Премиум активирован</p>
                </div>
            </div>

            <div class="balance-container">
                <div class="tokens" id="tokenAmountProfile">100 токенов</div>
                <div class="price" id="tokenPriceProfile">$5.00</div>
            </div>

            <div class="profile-info">
                <p><strong>Уровень:</strong> 10</p>
                <p><strong>Количество рефералов:</strong> 5</p>
                <p><strong>Донат:</strong> 0.1 TON</p>
                <p><strong>Сыгранных игр:</strong> 3</p>
                <p><strong>Дата присоединения:</strong> 01.01.2024</p>
            </div>
        </div>

        <!-- Friends Section -->
        <div class="friends-section" id="friendsSection">
            <h2>Реферальная информация</h2>
            <p>Реферальная ссылка: <a href="https://t.me/VeyaCrypto?start=12345" target="_blank">https://t.me/VeyaCrypto?start=12345</a></p>
            <p>Количество приглашенных: 10</p>
            <p>Заработанные токены рефералами: 150 токенов</p>
        </div>

        <!-- Activities Section -->
        <div class="activities-section" id="activitiesSection">
            <h2>Квесты</h2>
            <p>Квест: Подпишитесь на наш официальный телеграмм-канал Veya</p>
            <button class="button" onclick="subscribeTelegram()">Подписаться</button>
            <button class="button" onclick="checkSubscription()">Проверить подписку</button>
        </div>

        <!-- Games Section -->
        <div class="games-section" id="gamesSection">
            <h2>Игры</h2>
            <button class="button" onclick="playGame()">Играть</button>
        </div>

        <!-- Footer -->
        <div class="footer">
            <p>Все права защищены. © Veya 2025</p>
        </div>

        <!-- Button Container -->
        <div class="button-container">
            <button class="button" onclick="showFriends()">Friends</button>
            <button class="button" onclick="showActivities()">Activities</button>
            <button class="button" onclick="showHome()">Home</button>
            <button class="button" onclick="showGames()">Games</button>
            <button class="button" onclick="showProfile()">Profile</button>
        </div>
    </div>

    <script>
        // Sample Profile Data
        let user = {
            rank: 10,
            walletStatus: '1234...5678',
            subscriptionStatus: 'Премиум активирован',
            tokens: 100,
            tokenPrice: 5.00,
            level: 10,
            referrals: 5,
            donation: 0.1,
            playedGames: 3,
            joinDate: '01.01.2024'
        };

        // Function to show the profile section
        function showProfile() {
            hideSections();
            document.getElementById('profileSection').style.display = 'block';
        }

        // Function to show the home section
        function showHome() {
            hideSections();
            document.getElementById('homeSection').style.display = 'block';
        }

        // Function to show the friends section
        function showFriends() {
            hideSections();
            document.getElementById('friendsSection').style.display = 'block';
        }

        // Function to show the activities section
        function showActivities() {
            hideSections();
            document.getElementById('activitiesSection').style.display = 'block';
        }

        // Function to show the games section
        function showGames() {
            hideSections();
            document.getElementById('gamesSection').style.display = 'block';
        }

        // Hide all sections
        function hideSections() {
            const sections = document.querySelectorAll('.profile-section, .friends-section, .activities-section, .games-section, .home-container');
            sections.forEach(section => {
                section.style.display = 'none';
            });
        }

        // Initialize profile section
        function initializeProfile() {
            document.getElementById('tokenAmountProfile').textContent = `${user.tokens} токенов`;
            document.getElementById('tokenPriceProfile').textContent = `$${user.tokenPrice * user.tokens}`;
        }

        // Initialize home section
        function initializeHome() {
            document.getElementById('tokenAmount').textContent = `${user.tokens} токенов`;
            document.getElementById('tokenPrice').textContent = `$${user.tokenPrice * user.tokens}`;
        }

        // Initialization
        initializeProfile();
        initializeHome();
        showHome();
    </script>
</body>
</html>
