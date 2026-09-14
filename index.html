<!DOCTYPE html>  
<html lang="en">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>SLA // Software Lifecycle & Architecture</title>  
    <script src="https://cdn.tailwindcss.com"></script>  
    <style>  
        @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;600;700&family=Inter:wght@400;500;600;700&display=swap');  
        body { font-family: 'Inter', sans-serif; }  
        .font-mono { font-family: 'JetBrains Mono', monospace; }  
        .pawn-human { background: #06b6d4; border: 2px solid #ecfeff; box-shadow: 0 0 10px rgba(6,182,212,0.8); }  
        .pawn-ai { background: #a855f7; border: 2px solid #faf5ff; box-shadow: 0 0 10px rgba(168,85,247,0.8); }  
        .pawn-lead { border-width: 3px; border-color: #facc15 !important; }  
        .slot-hover:hover { border-color: #06b6d4; background-color: rgba(6,182,212,0.1); }  
    </style>  
</head>  
<body class="bg-slate-950 text-slate-100 min-h-screen flex flex-col font-sans select-none">  
  
    <!-- TOP TELEMETRY BAR -->  
    <header class="bg-slate-900 border-b border-slate-800 px-6 py-3 flex justify-between items-center z-30 shadow-lg">  
        <div class="flex items-center space-x-4">  
            <div class="flex items-center space-x-2">  
                <div class="h-3 w-3 rounded-full bg-cyan-400 animate-pulse"></div>  
                <h1 class="font-mono font-bold text-sm tracking-wider text-cyan-400">SLA: THE BOARD GAME</h1>  
            </div>  
            <span class="text-xs text-slate-500 font-mono hidden md:inline">// 2-Player Software Race</span>  
        </div>  
          
        <!-- ROUND TRACKER -->  
        <div class="flex items-center space-x-6 text-xs font-mono">  
            <div class="bg-slate-950 px-3 py-1.5 rounded-lg border border-slate-800">  
                YEAR: <span id="val-year" class="text-cyan-400 font-bold">1</span> / 7  
            </div>  
            <div class="bg-slate-950 px-3 py-1.5 rounded-lg border border-slate-800">  
                SEASON: <span id="val-season" class="text-amber-400 font-bold">SPRING SCHEDULE</span>  
            </div>  
            <button onclick="initGame()" class="text-xs bg-slate-800 hover:bg-slate-700 text-slate-300 px-3 py-1.5 rounded border border-slate-700 transition">Reset Board</button>  
        </div>  
    </header>  
  
    <!-- ACTIVE TURN & CONTEXT BANNER -->  
    <div id="turn-ribbon" class="bg-slate-900/90 border-b border-slate-800 px-6 py-2.5 flex justify-between items-center z-20">  
        <div class="flex items-center space-x-3 text-xs font-mono">  
            <span id="turn-dot" class="h-2.5 w-2.5 rounded-full bg-cyan-400 animate-ping"></span>  
            <span id="turn-msg" class="text-slate-200">Starting Founding Setup...</span>  
        </div>  
        <div id="turn-actions" class="flex space-x-2"></div>  
    </div>  
  
    <!-- MAIN GAME DESK (PHYSICAL BOARD LAYOUT) -->  
    <main class="flex-1 max-w-[1700px] w-full mx-auto p-4 grid grid-cols-1 lg:grid-cols-12 gap-4">  
  
        <!-- ==================================================== -->  
        <!-- LEFT: SHARED CENTRAL BOARD (THE WORKER ARENA) (7 COLS) -->  
        <!-- ==================================================== -->  
        <section class="lg:col-span-7 space-y-4">  
              
            <!-- 1. SPRING WAKE-UP SCHEDULE (1 TO 7) -->  
            <div class="bg-slate-900/90 border border-slate-800 rounded-2xl p-4 shadow-xl">  
                <div class="flex justify-between items-center mb-2.5">  
                    <h2 class="text-xs font-mono font-bold text-amber-400 tracking-wider">SPRING SPRINT SCHEDULE (TURN ORDER & BONUSES)</h2>  
                    <span class="text-[10px] text-slate-500 font-mono">Pick a time slot: earlier goes first, later yields bonuses</span>  
                </div>  
                <div id="track-spring" class="grid grid-cols-7 gap-2 text-center font-mono">  
                    <!-- 7 Wakeup Slots generated via JS -->  
                </div>  
            </div>  
  
            <!-- 2. THE WORKER PLACEMENT BOARD (SUMMER & WINTER SPACES) -->  
            <div class="bg-slate-900/90 border border-slate-800 rounded-2xl p-5 shadow-2xl space-y-5">  
                  
                <!-- SUMMER BOARD (PREPARATION & ARCHITECTURE) -->  
                <div>  
                    <div class="flex items-center justify-between border-b border-slate-800 pb-2 mb-3">  
                        <div class="flex items-center space-x-2">  
                            <span class="h-2 w-2 rounded-full bg-amber-400"></span>  
                            <h3 class="text-xs font-mono font-bold text-amber-400 tracking-wider">SUMMER ACTIONS (CODE DESIGN & CAPITAL)</h3>  
                        </div>  
                        <span class="text-[10px] text-slate-500 font-mono">1 Worker Per Slot • Lead Architect Can Share</span>  
                    </div>  
                      
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-3">  
                        <!-- Space: Commit Code -->  
                        <div id="board-slot-commit" onclick="onBoardSlotClick('COMMIT')" class="slot-hover bg-slate-950 border-2 border-slate-800 rounded-xl p-3 cursor-pointer flex flex-col justify-between h-28 relative transition">  
                            <div>  
                                <div class="text-xs font-bold text-slate-200">1. Commit Code</div>  
                                <div class="text-[10px] text-slate-400 mt-0.5">Write a code card into an open project repo.</div>  
                            </div>  
                            <div class="flex justify-between items-end">  
                                <span class="text-[9px] font-mono text-emerald-400">Requires: Code Card</span>  
                                <div id="pawn-commit" class="h-7 w-7 rounded-full border border-dashed border-slate-700 flex items-center justify-center text-[10px] font-bold"></div>  
                            </div>  
                        </div>  
  
                        <!-- Space: Raise Grant -->  
                        <div id="board-slot-fund" onclick="onBoardSlotClick('FUND')" class="slot-hover bg-slate-950 border-2 border-slate-800 rounded-xl p-3 cursor-pointer flex flex-col justify-between h-28 relative transition">  
                            <div>  
                                <div class="text-xs font-bold text-slate-200">2. Angel Round</div>  
                                <div class="text-[10px] text-slate-400 mt-0.5">Secure venture seed funding.</div>  
                            </div>  
                            <div class="flex justify-between items-end">  
                                <span class="text-[9px] font-mono text-emerald-400">Gain +$2 Cash</span>  
                                <div id="pawn-fund" class="h-7 w-7 rounded-full border border-dashed border-slate-700 flex items-center justify-center text-[10px] font-bold"></div>  
                            </div>  
                        </div>  
  
                        <!-- Space: Business Advisor -->  
                        <div id="board-slot-advisor" onclick="onBoardSlotClick('ADVISOR')" class="slot-hover bg-slate-950 border-2 border-slate-800 rounded-xl p-3 cursor-pointer flex flex-col justify-between h-28 relative transition">  
                            <div>  
                                <div class="text-xs font-bold text-slate-200">3. Business Advisor</div>  
                                <div class="text-[10px] text-slate-400 mt-0.5">Consult with commercial strategist.</div>  
                            </div>  
                            <div class="flex justify-between items-end">  
                                <span class="text-[9px] font-mono text-amber-400">Play: Yellow Card</span>  
                                <div id="pawn-advisor" class="h-7 w-7 rounded-full border border-dashed border-slate-700 flex items-center justify-center text-[10px] font-bold"></div>  
                            </div>  
                        </div>  
                    </div>  
                </div>  
  
                <!-- WINTER BOARD (PRODUCTION, RELEASES & REVENUE) -->  
                <div>  
                    <div class="flex items-center justify-between border-b border-slate-800 pb-2 mb-3">  
                        <div class="flex items-center space-x-2">  
                            <span class="h-2 w-2 rounded-full bg-cyan-400"></span>  
                            <h3 class="text-xs font-mono font-bold text-cyan-400 tracking-wider">WINTER ACTIONS (RELEASE, PIPELINES & SLAS)</h3>  
                        </div>  
                        <span class="text-[10px] text-slate-500 font-mono">1 Worker Per Slot • Lead Architect Can Share</span>  
                    </div>  
                      
                    <div class="grid grid-cols-1 sm:grid-cols-4 gap-3">  
                        <!-- Space: Extract Code (Harvest) -->  
                        <div id="board-slot-extract" onclick="onBoardSlotClick('EXTRACT')" class="slot-hover bg-slate-950 border-2 border-slate-800 rounded-xl p-3 cursor-pointer flex flex-col justify-between h-28 relative transition">  
                            <div>  
                                <div class="text-xs font-bold text-slate-200">1. Extract Code</div>  
                                <div class="text-[10px] text-slate-400 mt-0.5">Sweep repo code into memory cache.</div>  
                            </div>  
                            <div class="flex justify-between items-end">  
                                <span class="text-[9px] font-mono text-cyan-400">Harvests Repos</span>  
                                <div id="pawn-extract" class="h-7 w-7 rounded-full border border-dashed border-slate-700 flex items-center justify-center text-[10px] font-bold"></div>  
                            </div>  
                        </div>  
  
                        <!-- Space: Compile Release (Make Wine) -->  
                        <div id="board-slot-compile" onclick="onBoardSlotClick('COMPILE')" class="slot-hover bg-slate-950 border-2 border-slate-800 rounded-xl p-3 cursor-pointer flex flex-col justify-between h-28 relative transition">  
                            <div>  
                                <div class="text-xs font-bold text-slate-200">2. Build Release</div>  
                                <div class="text-[10px] text-slate-400 mt-0.5">Compile cached fragments to live builds.</div>  
                            </div>  
                            <div class="flex justify-between items-end">  
                                <span class="text-[9px] font-mono text-cyan-400">Memory $\to$ Builds</span>  
                                <div id="pawn-compile" class="h-7 w-7 rounded-full border border-dashed border-slate-700 flex items-center justify-center text-[10px] font-bold"></div>  
                            </div>  
                        </div>  
  
                        <!-- Space: Deliver Client SLA (Orders) -->  
                        <div id="board-slot-sla" onclick="onBoardSlotClick('SLA')" class="slot-hover bg-slate-950 border-2 border-slate-800 rounded-xl p-3 cursor-pointer flex flex-col justify-between h-28 relative transition">  
                            <div>  
                                <div class="text-xs font-bold text-slate-200">3. Deliver SLA</div>  
                                <div class="text-[10px] text-slate-400 mt-0.5">Ship matching software for ARR.</div>  
                            </div>  
                            <div class="flex justify-between items-end">  
                                <span class="text-[9px] font-mono text-purple-400">Play: Purple Card</span>  
                                <div id="pawn-sla" class="h-7 w-7 rounded-full border border-dashed border-slate-700 flex items-center justify-center text-[10px] font-bold"></div>  
                            </div>  
                        </div>  
  
                        <!-- Space: Principal Architect -->  
                        <div id="board-slot-principal" onclick="onBoardSlotClick('PRINCIPAL')" class="slot-hover bg-slate-950 border-2 border-slate-800 rounded-xl p-3 cursor-pointer flex flex-col justify-between h-28 relative transition">  
                            <div>  
                                <div class="text-xs font-bold text-slate-200">4. Lead Principal</div>  
                                <div class="text-[10px] text-slate-400 mt-0.5">Deploy technical staff engineer.</div>  
                            </div>  
                            <div class="flex justify-between items-end">  
                                <span class="text-[9px] font-mono text-blue-400">Play: Blue Card</span>  
                                <div id="pawn-principal" class="h-7 w-7 rounded-full border border-dashed border-slate-700 flex items-center justify-center text-[10px] font-bold"></div>  
                            </div>  
                        </div>  
                    </div>  
                </div>  
  
            </div>  
  
            <!-- 3. RIVAL COMPETITOR MAT (LIVE INTELLIGENCE) -->  
            <div class="bg-slate-900/80 border border-slate-800 rounded-2xl p-4 shadow-xl flex justify-between items-center font-mono">  
                <div class="flex items-center space-x-3">  
                    <div class="h-8 w-8 rounded-full pawn-ai flex items-center justify-center text-xs font-bold text-white">AI</div>  
                    <div>  
                        <div class="text-xs font-bold text-purple-400">RIVAL STARTUP SYNDICATE</div>  
                        <div id="ai-status-text" class="text-[10px] text-slate-400">Waiting for spring deployment...</div>  
                    </div>  
                </div>  
                <div class="flex space-x-4 text-xs">  
                    <div class="bg-slate-950 px-3 py-1.5 rounded-lg border border-slate-800 text-center">  
                        <span class="text-[9px] text-slate-500 block">REVENUE</span>  
                        <strong id="val-ai-arr" class="text-purple-400 font-bold text-sm">0 ARR</strong>  
                    </div>  
                    <div class="bg-slate-950 px-3 py-1.5 rounded-lg border border-slate-800 text-center">  
                        <span class="text-[9px] text-slate-500 block">CAPITAL</span>  
                        <strong id="val-ai-cap" class="text-emerald-400 font-bold text-sm">$4</strong>  
                    </div>  
                    <div class="bg-slate-950 px-3 py-1.5 rounded-lg border border-slate-800 text-center">  
                        <span class="text-[9px] text-slate-500 block">WORKERS</span>  
                        <strong id="val-ai-workers" class="text-slate-200 font-bold text-sm">3 / 3</strong>  
                    </div>  
                </div>  
            </div>  
        </section>  
  
        <!-- ==================================================== -->  
        <!-- RIGHT: YOUR PERSONAL WORKBENCH & INVENTORY (5 COLS) -->  
        <!-- ==================================================== -->  
        <section class="lg:col-span-5 space-y-4">  
              
            <!-- YOUR COMPANY VITALS & WORKFORCE POOL -->  
            <div class="bg-slate-900/90 border border-slate-800 rounded-2xl p-4 shadow-xl">  
                <div class="flex justify-between items-center border-b border-slate-800 pb-2 mb-3">  
                    <div class="flex items-center space-x-2">  
                        <div class="h-3 w-3 rounded-full pawn-human"></div>  
                        <h2 class="text-xs font-mono font-bold text-cyan-400 tracking-wider">YOUR STARTUP WORKBENCH</h2>  
                    </div>  
                    <span id="label-your-order" class="text-[10px] font-mono text-slate-400 bg-slate-950 px-2 py-0.5 rounded border border-slate-800">Sprint Pos: -</span>  
                </div>  
  
                <div class="grid grid-cols-3 gap-2 text-center font-mono mb-4">  
                    <div class="bg-slate-950 p-2 rounded-xl border border-slate-800">  
                        <div class="text-[9px] text-slate-400">ANNUAL REV (ARR)</div>  
                        <div id="val-player-arr" class="text-xl font-bold text-cyan-400">0</div>  
                        <div class="text-[8px] text-slate-500">Target: 20</div>  
                    </div>  
                    <div class="bg-slate-950 p-2 rounded-xl border border-slate-800">  
                        <div class="text-[9px] text-slate-400">BANK BALANCE</div>  
                        <div id="val-player-cap" class="text-xl font-bold text-emerald-400">$4</div>  
                        <div class="text-[8px] text-slate-500">Liquid Cash</div>  
                    </div>  
                    <div class="bg-slate-950 p-2 rounded-xl border border-slate-800">  
                        <div class="text-[9px] text-slate-400">RESIDUAL INCOME</div>  
                        <div id="val-player-res" class="text-xl font-bold text-amber-400">$0</div>  
                        <div class="text-[8px] text-slate-500">Paid Every Year</div>  
                    </div>  
                </div>  
  
                <!-- 3 WORKERS (2 DEVS + 1 LEAD ARCHITECT) -->  
                <div>  
                    <div class="text-[10px] font-mono text-slate-400 mb-2 flex justify-between">  
                        <span>YOUR WORKFORCE (3 WORKERS SHARED ALL YEAR)</span>  
                        <span id="label-workers-avail" class="text-cyan-400 font-bold">3 Available</span>  
                    </div>  
                    <div id="pool-workers" class="flex gap-2 font-mono text-xs">  
                        <!-- Worker tokens rendered via JS -->  
                    </div>  
                </div>  
            </div>  
  
            <!-- CODE REPOSITORIES & PRODUCTION INFRASTRUCTURE -->  
            <div class="bg-slate-900/90 border border-slate-800 rounded-2xl p-4 shadow-xl space-y-3 font-mono">  
                <div class="flex justify-between items-center border-b border-slate-800 pb-2">  
                    <span class="text-xs font-bold text-slate-200">PRODUCTION INFRASTRUCTURE</span>  
                    <button onclick="upgradeCluster()" class="text-[10px] bg-cyan-950 text-cyan-300 hover:bg-cyan-900 border border-cyan-800 px-2 py-1 rounded transition">  
                        Upgrade Cluster ($4)  
                    </button>  
                </div>  
  
                <!-- 3 Repos (Fields) -->  
                <div>  
                    <span class="text-[10px] text-slate-400 block mb-1.5">GIT REPOSITORIES (COMMITTED SOURCE CODE)</span>  
                    <div id="container-repos" class="grid grid-cols-3 gap-2 text-xs">  
                        <!-- 3 Repos rendered via JS -->  
                    </div>  
                </div>  
  
                <!-- RAM Memory Buffer (Crush Pad) & Live Builds (Cellar) -->  
                <div class="grid grid-cols-2 gap-3 pt-1">  
                    <!-- Memory Buffer -->  
                    <div class="bg-slate-950 p-2.5 rounded-xl border border-slate-800">  
                        <span class="text-[10px] text-slate-400 block mb-1">MEMORY CACHE (RAM)</span>  
                        <div id="container-buffer" class="min-h-[40px] flex flex-wrap gap-1 items-center text-xs">  
                            <span class="text-slate-600 text-[10px] italic">Cache Empty</span>  
                        </div>  
                    </div>  
  
                    <!-- Live Builds -->  
                    <div class="bg-slate-950 p-2.5 rounded-xl border border-slate-800">  
                        <div class="flex justify-between text-[10px] text-slate-400 mb-1">  
                            <span>DEPLOYED BUILDS</span>  
                            <span id="label-cluster-tier" class="text-cyan-400 font-bold">Tier 3 Max</span>  
                        </div>  
                        <div id="container-builds" class="min-h-[40px] space-y-1 text-xs">  
                            <span class="text-slate-600 text-[10px] italic">No active builds</span>  
                        </div>  
                    </div>  
                </div>  
                <div class="text-[10px] text-slate-500 leading-tight">  
                    ℹ️ <strong>Automated Hardening:</strong> Code on your Live Servers automatically increases +1 Quality Level at the end of each Year as automated test suites fix bugs!  
                </div>  
            </div>  
  
            <!-- CARDS IN HAND -->  
            <div class="bg-slate-900/90 border border-slate-800 rounded-2xl p-4 shadow-xl font-mono space-y-2">  
                <div class="flex justify-between items-center border-b border-slate-800 pb-2">  
                    <span class="text-xs font-bold text-slate-200">CARDS IN HAND (<span id="count-hand">0</span>)</span>  
                    <span class="text-[10px] text-slate-500">Green = Code • Purple = Deals • Yellow = Advisors • Blue = Staff</span>  
                </div>  
                <div id="container-hand" class="grid grid-cols-1 sm:grid-cols-2 gap-2 max-h-56 overflow-y-auto pr-1">  
                    <!-- Hand cards rendered here -->  
                </div>  
            </div>  
  
        </section>  
  
    </main>  
  
    <!-- ==================================================== -->  
    <!-- INTERACTIVE ACTION MODAL (BOTTOM DRAWER PICKER) -->  
    <!-- ==================================================== -->  
    <div id="modal-picker" class="fixed inset-0 z-50 bg-slate-950/80 backdrop-blur-sm hidden flex items-center justify-center p-4">  
        <div class="bg-slate-900 border border-slate-800 rounded-3xl max-w-lg w-full p-6 font-mono shadow-2xl space-y-4">  
            <div class="border-b border-slate-800 pb-3 flex justify-between items-center">  
                <div>  
                    <span id="picker-badge" class="text-[10px] font-bold text-cyan-400 tracking-widest block uppercase">ACTION IN PROGRESS</span>  
                    <h3 id="picker-title" class="text-sm font-bold text-white mt-0.5">Select Software Asset</h3>  
                </div>  
                <button onclick="closePicker()" class="text-slate-400 hover:text-slate-200 text-xs px-2 py-1 rounded border border-slate-800">Cancel</button>  
            </div>  
              
            <div id="picker-body" class="text-xs text-slate-300 space-y-2 max-h-72 overflow-y-auto pr-1">  
                <!-- Picker cards/options rendered here -->  
            </div>  
              
            <div class="pt-2 border-t border-slate-800 flex justify-end">  
                <button onclick="closePicker()" class="bg-slate-800 hover:bg-slate-700 text-slate-300 text-xs px-4 py-2 rounded-xl transition">Never Mind</button>  
            </div>  
        </div>  
    </div>  
  
    <!-- ==================================================== -->  
    <!-- GAME LOGIC ENGINE -->  
    <!-- ==================================================== -->  
    <script>  
        // MASTER CARD DECKS (PURE TECH EQUIVALENTS)  
        const DECK_MODULES = [  
            { id: "m1", type: "MODULE", sub: "FRONTEND", name: "Tailwind UI Kit", val: 1 },  
            { id: "m2", type: "MODULE", sub: "FRONTEND", name: "React Portal Core", val: 2 },  
            { id: "m3", type: "MODULE", sub: "FRONTEND", name: "WebGL 3D Engine", val: 3 },  
            { id: "m4", type: "MODULE", sub: "BACKEND", name: "Node Express API", val: 1 },  
            { id: "m5", type: "MODULE", sub: "BACKEND", name: "Rust Memory Core", val: 2 },  
            { id: "m6", type: "MODULE", sub: "BACKEND", name: "Postgres Cluster Pool", val: 3 },  
            { id: "m7", type: "MODULE", sub: "FULLSTACK", name: "Kafka Broker Mesh", val: 4 },  
            { id: "m8", type: "MODULE", sub: "FULLSTACK", name: "Raft Consensus Layer", val: 5 }  
        ];  
  
        const DECK_SLAS = [  
            { id: "s1", type: "SLA", title: "Local E-Commerce Portal", reqType: "FRONTEND", minTier: 2, arr: 2, residual: 1 },  
            { id: "s2", type: "SLA", title: "Fintech Core Gateway", reqType: "BACKEND", minTier: 3, arr: 3, residual: 1 },  
            { id: "s3", type: "SLA", title: "Enterprise Event Mesh", reqType: "FULLSTACK", minTier: 4, arr: 5, residual: 2 },  
            { id: "s4", type: "SLA", title: "GovTech Secure Records", reqType: "BACKEND", minTier: 2, arr: 2, residual: 2 },  
            { id: "s5", type: "SLA", title: "Global Telecom 99.999%", reqType: "FULLSTACK", minTier: 5, arr: 6, residual: 3 }  
        ];  
  
        const DECK_ADVISORS = [  
            { id: "a1", type: "ADVISOR", title: "Angel Investor", desc: "Gain +$4 Venture Seed Capital.", run: (p) => { p.capital += 4; } },  
            { id: "a2", type: "ADVISOR", title: "Sales Closer", desc: "Gain +1 ARR directly.", run: (p) => { p.arr += 1; } },  
            { id: "a3", type: "ADVISOR", title: "Talent Recruiter", desc: "Add 1 temporary Junior Dev for this year.", run: (p) => { p.workers.push({ id: 99, type: 'JUNIOR', available: true }); } },  
            { id: "a4", type: "ADVISOR", title: "Growth Mentor", desc: "Draw 2 Code cards & gain +$1 Capital.", run: (p) => { drawCard('MODULE'); drawCard('MODULE'); p.capital += 1; } }  
        ];  
  
        const DECK_PRINCIPALS = [  
            { id: "p1", type: "PRINCIPAL", title: "Staff Architect", desc: "Instantly upgrade all deployed builds by +1 Tier.", run: (p) => { p.builds.forEach(b => b.tier++); } },  
            { id: "p2", type: "PRINCIPAL", title: "VP of Cloud", desc: "Upgrade your Cluster Infrastructure for free.", run: (p) => { if (p.clusterTier < 3) p.clusterTier++; } },  
            { id: "p3", type: "PRINCIPAL", title: "Lead DevOps", desc: "Instantly compile all memory code into live builds.", run: (p) => {  
                while(p.buffer.length) {  
                    const f = p.buffer.pop();  
                    p.builds.push({ name: `${f.name} Release`, type: f.type, tier: f.val });  
                }  
            }}  
        ];  
  
        // 7-TIER SPRING SPRINT SCHEDULE  
        const SPRING_SLOTS = [  
            { pos: 1, label: "1: First Turn (No Bonus)", bonus: (p) => {} },  
            { pos: 2, label: "2: +1 Code Card", bonus: (p) => { drawCard('MODULE'); } },  
            { pos: 3, label: "3: +1 Client Deal", bonus: (p) => { drawCard('SLA'); } },  
            { pos: 4, label: "4: +$1 Cash Grant", bonus: (p) => { p.capital += 1; } },  
            { pos: 5, label: "5: +1 Advisor Card", bonus: (p) => { drawCard('ADVISOR'); } },  
            { pos: 6, label: "6: +1 Revenue (ARR)", bonus: (p) => { p.arr += 1; } },  
            { pos: 7, label: "7: +1 Contractor", bonus: (p) => { p.workers.push({ id: 88, type: 'JUNIOR', available: true }); } }  
        ];  
  
        function shuffle(arr) {  
            const copy = JSON.parse(JSON.stringify(arr));  
            for (let i = copy.length - 1; i > 0; i--) {  
                const j = Math.floor(Math.random() * (i + 1));  
                [copy[i], copy[j]] = [copy[j], copy[i]];  
            }  
            return copy;  
        }  
  
        // GLOBAL GAME STATE  
        let G = null;  
  
        function initGame() {  
            G = {  
                year: 1,  
                season: "SPRING", // SPRING, SUMMER, WINTER, HARDEN  
                activePlayer: "HUMAN", // HUMAN or AI  
                decks: {  
                    MODULE: shuffle(DECK_MODULES),  
                    SLA: shuffle(DECK_SLAS),  
                    ADVISOR: shuffle(DECK_ADVISORS),  
                    PRINCIPAL: shuffle(DECK_PRINCIPALS)  
                },  
                human: {  
                    arr: 0,  
                    capital: 4,  
                    residual: 0,  
                    clusterTier: 1, // 1: T3 max, 2: T6 max, 3: T9 max  
                    springPos: null,  
                    passedSummer: false,  
                    passedWinter: false,  
                    workers: [  
                        { id: 1, type: "JUNIOR", available: true },  
                        { id: 2, type: "JUNIOR", available: true },  
                        { id: 3, type: "ARCHITECT", available: true } // Grande Worker  
                    ],  
                    repos: [  
                        { name: "Repo 1", module: null },  
                        { name: "Repo 2", module: null },  
                        { name: "Repo 3", module: null }  
                    ],  
                    buffer: [],  
                    builds: [],  
                    hand: []  
                },  
                ai: {  
                    arr: 0,  
                    capital: 4,  
                    residual: 0,  
                    springPos: null,  
                    passedSummer: false,  
                    passedWinter: false,  
                    workers: 3, // Abstracted pool  
                    hasLead: true  
                },  
                boardSlots: {  
                    commit: null, // null, "HUMAN", "AI", or array for Grande  
                    fund: null,  
                    advisor: null,  
                    extract: null,  
                    compile: null,  
                    sla: null,  
                    principal: null  
                }  
            };  
  
            // Deal initial hand (1 of each card type)  
            drawCard('MODULE');  
            drawCard('SLA');  
            drawCard('ADVISOR');  
            drawCard('PRINCIPAL');  
  
            startSpringPhase();  
            render();  
        }  
  
        function drawCard(type) {  
            const deck = G.decks[type];  
            if (!deck || deck.length === 0) return;  
            const card = deck.pop();  
            G.human.hand.push(card);  
        }  
  
        // =========================================================  
        // SPRING PHASE (TURN ORDER & BONUSES)  
        // =========================================================  
        function startSpringPhase() {  
            G.season = "SPRING";  
            G.human.springPos = null;  
            G.ai.springPos = null;  
            G.human.passedSummer = false;  
            G.human.passedWinter = false;  
            G.ai.passedSummer = false;  
            G.ai.passedWinter = false;  
  
            // Reset board slots  
            Object.keys(G.boardSlots).forEach(k => G.boardSlots[k] = null);  
  
            // Determine who picks first: player with lower ARR picks first  
            if (G.year > 1 && G.ai.arr < G.human.arr) {  
                // AI picks first  
                aiChooseSpring();  
                setBanner("Spring Schedule: Competitor selected slot " + G.ai.springPos + ". Now click your time slot (1-7) below.");  
            } else {  
                setBanner("Spring Schedule: Click a time slot (1 to 7) below to choose your turn order & bonus.");  
            }  
            render();  
        }  
  
        function selectSpring(pos) {  
            if (G.season !== 'SPRING') return;  
            if (G.ai.springPos === pos) {  
                alert("That schedule slot is already taken by your rival!");  
                return;  
            }  
  
            G.human.springPos = pos;  
            const item = SPRING_SLOTS.find(s => s.pos === pos);  
            item.bonus(G.human);  
  
            if (!G.ai.springPos) {  
                aiChooseSpring();  
            }  
  
            // Determine Summer first turn  
            G.activePlayer = G.human.springPos < G.ai.springPos ? "HUMAN" : "AI";  
            startSummerPhase();  
        }  
  
        function aiChooseSpring() {  
            const free = [1,2,3,4,5,6,7].filter(p => p !== G.human.springPos);  
            // AI prefers slots 3 (Deals), 4 ($), or 6 (ARR)  
            const pick = free[Math.floor(Math.random() * Math.min(3, free.length))];  
            G.ai.springPos = pick;  
            if (pick === 4) G.ai.capital += 1;  
            if (pick === 6) G.ai.arr += 1;  
        }  
  
        // =========================================================  
        // SUMMER & WINTER WORKER PLACEMENT LOOPS  
        // =========================================================  
        function startSummerPhase() {  
            G.season = "SUMMER";  
            stepLoop();  
        }  
  
        function startWinterPhase() {  
            G.season = "WINTER";  
            // Determine who goes first in winter  
            G.activePlayer = G.human.springPos < G.ai.springPos ? "HUMAN" : "AI";  
            stepLoop();  
        }  
  
        function stepLoop() {  
            render();  
  
            // Check if season is complete  
            if (G.season === 'SUMMER') {  
                if (G.human.passedSummer && G.ai.passedSummer) {  
                    startWinterPhase();  
                    return;  
                }  
            } else if (G.season === 'WINTER') {  
                if (G.human.passedWinter && G.ai.passedWinter) {  
                    endOfYearHardening();  
                    return;  
                }  
            }  
  
            // Update banner  
            if (G.activePlayer === "HUMAN") {  
                const seasonName = G.season;  
                const hasPassed = (seasonName === 'SUMMER' && G.human.passedSummer) || (seasonName === 'WINTER' && G.human.passedWinter);  
                  
                if (hasPassed) {  
                    G.activePlayer = "AI";  
                    stepLoop();  
                    return;  
                }  
  
                setBanner(`YOUR TURN (${seasonName}): Click an open action circle on the board, or click 'Pass' to save staff.`);  
                document.getElementById('turn-actions').innerHTML = `  
                    <button onclick="passSeason()" class="bg-amber-500/20 text-amber-300 hover:bg-amber-500/30 border border-amber-500/40 text-xs px-3 py-1 rounded transition">Pass ${seasonName} ➔</button>  
                `;  
            } else {  
                setBanner(`COMPETITOR'S TURN (${G.season}): Thinking...`);  
                document.getElementById('turn-actions').innerHTML = "";  
                setTimeout(runAITurn, 800);  
            }  
        }  
  
        function passSeason() {  
            if (G.season === 'SUMMER') G.human.passedSummer = true;  
            if (G.season === 'WINTER') G.human.passedWinter = true;  
            G.activePlayer = "AI";  
            stepLoop();  
        }  
  
        // =========================================================  
        // PLAYER BOARD SLOT CLICK HANDLER  
        // =========================================================  
        function onBoardSlotClick(actionKey) {  
            if (G.activePlayer !== "HUMAN") return;  
              
            const isSummer = ['COMMIT', 'FUND', 'ADVISOR'].includes(actionKey);  
            const isWinter = ['EXTRACT', 'COMPILE', 'SLA', 'PRINCIPAL'].includes(actionKey);  
  
            if (isSummer && G.season !== 'SUMMER') return alert("That action space is only active during Summer!");  
            if (isWinter && G.season !== 'WINTER') return alert("That action space is only active during Winter!");  
  
            const slotId = actionKey.toLowerCase();  
            const occupant = G.boardSlots[slotId];  
  
            // Determine which worker to use  
            let workerToUse = null;  
            if (occupant) {  
                // Slot blocked! Check if Lead Architect is available  
                workerToUse = G.human.workers.find(w => w.available && w.type === 'ARCHITECT');  
                if (!workerToUse) {  
                    alert("That space is blocked by your rival! You need an available Lead Architect to share it.");  
                    return;  
                }  
            } else {  
                workerToUse = G.human.workers.find(w => w.available);  
                if (!workerToUse) {  
                    alert("All your workers have been assigned! Click 'Pass' to proceed.");  
                    return;  
                }  
            }  
  
            // Execute the action (with interactive pickers where needed)  
            if (actionKey === 'COMMIT') {  
                const modules = G.human.hand.filter(c => c.type === 'MODULE');  
                const emptyRepos = G.human.repos.filter(r => !r.module);  
                if (modules.length === 0) return alert("You don't have any Code cards in hand to write!");  
                if (emptyRepos.length === 0) return alert("All your project repositories are full! Extract them in Winter first.");  
  
                openPicker("COMMIT CODE MODULE", "Select a code module to write into an open repository folder:", modules, (selectedCard) => {  
                    // Place in first empty repo  
                    emptyRepos[0].module = selectedCard;  
                    G.human.hand.splice(G.human.hand.indexOf(selectedCard), 1);  
                    completeWorkerPlacement(slotId, workerToUse);  
                });  
            }   
            else if (actionKey === 'FUND') {  
                G.human.capital += 2;  
                completeWorkerPlacement(slotId, workerToUse);  
            }  
            else if (actionKey === 'ADVISOR') {  
                const advisors = G.human.hand.filter(c => c.type === 'ADVISOR');  
                if (advisors.length === 0) return alert("You don't have any yellow Advisor cards in hand!");  
  
                openPicker("MEET BUSINESS ADVISOR", "Select an advisor card to consult with:", advisors, (selectedCard) => {  
                    selectedCard.run(G.human);  
                    G.human.hand.splice(G.human.hand.indexOf(selectedCard), 1);  
                    completeWorkerPlacement(slotId, workerToUse);  
                });  
            }  
            else if (actionKey === 'EXTRACT') {  
                let count = 0;  
                G.human.repos.forEach(r => {  
                    if (r.module) {  
                        G.human.buffer.push({ name: r.module.name, type: r.module.sub, val: r.module.val });  
                        r.module = null;  
                        count++;  
                    }  
                });  
                if (count === 0) return alert("No committed code in your repositories to extract!");  
                completeWorkerPlacement(slotId, workerToUse);  
            }  
            else if (actionKey === 'COMPILE') {  
                if (G.human.buffer.length === 0) return alert("Memory cache is empty! Extract code from repositories first.");  
                const frag = G.human.buffer.pop();  
                G.human.builds.push({ name: `${frag.name} Build`, type: frag.type, tier: frag.val });  
                completeWorkerPlacement(slotId, workerToUse);  
            }  
            else if (actionKey === 'SLA') {  
                const slas = G.human.hand.filter(c => c.type === 'SLA');  
                if (slas.length === 0) return alert("You don't have any purple Client Deal cards in hand!");  
  
                // Find qualifying SLAs  
                const eligible = slas.filter(sla => {  
                    return G.human.builds.some(b => b.tier >= sla.minTier && (b.type === sla.reqType || sla.reqType === 'FULLSTACK'));  
                });  
  
                if (eligible.length === 0) {  
                    return alert("None of your live builds currently meet the requirements of your client deals!");  
                }  
  
                openPicker("DELIVER CLIENT CONTRACT", "Select a deal to fulfill using your matching server build:", eligible, (selectedSla) => {  
                    const matchIdx = G.human.builds.findIndex(b => b.tier >= selectedSla.minTier && (b.type === selectedSla.reqType || selectedSla.reqType === 'FULLSTACK'));  
                    G.human.builds.splice(matchIdx, 1);  
                    G.human.hand.splice(G.human.hand.indexOf(selectedSla), 1);  
                    G.human.arr += selectedSla.arr;  
                    G.human.residual += selectedSla.residual;  
                    completeWorkerPlacement(slotId, workerToUse);  
                });  
            }  
            else if (actionKey === 'PRINCIPAL') {  
                const principals = G.human.hand.filter(c => c.type === 'PRINCIPAL');  
                if (principals.length === 0) return alert("You don't have any blue Staff Engineer cards in hand!");  
  
                openPicker("CONSULT LEAD PRINCIPAL", "Select a principal engineer to deploy:", principals, (selectedCard) => {  
                    selectedCard.run(G.human);  
                    G.human.hand.splice(G.human.hand.indexOf(selectedCard), 1);  
                    completeWorkerPlacement(slotId, workerToUse);  
                });  
            }  
        }  
  
        function completeWorkerPlacement(slotId, worker) {  
            worker.available = false;  
            // Record occupant  
            if (!G.boardSlots[slotId]) {  
                G.boardSlots[slotId] = "HUMAN";  
            } else {  
                G.boardSlots[slotId] = "SHARED";  
            }  
            closePicker();  
            G.activePlayer = "AI";  
            stepLoop();  
        }  
  
        // =========================================================  
        // AI OPPONENT LOGIC (COMPETITIVE BLOCKING)  
        // =========================================================  
        function runAITurn() {  
            const season = G.season;  
            if (season === 'SUMMER') {  
                if (G.ai.workers <= 0 || Math.random() > 0.8) {  
                    G.ai.passedSummer = true;  
                    document.getElementById('ai-status-text').textContent = "Passed for Summer.";  
                } else {  
                    // Try to place worker  
                    let target = null;  
                    if (!G.boardSlots.commit) target = "commit";  
                    else if (!G.boardSlots.fund) target = "fund";  
                      
                    if (target) {  
                        G.boardSlots[target] = "AI";  
                        G.ai.workers--;  
                        if (target === 'fund') G.ai.capital += 2;  
                        document.getElementById('ai-status-text').textContent = `Assigned worker to ${target.toUpperCase()} (Blocked).`;  
                    } else {  
                        G.ai.passedSummer = true;  
                    }  
                }  
            } else if (season === 'WINTER') {  
                if (G.ai.workers <= 0 || Math.random() > 0.8) {  
                    G.ai.passedWinter = true;  
                    document.getElementById('ai-status-text').textContent = "Passed for Winter.";  
                } else {  
                    let target = null;  
                    if (!G.boardSlots.sla && Math.random() > 0.4) {  
                        target = "sla";  
                        G.ai.arr += 2;  
                    } else if (!G.boardSlots.compile) {  
                        target = "compile";  
                    }  
  
                    if (target) {  
                        G.boardSlots[target] = "AI";  
                        G.ai.workers--;  
                        document.getElementById('ai-status-text').textContent = `Assigned worker to ${target.toUpperCase()} (Blocked).`;  
                    } else {  
                        G.ai.passedWinter = true;  
                    }  
                }  
            }  
  
            G.activePlayer = "HUMAN";  
            stepLoop();  
        }  
  
        // =========================================================  
        // END OF YEAR AGING & HARVEST  
        // =========================================================  
        function endOfYearHardening() {  
            G.season = "HARDEN";  
            setBanner("END OF YEAR: Automated tests run! Live builds increase +1 Tier. Payouts distributed.");  
  
            // Build aging  
            const maxTier = G.human.clusterTier === 3 ? 9 : (G.human.clusterTier === 2 ? 6 : 3);  
            G.human.builds.forEach(b => {  
                if (b.tier < maxTier) b.tier++;  
            });  
  
            // Residual revenue payouts  
            G.human.capital += G.human.residual;  
            G.ai.capital += G.ai.residual;  
  
            // Retrieve all workers  
            G.human.workers.forEach(w => w.available = true);  
            G.ai.workers = 3;  
  
            // Check Game End (20 ARR)  
            if (G.human.arr >= 20 || G.ai.arr >= 20 || G.year >= 7) {  
                const won = G.human.arr >= G.ai.arr;  
                setTimeout(() => {  
                    alert(`GAME OVER!\nFinal ARR — You: ${G.human.arr} | Competitor: ${G.ai.arr}\n\n${won ? 'You won the software market!' : 'The competitor scaled faster.'}`);  
                    initGame();  
                }, 500);  
                return;  
            }  
  
            G.year++;  
            setTimeout(startSpringPhase, 1800);  
            render();  
        }  
  
        function upgradeCluster() {  
            if (G.human.capital < 4) return alert("You need $4 cash to upgrade your servers.");  
            if (G.human.clusterTier >= 3) return alert("Your cluster is already at maximum Enterprise scale!");  
            G.human.capital -= 4;  
            G.human.clusterTier++;  
            render();  
        }  
  
        // =========================================================  
        // MODAL PICKER CONTROLS  
        // =========================================================  
        function openPicker(title, sub, cards, onSelectCallback) {  
            const modal = document.getElementById('modal-picker');  
            document.getElementById('picker-title').textContent = title;  
            const body = document.getElementById('picker-body');  
            body.innerHTML = `  
                <p class="text-slate-400 mb-2">${sub}</p>  
                <div class="space-y-2">  
                    ${cards.map((c, i) => `  
                        <div onclick="selectPickerCard(${i})" class="bg-slate-950 p-3 rounded-xl border border-slate-800 hover:border-cyan-500 cursor-pointer transition flex justify-between items-center">  
                            <div>  
                                <strong class="text-slate-200 text-xs block">${c.name || c.title}</strong>  
                                <span class="text-[10px] text-slate-400">${c.desc || (c.sub + ' • Level ' + c.val) || ('Req: ' + c.reqType + ' Tier ' + c.minTier)}</span>  
                            </div>  
                            <button class="bg-cyan-500/20 text-cyan-400 text-[10px] px-2.5 py-1 rounded border border-cyan-500/30">Select</button>  
                        </div>  
                    `).join('')}  
                </div>  
            `;  
            window._pickerCards = cards;  
            window._pickerCallback = onSelectCallback;  
            modal.classList.remove('hidden');  
        }  
  
        function selectPickerCard(idx) {  
            if (window._pickerCallback && window._pickerCards) {  
                window._pickerCallback(window._pickerCards[idx]);  
            }  
        }  
  
        function closePicker() {  
            document.getElementById('modal-picker').classList.add('hidden');  
        }  
  
        function setBanner(msg) {  
            document.getElementById('turn-msg').textContent = msg;  
        }  
  
        // =========================================================  
        // UI RENDER LOOP  
        // =========================================================  
        function render() {  
            if (!G) return;  
  
            // Header Telemetry  
            document.getElementById('val-year').textContent = G.year;  
            document.getElementById('val-season').textContent = G.season;  
  
            // Player Stats  
            document.getElementById('val-player-arr').textContent = G.human.arr;  
            document.getElementById('val-player-cap').textContent = `$${G.human.capital}`;  
            document.getElementById('val-player-res').textContent = `$${G.human.residual}`;  
            document.getElementById('label-your-order').textContent = `Sprint Pos: ${G.human.springPos || '-'}`;  
  
            // AI Stats  
            document.getElementById('val-ai-arr').textContent = `${G.ai.arr} ARR`;  
            document.getElementById('val-ai-cap').textContent = `$${G.ai.capital}`;  
            document.getElementById('val-ai-workers').textContent = `${G.ai.workers} / 3`;  
  
            // Worker Pool Render  
            const availWorkers = G.human.workers.filter(w => w.available).length;  
            document.getElementById('label-workers-avail').textContent = `${availWorkers} Available`;  
            document.getElementById('pool-workers').innerHTML = G.human.workers.map(w => `  
                <div class="px-2.5 py-1 rounded-lg text-xs font-bold border flex items-center space-x-1.5 ${w.available ? (w.type === 'ARCHITECT' ? 'bg-amber-950/80 text-amber-300 border-amber-500 pawn-lead' : 'bg-cyan-950/80 text-cyan-300 border-cyan-500') : 'bg-slate-900 text-slate-600 border-slate-800 line-through opacity-40'}">  
                    <span class="h-2 w-2 rounded-full ${w.type === 'ARCHITECT' ? 'bg-amber-400' : 'bg-cyan-400'}"></span>  
                    <span>${w.type === 'ARCHITECT' ? 'Lead Arch' : 'Junior Dev'}</span>  
                </div>  
            `).join('');  
  
            // Spring Track Render  
            document.getElementById('track-spring').innerHTML = SPRING_SLOTS.map(s => {  
                const isHuman = G.human.springPos === s.pos;  
                const isAI = G.ai.springPos === s.pos;  
                let ring = "border-slate-800 hover:border-slate-600";  
                let tag = "";  
                if (isHuman) { ring = "border-cyan-500 bg-cyan-950/40 text-cyan-300"; tag = "YOU"; }  
                if (isAI) { ring = "border-purple-500 bg-purple-950/40 text-purple-300"; tag = "AI"; }  
  
                return `  
                    <div onclick="selectSpring(${s.pos})" class="p-2 rounded-xl border ${ring} bg-slate-950 cursor-pointer flex flex-col justify-between h-24 transition">  
                        <div class="font-bold text-xs text-slate-200">${s.pos}</div>  
                        <div class="text-[9px] text-slate-400 leading-tight">${s.label.split(': ')[1]}</div>  
                        <div class="text-[8px] font-bold text-cyan-400">${tag}</div>  
                    </div>  
                `;  
            }).join('');  
  
            // Board Pawns  
            const slots = ['commit', 'fund', 'advisor', 'extract', 'compile', 'sla', 'principal'];  
            slots.forEach(s => {  
                const el = document.getElementById(`pawn-${s}`);  
                const occ = G.boardSlots[s];  
                if (el) {  
                    if (occ === 'HUMAN') {  
                        el.className = "h-7 w-7 rounded-full pawn-human flex items-center justify-center text-[9px] font-bold text-slate-950";  
                        el.textContent = "YOU";  
                    } else if (occ === 'AI') {  
                        el.className = "h-7 w-7 rounded-full pawn-ai flex items-center justify-center text-[9px] font-bold text-white";  
                        el.textContent = "AI";  
                    } else if (occ === 'SHARED') {  
                        el.className = "h-7 w-7 rounded-full pawn-human pawn-lead flex items-center justify-center text-[8px] font-bold text-slate-950";  
                        el.textContent = "BOTH";  
                    } else {  
                        el.className = "h-7 w-7 rounded-full border border-dashed border-slate-700 flex items-center justify-center text-[10px]";  
                        el.textContent = "";  
                    }  
                }  
            });  
  
            // Repos  
            document.getElementById('container-repos').innerHTML = G.human.repos.map(r => `  
                <div class="bg-slate-950 p-2 rounded-xl border border-slate-800 text-center">  
                    <span class="text-slate-500 text-[9px] block">${r.name}</span>  
                    <strong class="${r.module ? 'text-emerald-400 text-xs' : 'text-slate-600 text-xs italic'}">  
                        ${r.module ? r.module.name : 'Empty'}  
                    </strong>  
                </div>  
            `).join('');  
  
            // Buffer  
            document.getElementById('container-buffer').innerHTML = G.human.buffer.length ? G.human.buffer.map(b => `  
                <span class="bg-slate-900 border border-slate-800 text-cyan-400 px-2 py-0.5 rounded text-[10px]">${b.name} (T${b.val})</span>  
            `).join('') : '<span class="text-slate-600 text-[10px] italic">Cache Empty</span>';  
  
            // Builds  
            const tierMax = G.human.clusterTier === 3 ? 9 : (G.human.clusterTier === 2 ? 6 : 3);  
            document.getElementById('label-cluster-tier').textContent = `Tier ${tierMax} Max`;  
            document.getElementById('container-builds').innerHTML = G.human.builds.length ? G.human.builds.map(b => `  
                <div class="flex justify-between bg-slate-900 p-1.5 rounded border border-slate-800 text-[10px]">  
                    <span class="text-slate-300 truncate mr-2">${b.name}</span>  
                    <span class="text-emerald-400 font-bold">Tier ${b.tier}</span>  
                </div>  
            `).join('') : '<span class="text-slate-600 text-[10px] italic">No active builds</span>';  
  
            // Hand  
            document.getElementById('count-hand').textContent = G.human.hand.length;  
            document.getElementById('container-hand').innerHTML = G.human.hand.map(c => {  
                let border = "border-slate-800";  
                let tagClass = "text-slate-400";  
                if (c.type === 'MODULE') { border = "border-emerald-900/60"; tagClass = "text-emerald-400"; }  
                if (c.type === 'SLA') { border = "border-purple-900/60"; tagClass = "text-purple-400"; }  
                if (c.type === 'ADVISOR') { border = "border-amber-900/60"; tagClass = "text-amber-400"; }  
                if (c.type === 'PRINCIPAL') { border = "border-blue-900/60"; tagClass = "text-blue-400"; }  
  
                return `  
                    <div class="bg-slate-950 p-2.5 rounded-xl border ${border} text-xs space-y-1">  
                        <div class="flex justify-between text-[9px]">  
                            <span class="${tagClass} font-bold">${c.type}</span>  
                            <span class="text-slate-500">${c.sub || ''}</span>  
                        </div>  
                        <div class="font-bold text-slate-200 text-xs truncate">${c.name || c.title}</div>  
                    </div>  
                `;  
            }).join('');  
        }  
  
        window.onload = initGame;  
    </script>  
</body>  
</html>  
