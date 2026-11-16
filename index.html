```html
<!DOCTYPE html>
<html lang="en" class="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Nick FX — Institutional Deriv Synthetic Terminal & Capital Protection Suite</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;500;600;700&display=swap" rel="stylesheet">
  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
            mono: ['JetBrains Mono', 'monospace'],
          }
        }
      }
    }
  </script>
  <style>
    body {
      background-color: #020617; /* slate-950 */
      color: #e2e8f0;
      font-family: 'Inter', sans-serif;
      overflow-x: hidden;
    }
    .mono { font-family: 'JetBrains Mono', monospace; }
    ::-webkit-scrollbar { width: 6px; height: 6px; }
    ::-webkit-scrollbar-track { background: #0f172a; }
    ::-webkit-scrollbar-thumb { background: #334155; border-radius: 999px; }
    ::-webkit-scrollbar-thumb:hover { background: #475569; }
    .panel {
      background: rgba(15, 23, 42, 0.88);
      backdrop-filter: blur(12px);
      border: 1px solid rgba(51, 65, 85, 0.65);
    }
    @keyframes pulseEdge {
      0%, 100% { box-shadow: 0 0 12px rgba(16, 185, 129, 0.25); }
      50% { box-shadow: 0 0 24px rgba(16, 185, 129, 0.55); }
    }
    .verified-glow { animation: pulseEdge 2s infinite; }
  </style>
</head>
<body class="min-h-screen flex flex-col selection:bg-emerald-500/30 selection:text-emerald-200">

  <!-- ===================================================================== -->
  <!-- 1. EMAIL & PASSWORD AUTHENTICATION GATEWAY                            -->
  <!-- ===================================================================== -->
  <div id="authGateway" class="fixed inset-0 z-50 flex items-center justify-center bg-[#020617] p-4">
    <div class="w-full max-w-md panel rounded-2xl p-6 sm:p-8 shadow-2xl border border-slate-800">
      <div class="flex items-center gap-3 mb-6">
        <div class="w-11 h-11 rounded-xl bg-gradient-to-br from-emerald-500 to-cyan-600 flex items-center justify-center font-black text-slate-950 text-lg shadow-lg shadow-emerald-950">
          NFX
        </div>
        <div>
          <h1 class="text-2xl font-extrabold tracking-tight text-white">NICK <span class="text-emerald-400">FX</span></h1>
          <p class="text-xs text-slate-400">Deriv Synthetic Terminal & Capital Shield</p>
        </div>
      </div>

      <!-- Login / Register Switcher -->
      <div class="grid grid-cols-2 gap-1 p-1 bg-slate-950 rounded-xl border border-slate-800 mb-5">
        <button id="authTabLogin" type="button" onclick="setAuthTab('login')" class="py-2.5 text-sm font-bold rounded-lg bg-emerald-500 text-slate-950 transition">Sign In</button>
        <button id="authTabRegister" type="button" onclick="setAuthTab('register')" class="py-2.5 text-sm font-semibold rounded-lg text-slate-400 hover:text-white transition">Create Account</button>
      </div>

      <form onsubmit="submitAuthForm(event)" class="space-y-4">
        <div>
          <label class="block text-xs font-semibold uppercase tracking-wider text-slate-400 mb-1.5">Email Address</label>
          <input id="authEmailInput" type="email" required placeholder="trader@nickfx.io"
            class="w-full px-4 py-3 rounded-xl bg-slate-950 border border-slate-800 text-white placeholder-slate-600 focus:outline-none focus:border-emerald-500 transition" />
        </div>
        <div>
          <label class="block text-xs font-semibold uppercase tracking-wider text-slate-400 mb-1.5">Password</label>
          <input id="authPasswordInput" type="password" required minlength="4" placeholder="••••••••"
            class="w-full px-4 py-3 rounded-xl bg-slate-950 border border-slate-800 text-white placeholder-slate-600 focus:outline-none focus:border-emerald-500 transition" />
        </div>

        <div id="authErrorBox" class="hidden text-xs p-3 rounded-xl bg-rose-950/70 border border-rose-500/40 text-rose-200"></div>

        <button id="authSubmitButton" type="submit"
          class="w-full py-3.5 rounded-xl bg-gradient-to-r from-emerald-500 to-cyan-500 hover:from-emerald-400 hover:to-cyan-400 text-slate-950 font-extrabold text-sm shadow-lg shadow-emerald-950/60 transition cursor-pointer">
          Sign In to Nick FX
        </button>
      </form>

      <div class="mt-6 pt-4 border-t border-slate-800 flex items-center justify-between text-xs text-slate-400">
        <span>Isolated User Vaults & Guardrails</span>
        <button type="button" onclick="quickDemoLogin()" class="text-cyan-400 hover:text-cyan-300 font-bold underline cursor-pointer">
          Quick Demo Login
        </button>
      </div>
    </div>
  </div>

  <!-- ===================================================================== -->
  <!-- 2. DERIV ACCOUNT CONNECTION MODAL (API TOKEN & OAUTH 2.0)             -->
  <!-- ===================================================================== -->
  <div id="derivConnectModal" class="hidden fixed inset-0 z-50 flex items-center justify-center bg-black/80 backdrop-blur-sm p-4">
    <div class="w-full max-w-lg panel rounded-2xl p-6 border border-slate-700 shadow-2xl max-h-[90vh] overflow-y-auto">
      <div class="flex items-center justify-between pb-4 border-b border-slate-800">
        <div class="flex items-center gap-2.5">
          <span class="w-3 h-3 rounded-full bg-rose-500"></span>
          <h2 class="text-lg font-extrabold text-white">Connect Deriv Account (WebSocket v3)</h2>
        </div>
        <button type="button" onclick="closeDerivModal()" class="p-2 rounded-lg text-slate-400 hover:text-white hover:bg-slate-800">✕</button>
      </div>

      <div class="mt-4 space-y-5">
        <!-- Custom App ID -->
        <div class="p-3.5 rounded-xl bg-slate-950 border border-slate-800 flex items-center justify-between gap-3">
          <div>
            <div class="text-xs font-bold text-slate-300">Deriv WebSocket App ID</div>
            <div class="text-[11px] text-slate-500">Default public App ID is 1089</div>
          </div>
          <input id="derivAppIdInput" type="text" value="1089"
            class="w-28 px-3 py-2 rounded-lg bg-slate-900 border border-slate-700 text-xs text-cyan-300 font-bold mono text-center" />
        </div>

        <!-- Method 1: API Token -->
        <div class="p-4 rounded-xl bg-slate-950 border border-slate-800">
          <div class="flex items-center justify-between mb-1.5">
            <span class="text-xs font-extrabold uppercase tracking-wider text-emerald-400">1. Personal Access / API Token</span>
            <a href="https://app.deriv.com/account/api-token" target="_blank" rel="noopener" class="text-xs text-cyan-400 hover:underline">Create Token ↗</a>
          </div>
          <p class="text-xs text-slate-400 mb-3">Paste a Deriv API token with <b>Read</b> & <b>Trade</b> scopes enabled. Automatically imports all linked Real (`CR`) and Demo (`VRTC`) accounts.</p>
          <div class="flex flex-col sm:flex-row gap-2">
            <input id="derivApiTokenInput" type="password" placeholder="Paste Deriv API Token..."
              class="flex-1 px-3.5 py-2.5 rounded-xl bg-slate-900 border border-slate-700 text-sm text-white mono focus:outline-none focus:border-emerald-500" />
            <button type="button" onclick="authorizeDerivToken()" class="px-5 py-2.5 rounded-xl bg-emerald-500 hover:bg-emerald-400 text-slate-950 font-extrabold text-sm transition whitespace-nowrap">
              Authorize
            </button>
          </div>
        </div>

        <!-- Method 2: OAuth 2.0 -->
        <div class="p-4 rounded-xl bg-slate-950 border border-slate-800">
          <span class="block text-xs font-extrabold uppercase tracking-wider text-cyan-400 mb-1.5">2. Deriv OAuth 2.0 Official Redirect</span>
          <p class="text-xs text-slate-400 mb-3">Authenticate securely on Deriv's official portal without handling raw tokens.</p>
          <button type="button" onclick="launchDerivOAuth()" class="w-full py-2.5 px-4 rounded-xl bg-rose-600 hover:bg-rose-500 text-white font-bold text-sm transition">
            Login via oauth.deriv.com ↗
          </button>
        </div>

        <!-- Imported Accounts -->
        <div id="importedAccountsSection" class="hidden p-4 rounded-xl bg-slate-900 border border-emerald-500/30">
          <div class="flex items-center justify-between mb-2">
            <span class="text-xs font-bold uppercase text-emerald-400">Authorized Deriv Accounts</span>
            <button type="button" onclick="disconnectDerivAccount()" class="text-xs text-rose-400 hover:underline">Disconnect</button>
          </div>
          <div id="importedAccountsList" class="space-y-2"></div>
        </div>

        <div id="derivModalMessage" class="text-xs text-slate-400"></div>
      </div>
    </div>
  </div>

  <!-- ===================================================================== -->
  <!-- 3. MAIN APPLICATION WORKSPACE                                         -->
  <!-- ===================================================================== -->
  <div id="mainWorkspace" class="hidden flex-1 flex flex-col">

    <!-- HEADER BAR -->
    <header class="sticky top-0 z-30 panel border-b border-slate-800 px-3 sm:px-6 py-3">
      <div class="max-w-[1650px] mx-auto flex flex-wrap items-center justify-between gap-3">
        <!-- Brand & Live Stream Badge -->
        <div class="flex items-center gap-3">
          <div class="w-9 h-9 rounded-xl bg-gradient-to-br from-emerald-500 to-cyan-600 flex items-center justify-center font-black text-slate-950 text-sm shadow">
            NFX
          </div>
          <div>
            <div class="flex items-center gap-2">
              <span class="font-extrabold text-white tracking-tight text-base sm:text-lg">NICK <span class="text-emerald-400">FX</span></span>
              <span id="connStatusBadge" class="inline-flex items-center gap-1.5 px-2.5 py-0.5 rounded-full text-[11px] font-semibold bg-amber-500/15 text-amber-300 border border-amber-500/30">
                <span id="connStatusDot" class="w-2 h-2 rounded-full bg-amber-400 animate-pulse"></span>
                <span id="connStatusText">Connecting WS v3...</span>
              </span>
            </div>
            <div class="flex items-center gap-2 text-[11px] text-slate-400">
              <span id="headerUserEmail">trader@nickfx.io</span>
              <span>•</span>
              <button type="button" onclick="logoutUser()" class="text-rose-400 hover:underline">Logout</button>
            </div>
          </div>
        </div>

        <!-- Account Switcher, Balance, Deriv Connect & Global Kill Switch -->
        <div class="flex flex-wrap items-center gap-2 sm:gap-3">
          <div class="flex items-center bg-slate-950 border border-slate-800 rounded-xl px-3 py-1.5 gap-2">
            <div>
              <div class="flex items-center gap-1.5">
                <span id="activeAccBadge" class="px-1.5 py-0.5 rounded text-[10px] font-bold uppercase bg-cyan-500/20 text-cyan-300">PRACTICE SIM</span>
                <select id="headerAccountSelect" onchange="selectTradingAccount(this.value)" class="bg-transparent text-xs text-slate-300 font-mono focus:outline-none cursor-pointer">
                  <option value="SIM_USD" class="bg-slate-900">Practice Sim ($10,000.00)</option>
                </select>
              </div>
              <div id="headerBalanceText" class="text-sm sm:text-base font-extrabold text-white mono">$10,000.00 USD</div>
            </div>
          </div>

          <button type="button" onclick="openDerivModal()" class="px-3.5 py-2.5 rounded-xl bg-cyan-600 hover:bg-cyan-500 text-slate-950 text-xs sm:text-sm font-extrabold shadow-lg shadow-cyan-950/50 transition flex items-center gap-1.5 cursor-pointer">
            <span>⚡</span>
            <span id="headerDerivBtnText">Connect Deriv</span>
          </button>

          <button id="globalKillSwitchBtn" type="button" onclick="toggleGlobalKillSwitch()" class="px-4 py-2.5 rounded-xl bg-red-600 hover:bg-red-500 text-white text-xs sm:text-sm font-black tracking-wide shadow-lg shadow-red-950/60 transition flex items-center gap-1.5 cursor-pointer">
            <span>🛑</span>
            <span id="globalKillSwitchLabel">GLOBAL KILL SWITCH</span>
          </button>
        </div>
      </div>

      <!-- NAVIGATION TABS -->
      <nav class="max-w-[1650px] mx-auto mt-3 pt-2.5 border-t border-slate-800/80 flex items-center gap-2 overflow-x-auto">
        <button type="button" onclick="switchWorkspaceTab('terminal')" id="tabBtn-terminal" class="ws-tab px-4 py-2 rounded-xl text-xs sm:text-sm font-bold bg-emerald-500/15 text-emerald-300 border border-emerald-500/40 whitespace-nowrap">
          📊 Terminal & 4-Factor Oracle
        </button>
        <button type="button" onclick="switchWorkspaceTab('scanner')" id="tabBtn-scanner" class="ws-tab px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold text-slate-400 hover:text-white hover:bg-slate-900 whitespace-nowrap">
          📡 Multi-Volatility Scanner (All 35 Indices)
        </button>
        <button type="button" onclick="switchWorkspaceTab('bots')" id="tabBtn-bots" class="ws-tab px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold text-slate-400 hover:text-white hover:bg-slate-900 whitespace-nowrap">
          🤖 Free Bot Store (6 Bots)
        </button>
        <button type="button" onclick="switchWorkspaceTab('ai')" id="tabBtn-ai" class="ws-tab px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold text-slate-400 hover:text-white hover:bg-slate-900 whitespace-nowrap">
          🧠 AI Bot Studio & Backtester
        </button>
        <button type="button" onclick="switchWorkspaceTab('risk')" id="tabBtn-risk" class="ws-tab px-4 py-2 rounded-xl text-xs sm:text-sm font-semibold text-slate-400 hover:text-white hover:bg-slate-900 whitespace-nowrap">
          🛡️ Capital Protection & Risk Calculator
        </button>
      </nav>
    </header>

    <!-- KILL SWITCH LOCK BANNER -->
    <div id="killSwitchAlertBanner" class="hidden bg-red-600 text-white text-center py-2 px-4 text-xs sm:text-sm font-extrabold tracking-wide">
      🛑 GLOBAL KILL SWITCH ENGAGED — ALL MANUAL & BOT ORDERS ARE HARD-BLOCKED. CLICK "RESUME TRADING" TO UNLOCK.
    </div>

    <!-- =================================================================== -->
    <!-- VIEW 1: TERMINAL & 4-FACTOR CONFLUENCE ORACLE                       -->
    <!-- =================================================================== -->
    <main class="flex-1 max-w-[1650px] w-full mx-auto p-3 sm:p-5">
      <section id="tabView-terminal" class="grid grid-cols-1 lg:grid-cols-12 gap-4">

        <!-- LEFT 8 COLUMNS -->
        <div class="lg:col-span-8 space-y-4">

          <!-- Live Multi-Volatility Quick Strip -->
          <div id="quickScannerStrip" class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-6 gap-2">
            <!-- Populated dynamically -->
          </div>

          <!-- Active Index Selector & Telemetry Header -->
          <div class="panel rounded-2xl p-4 flex flex-wrap items-center justify-between gap-4">
            <div class="flex-1 min-w-[250px]">
              <label class="block text-[11px] font-bold uppercase tracking-wider text-slate-400 mb-1">Active Deriv Synthetic Index (All 35 Indices)</label>
              <select id="activeSymbolDropdown" onchange="selectTradingSymbol(this.value)"
                class="w-full px-3.5 py-2.5 rounded-xl bg-slate-950 border border-slate-700 text-sm font-bold text-white focus:outline-none focus:border-emerald-500">
                <!-- Populated dynamically from full 35-index catalog -->
              </select>
            </div>

            <div class="flex items-center gap-3">
              <div class="px-4 py-2 rounded-xl bg-slate-950 border border-slate-800 text-right">
                <div class="text-[10px] font-bold uppercase text-slate-400">Live Spot Price</div>
                <div id="telemetrySpotPrice" class="text-xl sm:text-2xl font-black mono text-white">0.0000</div>
              </div>
              <div class="px-4 py-2 rounded-xl bg-slate-950 border border-slate-800 text-center">
                <div class="text-[10px] font-bold uppercase text-slate-400">Last Digit</div>
                <div id="telemetryLastDigit" class="text-xl sm:text-2xl font-black mono text-emerald-400">-</div>
              </div>
              <div class="hidden sm:block px-3.5 py-2 rounded-xl bg-slate-950 border border-slate-800 text-center">
                <div class="text-[10px] font-bold uppercase text-slate-400">Ticks Buffered</div>
                <div id="telemetryTickCount" class="text-lg font-extrabold mono text-cyan-400">0</div>
              </div>
            </div>
          </div>

          <!-- High-DPI HTML5 Canvas Chart (Price + EMA 9 + EMA 21 + Bollinger Bands) -->
          <div class="panel rounded-2xl p-4">
            <div class="flex flex-wrap items-center justify-between gap-2 mb-3">
              <div class="flex flex-wrap items-center gap-3 text-xs">
                <span class="font-extrabold text-white">Tick Chart & Bollinger/EMA Overlay</span>
                <span class="inline-flex items-center gap-1 text-cyan-400"><span class="w-2.5 h-0.5 bg-cyan-400"></span>Spot</span>
                <span class="inline-flex items-center gap-1 text-emerald-400"><span class="w-2.5 h-0.5 bg-emerald-400"></span>EMA(9)</span>
                <span class="inline-flex items-center gap-1 text-amber-400"><span class="w-2.5 h-0.5 bg-amber-400"></span>EMA(21)</span>
                <span class="inline-flex items-center gap-1 text-slate-400"><span class="w-2.5 h-0.5 bg-slate-400"></span>BB(20,2)</span>
              </div>
              <div class="flex items-center gap-2 text-xs">
                <span class="text-slate-400">Analysis Window:</span>
                <select id="analysisWindowDropdown" onchange="setAnalysisSampleSize(this.value)" class="bg-slate-950 border border-slate-800 rounded-lg px-2.5 py-1 text-white mono">
                  <option value="60">60 Ticks</option>
                  <option value="120" selected>120 Ticks</option>
                  <option value="250">250 Ticks</option>
                </select>
              </div>
            </div>
            <div class="w-full h-64 sm:h-72 rounded-xl bg-slate-950 border border-slate-800 overflow-hidden relative">
              <canvas id="priceChartCanvas" class="w-full h-full block"></canvas>
            </div>
          </div>

          <!-- 4-FACTOR CONFLUENCE & CHI-SQUARE ANTI-BLOWUP ENGINE -->
          <div id="oraclePanel" class="panel rounded-2xl p-5 border border-slate-700 transition-all">
            <div class="flex flex-wrap items-start justify-between gap-3 pb-4 border-b border-slate-800">
              <div>
                <div class="flex items-center gap-2">
                  <span class="text-xs font-black uppercase tracking-wider text-emerald-400">4-Factor Confluence & Chi-Square Anti-Blowup Engine</span>
                </div>
                <p id="oracleExplanationText" class="text-xs text-slate-400 mt-1">
                  Evaluating statistical uniformity and multi-indicator confluence to block random RNG noise...
                </p>
              </div>
              <div id="oracleVerdictPill" class="px-4 py-2.5 rounded-xl bg-rose-950/70 border border-rose-500/40 text-right">
                <div class="text-[10px] font-bold uppercase text-rose-300">Signal Gate Status</div>
                <div id="oracleVerdictHeadline" class="text-xs sm:text-sm font-black text-rose-300">NO EDGE — RANDOM NOISE (TRADE BLOCKED)</div>
              </div>
            </div>

            <!-- 4 Factors Grid -->
            <div clas