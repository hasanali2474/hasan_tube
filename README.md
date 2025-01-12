الكود
<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>قناة Hasan Tube</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Cairo', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            transition: background-color 0.3s, color 0.3s;
        }
        header {
            background-color: rgba(0, 0, 0, 0.85);
            padding: 40px;
            border-bottom: 5px solid #007bff;
            text-align: center;
            color: #fff;
        }
        h1 {
            margin: 0;
            font-size: 48px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
        }
        .logo {
            font-size: 36px;
            font-weight: 700;
            margin-bottom: 10px;
        }
        .hero-image {
            width: 100%;
            height: auto;
            max-height: 400px;
            object-fit: cover;
            border-radius: 10px;
            margin-bottom: 20px;
        }
        nav {
            margin: 50px 0;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        nav button {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 15px 30px;
            margin: 10px;
            cursor: pointer;
            border-radius: 5px;
            font-size: 20px;
            transition: background-color 0.3s, transform 0.3s;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        nav button:hover {
            background-color: #0056b3;
            transform: scale(1.05);
        }
        .icon {
            margin-right: 8px;
        }
        .settings {
            position: relative;
            display: inline-block;
        }
        .popup {
            display: none;
            position: fixed;
            z-index: 10;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.2);
            padding: 20px;
            width: 300px;
        }
        .popup-header {
            font-size: 20px;
            font-weight: bold;
            margin-bottom: 10px;
        }
        .popup-content {
            margin: 15px 0;
        }
        .popup button {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 10px;
            border-radius: 5px;
            cursor: pointer;
            width: 100%;
            transition: background-color 0.3s;
        }
        .popup button:hover {
            background-color: #0056b3;
        }
        .videos-section {
            margin: 50px 0;
            text-align: center;
        }
        .video-card {
            display: inline-block;
            margin: 10px;
            border: 1px solid #ddd;
            border-radius: 10px;
            overflow: hidden;
            width: 300px;
            background-color: #fff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .video-card img {
            width: 100%;
            height: auto;
        }
        .video-title {
            padding: 10px;
            font-size: 18px;
            font-weight: bold;
        }
        .comments-section {
            margin-top: 20px;
            text-align: left;
            padding: 10px;
            border-top: 1px solid #ddd;
        }
        .comments-section h3 {
            margin-top: 0;
        }
        .comment {
            display: flex;
            align-items: center;
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            background-color: #f9f9f9;
        }
        .comment img {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            margin-left: 10px;
            margin-right: 10px;
        }
        .comment-input {
            width: 100%;
            padding: 10px;
            margin-top: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        footer {
            text-align: center;
            margin-top: 30px;
            font-size: 16px;
            background-color: rgba(0, 0, 0, 0.85);
            color: #fff;
            padding: 15px;
        }
        /* Styles for dark mode */
        body.dark-mode {
            background-color: #121212;
            color: #ffffff;
        }
        body.dark-mode header {
            background-color: #1e1e1e;
        }
        body.dark-mode .popup {
            background-color: #1e1e1e;
            color: #ffffff;
        }
        body.dark-mode .video-card {
            background-color: #1e1e1e;
            border: 1px solid #444;
        }
        body.dark-mode .comment {
            background-color: #2a2a2a;
            border: 1px solid #444;
        }
        body.dark-mode .comment-input {
            background-color: #333;
            color: #ffffff;
            border: 1px solid #444;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo" id="logo">hasan_tube</div>
        <h1 id="welcome-message">مرحبًا بكم في قناة Hasan Tube</h1>
    </header>
    <img src="https://example.com/hero-image.jpg" alt="صورة قناة Hasan Tube" class="hero-image"> <!-- استبدل هذا بالرابط الصحيح -->
    <nav>
        <button onclick="window.open('https://youtu.be/oM41ZNcLESM?si=GbIaObMi-yUGqEBa', '_blank')"><i class="fas fa-video icon"></i><span id="latest-video">آخر فيديو</span></button>
        <button onclick="window.open('https://www.youtube.com/@hasan_tube_1791', '_blank')"><i class="fas fa-bell icon"></i><span id="subscribe">الاشتراك</span></button>
        <button onclick="window.open('رابط_اللعبة', '_blank')"><i class="fas fa-gamepad icon"></i><span id="play-game">العب اللعبة</span></button>
        <button onclick="window.open('https://www.youtube.com/@hasan_tube_1791', '_blank')"><i class="fas fa-chevron-right icon"></i><span id="go-channel">انتقل للقناة</span></button>
        <div class="settings">
            <button onclick="togglePopup()"><i class="fas fa-cog icon"></i>الإعدادات</button>
        </div>
    </nav>
    
    <div class="videos-section">
        <h2 id="latest-videos">أحدث الفيديوهات</h2>
        <div class="video-card">
            <img src="https://example.com/video1.jpg" alt="فيديو 1"> <!-- استبدل هذا بالرابط الصحيح -->
            <div class="video-title" id="video1-title">افتتاح سيرفر hasan_tube | شرح الميني جيمز</div>
            <div class="comments-section">
                <h3>التعليقات</h3>
                <div id="comments1"></div>
                <input type="text" id="username1" placeholder="اسم المستخدم" class="comment-input" />
                <textarea class="comment-input" id="commentInput1" placeholder="أضف تعليقك هنا..."></textarea>
                <button onclick="addComment('comments1', 'commentInput1', 'username1')">إرسال</button>
            </div>
        </div>
        <div class="video-card">
            <img src="https://example.com/video2.jpg" alt="فيديو 2"> <!-- استبدل هذا بالرابط الصحيح -->
            <div class="video-title" id="video2-title">مون كرافت طرق السبون</div>
            <div class="comments-section">
                <h3>التعليقات</h3>
                <div id="comments2"></div>
                <input type="text" id="username2" placeholder="اسم المستخدم" class="comment-input" />
                <textarea class="comment-input" id="commentInput2" placeholder="أضف تعليقك هنا..."></textarea>
                <button onclick="addComment('comments2', 'commentInput2', 'username2')">إرسال</button>
            </div>
        </div>
        <div class="video-card">
            <img src="https://example.com/video3.jpg" alt="فيديو 3"> <!-- استبدل هذا بالرابط الصحيح -->
            <div class="video-title" id="video3-title">مون كرافت بنار البيت الاسطوري</div>
            <div class="comments-section">
                <h3>التعليقات</h3>
                <div id="comments3"></div>
                <input type="text" id="username3" placeholder="اسم المستخدم" class="comment-input" />
                <textarea class="comment-input" id="commentInput3" placeholder="أضف تعليقك هنا..."></textarea>
                <button onclick="addComment('comments3', 'commentInput3', 'username3')">إرسال</button>
            </div>
        </div>
    </div>
    
    <div class="popup" id="settingsPopup">
        <div class="popup-header">الإعدادات</div>
        <div class="popup-content">
            <label>
                <input type="checkbox" id="darkModeToggle" onchange="toggleDarkMode()"> تفعيل الوضع الداكن
            </label>
            <div>
                <label for="languageSelect">اختر اللغة:</label>
                <select id="languageSelect" onchange="changeLanguage()">
                    <option value="ar">العربية</option>
                    <option value="en">الإنجليزية</option>
                </select>
            </div>
        </div>
        <button onclick="closePopup()">إغلاق</button>
    </div>

    <footer>
        &copy; 2025 قناة Hasan Tube. جميع الحقوق محفوظة.
    </footer>

    <script>
        function togglePopup() {
            const popup = document.getElementById('settingsPopup');
            popup.style.display = popup.style.display === 'block' ? 'none' : 'block';
        }

        function closePopup() {
            document.getElementById('settingsPopup').style.display = 'none';
        }

        function changeLanguage() {
            const selectedLanguage = document.getElementById('languageSelect').value;
            const translations = {
                ar: {
                    welcome: "مرحبًا بكم في قناة Hasan Tube",
                    latestVideo: "آخر فيديو",
                    subscribe: "الاشتراك",
                    playGame: "العب اللعبة",
                    goChannel: "انتقل للقناة",
                    latestVideos: "أحدث الفيديوهات",
                    video1Title: "افتتاح سيرفر hasan_tube | شرح الميني جيمز",
                    video2Title: "مون كرافت طرق السبون",
                    video3Title: "مون كرافت بنار البيت الاسطوري",
                },
                en: {
                    welcome: "Welcome to Hasan Tube Channel",
                    latestVideo: "Latest Video",
                    subscribe: "Subscribe",
                    playGame: "Play Game",
                    goChannel: "Go to Channel",
                    latestVideos: "Latest Videos",
                    video1Title: "Opening hasan_tube Server | Mini Games Explanation",
                    video2Title: "Minecraft Spawn Methods",
                    video3Title: "Minecraft Fire in the Legendary House",
                }
            };

            document.getElementById('welcome-message').innerText = translations[selectedLanguage].welcome;
            document.getElementById('latest-video').innerText = translations[selectedLanguage].latestVideo;
            document.getElementById('subscribe').innerText = translations[selectedLanguage].subscribe;
            document.getElementById('play-game').innerText = translations[selectedLanguage].playGame;
            document.getElementById('go-channel').innerText = translations[selectedLanguage].goChannel;
            document.getElementById('latest-videos').innerText = translations[selectedLanguage].latestVideos;
            document.getElementById('video1-title').innerText = translations[selectedLanguage].video1Title;
            document.getElementById('video2-title').innerText = translations[selectedLanguage].video2Title;
            document.getElementById('video3-title').innerText = translations[selectedLanguage].video3Title;
        }

        function toggleDarkMode() {
            const body = document.body;
            const isDarkMode = document.getElementById('darkModeToggle').checked;

            if (isDarkMode) {
                body.classList.add('dark-mode');
            } else {
                body.classList.remove('dark-mode');
            }
        }

        function addComment(commentsId, inputId, usernameId) {
            const commentInput = document.getElementById(inputId);
            const commentText = commentInput.value;
            const username = document.getElementById(usernameId).value || "مستخدم";
            const timestamp = new Date().toLocaleString(); // الحصول على التاريخ والوقت الحالي

            if (commentText.trim() !== "") {
                const commentsDiv = document.getElementById(commentsId);
                const newComment = document.createElement("div");
                newComment.className = "comment";
                newComment.innerHTML = `
                    <span>${username}: ${commentText} <small style="color: gray;">(${timestamp})</small></span> 
                    <button onclick="editComment(this)">تعديل</button>
                    <button onclick="deleteComment(this)">حذف</button>
                `;
                commentsDiv.appendChild(newComment);
                commentInput.value = ""; // مسح حقل التعليق
            } else {
                alert("يرجى كتابة تعليق.");
            }
        }

        function editComment(button) {
            const commentDiv = button.parentElement;
            const commentText = commentDiv.querySelector('span').innerText.split(': ')[1];
            const username = commentDiv.querySelector('span').innerText.split(': ')[0];

            const newCommentText = prompt("تعديل التعليق:", commentText);
            if (newCommentText !== null) {
                commentDiv.querySelector('span').innerText = `${username}: ${newCommentText}`;
            }
        }

        function deleteComment(button) {
            const commentDiv = button.parentElement;
            commentDiv.remove();
        }
    </script>
</body>
</html>
