<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>사과와 배 갤러리</title>
    <!-- Tailwind CSS CDN 로드 -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Inter 폰트 설정 및 배경색 지정 */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f7f7f7;
        }
    </style>
</head>
<!-- 최소 높이를 설정하고 내용을 중앙에 배치하여 깔끔한 화면을 구성합니다. -->
<body class="p-4 sm:p-8 min-h-screen flex items-center justify-center">

    <!-- 메인 컨테이너: 최대 너비 제한, 그림자 및 둥근 모서리 적용 -->
    <div class="w-full max-w-4xl bg-white shadow-2xl rounded-2xl p-6 md:p-10 border border-gray-100">
        
        <!-- 제목 섹션 -->
        <header class="text-center mb-10">
            <h1 class="text-5xl font-extrabold text-red-600 mb-2 tracking-tight">🍎 사과와 배 🍐</h1>
            <p class="text-xl text-gray-500 font-light">한국의 대표적인 과일 정보 카드</p>
        </header>

        <!-- 과일 카드 컨테이너: 모바일에서는 1열, 데스크톱에서는 2열 그리드 배치 -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">

            <!-- 1. 사과 카드 -->
            <div id="apple-card" class="bg-white border-t-4 border-red-500 rounded-xl overflow-hidden shadow-lg transform transition duration-500 hover:shadow-red-300/50 hover:shadow-2xl hover:-translate-y-1">
                
                <!-- 이미지 영역 (GitHub Raw URL로 수정됨) -->
                <div class="h-64 overflow-hidden bg-red-50">
                    <img src="https://raw.githubusercontent.com/mchan0418/image/main/%EC%82%AC%EA%B3%BC.jpg" 
                         alt="탐스러운 붉은 사과" 
                         class="w-full h-full object-cover transition duration-500 hover:scale-105"
                         <!-- 이미지 로드 실패 시 플레이스홀더를 표시하는 폴백 로직 추가 -->
                         onerror="this.onerror=null;this.src='https://placehold.co/600x400/f87171/ffffff?text=Apple';"
                    >
                </div>

                <!-- 내용 영역 -->
                <div class="p-6">
                    <h2 class="text-3xl font-bold text-red-700 mb-3 border-b pb-2 border-red-100">사과 (Apple)</h2>
                    <p class="text-gray-700 leading-relaxed text-base">
                        사과는 장미과 사과나무의 열매로, <span class="font-semibold text-red-600">비타민 C와 식이섬유</span>가 풍부합니다.
                        새콤달콤한 맛과 아삭한 식감으로 전 세계적으로 사랑받는 과일입니다. "하루에 사과 하나면 의사가 필요 없다"는 말이 있을 정도로 건강에 좋습니다.
                    </p>
                    <!-- 액션 버튼 -->
                    <a href="#" class="mt-4 inline-block text-red-500 hover:text-red-600 font-bold transition duration-300">자세히 보기 &rarr;</a>
                </div>
            </div>

            <!-- 2. 배 카드 -->
            <div id="pear-card" class="bg-white border-t-4 border-green-500 rounded-xl overflow-hidden shadow-lg transform transition duration-500 hover:shadow-green-300/50 hover:shadow-2xl hover:-translate-y-1">
                
                <!-- 이미지 영역 (GitHub Raw URL로 수정됨) -->
                <div class="h-64 overflow-hidden bg-green-50">
                    <img src="https://raw.githubusercontent.com/mchan0418/image/main/%EB%B0%B0.jpg" 
                         alt="시원하고 달콤한 배" 
                         class="w-full h-full object-cover transition duration-500 hover:scale-105"
                         <!-- 이미지 로드 실패 시 플레이스홀더를 표시하는 폴백 로직 추가 -->
                         onerror="this.onerror=null;this.src='https://placehold.co/600x400/34d399/ffffff?text=Pear';" 
                    >
                </div>

                <!-- 내용 영역 -->
                <div class="p-6">
                    <h2 class="text-3xl font-bold text-green-700 mb-3 border-b pb-2 border-green-100">배 (Pear)</h2>
                    <p class="text-gray-700 leading-relaxed text-base">
                        배는 시원하고 달콤한 맛이 일품인 과일로, <span class="font-semibold text-green-600">기관지 건강에 도움</span>을 주는 것으로 알려져 있습니다.
                        수분이 많아 갈증 해소에 탁월하며, 한국에서는 제사상이나 명절 선물로도 많이 사용됩니다.
                    </p>
                    <!-- 액션 버튼 -->
                    <a href="#" class="mt-4 inline-block text-green-500 hover:text-green-600 font-bold transition duration-300">자세히 보기 &rarr;</a>
                </div>
            </div>

        </div>

        <!-- 푸터 -->
        <footer class="text-center mt-12 text-gray-400 text-xs">
            <p>&copy; 2025 과일 정보 제공 웹 앱. 이제 실제 이미지를 사용합니다.</p>
        </footer>

    </div>

</body>
</html>
