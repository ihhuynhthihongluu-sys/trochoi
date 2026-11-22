<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hành Trình Mùa Thu 1945 - Game Trắc Nghiệm Lịch Sử Nghệ Thuật</title>
  
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  
  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Be+Vietnam+Pro:ital,wght@0,400;0,500;0,600;0,700;0,800;1,400&family=Merriweather:ital,wght@0,400;0,700;1,400&family=Playfair+Display:ital,wght@0,700;0,900;1,700&display=swap" rel="stylesheet">
  
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            paper: {
              50: '#FDFBF7',
              100: '#FAF4E8',
              200: '#F3E7D3',
              300: '#E7D5BA',
              400: '#D6BF9C',
              800: '#4A3B32',
              900: '#2A1F1A'
            },
            rev: {
              red: '#B91C1C',
              darkred: '#7F1D1D',
              gold: '#D97706',
              brightgold: '#F59E0B',
              ink: '#1C1917'
            }
          },
          fontFamily: {
            display: ['Playfair Display', 'Georgia', 'serif'],
            serif: ['Merriweather', 'Georgia', 'serif'],
            sans: ['Be Vietnam Pro', 'sans-serif']
          }
        }
      }
    }
  </script>

  <style>
    body {
      background-color: #160F0C;
      color: #1C1917;
      font-family: 'Be Vietnam Pro', sans-serif;
      background-image: 
        radial-gradient(#38271E 1px, transparent 1px),
        linear-gradient(to bottom, rgba(22, 15, 12, 0.97), rgba(15, 10, 8, 0.99));
      background-size: 24px 24px, 100% 100%;
    }

    .paper-card {
      background-color: #FAF4E8;
      background-image: radial-gradient(#E7D5BA 0.8px, transparent 0.8px);
      background-size: 14px 14px;
      box-shadow: 0 15px 40px -5px rgba(0, 0, 0, 0.75), 0 4px 10px -2px rgba(0, 0, 0, 0.5);
      border: 2px solid #D6BF9C;
    }

    .wood-frame {
      border: 3px solid #78350F;
      box-shadow: inset 0 0 0 2px #F3E7D3, 0 8px 24px rgba(0,0,0,0.5);
    }

    .stamp-badge {
      border: 2.5px dashed #B91C1C;
      color: #B91C1C;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      transform: rotate(-1.2deg);
      font-weight: 800;
      background-color: rgba(254, 243, 199, 0.6);
    }

    .option-btn {
      transition: all 0.25s cubic-bezier(0.4, 0, 0.2, 1);
    }
    .option-btn:hover:not(:disabled) {
      transform: translateY(-2px);
      box-shadow: 0 6px 18px rgba(185, 28, 28, 0.18);
    }

    /* Ken Burns Smooth Scene Motion */
    @keyframes kenburns {
      0% { transform: scale(1) translate(0, 0); }
      50% { transform: scale(1.05) translate(-1%, -1%); }
      100% { transform: scale(1) translate(0, 0); }
    }
    .ken-burns-anim {
      animation: kenburns 16s ease-in-out infinite alternate;
    }

    /* Autumn Light Overlay Animation */
    @keyframes autumnSunbeam {
      0%, 100% { opacity: 0.35; transform: rotate(0deg); }
      50% { opacity: 0.65; transform: rotate(1deg); }
    }
    .sunbeam-overlay {
      background: radial-gradient(circle at 80% 20%, rgba(245, 158, 11, 0.25) 0%, rgba(185, 28, 28, 0.08) 50%, transparent 80%);
      animation: autumnSunbeam 8s ease-in-out infinite;
    }

    /* Star Sparkles Animation for Correct Answer */
    @keyframes starBurst {
      0% { transform: scale(0) rotate(0deg); opacity: 1; }
      100% { transform: scale(1.8) rotate(180deg); opacity: 0; }
    }
    .star-sparkle {
      animation: starBurst 0.8s cubic-bezier(0.1, 0.8, 0.3, 1) forwards;
    }

    /* Scrollbar Styling */
    ::-webkit-scrollbar {
      width: 6px;
      height: 6px;
    }
    ::-webkit-scrollbar-track {
      background: #E7D5BA;
      border-radius: 4px;
    }
    ::-webkit-scrollbar-thumb {
      background: #9A7B56;
      border-radius: 4px;
    }
    ::-webkit-scrollbar-thumb:hover {
      background: #78350F;
    }

    @keyframes pulseScale {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.03); }
    }
    .pulse-scale {
      animation: pulseScale 2.2s infinite ease-in-out;
    }
  </style>
