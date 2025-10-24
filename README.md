<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>사과와 배 갤러리</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Inter 폰트 설정 */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f7f7;
        }
    </style>
</head>
<body class="p-4 sm:p-8 min-h-screen flex items-center justify-center">

    <div class="w-full max-w-4xl bg-white shadow-xl rounded-xl p-6 md:p-10">
        
        <!-- 제목 섹션 -->
        <header class="text-center mb-10">
            <h1 class="text-4xl font-extrabold text-red-600 mb-2">🍎 사과와 배 🍐</h1>
            <p class="text-xl text-gray-600">한국의 대표적인 과일 갤러리</p>
        </header>

        <!-- 과일 카드 컨테이너 -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">

            <!-- 1. 사과 카드 -->
            <div id="apple-card" class="bg-white border border-red-200 rounded-xl overflow-hidden shadow-lg transform transition duration-300 hover:shadow-2xl hover:-translate-y-1">
                
                <!-- 이미지 영역 -->
                <div class="h-64 overflow-hidden">
                    <!-- 사과 이미지 (업로드된 파일 사용) -->
                    <img src="uploaded:mchan0418/image/image-238a74483f1442858dfa3a982435151c8dac6270/사과.jpg" alt="탐스러운 붉은 사과" class="w-full h-full object-cover">
                </div>

                <!-- 내용 영역 -->
                <div class="p-6">
                    <h2 class="text-3xl font-bold text-red-700 mb-3">사과 (Apple)</h2>
                    <p class="text-gray-700 leading-relaxed">
                        사과는 장미과 사과나무의 열매로, <span class="font-semibold text-red-600">비타민 C와 식이섬유</span>가 풍부합니다.
                        새콤달콤한 맛과 아삭한 식감으로 전 세계적으로 사랑받는 과일입니다. "하루에 사과 하나면 의사가 필요 없다"는 말이 있을 정도로 건강에 좋습니다.
                    </p>
                    <a href="#" class="mt-4 inline-block text-red-500 hover:text-red-600 font-medium">더 알아보기 &rarr;</a>
                </div>
            </div>

            <!-- 2. 배 카드 -->
            <div id="pear-card" class="bg-white border border-green-200 rounded-xl overflow-hidden shadow-lg transform transition duration-300 hover:shadow-2xl hover:-translate-y-1">
                
                <!-- 이미지 영역 -->
                <div class="h-64 overflow-hidden">
                    <!-- 배 이미지 (업로드된 파일 사용) -->
                    <img src="uploaded:mchan0418/image/image-238a74483f1442858dfa3a982435151c8dac6270/배.jpg" alt="시원하고 달콤한 배" class="w-full h-full object-cover">
                </div>

                <!-- 내용 영역 -->
                <div class="p-6">
                    <h2 class="text-3xl font-bold text-green-700 mb-3">배 (Pear)</h2>
                    <p class="text-gray-700 leading-relaxed">
                        배는 시원하고 달콤한 맛이 일품인 과일로, <span class="font-semibold text-green-600">기관지 건강에 도움</span>을 주는 것으로 알려져 있습니다.
                        수분이 많아 갈증 해소에 탁월하며, 한국에서는 제사상이나 명절 선물로도 많이 사용됩니다.
                    </p>
                    <a href="#" class="mt-4 inline-block text-green-500 hover:text-green-600 font-medium">더 알아보기 &rarr;</a>
                </div>
            </div>

        </div>

        <!-- 푸터 -->
        <footer class="text-center mt-10 text-gray-500 text-sm">
            <p>&copy; 2025 과일 정보 제공 웹 앱. 모든 이미지는 사용자 제공입니다.</p>
        </footer>

    </div>

</body>
</html>
