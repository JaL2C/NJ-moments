# NJ-moments
A website about meeeeeee
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>自我介紹簡報</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f4f8; /* Light blue-gray background */
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            overflow-x: hidden; /* Prevent horizontal scroll */
        }
        .slide-container {
            display: flex;
            overflow-x: auto; /* Enable horizontal scrolling for slides */
            scroll-snap-type: x mandatory; /* Snap to slides */
            width: 100%;
            height: 100vh; /* Full viewport height */
            -webkit-overflow-scrolling: touch; /* Smooth scrolling on iOS */
        }
        .slide {
            flex: 0 0 100%; /* Each slide takes full width */
            width: 100%;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background-color: white;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
            border-radius: 1.5rem; /* Rounded corners for slides */
            padding: 2rem;
            text-align: center;
            scroll-snap-align: start; /* Align slides to the start */
            transition: transform 0.5s ease-in-out;
            margin: 0 1rem; /* Spacing between slides */
            box-sizing: border-box; /* Include padding in width */
        }

        /* Responsive adjustments for smaller screens */
        @media (max-width: 768px) {
            .slide {
                padding: 1rem;
                border-radius: 1rem;
                margin: 0 0.5rem;
            }
            .slide h1 {
                font-size: 2.5rem;
            }
            .slide h2 {
                font-size: 1.75rem;
            }
            .slide p, .slide li {
                font-size: 0.9rem;
            }
        }

        .slide-content {
            max-width: 90%; /* Limit content width */
            margin: auto;
        }

        .slide-image {
            max-width: 80%;
            max-height: 40vh;
            object-fit: contain;
            border-radius: 1rem;
            margin-top: 1.5rem;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        /* Navigation buttons */
        .nav-button {
            position: fixed;
            top: 50%;
            transform: translateY(-50%);
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            border: none;
            padding: 0.75rem 1.25rem;
            border-radius: 9999px; /* Fully rounded */
            font-size: 1.5rem;
            cursor: pointer;
            z-index: 100;
            transition: background-color 0.3s ease;
        }
        .nav-button:hover {
            background-color: rgba(0, 0, 0, 0.7);
        }
        .nav-button.left {
            left: 1rem;
        }
        .nav-button.right {
            right: 1rem;
        }
    </style>
</head>
<body>

    <div class="slide-container" id="slideContainer">

        <div class="slide bg-gradient-to-br from-blue-500 to-purple-600 text-white">
            <div class="slide-content">
                <h1 class="text-5xl md:text-6xl font-extrabold mb-4 drop-shadow-lg">自我介紹</h1>
                <h2 class="text-3xl md:text-4xl font-semibold mb-6">認識 [您的名字]</h2>
                <p class="text-xl md:text-2xl mb-2">[您的名字]</p>
                <p class="text-lg md:text-xl">[您的職稱/身份，例如：軟體工程師 / 學生]</p>
                <p class="text-base md:text-lg mt-4">聯絡方式：[您的電子郵件] | [您的LinkedIn]</p>
                <img src="https://placehold.co/300x300/60a5fa/ffffff?text=您的專業照片" alt="您的專業照片" class="slide-image mx-auto mt-8 w-48 h-48 rounded-full object-cover border-4 border-white">
            </div>
        </div>

        <div class="slide">
            <div class="slide-content">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-6">關於我</h2>
                <p class="text-lg md:text-xl text-gray-700 leading-relaxed mb-6">
                    我是一個熱愛學習、充滿好奇心的 <span class="font-semibold text-blue-600">[您的職業/身份]</span>，致力於 <span class="font-semibold text-purple-600">[您的目標或熱情所在]</span>。
                </p>
                <p class="text-lg md:text-xl text-gray-700 leading-relaxed">
                    我的關鍵詞是：<span class="font-bold text-green-600">創新</span>、<span class="font-bold text-yellow-600">解決問題</span>、<span class="font-bold text-red-600">團隊合作</span>。
                </p>
                <img src="https://placehold.co/400x250/cbd5e1/334155?text=展現您個性的生活照" alt="展現您個性的生活照" class="slide-image mx-auto">
            </div>
        </div>

        <div class="slide">
            <div class="slide-content">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-6">學術背景與教育</h2>
                <ul class="text-left text-lg md:text-xl text-gray-700 space-y-4">
                    <li class="flex items-start">
                        <span class="text-blue-500 mr-3 text-2xl">&#x2022;</span>
                        <div>
                            <span class="font-semibold">最高學歷：</span><br>
                            [您的學位]，[您的主修]，[您的學校名稱]，[畢業年份]
                            <p class="text-sm text-gray-500 mt-1">例如：碩士，資訊工程，國立台灣大學，2023年</p>
                        </div>
                    </li>
                    <li class="flex items-start">
                        <span class="text-blue-500 mr-3 text-2xl">&#x2022;</span>
                        <div>
                            <span class="font-semibold">其他學歷/重要課程：</span><br>
                            [其他學位、證書或相關課程]
                        </div>
                    </li>
                    <li class="flex items-start">
                        <span class="text-blue-500 mr-3 text-2xl">&#x2022;</span>
                        <div>
                            <span class="font-semibold">學術成就/榮譽：</span><br>
                            [例如：書卷獎、論文發表、專題研究]
                        </div>
                    </li>
                </ul>
                <img src="https://placehold.co/400x250/e0e7ff/4338ca?text=學校校園照片或畢業照" alt="學校校園照片或畢業照" class="slide-image mx-auto">
            </div>
        </div>

        <div class="slide">
            <div class="slide-content">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-6">我的專業經驗</h2>
                <div class="space-y-6 text-left text-gray-700">
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-purple-700 mb-2">[公司名稱1]</h3>
                        <p class="text-lg md:text-xl mb-1">[您的職位]，[任職期間]</p>
                        <ul class="list-disc list-inside ml-4 space-y-1 text-base md:text-lg">
                            <li>主要職責與成就：[列出1-2項關鍵職責和具體成就，使用量化數據]</li>
                            <li>[另一個成就]</li>
                        </ul>
                    </div>
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-purple-700 mb-2">[公司名稱2]</h3>
                        <p class="text-lg md:text-xl mb-1">[您的職位]，[任職期間]</p>
                        <ul class="list-disc list-inside ml-4 space-y-1 text-base md:text-lg">
                            <li>主要職責與成就：[列出1-2項關鍵職責和具體成就，使用量化數據]</li>
                            <li>[另一個成就]</li>
                        </ul>
                    </div>
                </div>
                <img src="https://placehold.co/400x250/d1e7dd/2f6c4f?text=公司Logo或工作場景" alt="公司Logo或工作場景" class="slide-image mx-auto">
            </div>
        </div>

        <div class="slide">
            <div class="slide-content">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-6">我的技能與專長</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 text-left text-gray-700">
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-blue-700 mb-3">硬技能 (Hard Skills)</h3>
                        <ul class="list-disc list-inside ml-4 space-y-2 text-lg md:text-xl">
                            <li>程式語言：<span class="font-medium">[例如：Python, Java, JavaScript]</span></li>
                            <li>軟體/工具：<span class="font-medium">[例如：Figma, Photoshop, Tableau]</span></li>
                            <li>技術領域：<span class="font-medium">[例如：機器學習, 數據分析]</span></li>
                        </ul>
                    </div>
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-green-700 mb-3">軟技能 (Soft Skills)</h3>
                        <ul class="list-disc list-inside ml-4 space-y-2 text-lg md:text-xl">
                            <li>溝通能力</li>
                            <li>解決問題</li>
                            <li>團隊合作</li>
                            <li>領導力</li>
                            <li>適應力</li>
                        </ul>
                    </div>
                </div>
                <img src="https://placehold.co/400x250/cce5ff/0056b3?text=技能圖示或技能樹" alt="技能圖示或技能樹" class="slide-image mx-auto">
            </div>
        </div>

        <div class="slide">
            <div class="slide-content">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-6">我的興趣與嗜好</h2>
                <div class="space-y-6 text-left text-gray-700">
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-red-700 mb-2">興趣1：[例如：閱讀]</h3>
                        <p class="text-lg md:text-xl">簡短描述為何喜歡，以及從中獲得了什麼。</p>
                    </div>
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-yellow-700 mb-2">興趣2：[例如：攝影]</h3>
                        <p class="text-lg md:text-xl">簡短描述為何喜歡，以及從中獲得了什麼。</p>
                    </div>
                    <p class="text-base md:text-lg italic mt-4">這些興趣如何豐富您的生活或幫助您發展特定技能。</p>
                </div>
                <img src="https://placehold.co/400x250/ffe0b2/e65100?text=展示您興趣的照片" alt="展示您興趣的照片" class="slide-image mx-auto">
            </div>
        </div>

        <div class="slide">
            <div class="slide-content">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-6">我的熱情與價值觀</h2>
                <div class="space-y-6 text-left text-gray-700">
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-indigo-700 mb-2">我的熱情：</h3>
                        <p class="text-lg md:text-xl">[例如：透過科技改善生活、推動永續發展]</p>
                    </div>
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-teal-700 mb-2">核心價值觀：</h3>
                        <ul class="list-disc list-inside ml-4 space-y-1 text-lg md:text-xl">
                            <li>誠信</li>
                            <li>創新</li>
                            <li>責任</li>
                            <li>同理心</li>
                            <li>持續成長</li>
                        </ul>
                    </div>
                    <p class="text-base md:text-lg italic mt-4">這些熱情和價值觀如何引導您的決策和行為。</p>
                </div>
                <img src="https://placehold.co/400x250/d0f0c0/007f00?text=表達熱情或價值觀的圖片" alt="表達熱情或價值觀的圖片" class="slide-image mx-auto">
            </div>
        </div>

        <div class="slide">
            <div class="slide-content">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-6">重要成就與專案</h2>
                <div class="space-y-6 text-left text-gray-700">
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-orange-700 mb-2">專案/成就1：[專案名稱/成就]</h3>
                        <ul class="list-disc list-inside ml-4 space-y-1 text-base md:text-lg">
                            <li><span class="font-medium">角色：</span>[您的角色]</li>
                            <li><span class="font-medium">挑戰與解決方案：</span>[簡述遇到的挑戰及如何克服]</li>
                            <li><span class="font-medium">成果：</span>[具體成果，使用量化數據]</li>
                        </ul>
                    </div>
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-orange-700 mb-2">專案/成就2：[專案名稱/成就]</h3>
                        <ul class="list-disc list-inside ml-4 space-y-1 text-base md:text-lg">
                            <li><span class="font-medium">角色：</span>[您的角色]</li>
                            <li><span class="font-medium">挑戰與解決方案：</span>[簡述遇到的挑戰及如何克服]</li>
                            <li><span class="font-medium">成果：</span>[具體成果，使用量化數據]</li>
                        </ul>
                    </div>
                </div>
                <img src="https://placehold.co/400x250/f0e68c/8b4513?text=專案成果截圖或圖片" alt="專案成果截圖或圖片" class="slide-image mx-auto">
            </div>
        </div>

        <div class="slide">
            <div class="slide-content">
                <h2 class="text-4xl md:text-5xl font-bold text-gray-800 mb-6">未來目標與展望</h2>
                <div class="space-y-6 text-left text-gray-700">
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-cyan-700 mb-2">短期目標：</h3>
                        <p class="text-lg md:text-xl">[例如：學習新技能、完成某項認證]</p>
                    </div>
                    <div>
                        <h3 class="text-2xl md:text-3xl font-semibold text-cyan-700 mb-2">長期目標：</h3>
                        <p class="text-lg md:text-xl">[例如：成為領域專家、創業、在特定產業做出貢獻]</p>
                    </div>
                    <p class="text-base md:text-lg italic mt-4">您希望在未來如何成長和發展，以及對未來的期待和願景。</p>
                </div>
                <img src="https://placehold.co/400x250/b0e0e6/006064?text=代表未來或成長的圖片" alt="代表未來或成長的圖片" class="slide-image mx-auto">
            </div>
        </div>

        <div class="slide bg-gradient-to-br from-green-500 to-blue-500 text-white">
            <div class="slide-content">
                <h1 class="text-5xl md:text-6xl font-extrabold mb-4 drop-shadow-lg">謝謝聆聽！</h1>
                <p class="text-2xl md:text-3xl font-semibold mb-6">請問有任何問題嗎？</p>
                <p class="text-xl md:text-2xl mb-2">再次聯絡方式：</p>
                <p class="text-lg md:text-xl">[您的電子郵件]</p>
                <p class="text-lg md:text-xl">[您的LinkedIn]</p>
                <img src="https://placehold.co/300x300/a7f3d0/065f46?text=簡潔的感謝圖片" alt="簡潔的感謝圖片" class="slide-image mx-auto mt-8 w-48 h-48 rounded-full object-cover border-4 border-white">
            </div>
        </div>

    </div>

    <button class="nav-button left" onclick="prevSlide()">&#10094;</button>
    <button class="nav-button right" onclick="nextSlide()">&#10095;</button>

    <script>
        const slideContainer = document.getElementById('slideContainer');
        const slides = document.querySelectorAll('.slide');
        let currentSlideIndex = 0;

        // Function to scroll to a specific slide
        function scrollToSlide(index) {
            if (index >= 0 && index < slides.length) {
                slideContainer.scrollTo({
                    left: slides[index].offsetLeft - slideContainer.offsetLeft,
                    behavior: 'smooth'
                });
                currentSlideIndex = index;
            }
        }

        // Next slide
        function nextSlide() {
            scrollToSlide(currentSlideIndex + 1);
        }

        // Previous slide
        function prevSlide() {
            scrollToSlide(currentSlideIndex - 1);
        }

        // Keyboard navigation (optional, for desktop experience)
        document.addEventListener('keydown', (e) => {
            if (e.key === 'ArrowRight') {
                nextSlide();
            } else if (e.key === 'ArrowLeft') {
                prevSlide();
            }
        });

        // Update current slide index on scroll (for touch/drag)
        slideContainer.addEventListener('scroll', () => {
            const scrollLeft = slideContainer.scrollLeft;
            const slideWidth = slides[0].offsetWidth + (parseFloat(getComputedStyle(slides[0]).marginLeft) * 2); // Slide width + margins
            currentSlideIndex = Math.round(scrollLeft / slideWidth);
        });

        // Ensure initial scroll position is correct on load
        window.onload = () => {
            scrollToSlide(0);
        };

        // Handle resize to adjust scroll position
        window.addEventListener('resize', () => {
            scrollToSlide(currentSlideIndex);
        });
    </script>
</body>
</html>
