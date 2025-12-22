<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>4-7-8 呼吸冥想</title>
    <style>
        :root {
            /* 核心色彩定義 - 更深邃、寧靜的色盤 */
            --bg-gradient: radial-gradient(circle at center, #2a2d3e 0%, #13151a 100%);
            --text-color: #e0e0e0;
            --text-muted: #888aa0;
            
            /* 呼吸環色彩 */
            --circle-outer-border: rgba(255, 255, 255, 0.08);
            --circle-outer-glow: 0 0 30px rgba(79, 172, 254, 0.2);
            --circle-inner-bg: radial-gradient(circle, rgba(0, 242, 96, 0.9) 0%, rgba(5, 117, 230, 0.7) 90%);
            --circle-inner-glow: 0 0 50px rgba(5, 117, 230, 0.5);

            /* UI 元素色彩 */
            --accent-gradient: linear-gradient(135deg, #4facfe 0%, #00f260 100%);
            --button-shadow: 0 10px 20px -10px rgba(79, 172, 254, 0.5);
            --panel-bg: rgba(40, 44, 52, 0.85); /* 半透明背景 */
            --panel-border: 1px solid rgba(255, 255, 255, 0.1);
        }

        body {
            margin: 0;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: var(--bg-gradient);
            color: var(--text-color);
            /* 使用更現代的系統字體堆疊 */
            font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
            overflow: hidden;
            letter-spacing: 0.5px;
        }

        /* 主容器 */
        .container {
            text-align: center;
            position: relative;
            width: 100%;
            max-width: 500px;
            padding: 20px;
            box-sizing: border-box;
        }

        /* --- 呼吸圓圈核心區域 --- */
        .breathing-circle-wrapper {
            position: relative;
            width: 320px; /* 稍微加大 */
            height: 320px;
            margin: 0 auto 40px auto; /* 增加底部間距 */
            display: flex;
            justify-content: center;
            align-items: center;
        }

        /* 外圈 (固定裝飾) */
        .outer-circle {
            position: absolute;
            width: 100%;
            height: 100%;
            border-radius: 50%;
            border: 2px solid var(--circle-outer-border);
            box-shadow: var(--circle-outer-glow), inset 0 0 20px rgba(0,0,0,0.2);
            z-index: 1;
        }

        /* 內圈 (動畫主體) */
        .inner-circle {
            position: absolute;
            width: 92%; /* 稍微留白邊 */
            height: 92%;
            background: var(--circle-inner-bg);
            border-radius: 50%;
            transform: scale(0); 
            opacity: 0.95;
            z-index: 2;
            will-change: transform;
            box-shadow: var(--circle-inner-glow);
            /* 關鍵：使用 ease-in-out 讓呼吸感更自然 */
            transition-timing-function: ease-in-out !important; 
        }

        /* 文字提示 */
        .status-text {
            position: absolute;
            z-index: 3;
            font-size: 2.2rem;
            font-weight: 600;
            letter-spacing: 2px;
            text-shadow: 0 2px 10px rgba(0,0,0,0.5);
            pointer-events: none;
        }
        
        /* 計時器大數字 */
        .timer-display {
            font-size: 6rem;
            font-weight: 200; /* 輕量字重更有質感 */
            margin-bottom: 30px;
            font-variant-numeric: tabular-nums;
            text-shadow: 0 0 20px rgba(255,255,255,0.1);
        }

        /* --- 控制按鈕區域 --- */
        .controls {
            display: flex;
            gap: 20px;
            justify-content: center;
            margin-top: 20px;
        }

        button {
            background: var(--accent-gradient);
            border: none;
            padding: 14px 32px; /* 加大按鈕 */
            color: white;
            font-size: 1.1rem;
            font-weight: 600;
            border-radius: 16px; /* 更圓潤的角 */
            cursor: pointer;
            transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
            outline: none;
            box-shadow: var(--button-shadow);
            letter-spacing: 1px;
        }

        button:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 30px -10px rgba(79, 172, 254, 0.7);
        }
        
        button:active {
            transform: translateY(-1px) scale(0.98);
        }

        /* 次要按鈕樣式 */
        button.secondary {
            background: rgba(255, 255, 255, 0.05);
            box-shadow: none;
            border: 1px solid rgba(255, 255, 255, 0.1);
            color: var(--text-color);
        }
        button.secondary:hover {
            background: rgba(255, 255, 255, 0.1);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        button:disabled {
            opacity: 0.4;
            cursor: not-allowed;
            transform: none !important;
            box-shadow: none !important;
        }

        /* --- 設定面板 (毛玻璃效果) --- */
        .settings-panel {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%) scale(0.9);
            
            /* 毛玻璃核心樣式 */
            background-color: var(--panel-bg);
            backdrop-filter: blur(20px); /* 模糊背景 */
            -webkit-backdrop-filter: blur(20px); /* Safari 支援 */
            border: var(--panel-border);
            
            padding: 40px;
            border-radius: 24px;
            box-shadow: 0 20px 50px rgba(0,0,0,0.5);
            z-index: 10;
            width: 85%;
            max-width: 340px;
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.4s cubic-bezier(0.25, 0.8, 0.25, 1), transform 0.4s cubic-bezier(0.25, 0.8, 0.25, 1);
        }

        .settings-panel.active {
            opacity: 1;
            pointer-events: auto;
            transform: translate(-50%, -50%) scale(1);
        }

        .settings-panel h2 {
            margin-top: 0;
            margin-bottom: 30px;
            text-align: center;
            font-weight: 400;
            letter-spacing: 1px;
        }

        .form-group {
            margin-bottom: 20px;
            text-align: left;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-size: 0.95rem;
            color: var(--text-muted);
            font-weight: 500;
        }

        .form-group input {
            width: 100%;
            padding: 12px 16px;
            border-radius: 12px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            background: rgba(0, 0, 0, 0.2);
            color: white;
            font-size: 1.1rem;
            box-sizing: border-box;
            transition: border-color 0.3s, box-shadow 0.3s;
            outline: none;
        }
        
        .form-group input:focus {
            border-color: #4facfe;
            box-shadow: 0 0 0 3px rgba(79, 172, 254, 0.2);
        }

        .overlay {
            position: fixed;
            top: 0; left: 0; right: 0; bottom: 0;
            background: rgba(0,0,0,0.6);
            backdrop-filter: blur(5px);
            z-index: 9;
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.4s ease;
        }
        .overlay.active {
            opacity: 1;
            pointer-events: auto;
        }

        /* 進度指示 */
        .cycle-info {
            margin-top: 25px;
            font-size: 1rem;
            color: var(--text-muted);
            font-weight: 500;
            letter-spacing: 1px;
        }

    </style>
</head>
<body>

    <div class="container">
        <div class="breathing-circle-wrapper">
            <div class="outer-circle"></div>
            <div class="inner-circle" id="innerCircle"></div>
            <div class="status-text" id="statusText">準備</div>
        </div>

        <div class="timer-display" id="timerDisplay">0</div>

        <div class="controls">
            <button id="btnStart">開始</button>
            <button id="btnSettings" class="secondary">設定</button>
        </div>
        
        <div class="cycle-info" id="cycleInfo">循環: 0 / 6</div>
    </div>

    <div class="overlay" id="overlay"></div>
    <div class="settings-panel" id="settingsPanel">
        <h2>參數設定</h2>
        <div class="form-group">
            <label>吸氣</label>
            <input type="number" id="inputP1" value="4" min="1">
        </div>
        <div class="form-group">
            <label>屏氣</label>
            <input type="number" id="inputP2" value="7" min="1">
        </div>
        <div class="form-group">
            <label>吐氣</label>
            <input type="number" id="inputP3" value="8" min="1">
        </div>
        <div class="form-group">
            <label>循環次數</label>
            <input type="number" id="inputCycles" value="6" min="1">
        </div>
        <div class="controls" style="margin-top: 30px;">
            <button id="btnSave" style="width: 100%;">儲存並關閉</button>
        </div>
    </div>

    <script>
        // 音效控制器 (Web Audio API) - 保持不變
        class AudioController {
            constructor() {
                this.ctx = null;
            }

            init() {
                if (!this.ctx) {
                    this.ctx = new (window.AudioContext || window.webkitAudioContext)();
                }
                if (this.ctx.state === 'suspended') {
                    this.ctx.resume();
                }
            }

            // 叮聲
            playDing() {
                if (!this.ctx) return;
                const osc = this.ctx.createOscillator();
                const gain = this.ctx.createGain();
                
                osc.type = 'sine';
                osc.frequency.setValueAtTime(880, this.ctx.currentTime); // A5
                osc.frequency.exponentialRampToValueAtTime(0.01, this.ctx.currentTime + 1.5);

                gain.gain.setValueAtTime(0.3, this.ctx.currentTime);
                gain.gain.exponentialRampToValueAtTime(0.001, this.ctx.currentTime + 1.2);

                osc.connect(gain);
                gain.connect(this.ctx.destination);
                osc.start();
                osc.stop(this.ctx.currentTime + 1.5);
            }

            // 鼓聲
            playDrum() {
                if (!this.ctx) return;
                const osc = this.ctx.createOscillator();
                const gain = this.ctx.createGain();

                osc.type = 'triangle';
                osc.frequency.setValueAtTime(100, this.ctx.currentTime);
                osc.frequency.exponentialRampToValueAtTime(30, this.ctx.currentTime + 0.5);

                gain.gain.setValueAtTime(0.6, this.ctx.currentTime);
                gain.gain.exponentialRampToValueAtTime(0.001, this.ctx.currentTime + 0.5);

                osc.connect(gain);
                gain.connect(this.ctx.destination);
                osc.start();
                osc.stop(this.ctx.currentTime + 0.5);
            }

            // 喀喀聲
            playClick() {
                if (!this.ctx) return;
                const osc = this.ctx.createOscillator();
                const gain = this.ctx.createGain();

                osc.type = 'square';
                osc.frequency.setValueAtTime(800, this.ctx.currentTime);
                
                // 很短促的聲音
                gain.gain.setValueAtTime(0.2, this.ctx.currentTime);
                gain.gain.exponentialRampToValueAtTime(0.001, this.ctx.currentTime + 0.1);

                osc.connect(gain);
                gain.connect(this.ctx.destination);
                osc.start();
                osc.stop(this.ctx.currentTime + 0.1);
            }
        }

        // 應用程式邏輯
        const audio = new AudioController();
        
        // DOM 元素
        const els = {
            innerCircle: document.getElementById('innerCircle'),
            statusText: document.getElementById('statusText'),
            timerDisplay: document.getElementById('timerDisplay'),
            btnStart: document.getElementById('btnStart'),
            btnSettings: document.getElementById('btnSettings'),
            cycleInfo: document.getElementById('cycleInfo'),
            settingsPanel: document.getElementById('settingsPanel'),
            overlay: document.getElementById('overlay'),
            btnSave: document.getElementById('btnSave'),
            inputs: {
                p1: document.getElementById('inputP1'),
                p2: document.getElementById('inputP2'),
                p3: document.getElementById('inputP3'),
                cycles: document.getElementById('inputCycles'),
            }
        };

        // 狀態變數
        let config = {
            p1: 4, // 秒
            p2: 7,
            p3: 8,
            cycles: 6
        };
        
        let state = {
            isRunning: false,
            currentCycle: 0,
            timer: null,
            animationFrame: null,
            phaseStartTime: 0
        };

        // 初始化
        function init() {
            updateCycleDisplay();
            els.btnStart.addEventListener('click', toggleStart);
            els.btnSettings.addEventListener('click', openSettings);
            els.btnSave.addEventListener('click', saveSettings);
            els.overlay.addEventListener('click', closeSettings); // 點擊背景關閉
        }

        function openSettings() {
            if (state.isRunning) return; // 執行中不可設定
            els.settingsPanel.classList.add('active');
            els.overlay.classList.add('active');
        }

        function closeSettings() {
            els.settingsPanel.classList.remove('active');
            els.overlay.classList.remove('active');
        }

        function saveSettings() {
            config.p1 = parseInt(els.inputs.p1.value) || 4;
            config.p2 = parseInt(els.inputs.p2.value) || 7;
            config.p3 = parseInt(els.inputs.p3.value) || 8;
            config.cycles = parseInt(els.inputs.cycles.value) || 6;
            updateCycleDisplay();
            closeSettings();
        }

        function toggleStart() {
            if (state.isRunning) {
                stopBreathing();
            } else {
                startBreathing();
            }
        }

        function updateCycleDisplay() {
            els.cycleInfo.textContent = `循環: ${state.currentCycle} / ${config.cycles}`;
        }

        function startBreathing() {
            audio.init(); // 啟動音效環境
            state.isRunning = true;
            state.currentCycle = 0;
            els.btnStart.textContent = '停止練習';
            // 停止按鈕樣式調整
            els.btnStart.style.background = 'linear-gradient(135deg, #ff6b6b 0%, #ee5253 100%)';
            els.btnStart.style.boxShadow = '0 10px 20px -10px rgba(255, 107, 107, 0.5)';

            els.btnSettings.disabled = true;
            
            // 重置圓圈
            els.innerCircle.style.transition = 'none';
            els.innerCircle.style.transform = 'scale(0)'; 
            
            // 開始循環
            runCycle();
        }

        function stopBreathing() {
            state.isRunning = false;
            clearTimeout(state.timer);
            cancelAnimationFrame(state.animationFrame);
            
            els.btnStart.textContent = '開始練習';
            els.btnStart.style.background = ''; // 回復預設 CSS
            els.btnStart.style.boxShadow = '';
            els.btnSettings.disabled = false;
            els.statusText.textContent = '準備';
            els.timerDisplay.textContent = '0';
            // 停止時使用柔和的縮小動畫
            els.innerCircle.style.transition = 'transform 0.8s cubic-bezier(0.25, 0.8, 0.25, 1)';
            els.innerCircle.style.transform = 'scale(0)';
        }

        async function runCycle() {
            if (!state.isRunning) return;
            
            state.currentCycle++;
            if (state.currentCycle > config.cycles) {
                stopBreathing();
                els.statusText.textContent = '完成';
                return;
            }
            updateCycleDisplay();

            // 階段一：慢慢變大 (4秒) -> 叮聲
            els.innerCircle.style.transition = 'none';
            els.innerCircle.style.transform = 'scale(0)';
            void els.innerCircle.offsetWidth; // 強制 Reflow

            await runPhase('吸氣', config.p1, 'scale(1)', 'ding');
            if (!state.isRunning) return;

            // 階段二：慢慢縮小 (7秒) -> 鼓聲
            await runPhase('屏氣', config.p2, 'scale(0)', 'drum');
            if (!state.isRunning) return;

            // 階段三：慢慢變大 (8秒) -> 喀喀聲
            await runPhase('吐氣', config.p3, 'scale(1)', 'click');
            if (!state.isRunning) return;

            // 遞迴調用下一輪
            runCycle();
        }

        function runPhase(text, durationSec, cssTransform, soundType) {
            return new Promise(resolve => {
                els.statusText.textContent = text;
                
                // 設定 CSS Transition - **重要修改：使用 ease-in-out**
                // 雖然 CSS 已經設定了預設的 timing-function，但這裡重新指定時間是必要的
                // 為了確保視覺的自然感，我們在 JS 中也明確指定 ease-in-out
                els.innerCircle.style.transition = `transform ${durationSec}s cubic-bezier(0.42, 0, 0.58, 1)`;
                els.innerCircle.style.transform = cssTransform;

                let startTime = Date.now();
                
                // 倒數計時顯示 UI Loop
                function updateTimer() {
                    if (!state.isRunning) return;
                    
                    let elapsed = (Date.now() - startTime) / 1000;
                    let remaining = Math.ceil(durationSec - elapsed);
                    
                    if (remaining < 0) remaining = 0;
                    els.timerDisplay.textContent = remaining;

                    if (elapsed < durationSec) {
                        state.animationFrame = requestAnimationFrame(updateTimer);
                    } else {
                        // 階段結束
                        playSound(soundType);
                        resolve();
                    }
                }
                
                state.animationFrame = requestAnimationFrame(updateTimer);
            });
        }

        function playSound(type) {
            if (!state.isRunning) return;
            switch(type) {
                case 'ding': audio.playDing(); break;
                case 'drum': audio.playDrum(); break;
                case 'click': audio.playClick(); break;
            }
        }

        // 啟動
        init();

    </script>
</body>
</html>