</head>
<body class="min-h-screen flex flex-col justify-between p-2 sm:p-4 md:p-6 text-stone-900 selection:bg-rev-red selection:text-white">

  <!-- TOP APP NAVIGATION HEADER -->
  <header class="max-w-5xl w-full mx-auto mb-3 bg-paper-100 border-2 border-rev-gold/60 rounded-2xl p-3 sm:p-4 shadow-2xl flex items-center justify-between gap-3">
    <div class="flex items-center space-x-3">
      <div class="w-10 h-10 sm:w-12 sm:h-12 rounded-2xl bg-gradient-to-br from-rev-red to-rev-darkred flex items-center justify-center text-rev-brightgold text-2xl font-black shadow-lg border-2 border-rev-gold shrink-0 transform rotate-[-2deg]">
        ★
      </div>
      <div>
        <h1 class="font-display font-black text-lg sm:text-2xl text-rev-darkred tracking-tight leading-none flex items-center gap-2">
          HÀNH TRÌNH MÙA THU 1945
          <span class="text-[10px] sm:text-xs font-sans font-bold bg-rev-gold/20 text-amber-900 border border-rev-gold px-2 py-0.5 rounded-full uppercase tracking-wider">Phiên bản Nghệ Thuật</span>
        </h1>
        <p class="text-[11px] sm:text-xs text-amber-900 font-semibold tracking-wide mt-0.5">
          ĐẤU TRƯỜNG TRẮC NGHIỆM LỊCH SỬ CÁCH MẠNG THÁNG TÁM
        </p>
      </div>
    </div>

    <!-- Sound & Control Buttons -->
    <div class="flex items-center space-x-2">
      <button id="btnSound" onclick="toggleSound()" class="px-3 py-1.5 rounded-xl bg-paper-200 hover:bg-paper-300 text-stone-800 transition-colors text-xs font-bold border border-paper-400 flex items-center gap-1.5 shadow-sm">
        <span id="soundIcon">🔊</span>
        <span class="hidden sm:inline">Âm thanh</span>
      </button>

      <button onclick="confirmRestart()" class="px-3 py-1.5 rounded-xl bg-rev-red hover:bg-rev-darkred text-white transition-colors text-xs font-bold shadow flex items-center gap-1 border border-rev-gold">
        🔄 <span class="hidden sm:inline">Chơi lại</span>
      </button>
    </div>
  </header>

  <!-- MAIN APPLICATION AREA -->
  <main class="max-w-5xl w-full mx-auto flex-1 flex flex-col justify-center">

    <!-- 1. WELCOME & MODE SELECTION SCREEN -->
    <section id="welcomeScreen" class="paper-card rounded-3xl p-5 sm:p-8 md:p-10 wood-frame max-w-3xl mx-auto w-full my-auto space-y-6 text-center">
      
      <!-- Poster Banner Scene SVG -->
      <div class="relative w-full h-40 sm:h-52 rounded-2xl overflow-hidden border-2 border-rev-gold shadow-md bg-stone-900 flex items-center justify-center">
        <svg class="w-full h-full object-cover ken-burns-anim" viewBox="0 0 800 300" preserveAspectRatio="xMidYMid slice">
          <defs>
            <linearGradient id="skyGrad" x1="0" y1="0" x2="0" y2="1">
              <stop offset="0%" stop-color="#7F1D1D"/>
              <stop offset="60%" stop-color="#D97706"/>
              <stop offset="100%" stop-color="#FAF4E8"/>
            </linearGradient>
          </defs>
          <rect width="800" height="300" fill="url(#skyGrad)"/>
          
          <!-- Sunburst Rays -->
          <g opacity="0.25" stroke="#F59E0B" stroke-width="4">
            <line x1="400" y1="150" x2="0" y2="0"/><line x1="400" y1="150" x2="200" y2="0"/>
            <line x1="400" y1="150" x2="400" y2="0"/><line x1="400" y1="150" x2="600" y2="0"/>
            <line x1="400" y1="150" x2="800" y2="0"/><line x1="400" y1="150" x2="800" y2="150"/>
            <line x1="400" y1="150" x2="800" y2="300"/><line x1="400" y1="150" x2="0" y2="300"/>
          </g>

          <!-- Hanoi Opera House Silhouette -->
          <path d="M 220 230 L 220 170 L 250 170 L 250 150 L 350 150 L 350 120 L 450 120 L 450 150 L 550 150 L 550 170 L 580 170 L 580 230 Z" fill="#2A1F1A" opacity="0.85"/>
          <polygon points="350,120 400,80 450,120" fill="#2A1F1A"/>

          <!-- Flag Pole and Large Waving Red Flag with Yellow Star -->
          <line x1="400" y1="80" x2="400" y2="20" stroke="#FAF4E8" stroke-width="4"/>
          <path d="M 400 20 Q 430 10 460 25 Q 490 40 520 20 L 520 70 Q 490 90 460 75 Q 430 60 400 70 Z" fill="#B91C1C" stroke="#F59E0B" stroke-width="2"/>
          <polygon points="460,40 466,54 481,54 469,63 473,77 460,68 447,77 451,63 439,54 454,54" fill="#F59E0B"/>

          <!-- People Crowd Silhouettes -->
          <path d="M 0 300 Q 150 250 300 270 T 600 260 T 800 300 Z" fill="#1C1917"/>
          <circle cx="150" cy="245" r="14" fill="#1C1917"/>
          <circle cx="210" cy="235" r="16" fill="#1C1917"/>
          <circle cx="280" cy="240" r="15" fill="#1C1917"/>
          <circle cx="520" cy="238" r="16" fill="#1C1917"/>
          <circle cx="620" cy="245" r="15" fill="#1C1917"/>
          <!-- Raised arms & banners -->
          <line x1="210" y1="235" x2="225" y2="205" stroke="#1C1917" stroke-width="4"/>
          <line x1="520" y1="238" x2="505" y2="200" stroke="#1C1917" stroke-width="4"/>
        </svg>

        <div class="absolute inset-0 bg-gradient-to-t from-stone-950/90 via-transparent to-transparent flex items-end justify-center pb-3">
          <span class="stamp-badge px-4 py-1 text-xs sm:text-sm font-black shadow-lg">
            CHINH PHỤC CÁC MỐC THỜI CƠ VÀNG 1945
          </span>
        </div>
      </div>

      <div class="space-y-2">
        <h2 class="font-display font-black text-3xl sm:text-4xl text-rev-darkred">
          Hành Trình Mùa Thu Lịch Sử
        </h2>
        <p class="text-xs sm:text-sm text-stone-700 max-w-xl mx-auto italic leading-relaxed font-serif">
          Họp Hội nghị Tân Trào, Phá kho thóc cứu đói, Tổng khởi nghĩa Hà Nội - Huế - Sài Gòn đến Quảng trường Ba Đình 2/9. Hãy cùng sống lại những khoảnh khắc sục sôi hào hùng!
        </p>
      </div>

      <!-- Player Profile Form & Mode Selection -->
      <div class="bg-paper-50 p-5 rounded-2xl border border-paper-300 space-y-5 text-left max-w-md mx-auto shadow-inner">
        
        <div class="space-y-1.5">
          <label class="block text-xs font-bold text-amber-900 uppercase tracking-wider">
            👤 Tên Chiến Sĩ / Người Chơi:
          </label>
          <input type="text" id="inputPlayerName" placeholder="Nhập tên của bạn..." value="Chiến sĩ Mùa Thu"
                 class="w-full bg-paper-100 border-2 border-paper-400 rounded-xl px-4 py-2.5 text-sm font-bold text-stone-900 focus:outline-none focus:border-rev-red focus:ring-2 focus:ring-rev-red/20 transition-all">
        </div>

        <!-- Mode Selection -->
        <div class="space-y-2 pt-1 border-t border-paper-300">
          <label class="block text-xs font-bold text-amber-900 uppercase tracking-wider">
            ⏱️ Chọn Chế Độ Chơi:
          </label>
          <div class="grid grid-cols-3 gap-2">
            
            <button type="button" onclick="selectGameMode('part')" id="modeBtnPart" class="p-2.5 rounded-xl border-2 border-rev-red bg-red-50 text-left transition-all">
              <div class="font-serif font-bold text-xs text-rev-darkred">🌱 Khởi Nghĩa</div>
              <p class="text-[9px] text-stone-600 mt-0.5">10 câu • 20s/câu</p>
            </button>

            <button type="button" onclick="selectGameMode('full')" id="modeBtnFull" class="p-2.5 rounded-xl border-2 border-paper-300 bg-paper-100 text-left transition-all opacity-70">
              <div class="font-serif font-bold text-xs text-amber-900">🚩 Tổng Khởi Nghĩa</div>
              <p class="text-[9px] text-stone-600 mt-0.5">15 câu • 15s/câu</p>
            </button>

            <button type="button" onclick="selectGameMode('survival')" id="modeBtnSurvival" class="p-2.5 rounded-xl border-2 border-paper-300 bg-paper-100 text-left transition-all opacity-70">
              <div class="font-serif font-bold text-xs text-amber-900">⭐ Sinh Tồn 3 Tim</div>
              <p class="text-[9px] text-stone-600 mt-0.5">15 câu • 12s • 3 Tim</p>
            </button>

          </div>
        </div>

      </div>

      <!-- Start Button & Leaderboard -->
      <div class="space-y-3 pt-1">
        <button onclick="startGame()" class="pulse-scale px-10 py-3.5 bg-gradient-to-r from-rev-red to-rev-darkred hover:from-red-700 hover:to-red-950 text-white font-display font-black text-lg rounded-2xl shadow-xl border-2 border-rev-gold transition-all transform hover:-translate-y-0.5">
          🚩 BẮT ĐẦU HÀNH TRÌNH THÁNG 8
        </button>

        <div>
          <button onclick="toggleLeaderboardModal()" class="text-xs font-bold text-rev-gold hover:text-rev-darkred underline">
            🏆 Xem Bảng Vàng Kỷ Lục
          </button>
        </div>
      </div>

    </section>

    <!-- 2. MAIN QUIZ GAMEPLAY SCREEN -->
    <section id="quizScreen" class="hidden flex-1 flex flex-col space-y-3">
      
      <!-- TOP INTERACTIVE CAMPAIGN MAP & DASHBOARD -->
      <div class="paper-card rounded-2xl p-3 sm:p-4 border border-paper-400 shadow-md space-y-3">
        
        <!-- Header Info Row -->
        <div class="flex flex-wrap items-center justify-between gap-2 border-b border-paper-300 pb-2">
          
          <div class="flex items-center space-x-2 sm:space-x-3">
            <div id="activeAvatarBadge" class="w-9 h-9 rounded-xl bg-amber-100 border border-rev-gold flex items-center justify-center text-lg shadow-sm">
              ⭐
            </div>
            <div>
              <div class="font-serif font-bold text-xs sm:text-sm text-rev-darkred" id="activePlayerDisplayName">
                Chiến sĩ Mùa Thu
              </div>
              <div class="text-[10px] sm:text-[11px] text-stone-600 font-medium" id="activeModeBadge">
                Chế độ: Khởi Nghĩa Từng Phần (20s)
              </div>
            </div>
          </div>

          <!-- Hearts, Combo & Score -->
          <div class="flex items-center space-x-3">
            
            <div id="livesContainer" class="flex items-center space-x-1 text-sm">
              <span class="text-red-600">❤️</span>
              <span class="text-red-600">❤️</span>
              <span class="text-red-600">❤️</span>
            </div>

            <div id="comboBadge" class="hidden bg-amber-100 text-amber-900 border border-amber-400 text-xs font-bold px-2 py-0.5 rounded-full animate-bounce">
              🔥 Combo x<span id="comboVal">1</span>
            </div>

            <div class="bg-paper-200 px-3 py-1 rounded-xl border border-paper-400 font-mono font-bold text-xs sm:text-sm text-rev-darkred">
              Điểm: <span id="scoreVal" class="text-sm sm:text-base text-rev-red">0</span>
            </div>

          </div>
        </div>

        <!-- VISUAL CAMPAIGN TIMELINE MAP -->
        <div class="space-y-1">
          <div class="flex justify-between items-center text-[10px] sm:text-xs font-bold text-stone-700">
            <span>🗺️ BẢN ĐỒ TIẾN TRÌNH CÁCH MẠNG:</span>
            <span id="milestoneTitle" class="text-rev-darkred font-serif">1. Việt Bắc Tân Trào</span>
          </div>

          <!-- Interactive Node Map Graphic -->
          <div class="relative w-full bg-stone-300 h-3.5 rounded-full overflow-hidden border border-stone-400 shadow-inner">
            <div id="timelineProgressBar" class="h-full bg-gradient-to-r from-rev-gold via-rev-red to-red-700 transition-all duration-500 rounded-full" style="width: 10%"></div>
          </div>

          <!-- 6 Key Milestone Nodes -->
          <div class="grid grid-cols-6 text-[9px] sm:text-[10px] font-bold text-stone-600 text-center pt-0.5">
            <span id="node-0" class="text-rev-red font-black">1. Tân Trào</span>
            <span id="node-1">2. Cứu Đói</span>
            <span id="node-2">3. 4 Tỉnh</span>
            <span id="node-3">4. Hà Nội</span>
            <span id="node-4">5. Huế/Sài Gòn</span>
            <span id="node-5">6. Ba Đình</span>
          </div>
        </div>

      </div>

      <!-- QUESTION CONTAINER WITH ILLUSTRATED SCENE STAGE & DYNAMIC MASCOT -->
      <div class="paper-card rounded-3xl p-4 sm:p-6 wood-frame flex-1 flex flex-col justify-between space-y-4">
        
        <!-- Header Question Bar & Lifelines -->
        <div class="flex flex-wrap items-center justify-between gap-2 border-b border-paper-300 pb-2.5">
          
          <div class="flex items-center space-x-2">
            <span class="stamp-badge px-2.5 py-0.5 text-xs" id="questionNumberBadge">
              CÂU 1 / 15
            </span>
            <span class="bg-amber-100 text-amber-900 text-[10px] font-bold px-2 py-0.5 rounded border border-amber-300" id="difficultyBadge">
              Nhận biết
            </span>
          </div>

          <!-- Lifelines Buttons -->
          <div class="flex items-center space-x-1.5 sm:space-x-2">
            <button id="btnLifelineHint" onclick="useLifeline('hint')" title="Quân sư gợi ý tư liệu" class="px-2.5 py-1 rounded-xl bg-amber-100 hover:bg-amber-200 text-amber-900 border border-amber-300 text-xs font-bold transition-all flex items-center gap-1 shadow-sm disabled:opacity-40 disabled:cursor-not-allowed">
              💡 <span class="hidden sm:inline">Quân sư</span>
            </button>

            <button id="btnLifeline5050" onclick="useLifeline('5050')" title="Loại 2 đáp án sai" class="px-2.5 py-1 rounded-xl bg-amber-100 hover:bg-amber-200 text-amber-900 border border-amber-300 text-xs font-bold transition-all flex items-center gap-1 shadow-sm disabled:opacity-40 disabled:cursor-not-allowed">
              ⚖️ <span class="hidden sm:inline">50:50</span>
            </button>

            <button id="btnLifelineDouble" onclick="useLifeline('double')" title="x2 Điểm thời cơ" class="px-2.5 py-1 rounded-xl bg-amber-100 hover:bg-amber-200 text-amber-900 border border-amber-300 text-xs font-bold transition-all flex items-center gap-1 shadow-sm disabled:opacity-40 disabled:cursor-not-allowed">
              ⭐ <span class="hidden sm:inline">x2 Điểm</span>
            </button>
          </div>

          <!-- Timer Bar -->
          <div id="timerContainer" class="flex items-center space-x-2">
            <span class="text-xs font-bold text-stone-600">⏱️:</span>
            <div class="w-24 sm:w-32 bg-stone-200 h-3 rounded-full overflow-hidden border border-stone-300">
              <div id="timerBar" class="h-full bg-emerald-600 transition-all duration-1000 rounded-full" style="width: 100%"></div>
            </div>
            <span id="timerVal" class="font-mono font-bold text-xs text-rev-darkred min-w-[24px]">20s</span>
          </div>

        </div>

        <!-- MIDDLE SECTION: SCENE STAGE (SVG) + DYNAMIC MASCOT + QUESTION TEXT -->
        <div class="grid grid-cols-1 md:grid-cols-12 gap-4 items-center">
          
          <!-- DYNAMIC SVG SCENE STAGE (8 COLS ON DESKTOP) -->
          <div class="md:col-span-8 relative w-full h-36 sm:h-44 rounded-2xl overflow-hidden border border-paper-400 bg-stone-900 shadow-md">
            <!-- Sunbeam Ray Overlay -->
            <div class="absolute inset-0 sunbeam-overlay pointer-events-none"></div>

            <!-- Dynamic SVG Scene Inject Container -->
            <div id="sceneSvgContainer" class="w-full h-full">
              <!-- SVG elements injected dynamically -->
            </div>

            <!-- Sparkle burst overlay for correct answers -->
            <div id="sparkleOverlay" class="hidden absolute inset-0 flex items-center justify-center pointer-events-none">
              <div class="w-32 h-32 text-rev-brightgold star-sparkle text-7xl flex items-center justify-center">
                ★
              </div>
            </div>
          </div>

          <!-- DYNAMIC MASCOT / HERALD (4 COLS ON DESKTOP) -->
          <div class="md:col-span-4 bg-paper-50 p-3 rounded-2xl border border-paper-300 shadow-inner flex flex-row md:flex-col items-center justify-between text-center gap-2">
            <!-- Mascot SVG Container -->
            <div id="mascotSvgContainer" class="w-20 h-20 sm:w-24 sm:h-24 shrink-0 transition-transform duration-300">
              <!-- Mascot SVG injected dynamically -->
            </div>
            <div>
              <div id="mascotTitle" class="font-serif font-bold text-xs text-rev-darkred">Chiến Sĩ Tuyên Truyền</div>
              <p id="mascotSpeech" class="text-[10px] text-stone-600 italic">"Hãy chọn thời cơ chính xác!"</p>
            </div>
          </div>

        </div>

        <!-- Question Text & Hint Box -->
        <div class="space-y-2">
          <h3 id="questionText" class="font-serif font-bold text-sm sm:text-lg text-stone-900 leading-snug">
            Nội dung câu hỏi trắc nghiệm lịch sử...
          </h3>

          <!-- Hint Box -->
          <div id="hintBox" class="hidden bg-amber-100 border-l-4 border-amber-600 p-2.5 rounded-r-xl text-xs space-y-1 animate-fadeIn">
            <div class="font-bold text-amber-900 flex items-center gap-1">
              💡 Gợi ý Quân sư Lịch sử:
            </div>
            <p id="hintText" class="text-stone-800 italic font-serif"></p>
          </div>
        </div>

        <!-- Options Grid -->
        <div id="optionsGrid" class="grid grid-cols-1 md:grid-cols-2 gap-2.5 pt-1">
          <!-- 4 Options appended dynamically -->
        </div>

      </div>
    </section>

    <!-- 3. EXPLANATION & HISTORICAL DOCUMENT CARD MODAL -->
    <div id="explanationModal" class="hidden fixed inset-0 bg-black/80 backdrop-blur-sm z-50 flex items-center justify-center p-3 sm:p-4">
      <div class="paper-card rounded-3xl p-5 sm:p-6 max-w-xl w-full wood-frame space-y-4 shadow-2xl relative animate-fadeIn">
        
        <!-- Header Badge -->
        <div id="expHeaderBadge" class="flex items-center space-x-2 font-display font-black text-lg sm:text-2xl">
          <span id="expIcon">✅</span>
          <span id="expTitleText">CHÍNH XÁC HOÀN HẢO!</span>
        </div>

        <!-- Document Card Visual View -->
        <div class="flex items-center space-x-3 bg-paper-50 p-3 rounded-2xl border border-paper-300 shadow-sm">
          <div id="expMiniDocGraphic" class="w-16 h-16 rounded-xl bg-stone-900 border border-rev-gold shrink-0 overflow-hidden flex items-center justify-center text-amber-400 text-2xl">
            📜
          </div>
          <div class="space-y-0.5 text-xs">
            <span class="font-bold text-amber-900 block uppercase tracking-wider text-[10px]">TƯ LIỆU BỔ TRỢ LỊCH SỬ</span>
            <p id="expCorrectAnswer" class="font-serif font-bold text-rev-darkred text-xs sm:text-sm"></p>
          </div>
        </div>

        <!-- Detail Historical Explanation -->
        <div class="bg-amber-50/90 p-3.5 rounded-2xl border border-amber-200 space-y-1">
          <span class="font-bold text-rev-darkred block text-xs">📖 Diễn biến & Ý nghĩa lịch sử:</span>
          <p id="expDetailText" class="text-stone-800 text-xs sm:text-sm leading-relaxed italic font-serif"></p>
        </div>

        <div class="flex justify-between items-center pt-1">
          <div id="expBonusEarned" class="text-xs font-mono font-bold text-emerald-700">
            +100 điểm
          </div>

          <button onclick="nextQuestion()" class="px-6 py-2.5 bg-rev-red hover:bg-rev-darkred text-white font-serif font-bold text-xs sm:text-sm rounded-xl shadow border border-rev-gold transition-all">
            Tiếp theo ➔
          </button>
        </div>

      </div>
    </div>

    <!-- 4. FINAL RESULTS & REVIEW SCREEN -->
    <section id="resultScreen" class="hidden paper-card rounded-3xl p-5 sm:p-8 wood-frame max-w-4xl mx-auto w-full my-auto space-y-6 text-center">
      
      <div class="space-y-2">
        <div class="stamp-badge text-xs sm:text-sm px-5 py-1 inline-block">
          🏆 TỔNG KHỞI NGHĨA HOÀN THÀNH
        </div>
        <h2 class="font-display font-black text-2xl sm:text-4xl text-rev-darkred" id="finalTitleAward">
          NHÀ SỬ HỌC LỖI LẠC
        </h2>
        <p class="text-xs sm:text-sm text-stone-700 italic max-w-xl mx-auto font-serif">
          Chúc mừng bạn đã hoàn thành trọn vẹn các mốc thời cơ lịch sử của Cách mạng Tháng Tám 1945!
        </p>
      </div>

      <!-- Stats Scorecard -->
      <div class="grid grid-cols-2 md:grid-cols-4 gap-2.5 text-center">
        <div class="bg-paper-50 p-3 rounded-2xl border border-paper-300 shadow-sm">
          <div class="text-[10px] font-bold text-stone-500 uppercase">TỔNG ĐIỂM</div>
          <div class="font-mono font-black text-2xl sm:text-3xl text-rev-red mt-0.5" id="finalScore">0</div>
        </div>

        <div class="bg-paper-50 p-3 rounded-2xl border border-paper-300 shadow-sm">
          <div class="text-[10px] font-bold text-stone-500 uppercase">SỐ CÂU ĐÚNG</div>
          <div class="font-mono font-black text-2xl sm:text-3xl text-emerald-700 mt-0.5" id="finalCorrectCount">0/15</div>
        </div>

        <div class="bg-paper-50 p-3 rounded-2xl border border-paper-300 shadow-sm">
          <div class="text-[10px] font-bold text-stone-500 uppercase">MAX COMBO</div>
          <div class="font-mono font-black text-2xl sm:text-3xl text-amber-700 mt-0.5" id="finalMaxCombo">0</div>
        </div>

        <div class="bg-paper-50 p-3 rounded-2xl border border-paper-300 shadow-sm">
          <div class="text-[10px] font-bold text-stone-500 uppercase">ĐỘ CHÍNH XÁC</div>
          <div class="font-mono font-black text-2xl sm:text-3xl text-stone-800 mt-0.5" id="finalAccuracy">0%</div>
        </div>
      </div>

      <!-- REVIEW ALL QUESTIONS WITH MINI HISTORICAL CARDS -->
      <div class="space-y-2 text-left">
        <div class="flex justify-between items-center border-b border-paper-300 pb-1.5">
          <h3 class="font-serif font-bold text-sm sm:text-base text-rev-darkred flex items-center gap-2">
            📖 Bảng Xem Lại Bài Làm & Thẻ Tư Liệu
          </h3>
          <span class="text-[11px] text-stone-500">Xem chi tiết lời giải</span>
        </div>

        <div id="reviewQuestionsContainer" class="space-y-2.5 max-h-64 overflow-y-auto pr-1">
          <!-- Dynamic Review Cards appended here -->
        </div>
      </div>

      <!-- Action Buttons -->
      <div class="flex flex-wrap justify-center gap-3 pt-1">
        <button onclick="startGame()" class="px-7 py-3 bg-rev-red hover:bg-rev-darkred text-white font-serif font-bold text-xs sm:text-sm rounded-xl shadow border-2 border-rev-gold transition-all">
          🔄 Thử Thách Lại
        </button>

        <button onclick="toggleLeaderboardModal()" class="px-6 py-3 bg-paper-200 hover:bg-paper-300 text-stone-900 font-serif font-bold text-xs sm:text-sm rounded-xl shadow border border-paper-400 transition-all">
          🏆 Xem Bảng Vàng
        </button>
      </div>

    </section>

  </main>

  <!-- LEADERBOARD MODAL -->
  <div id="leaderboardModal" class="hidden fixed inset-0 bg-black/80 backdrop-blur-sm z-50 flex items-center justify-center p-4">
    <div class="paper-card rounded-3xl p-6 max-w-md w-full wood-frame space-y-4 shadow-2xl">
      <div class="flex justify-between items-center border-b border-paper-300 pb-2">
        <h3 class="font-serif font-bold text-base sm:text-lg text-rev-darkred flex items-center gap-2">
          🏆 BẢNG VÀNG KỶ LỤC CÁCH MẠNG
        </h3>
        <button onclick="toggleLeaderboardModal()" class="text-stone-500 hover:text-stone-800 font-bold text-lg">✕</button>
      </div>

      <div class="space-y-2 max-h-60 overflow-y-auto" id="leaderboardList">
        <!-- High scores list -->
      </div>

      <div class="flex justify-end pt-1">
        <button onclick="toggleLeaderboardModal()" class="px-5 py-2 bg-rev-red text-white font-bold text-xs rounded-xl shadow">
          Đóng
        </button>
      </div>
    </div>
  </div>

  <!-- SCRIPT: GAME ENGINE, SVG ENGINE & DATASET -->
  <script>
    /* ==========================================================================
       1. HISTORICAL QUESTIONS DATASET WITH ART THEME KEYS
       ========================================================================== */
    const masterQuestions = [
      {
        id: 1,
        theme: "coup",
        level: "Nhận biết",
        question: "Trong Chỉ thị 'Nhật - Pháp bắn nhau và hành động của chúng ta' (12/3/1945), Ban Thường vụ Trung ương Đảng đã xác định kẻ thù chính duy nhất của nhân dân Đông Dương là ai?",
        options: [
          "Phát xít Nhật",
          "Thực dân Pháp",
          "Phong kiến tay sai",
          "Liên quân Pháp - Nhật"
        ],
        correct: 0,
        hint: "Nhật đảo chính lật đổ toàn bộ chính quyền Pháp đêm 9/3/1945.",
        explanation: "Sau cuộc đảo chính ngày 9/3/1945, chính quyền Pháp hoàn toàn tan rã. Ban Thường vụ Trung ương Đảng xác định Phát xít Nhật trở thành kẻ thù chính duy nhất."
      },
      {
        id: 2,
        theme: "granary",
        level: "Nhận biết",
        question: "Khẩu hiệu trung tâm được Mặt trận Việt Minh phát động từ tháng 3/1945 nhằm giải quyết nạn đói khủng khiếp và tập hợp hàng triệu quần chúng là gì?",
        options: [
          "Tăng gia sản xuất",
          "Phá kho thóc Nhật, giải quyết nạn đói",
          "Tịch thu ruộng đất địa chủ",
          "Giảm thuế, giảm tức"
        ],
        correct: 1,
        hint: "Khẩu hiệu đánh trúng nhu cầu sống còn cấp bách của quần chúng nông dân.",
        explanation: "Khẩu hiệu 'Phá kho thóc Nhật, giải quyết nạn đói' đã thổi bùng cao trào kháng Nhật cứu nước, tập hợp hàng triệu quần chúng tham gia cách mạng."
      },
      {
        id: 3,
        theme: "tan_trao",
        level: "Thông hiểu",
        question: "Tháng 6/1945, Khu giải phóng Việt Bắc được thành lập gồm 6 tỉnh căn cứ địa cốt lõi nào?",
        options: [
          "Cao Bằng, Bắc Kạn, Lạng Sơn, Hà Giang, Tuyên Quang, Thái Nguyên",
          "Cao Bằng, Bắc Kạn, Lạng Sơn, Yên Bái, Phú Thọ, Tuyên Quang",
          "Bắc Giang, Hải Dương, Hà Tĩnh, Quảng Nam, Tuyên Quang, Thái Nguyên",
          "Hà Nội, Bắc Ninh, Hưng Yên, Hải Dương, Nam Định, Thái Bình"
        ],
        correct: 0,
        hint: "Tắt tên 6 tỉnh là 'Cao - Bắc - Lạng - Hà - Tuyên - Thái'.",
        explanation: "Khu giải phóng Việt Bắc gồm 6 tỉnh: Cao Bằng, Bắc Kạn, Lạng Sơn, Hà Giang, Tuyên Quang, Thái Nguyên - được ví như hình ảnh thu nhỏ của nước Việt Nam mới."
      },
      {
        id: 4,
        theme: "opportunity",
        level: "Thông hiểu",
        question: "Đảng ta xác định 'Thời cơ ngàn năm có một' cho Tổng khởi nghĩa xuất hiện trong khoảng thời gian nào?",
        options: [
          "Từ khi Nhật đảo chính Pháp đến khi Nhật đầu hàng",
          "Từ khi Nhật đầu hàng Đồng minh đến trước khi quân Đồng minh vào Đông Dương",
          "Từ sau khi quân Đồng minh vào Việt Nam giải giáp quân Nhật",
          "Sau khi Chủ tịch Hồ Chí Minh đọc Tuyên ngôn Độc lập"
        ],
        correct: 1,
        hint: "Đây là khoảng trống quyền lực khi chính quyền cũ tan rã và quân Đồng minh chưa tới.",
        explanation: "Từ sau khi Nhật đầu hàng (15/8) đến trước khi quân Đồng minh vào (cuối tháng 8) là thời điểm kẻ thù hoang mang cực độ, tạo ra thời cơ vàng cho nhân dân ta nổi dậy."
      },
      {
        id: 5,
        theme: "tan_trao",
        level: "Nhận biết",
        question: "Hội nghị toàn quốc của Đảng họp tại Tân Trào (từ ngày 13 đến 15/8/1945) đã đưa ra quyết định lịch sử nào?",
        options: [
          "Thông qua 10 chính sách lớn của Việt Minh",
          "Phát động Tổng khởi nghĩa trong cả nước",
          "Thành lập Mặt trận Việt Minh",
          "Soạn thảo Tuyên ngôn Độc lập"
        ],
        correct: 1,
        hint: "Thành lập Ủy ban Khởi nghĩa Toàn quốc và ban hành Quân lệnh số 1.",
        explanation: "Hội nghị toàn quốc của Đảng họp tại Tân Trào đã kịp thời quyết định phát động Tổng khởi nghĩa giành chính quyền trong cả nước trước khi quân Đồng minh vào."
      },
      {
        id: 6,
        theme: "tan_trao",
        level: "Thông hiểu",
        question: "Đại hội Quốc dân họp tại Tân Trào (ngày 16 và 17/8/1945) đã bầu ra cơ quan nào làm nhiệm vụ như Chính phủ lâm thời?",
        options: [
          "Ủy ban Khởi nghĩa Toàn quốc",
          "Ủy ban Dân tộc Giải phóng Việt Nam",
          "Ủy ban Lâm thời Hà Nội",
          "Hội đồng Cố vấn Tối cao"
        ],
        correct: 1,
        hint: "Cơ quan này do Chủ tịch Hồ Chí Minh làm Chủ tịch.",
        explanation: "Đại hội Quốc dân Tân Trào bầu ra Ủy ban Dân tộc Giải phóng Việt Nam do Hồ Chí Minh làm Chủ tịch, quy định Cờ đỏ sao vàng và bài Tiến quân ca."
      },
      {
        id: 7,
        theme: "four_provinces",
        level: "Nhận biết",
        question: "Bốn tỉnh dành được chính quyền sớm nhất trong cả nước (ngày 18/8/1945) gồm những tỉnh nào?",
        options: [
          "Bắc Giang, Hải Dương, Hà Tĩnh, Quảng Nam",
          "Hà Nội, Huế, Sài Gòn, Bắc Giang",
          "Cao Bằng, Lạng Sơn, Thái Nguyên, Tuyên Quang",
          "Hải Phòng, Nam Định, Thanh Hóa, Nghệ An"
        ],
        correct: 0,
        hint: "Bốn tỉnh từ Bắc đến Trung Bộ chớp thời cơ nổi dậy thắng lợi ngày 18/8.",
        explanation: "Bắc Giang, Hải Dương, Hà Tĩnh và Quảng Nam là 4 tỉnh đầu tiên trong cả nước khởi nghĩa giành được chính quyền vào ngày 18/8/1945."
      },
      {
        id: 8,
        theme: "hanoi",
        level: "Vận dụng",
        question: "Sự kiện lịch sử trọng đại nào diễn ra ngày 19/8/1945 tại Hà Nội có ý nghĩa cổ vũ quyết định cho cả nước?",
        options: [
          "Hàng vạn quần chúng chiếm Bắc Bộ Phủ, Phủ Khâm sứ và các cơ quan đầu não",
          "Bác Hồ đọc Tuyên ngôn Độc lập",
          "Vua Bảo Đại đọc tuyên ngôn thoái vị",
          "Thành lập Đội Việt Nam Tuyên truyền Giải phóng quân"
        ],
        correct: 0,
        hint: "Cuộc mít tinh tại Quảng trường Nhà hát Lớn chuyển thành cuộc khởi nghĩa vũ trang.",
        explanation: "Thắng lợi rực rỡ của cuộc khởi nghĩa tại Hà Nội ngày 19/8/1945 tạo nên hiệu ứng dây chuyền, cổ vũ nhân dân cả nước nhanh chóng nổi dậy."
      },
      {
        id: 9,
        theme: "hue",
        level: "Nhận biết",
        question: "Thắng lợi khởi nghĩa ở Cố đô Huế (23/8/1945) gắn liền với sự kiện biểu tượng nào diễn ra ngày 30/8/1945?",
        options: [
          "Vua Bảo Đại tuyên bố thoái vị và trao ấn kiếm cho Đại diện Chính phủ",
          "Xóa bỏ hoàn toàn triều đại nhà Lê",
          "Tuyên bố giải tán Bảo an binh Trung Bộ",
          "Đổi tên thành phố Huế"
        ],
        correct: 0,
        hint: "Chấm dứt vĩnh viễn chế độ quân chủ phong kiến tồn tại ngàn năm.",
        explanation: "Chiều 30/8/1945, Vua Bảo Đại đọc Tuyên ngôn thoái vị tại cửa Ngọ Môn Huế, nộp ấn kiếm cho đại diện Chính phủ lâm thời, chấm dứt chế độ phong kiến Việt Nam."
      },
      {
        id: 10,
        theme: "saigon",
        level: "Vận dụng",
        question: "Khởi nghĩa giành chính quyền ở Sài Gòn (25/8/1945) có sự tham gia nòng cốt của lực lượng quần chúng nào?",
        options: [
          "Thanh niên Tiền phong và Công đoàn Nam Bộ",
          "Đội Tự vệ Đỏ",
          "Hội Nông dân cứu quốc",
          "Lực lượng binh lính Pháp"
        ],
        correct: 0,
        hint: "Tổ chức thanh niên cứu quốc có quy mô hàng vạn thành viên tại Nam Bộ.",
        explanation: "Lực lượng Thanh niên Tiền phong cùng Công đoàn Nam Bộ là nòng cốt rầm rộ xuống đường làm chủ Sài Gòn trong ngày 25/8/1945."
      },
      {
        id: 11,
        theme: "badinh",
        level: "Nhận biết",
        question: "Ngày 2/9/1945, tại Quảng trường Ba Đình (Hà Nội), Chủ tịch Hồ Chí Minh thay mặt Chính phủ lâm thời đọc văn kiện nào?",
        options: [
          "Tuyên ngôn Độc lập",
          "Lời kêu gọi Toàn quốc kháng chiến",
          "Bản Yêu cầu của nhân dân An Nam",
          "Đường Kách mệnh"
        ],
        correct: 0,
        hint: "Văn kiện khai sinh ra nước Việt Nam Dân chủ Cộng hòa.",
        explanation: "Chủ tịch Hồ Chí Minh đã trang trọng đọc bản Tuyên ngôn Độc lập, tuyên bố với quốc dân và toàn thế giới về sự ra đời của nước Việt Nam Dân chủ Cộng hòa."
      },
      {
        id: 12,
        theme: "nature",
        level: "Vận dụng cao",
        question: "Xét về tính chất lịch sử, Cách mạng Tháng Tám năm 1945 ở Việt Nam là cuộc cách mạng:",
        options: [
          "Giải phóng dân tộc mang tính nhân văn và dân chủ sâu sắc",
          "Cách mạng tư sản dân quyền kiểu cũ",
          "Cách mạng xã hội chủ nghĩa thuần túy",
          "Cách mạng tư sản do tư sản lãnh đạo"
        ],
        correct: 0,
        hint: "Nhiệm vụ hàng đầu là đánh đuổi đế quốc, giải phóng dân tộc.",
        explanation: "Cách mạng Tháng Tám 1945 là cuộc cách mạng giải phóng dân tộc mang tính nhân văn và dân chủ sâu sắc, lật đổ ách thống trị thực dân phong kiến."
      },
      {
        id: 13,
        theme: "leadership",
        level: "Vận dụng cao",
        question: "Nguyên nhân quyết định nhất dẫn đến thắng lợi nhanh chóng và trọn vẹn của Cách mạng Tháng Tám năm 1945 là gì?",
        options: [
          "Sự lãnh đạo đúng đắn, sáng tạo của Đảng đứng đầu là Chủ tịch Hồ Chí Minh",
          "Nhật Bản đầu hàng Đồng minh",
          "Khối liên minh công nông",
          "Truyền thống yêu nước ngàn đời"
        ],
        correct: 0,
        hint: "Bộ não chiến lược chớp thời cơ chính xác và vạch đường lối cứu quốc.",
        explanation: "Sự lãnh đạo tài tình của Đảng và Chủ tịch Hồ Chí Minh với đường lối đúng đắn, chuẩn bị chu đáo và chớp thời cơ ngàn năm có một là nguyên nhân quyết định nhất."
      },
      {
        id: 14,
        theme: "unity",
        level: "Thông hiểu",
        question: "Bài học kinh nghiệm về xây dựng khối đại đoàn kết toàn dân tộc trong Cách mạng Tháng Tám thể hiện tập trung qua tổ chức nào?",
        options: [
          "Mặt trận Việt Minh",
          "Hội Phản đế đồng minh",
          "Mặt trận Dân chủ Đông Dương",
          "Hội Liên Việt"
        ],
        correct: 0,
        hint: "Thành lập năm 1941, tập hợp mọi lực lượng yêu nước không phân biệt giai cấp.",
        explanation: "Mặt trận Việt Minh (Việt Nam Độc lập Đồng minh) đã quy tụ rộng rãi mọi tầng lớp nhân dân vào khối đại đoàn kết dân tộc toàn diện."
      },
      {
        id: 15,
        theme: "global",
        level: "Thông hiểu",
        question: "Một trong những ý nghĩa quốc tế to lớn của thắng lợi Cách mạng Tháng Tám năm 1945 là gì?",
        options: [
          "Góp phần đánh bại phát xít và cổ vũ mạnh mẽ phong trào giải phóng dân tộc trên thế giới",
          "Chấm dứt hoàn toàn Chiến tranh lạnh",
          "Xóa bỏ tư bản chủ nghĩa toàn cầu",
          "Thành lập Liên Hợp Quốc"
        ],
        correct: 0,
        hint: "Giáng đòn tử thương vào hệ thống thuộc địa thực dân.",
        explanation: "Thắng lợi Cách mạng Tháng Tám cùng Đồng minh diệt phát xít, đồng thời cổ vũ mạnh mẽ các dân tộc bị áp bức tại Á - Phi - Mỹ Latinh nổi dậy giành độc lập."
      }
    ];

    /* ==========================================================================
       2. SVG GRAPHIC SCENE & MASCOT GENERATORS
       ========================================================================== */
    function getSceneSvgHTML(theme) {
      switch(theme) {
        case 'tan_trao':
          return `
            <svg class="w-full h-full object-cover ken-burns-anim" viewBox="0 0 600 250">
              <defs>
                <linearGradient id="g_tt" x1="0" y1="0" x2="0" y2="1">
                  <stop offset="0%" stop-color="#451a03"/><stop offset="100%" stop-color="#78350f"/>
                </linearGradient>
              </defs>
              <rect width="600" height="250" fill="url(#g_tt)"/>
              <!-- Banyan Tree Trunk & Canopy -->
              <path d="M 220 250 Q 250 140 180 90 Q 280 20 400 60 Q 480 10 520 90 Q 450 160 400 250 Z" fill="#15803d" opacity="0.85"/>
              <path d="M 260 250 Q 270 170 300 130 Q 320 180 340 250 Z" fill="#27272a"/>
              <!-- Tân Trào Revolutionary Hut -->
              <polygon points="80,180 150,130 220,180" fill="#a16207"/>
              <rect x="95" y="180" width="110" height="60" fill="#78350f"/>
              <rect x="135" y="200" width="30" height="40" fill="#27272a"/>
              <!-- Red Flag on Top of Hut -->
              <line x1="150" y1="130" x2="150" y2="80" stroke="#fef08a" stroke-width="3"/>
              <polygon points="150,80 190,92 150,105" fill="#b91c1c"/>
              <polygon points="167,90 170,96 177,96 171,100 173,106 167,102 161,106 163,100 157,96 164,96" fill="#f59e0b"/>
              <text x="30" y="40" fill="#fef08a" font-family="serif" font-weight="bold" font-size="18">LỜI KÊU GỌI TÂN TRÀO (8/1945)</text>
            </svg>`;

        case 'granary':
          return `
            <svg class="w-full h-full object-cover ken-burns-anim" viewBox="0 0 600 250">
              <rect width="600" height="250" fill="#292524"/>
              <!-- Granary Wooden Wall & Broken Doors -->
              <rect x="50" y="40" width="500" height="180" fill="#44403c" stroke="#78350f" stroke-width="4"/>
              <!-- Broken Wooden Lock -->
              <path d="M 260 90 L 300 40 L 340 90 L 340 180 L 260 180 Z" fill="#1c1917"/>
              <line x1="260" y1="110" x2="210" y2="160" stroke="#b91c1c" stroke-width="6"/>
              <!-- Rice Stalks & Torches Glowing -->
              <circle cx="120" cy="80" r="45" fill="#f59e0b" opacity="0.3"/>
              <circle cx="480" cy="80" r="45" fill="#f59e0b" opacity="0.3"/>
              <path d="M 115 110 L 120 70 L 125 110 Z" fill="#b91c1c"/>
              <path d="M 475 110 L 480 70 L 485 110 Z" fill="#b91c1c"/>
              <text x="180" y="225" fill="#fef08a" font-family="serif" font-weight="bold" font-size="18">PHÁ KHO THÓC CỨU ĐÓI</text>
            </svg>`;

        case 'hanoi':
          return `
            <svg class="w-full h-full object-cover ken-burns-anim" viewBox="0 0 600 250">
              <rect width="600" height="250" fill="#7f1d1d"/>
              <!-- Hanoi Opera House Front Columns -->
              <rect x="150" y="80" width="300" height="140" fill="#fef3c7" opacity="0.9"/>
              <polygon points="150,80 300,30 450,80" fill="#b91c1c"/>
              <rect x="180" y="100" width="20" height="120" fill="#78350f"/>
              <rect x="230" y="100" width="20" height="120" fill="#78350f"/>
              <rect x="350" y="100" width="20" height="120" fill="#78350f"/>
              <rect x="400" y="100" width="20" height="120" fill="#78350f"/>
              <!-- Red Flag Flying High -->
              <line x1="300" y1="30" x2="300" y2="-10" stroke="#fff" stroke-width="3"/>
              <polygon points="300,-10 360,8 300,26" fill="#b91c1c"/>
              <text x="150" y="235" fill="#fef08a" font-family="serif" font-weight="bold" font-size="18">KHỞI NGHĨA HÀ NỘI (19/8/1945)</text>
            </svg>`;

        case 'hue':
          return `
            <svg class="w-full h-full object-cover ken-burns-anim" viewBox="0 0 600 250">
              <rect width="600" height="250" fill="#451a03"/>
              <!-- Ngọ Môn Palace Gates -->
              <rect x="120" y="100" width="360" height="120" fill="#b91c1c"/>
              <polygon points="120,100 300,50 480,100" fill="#d97706"/>
              <rect x="250" y="140" width="100" height="80" fill="#1c1917"/>
              <!-- Royal Sword & Golden Seal Silhouette -->
              <path d="M 290 80 L 310 80 L 305 130 L 295 130 Z" fill="#f59e0b"/>
              <rect x="285" y="130" width="30" height="20" fill="#f59e0b"/>
              <text x="140" y="235" fill="#fef08a" font-family="serif" font-weight="bold" font-size="18">THOÁI VỊ TẠI CỐ ĐÔ HUẾ (23/8 - 30/8)</text>
            </svg>`;

        case 'saigon':
          return `
            <svg class="w-full h-full object-cover ken-burns-anim" viewBox="0 0 600 250">
              <rect width="600" height="250" fill="#14532d"/>
              <!-- Saigon Notre-Dame Towers Silhouette -->
              <polygon points="180,180 200,60 220,180" fill="#1c1917"/>
              <polygon points="380,180 400,60 420,180" fill="#1c1917"/>
              <rect x="220" y="110" width="160" height="90" fill="#1c1917"/>
              <!-- Youth Vanguard Star Banner -->
              <circle cx="300" cy="140" r="35" fill="#b91c1c"/>
              <polygon points="300,115 308,132 327,132 312,143 317,160 300,149 283,160 288,143 273,132 292,132" fill="#f59e0b"/>
              <text x="140" y="235" fill="#fef08a" font-family="serif" font-weight="bold" font-size="18">KHỞI NGHĨA SÀI GÒN (25/8/1945)</text>
            </svg>`;

        case 'badinh':
          return `
            <svg class="w-full h-full object-cover ken-burns-anim" viewBox="0 0 600 250">
              <defs>
                <linearGradient id="g_bd" x1="0" y1="0" x2="0" y2="1">
                  <stop offset="0%" stop-color="#b91c1c"/><stop offset="100%" stop-color="#d97706"/>
                </linearGradient>
              </defs>
              <rect width="600" height="250" fill="url(#g_bd)"/>
              <!-- Ba Dinh Podium & Vintage Microphone -->
              <rect x="220" y="140" width="160" height="80" fill="#faf4e8" stroke="#78350f" stroke-width="3"/>
              <line x1="300" y1="140" x2="300" y2="80" stroke="#1c1917" stroke-width="4"/>
              <ellipse cx="300" cy="75" rx="12" ry="16" fill="#71717a"/>
              <!-- Glowing Yellow Star Backdrop -->
              <polygon points="300,10 315,45 350,45 322,67 332,100 300,80 268,100 278,67 250,45 285,45" fill="#f59e0b" opacity="0.9"/>
              <text x="120" y="235" fill="#faf4e8" font-family="serif" font-weight="bold" font-size="18">TUYÊN NGÔN ĐỘC LẬP (2/9/1945)</text>
            </svg>`;

        default:
          return `
            <svg class="w-full h-full object-cover ken-burns-anim" viewBox="0 0 600 250">
              <rect width="600" height="250" fill="#7f1d1d"/>
              <polygon points="300,30 325,95 390,95 338,135 358,200 300,160 242,200 262,135 210,95 275,95" fill="#f59e0b"/>
              <text x="180" y="235" fill="#fef08a" font-family="serif" font-weight="bold" font-size="18">CÁCH MẠNG THÁNG TÁM 1945</text>
            </svg>`;
      }
    }

    function getMascotSvgHTML(state) {
      // state: 'thinking' | 'happy' | 'combo' | 'worried' | 'victory'
      let eyeExpression = `<circle cx="35" cy="38" r="3" fill="#1c1917"/><circle cx="55" cy="38" r="3" fill="#1c1917"/>`;
      let mouthExpression = `<path d="M 38 52 Q 45 58 52 52" fill="none" stroke="#1c1917" stroke-width="2.5" stroke-linecap="round"/>`;
      let hatColor = "#b91c1c";
      let starColor = "#f59e0b";

      if (state === 'happy') {
        mouthExpression = `<path d="M 35 50 Q 45 62 55 50 Z" fill="#b91c1c"/>`;
      } else if (state === 'combo') {
        eyeExpression = `<text x="30" y="42" font-size="12">🔥</text><text x="50" y="42" font-size="12">🔥</text>`;
        mouthExpression = `<path d="M 35 48 Q 45 64 55 48 Z" fill="#b91c1c"/>`;
      } else if (state === 'worried') {
        eyeExpression = `<circle cx="35" cy="36" r="2.5" fill="#1c1917"/><circle cx="55" cy="36" r="2.5" fill="#1c1917"/><circle cx="62" cy="30" r="4" fill="#38bdf8"/>`;
        mouthExpression = `<path d="M 38 56 Q 45 48 52 56" fill="none" stroke="#1c1917" stroke-width="2.5"/>`;
      } else if (state === 'victory') {
        eyeExpression = `<text x="30" y="40" font-size="11">⭐</text><text x="50" y="40" font-size="11">⭐</text>`;
        mouthExpression = `<path d="M 34 48 Q 45 64 56 48 Z" fill="#b91c1c"/>`;
      }

      return `
        <svg class="w-full h-full" viewBox="0 0 90 90">
          <!-- Background Badge Aura -->
          <circle cx="45" cy="45" r="40" fill="#faf4e8" stroke="#d6bf9c" stroke-width="2"/>
          <!-- Helmet / Guerrilla Cap -->
          <path d="M 20 34 Q 45 10 70 34 Z" fill="${hatColor}"/>
          <polygon points="45,16 48,23 55,23 50,27 52,34 45,30 38,34 40,27 35,23 42,23" fill="${starColor}"/>
          <!-- Face -->
          <circle cx="45" cy="44" r="20" fill="#fde68a" stroke="#78350f" stroke-width="1.5"/>
          ${eyeExpression}
          ${mouthExpression}
          <!-- Collar & Red Scarf -->
          <path d="M 28 62 L 45 74 L 62 62 L 55 85 L 35 85 Z" fill="#b91c1c"/>
        </svg>`;
    }

    /* ==========================================================================
       3. GLOBAL GAME STATE
       ========================================================================== */
    let playerName = "Chiến sĩ Mùa Thu";
    let gameMode = "part"; // 'part' (10q, 20s) | 'full' (15q, 15s) | 'survival' (15q, 12s, 3 lives)
    
    let currentQuestions = [];
    let currentIndex = 0;
    let score = 0;
    let combo = 0;
    let maxCombo = 0;
    let lives = 3;
    let timer = 20;
    let maxTimerPerQuestion = 20;
    let timerInterval = null;
    let isSoundOn = true;

    let lifelines = { hint: false, fiftyFifty: false, double: false };
    let isDoubleActive = false;
    let userAnswersLog = [];

    /* ==========================================================================
       4. WEB AUDIO API SYNTHESIZER
       ========================================================================== */
    const audioCtx = new (window.AudioContext || window.webkitAudioContext)();

    function playSound(type) {
      if (!isSoundOn) return;
      try {
        if (audioCtx.state === 'suspended') audioCtx.resume();
        const osc = audioCtx.createOscillator();
        const gain = audioCtx.createGain();
        osc.connect(gain);
        gain.connect(audioCtx.destination);
        const now = audioCtx.currentTime;

        if (type === 'click') {
          osc.type = 'sine';
          osc.frequency.setValueAtTime(420, now);
          osc.frequency.exponentialRampToValueAtTime(220, now + 0.04);
          gain.gain.setValueAtTime(0.1, now);
          gain.gain.linearRampToValueAtTime(0.01, now + 0.04);
          osc.start(now);
          osc.stop(now + 0.04);
        } else if (type === 'correct') {
          [523.25, 659.25, 783.99].forEach((freq, idx) => {
            const o = audioCtx.createOscillator();
            const g = audioCtx.createGain();
            o.connect(g);
            g.connect(audioCtx.destination);
            o.type = 'triangle';
            o.frequency.setValueAtTime(freq, now + idx * 0.07);
            g.gain.setValueAtTime(0.15, now + idx * 0.07);
            g.gain.exponentialRampToValueAtTime(0.01, now + idx * 0.07 + 0.22);
            o.start(now + idx * 0.07);
            o.stop(now + idx * 0.07 + 0.22);
          });
        } else if (type === 'wrong') {
          osc.type = 'sawtooth';
          osc.frequency.setValueAtTime(175, now);
          osc.frequency.linearRampToValueAtTime(105, now + 0.22);
          gain.gain.setValueAtTime(0.15, now);
          gain.gain.linearRampToValueAtTime(0.01, now + 0.22);
          osc.start(now);
          osc.stop(now + 0.22);
        } else if (type === 'lifeline') {
          osc.type = 'sine';
          osc.frequency.setValueAtTime(320, now);
          osc.frequency.exponentialRampToValueAtTime(640, now + 0.14);
          gain.gain.setValueAtTime(0.15, now);
          gain.gain.linearRampToValueAtTime(0.01, now + 0.14);
          osc.start(now);
          osc.stop(now + 0.14);
        }
      } catch (e) {
        console.warn("Audio exception:", e);
      }
    }

    function toggleSound() {
      isSoundOn = !isSoundOn;
      document.getElementById('soundIcon').innerText = isSoundOn ? "🔊" : "🔇";
      playSound('click');
    }

    /* ==========================================================================
       5. GAME SETUP & MODE CONTROLS
       ========================================================================== */
    function selectGameMode(modeKey) {
      gameMode = modeKey;
      ['part', 'full', 'survival'].forEach(k => {
        const btn = document.getElementById(`modeBtn${k.charAt(0).toUpperCase() + k.slice(1)}`);
        if (k === modeKey) {
          btn.className = "p-2.5 rounded-xl border-2 border-rev-red bg-red-50 text-left transition-all";
        } else {
          btn.className = "p-2.5 rounded-xl border-2 border-paper-300 bg-paper-100 text-left transition-all opacity-70";
        }
      });
      playSound('click');
    }

    function startGame() {
      const nameInput = document.getElementById('inputPlayerName').value.trim();
      playerName = nameInput !== "" ? nameInput : "Chiến sĩ Mùa Thu";

      score = 0;
      combo = 0;
      maxCombo = 0;
      lives = 3;
      currentIndex = 0;
      userAnswersLog = [];
      lifelines = { hint: false, fiftyFifty: false, double: false };
      isDoubleActive = false;

      // Configure Mode Settings
      let totalQCount = 15;
      if (gameMode === 'part') {
        totalQCount = 10;
        maxTimerPerQuestion = 20;
      } else if (gameMode === 'full') {
        totalQCount = 15;
        maxTimerPerQuestion = 15;
      } else if (gameMode === 'survival') {
        totalQCount = 15;
        maxTimerPerQuestion = 12;
      }

      // Prepare Randomized Dataset
      currentQuestions = JSON.parse(JSON.stringify(masterQuestions)).sort(() => 0.5 - Math.random()).slice(0, totalQCount);
      currentQuestions.forEach(q => {
        const origAns = q.options[q.correct];
        q.options.sort(() => 0.5 - Math.random());
        q.correct = q.options.indexOf(origAns);
      });

      // Update Top Bar
      document.getElementById('activePlayerDisplayName').innerText = playerName;
      document.getElementById('activeModeBadge').innerText = `Chế độ: ${
        gameMode === 'part' ? 'Khởi Nghĩa Từng Phần (20s)' : gameMode === 'full' ? 'Tổng Khởi Nghĩa (15s)' : 'Sinh Tồn 3 Tim (12s)'
      }`;
      document.getElementById('scoreVal').innerText = "0";

      resetLifelineButtonsUI();

      const heartsContainer = document.getElementById('livesContainer');
      if (gameMode === 'survival') {
        heartsContainer.classList.remove('hidden');
        updateLivesUI();
      } else {
        heartsContainer.classList.add('hidden');
      }

      document.getElementById('welcomeScreen').classList.add('hidden');
      document.getElementById('resultScreen').classList.add('hidden');
      document.getElementById('quizScreen').classList.remove('hidden');

      renderQuestion();
      playSound('click');
    }

    /* ==========================================================================
       6. QUESTION RENDER & GRAPHICS ENGINE
       ========================================================================== */
    function renderQuestion() {
      if (currentIndex >= currentQuestions.length || (gameMode === 'survival' && lives <= 0)) {
        finishGame();
        return;
      }

      const q = currentQuestions[currentIndex];

      document.getElementById('questionNumberBadge').innerText = `CÂU ${currentIndex + 1} / ${currentQuestions.length}`;
      document.getElementById('difficultyBadge').innerText = q.level;
      document.getElementById('questionText').innerText = q.question;

      document.getElementById('hintBox').classList.add('hidden');
      document.getElementById('hintText').innerText = "";

      // 1. Render SVG Scene Stage
      document.getElementById('sceneSvgContainer').innerHTML = getSceneSvgHTML(q.theme);

      // 2. Render Mascot State
      updateMascotUI('thinking', "Suy nghĩ kỹ thời cơ chính xác nhé!");

      // 3. Render Options
      const optionsGrid = document.getElementById('optionsGrid');
      optionsGrid.innerHTML = '';
      const labels = ['A', 'B', 'C', 'D'];

      q.options.forEach((opt, idx) => {
        const btn = document.createElement('button');
        btn.id = `optBtn_${idx}`;
        btn.className = "option-btn w-full text-left bg-paper-50 hover:bg-amber-100/90 border-2 border-paper-300 p-3 rounded-2xl text-xs sm:text-sm text-stone-900 font-medium transition-all flex items-start space-x-2.5 shadow-sm";
        btn.onclick = () => handleAnswer(idx);
        btn.innerHTML = `
          <span class="w-5 h-5 rounded-lg bg-paper-300 text-rev-darkred font-bold text-xs flex items-center justify-center shrink-0 mt-0.5 border border-paper-400">
            ${labels[idx]}
          </span>
          <span class="leading-relaxed flex-1">${opt}</span>
        `;
        optionsGrid.appendChild(btn);
      });

      updateTimelineMapUI();
      isDoubleActive = false;
      startTimer();
    }

    function updateMascotUI(state, text) {
      document.getElementById('mascotSvgContainer').innerHTML = getMascotSvgHTML(state);
      document.getElementById('mascotSpeech').innerText = `"${text}"`;
    }

    function startTimer() {
      clearInterval(timerInterval);
      timer = maxTimerPerQuestion;
      updateTimerUI();

      timerInterval = setInterval(() => {
        timer--;
        updateTimerUI();
        if (timer <= 4 && timer > 0) {
          updateMascotUI('worried', "Sắp hết thời gian rồi!");
        }
        if (timer <= 0) {
          clearInterval(timerInterval);
          handleAnswer(-1); // Timeout
        }
      }, 1000);
    }

    function updateTimerUI() {
      const timerVal = document.getElementById('timerVal');
      const timerBar = document.getElementById('timerBar');
      timerVal.innerText = `${timer}s`;
      const pct = (timer / maxTimerPerQuestion) * 100;
      timerBar.style.width = `${pct}%`;

      if (timer <= 4) {
        timerBar.className = "h-full bg-red-600 transition-all duration-1000 rounded-full animate-pulse";
      } else if (timer <= 8) {
        timerBar.className = "h-full bg-amber-500 transition-all duration-1000 rounded-full";
      } else {
        timerBar.className = "h-full bg-emerald-600 transition-all duration-1000 rounded-full";
      }
    }

    function updateLivesUI() {
      const container = document.getElementById('livesContainer');
      container.innerHTML = '';
      for (let i = 0; i < 3; i++) {
        const heart = document.createElement('span');
        heart.className = i < lives ? "text-red-600 text-sm" : "text-stone-300 text-sm opacity-40";
        heart.innerText = "❤️";
        container.appendChild(heart);
      }
    }

    function updateTimelineMapUI() {
      const pct = ((currentIndex + 1) / currentQuestions.length) * 100;
      document.getElementById('timelineProgressBar').style.width = `${pct}%`;

      // Highlight current Map Node
      const nodeIndex = Math.min(5, Math.floor((currentIndex / currentQuestions.length) * 6));
      for (let i = 0; i < 6; i++) {
        const el = document.getElementById(`node-${i}`);
        if (i <= nodeIndex) {
          el.className = "text-rev-red font-black border-b-2 border-rev-red pb-0.5";
        } else {
          el.className = "text-stone-500 font-medium";
        }
      }
      
      const nodeTitles = [
        "1. Việt Bắc Tân Trào",
        "2. Phá Kho Thóc Cứu Đói",
        "3. 4 Tỉnh Độc Lập (18/8)",
        "4. Khởi Nghĩa Hà Nội (19/8)",
        "5. Cố Đô Huế & Sài Gòn",
        "6. Ba Đình Tuyên Ngôn 2/9"
      ];
      document.getElementById('milestoneTitle').innerText = nodeTitles[nodeIndex];
    }

    /* ==========================================================================
       7. LIFELINES SYSTEM
       ========================================================================== */
    function resetLifelineButtonsUI() {
      ['hint', '5050', 'double'].forEach(key => {
        const btn = document.getElementById(key === 'hint' ? 'btnLifelineHint' : key === '5050' ? 'btnLifeline5050' : 'btnLifelineDouble');
        btn.disabled = false;
        btn.classList.remove('opacity-40', 'cursor-not-allowed');
      });
    }

    function useLifeline(type) {
      if (lifelines[type]) return;
      lifelines[type] = true;
      playSound('lifeline');

      const btn = document.getElementById(type === 'hint' ? 'btnLifelineHint' : type === '5050' ? 'btnLifeline5050' : 'btnLifelineDouble');
      btn.disabled = true;

      const q = currentQuestions[currentIndex];

      if (type === 'hint') {
        document.getElementById('hintBox').classList.remove('hidden');
        document.getElementById('hintText').innerText = q.hint;
      } else if (type === '5050') {
        let wrongIndices = [0, 1, 2, 3].filter(idx => idx !== q.correct);
        wrongIndices.sort(() => 0.5 - Math.random());
        let toHide = wrongIndices.slice(0, 2);

        toHide.forEach(idx => {
          const btnOpt = document.getElementById(`optBtn_${idx}`);
          if (btnOpt) btnOpt.style.visibility = 'hidden';
        });
      } else if (type === 'double') {
        isDoubleActive = true;
        btn.innerText = "⭐ Đã x2!";
      }
    }

    /* ==========================================================================
       8. ANSWER HANDLING & EXPLANATION MODAL
       ========================================================================== */
    function handleAnswer(selectedIndex) {
      clearInterval(timerInterval);

      const q = currentQuestions[currentIndex];
      const isCorrect = selectedIndex === q.correct;
      let pointsEarned = 0;

      if (isCorrect) {
        combo++;
        if (combo > maxCombo) maxCombo = combo;

        pointsEarned = 100 + timer * 5;
        if (combo > 1) pointsEarned = Math.round(pointsEarned * (1 + (combo - 1) * 0.25));
        if (isDoubleActive) pointsEarned *= 2;

        score += pointsEarned;
        document.getElementById('scoreVal').innerText = score;

        if (combo > 1) {
          const comboBadge = document.getElementById('comboBadge');
          comboBadge.classList.remove('hidden');
          document.getElementById('comboVal').innerText = combo;
          updateMascotUI('combo', `Xuất sắc! Combo x${combo}!`);
        } else {
          updateMascotUI('happy', "Hoan hô! Đáp án rất chính xác!");
        }

        // Trigger Sparkle animation
        const sparkle = document.getElementById('sparkleOverlay');
        sparkle.classList.remove('hidden');
        setTimeout(() => sparkle.classList.add('hidden'), 800);

        playSound('correct');
      } else {
        combo = 0;
        document.getElementById('comboBadge').classList.add('hidden');

        if (gameMode === 'survival') {
          lives--;
          updateLivesUI();
        }

        updateMascotUI('worried', "Chưa chính xác rồi, cố gắng câu sau!");
        playSound('wrong');
      }

      userAnswersLog.push({
        question: q.question,
        options: q.options,
        userIndex: selectedIndex,
        correctIndex: q.correct,
        isCorrect: isCorrect,
        explanation: q.explanation,
        theme: q.theme
      });

      showExplanationModal(isCorrect, q, pointsEarned, selectedIndex);
    }

    function showExplanationModal(isCorrect, q, pointsEarned, selectedIndex) {
      const modal = document.getElementById('explanationModal');
      const icon = document.getElementById('expIcon');
      const title = document.getElementById('expTitleText');
      const header = document.getElementById('expHeaderBadge');
      const bonusText = document.getElementById('expBonusEarned');

      if (isCorrect) {
        icon.innerText = "✅";
        title.innerText = "CHÍNH XÁC HOÀN HẢO!";
        header.className = "flex items-center space-x-2 font-display font-black text-lg sm:text-2xl text-emerald-800";
        bonusText.innerText = `+${pointsEarned} điểm ${isDoubleActive ? '(x2 Thưởng!)' : ''}`;
      } else {
        icon.innerText = selectedIndex === -1 ? "⏱️" : "❌";
        title.innerText = selectedIndex === -1 ? "HẾT GIỜ RỒI!" : "CHƯA CHÍNH XÁC!";
        header.className = "flex items-center space-x-2 font-display font-black text-lg sm:text-2xl text-rev-red";
        bonusText.innerText = gameMode === 'survival' ? "Trừ 1 Mạng tinh thần" : "Tiếp tục học hỏi!";
      }

      document.getElementById('expCorrectAnswer').innerText = `${['A','B','C','D'][q.correct]}. ${q.options[q.correct]}`;
      document.getElementById('expDetailText').innerText = q.explanation;
      document.getElementById('expMiniDocGraphic').innerHTML = getSceneSvgHTML(q.theme);

      modal.classList.remove('hidden');
    }

    function nextQuestion() {
      document.getElementById('explanationModal').classList.add('hidden');
      currentIndex++;
      renderQuestion();
    }

    /* ==========================================================================
       9. GAME FINISH & REVIEW LIST
       ========================================================================== */
    function finishGame() {
      clearInterval(timerInterval);

      document.getElementById('quizScreen').classList.add('hidden');
      document.getElementById('resultScreen').classList.remove('hidden');

      const correctCount = userAnswersLog.filter(a => a.isCorrect).length;
      const accuracy = Math.round((correctCount / currentQuestions.length) * 100);

      document.getElementById('finalScore').innerText = score;
      document.getElementById('finalCorrectCount').innerText = `${correctCount}/${currentQuestions.length}`;
      document.getElementById('finalMaxCombo').innerText = `${maxCombo}x`;
      document.getElementById('finalAccuracy').innerText = `${accuracy}%`;

      let titleAward = "CHIẾN SĨ TIÊN PHONG ⭐";
      if (accuracy >= 90) titleAward = "NHÀ SỬ HỌC LỖI LẠC 🏆";
      else if (accuracy >= 70) titleAward = "CHIẾN SĨ TIÊN PHONG ⭐";
      else titleAward = "CÁN BỘ CƠ SỞ 🚩";

      document.getElementById('finalTitleAward').innerText = titleAward;

      saveHighScore(playerName, score, accuracy, titleAward);
      renderReviewList();
    }

    function renderReviewList() {
      const container = document.getElementById('reviewQuestionsContainer');
      container.innerHTML = '';

      userAnswersLog.forEach((log, idx) => {
        const item = document.createElement('div');
        item.className = `p-3 rounded-2xl border text-xs space-y-2 transition-all ${
          log.isCorrect ? 'bg-emerald-50/80 border-emerald-300' : 'bg-red-50/80 border-red-300'
        }`;

        const userText = log.userIndex === -1 ? "Hết giờ" : `${['A','B','C','D'][log.userIndex]}. ${log.options[log.userIndex]}`;
        const correctText = `${['A','B','C','D'][log.correctIndex]}. ${log.options[log.correctIndex]}`;

        item.innerHTML = `
          <div class="flex items-start space-x-3">
            <div class="w-12 h-12 rounded-xl bg-stone-900 border border-rev-gold shrink-0 overflow-hidden">
              ${getSceneSvgHTML(log.theme)}
            </div>
            <div class="flex-1 space-y-1">
              <div class="flex justify-between items-start font-bold">
                <span class="text-stone-900">Câu ${idx + 1}: ${log.question}</span>
                <span class="${log.isCorrect ? 'text-emerald-700' : 'text-rev-red'} shrink-0 ml-2">
                  ${log.isCorrect ? '✅ Đúng' : '❌ Sai'}
                </span>
              </div>
              <div class="text-stone-700 space-y-0.5">
                <div><span class="font-bold">Lựa chọn của bạn:</span> <span class="${log.isCorrect ? 'text-emerald-800' : 'text-rev-red'}">${userText}</span></div>
                ${!log.isCorrect ? `<div><span class="font-bold text-emerald-800">Đáp án chuẩn:</span> ${correctText}</div>` : ''}
              </div>
              <div class="text-[11px] text-stone-600 italic border-t border-stone-300 pt-1 font-serif">
                📖 ${log.explanation}
              </div>
            </div>
          </div>
        `;
        container.appendChild(item);
      });
    }

    /* ==========================================================================
       10. LOCALSTORAGE LEADERBOARD
       ========================================================================== */
    function saveHighScore(name, scoreVal, accuracyVal, titleVal) {
      try {
        let scores = JSON.parse(localStorage.getItem('august1945_art_quiz_scores') || '[]');
        scores.push({
          name: name,
          score: scoreVal,
          accuracy: accuracyVal,
          title: titleVal,
          date: new Date().toLocaleDateString('vi-VN')
        });
        scores.sort((a, b) => b.score - a.score);
        scores = scores.slice(0, 10);
        localStorage.setItem('august1945_art_quiz_scores', JSON.stringify(scores));
      } catch (e) {
        console.warn("Storage error:", e);
      }
    }

    function toggleLeaderboardModal() {
      const modal = document.getElementById('leaderboardModal');
      const isHidden = modal.classList.contains('hidden');

      if (isHidden) {
        renderLeaderboardUI();
        modal.classList.remove('hidden');
      } else {
        modal.classList.add('hidden');
      }
      playSound('click');
    }

    function renderLeaderboardUI() {
      const container = document.getElementById('leaderboardList');
      container.innerHTML = '';

      let scores = [];
      try {
        scores = JSON.parse(localStorage.getItem('august1945_art_quiz_scores') || '[]');
      } catch (e) {}

      if (scores.length === 0) {
        container.innerHTML = `<p class="text-xs text-stone-500 text-center py-4">Chưa có kỷ lục nào. Hãy trở thành người đầu tiên!</p>`;
        return;
      }

      scores.forEach((s, idx) => {
        const item = document.createElement('div');
        item.className = "flex justify-between items-center bg-paper-50 p-2.5 rounded-xl border border-paper-300 text-xs";
        item.innerHTML = `
          <div class="flex items-center space-x-2">
            <span class="w-6 h-6 rounded-full ${idx === 0 ? 'bg-amber-400 text-stone-900 font-bold' : 'bg-paper-300 text-stone-700'} text-[11px] flex items-center justify-center shrink-0">
              ${idx + 1}
            </span>
            <div>
              <div class="font-serif font-bold text-rev-darkred">${s.name}</div>
              <div class="text-[10px] text-stone-500">${s.title} • ${s.date}</div>
            </div>
          </div>
          <div class="font-mono font-bold text-rev-red text-sm">
            ${s.score} điểm
          </div>
        `;
        container.appendChild(item);
      });
    }

    function confirmRestart() {
      if (confirm("Bạn có muốn bắt đầu lại lượt chơi mới không?")) {
        startGame();
      }
    }
  </script>
</body>
</html>
