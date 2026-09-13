<!DOCTYPE html>
<html lang="da">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Theos Træning</title>
    
    <!-- PWA settings til iPhone & Android -->
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="apple-mobile-web-app-title" content="Theos Træning">
    <meta name="theme-color" content="#000000">

    <style>
        :root {
            --bg-color: #000000;
            --card-bg: #181818;
            --accent-color: #ff4757;
            --text-color: #ffffff;
            --text-dim: #a0a0a0;
            --disabled-color: #222222;
            --success-color: #2ed573;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            margin: 0;
            padding: 16px;
            display: flex;
            flex-direction: column;
            align-items: center;
            -webkit-tap-highlight-color: transparent;
        }

        h1 { margin-bottom: 20px; font-size: 26px; text-align: center; font-weight: 800; letter-spacing: 0.5px; }

        .tabs-container {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
            justify-content: center;
            max-width: 500px;
            margin-bottom: 20px;
        }

        .tab-btn {
            background-color: #2c2c2e;
            color: var(--text-color);
            border: none;
            padding: 10px 14px;
            border-radius: 8px;
            cursor: pointer;
            font-weight: 600;
            font-size: 14px;
        }

        .tab-btn.active { background-color: var(--accent-color); }
        .tab-btn.disabled { background-color: var(--disabled-color); color: #555; cursor: not-allowed; opacity: 0.5; }

        .tab-content { display: none; width: 100%; max-width: 450px; }
        .tab-content.active { display: block; }

        .exercise-card {
            background-color: var(--card-bg);
            border: 1px solid #2a2a2a;
            border-radius: 12px;
            padding: 16px;
            margin-bottom: 16px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.5);
        }

        .exercise-title { font-size: 17px; font-weight: bold; margin-bottom: 12px; }

        .media-container {
            width: 100%;
            border-radius: 8px;
            overflow: hidden;
            background-color: #000;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .media-container video, .media-container img { width: 100%; height: auto; border-radius: 8px; }

        .placeholder-box {
            width: 100%;
            padding: 20px 0;
            background-color: #222;
            border: 2px dashed #444;
            border-radius: 8px;
            text-align: center;
            color: var(--text-dim);
            font-weight: 500;
        }

        .upload-btn-wrapper { margin-top: 10px; }
        .upload-btn {
            background-color: #333;
            color: #fff;
            padding: 8px 12px;
            border-radius: 6px;
            font-size: 13px;
            cursor: pointer;
            display: inline-block;
            border: 1px solid #555;
        }
        .file-input { display: none; }

        .log-input-group {
            display: flex;
            gap: 10px;
            margin-top: 12px;
            padding-top: 12px;
            border-top: 1px solid #2a2a2a;
        }

        .log-input-wrapper {
            display: flex;
            flex-direction: column;
            width: 50%;
        }

        .log-input-wrapper label {
            font-size: 11px;
            color: var(--text-dim);
            margin-bottom: 4px;
            text-transform: uppercase;
            font-weight: bold;
        }

        .log-input {
            width: 100%;
            padding: 8px;
            background-color: #2c2c2e;
            border: 1px solid #444;
            border-radius: 6px;
            color: #fff;
            font-size: 14px;
            box-sizing: border-box;
        }

        .timer-wrapper {
            margin-top: 12px;
            padding-top: 12px;
            border-top: 1px solid #2a2a2a;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .timer-controls { display: flex; align-items: center; gap: 6px; }

        .timer-display {
            font-family: monospace;
            font-size: 18px;
            font-weight: bold;
            color: var(--accent-color);
            min-width: 55px;
        }

        .timer-btn {
            color: white;
            border: none;
            padding: 6px 10px;
            border-radius: 6px;
            font-size: 12px;
            font-weight: bold;
            cursor: pointer;
        }

        .btn-start { background-color: #2ed573; }
        .btn-stop { background-color: #ff4757; }

        .run-select {
            background-color: #333;
            color: #fff;
            border: 1px solid #555;
            padding: 5px;
            border-radius: 6px;
        }

        .calendar-container { background-color: var(--card-bg); padding: 16px; border-radius: 12px; border: 1px solid #2a2a2a; }
        .calendar-grid { display: grid; grid-template-columns: repeat(7, 1fr); gap: 4px; text-align: center; margin-top: 10px; }
        .day-name { font-weight: bold; color: var(--text-dim); font-size: 11px; padding-bottom: 4px; }
        
        .day-cell {
            background-color: #2c2c2e;
            padding: 8px 2px;
            border-radius: 6px;
            min-height: 55px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
            font-size: 12px;
            cursor: pointer;
            user-select: none;
        }

        .day-cell.trained { border: 2px solid var(--success-color); background-color: #11261a; }
        .check-mark { color: var(--success-color); font-weight: bold; font-size: 18px; margin-top: 4px; }
        .weight-tag { font-size: 11px; color: var(--accent-color); font-weight: bold; margin-top: 4px; }
        
        .cal-btn {
            background-color: #333;
            border: none;
            color: #fff;
            font-size: 10px;
            padding: 4px 6px;
            border-radius: 4px;
            margin-top: 4px;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <h1>Theos Træning</h1>

    <div class="tabs-container">
        <button class="tab-btn active" onclick="openTab('mandag')">Mandag</button>
        <button class="tab-btn" onclick="openTab('tirsdag')">Tirsdag</button>
        <button class="tab-btn" onclick="openTab('onsdag')">Onsdag</button>
        <button class="tab-btn disabled">Torsdag (Rest)</button>
        <button class="tab-btn" onclick="openTab('fredag')">Fredag</button>
        <button class="tab-btn disabled">Lørdag (Rest)</button>
        <button class="tab-btn" onclick="openTab('sondag')">Søndag</button>
        <button class="tab-btn" onclick="openTab('dage')">Dage</button>
        <button class="tab-btn" onclick="openTab('vaegt')">Vægt</button>
    </div>

    <div id="mandag" class="tab-content active"><div id="list-mandag"></div></div>
    <div id="tirsdag" class="tab-content"><div id="list-tirsdag"></div></div>
    <div id="onsdag" class="tab-content"><div id="list-onsdag"></div></div>
    <div id="fredag" class="tab-content"><div id="list-fredag"></div></div>
    <div id="sondag" class="tab-content"><div id="list-sondag"></div></div>
    
    <div id="dage" class="tab-content">
        <div class="calendar-container">
            <h3 style="margin:0 0 10px 0; font-size: 16px; text-align: center;">Træningsdage (Klik for automatisk ✓)</h3>
            <div class="calendar-grid">
                <div class="day-name">Man</div><div class="day-name">Tir</div><div class="day-name">Ons</div>
                <div class="day-name">Tor</div><div class="day-name">Fre</div><div class="day-name">Lør</div>
                <div class="day-name">Søn</div>
            </div>
            <div class="calendar-grid" id="training-calendar-days"></div>
        </div>
    </div>

    <div id="vaegt" class="tab-content">
        <div class="exercise-card" style="margin-bottom: 20px;">
            <div class="exercise-title">Video</div>
            <div class="placeholder-box">Snart</div>
        </div>

        <div class="calendar-container">
            <h3 style="margin:0 0 10px 0; font-size: 16px; text-align: center;">Vægt Kalender</h3>
            <div class="calendar-grid">
                <div class="day-name">Man</div><div class="day-name">Tir</div><div class="day-name">Ons</div>
                <div class="day-name">Tor</div><div class="day-name">Fre</div><div class="day-name">Lør</div>
                <div class="day-name">Søn</div>
            </div>
            <div class="calendar-grid" id="weight-calendar-days"></div>
        </div>
    </div>

    <script>
        const program = {
            mandag: [
                { id: 'm1', name: 'Pec Deck Fly', upload: false },
                { id: 'm2', name: 'Machine Shoulder Press', upload: false },
                { id: 'm3', name: 'Seated Machine Triceps Dip', upload: false },
                { id: 'm4', name: 'Cable V-Bar Overhead Triceps Extension', upload: false },
                { id: 'm5', name: 'Lateral Raise', upload: false }
            ],
            tirsdag: [
                { id: 't1', name: 'Close Grip Cable Lat Pulldown', upload: false },
                { id: 't2', name: 'Cable Row', upload: false },
                { id: 't3', name: 'Machine Row', upload: false },
                { id: 't4', name: 'Machine Rear Delt Fly', upload: false },
                { id: 't5', name: 'Hammer Curl', upload: false },
                { id: 't6', name: 'Bayesian Curl', upload: false }
            ],
            onsdag: [
                { id: 'o1', name: 'Løb - 2-5 min', upload: false, isRun: true },
                { id: 'o2', name: 'Leg Extension', upload: false },
                { id: 'o3', name: 'Leg Press', upload: false },
                { id: 'o4', name: 'Calf Raise Seated', upload: false },
                { id: 'o5', name: 'Kneeling Cable Crunch', upload: true },
                { id: 'o6', name: 'Loaded Crunch', upload: true },
                { id: 'o7', name: 'Hip Adduction', upload: true },
                { id: 'o8', name: 'Back Extensions', upload: true }
            ],
            fredag: [
                { id: 'f1', name: 'Pec Deck Fly', upload: true },
                { id: 'f2', name: 'Wide Grip Lat Pulldown', upload: true },
                { id: 'f3', name: 'Overhand Grip Cable Row', upload: true },
                { id: 'f4', name: 'Preacher Curl', upload: true },
                { id: 'f5', name: 'Lying Chest Press', upload: true },
                { id: 'f6', name: 'Cable V Bar Pushdown', upload: true },
                { id: 'f7', name: 'Single Arm Tricep Pushdown', upload: true },
                { id: 'f8', name: 'Lateral Raise', upload: true }
            ],
            sondag: [
                { id: 's1', name: 'Løb - 2-5 min', upload: true, isRun: true },
                { id: 's2', name: 'Leg Extensions', upload: true },
                { id: 's3', name: 'Seated Hamstring Curl', upload: true },
                { id: 's4', name: 'Leg Press', upload: true },
                { id: 's5', name: 'Kneeling Cable Crunch', upload: true },
                { id: 's6', name: 'Back Extension', upload: true }
            ]
        };

        function renderProgram() {
            Object.keys(program).forEach(day => {
                const container = document.getElementById(`list-${day}`);
                if (!container) return;

                program[day].forEach((ex) => {
                    const containerId = `media-${ex.id}`;
                    const timerId = `timer-${ex.id}`;

                    const savedKg = localStorage.getItem(`kg-${ex.id}`) || '';
                    const savedReps = localStorage.getItem(`reps-${ex.id}`) || '';

                    let mediaHtml = ex.upload ? 
                        `<div class="placeholder-box">Ingen video valgt</div>` : 
                        `<div class="placeholder-box">Snart</div>`;

                    let uploadHtml = ex.upload ? `
                        <div class="upload-btn-wrapper">
                            <label class="upload-btn">Vælg video/billede
                                <input type="file" class="file-input" accept="video/*,image/*" onchange="loadMedia(event, '${containerId}')">
                            </label>
                        </div>` : '';

                    let timerControls = ex.isRun ? `
                        <select id="select-${timerId}" class="run-select">
                            <option value="120">2 min</option>
                            <option value="180">3 min</option>
                            <option value="240">4 min</option>
                            <option value="300">5 min</option>
                        </select>
                        <button class="timer-btn btn-start" onclick="startCustomTimer('${timerId}')">Start</button>
                        <button class="timer-btn btn-stop" onclick="stopTimer('${timerId}')">Stop</button>
                    ` : `
                        <button class="timer-btn btn-start" onclick="startTimer('${timerId}', 120)">Start</button>
                        <button class="timer-btn btn-stop" onclick="stopTimer('${timerId}')">Stop</button>
                    `;

                    const card = document.createElement('div');
                    card.className = 'exercise-card';
                    card.innerHTML = `
                        <div class="exercise-title">${ex.name}</div>
                        <div class="media-container" id="${containerId}">${mediaHtml}</div>
                        ${uploadHtml}
                        
                        <div class="log-input-group">
                            <div class="log-input-wrapper">
                                <label>Kg</label>
                                <input type="number" class="log-input" placeholder="0" value="${savedKg}" onchange="saveLog('kg-${ex.id}', this.value)">
                            </div>
                            <div class="log-input-wrapper">
                                <label>Reps</label>
                                <input type="number" class="log-input" placeholder="0" value="${savedReps}" onchange="saveLog('reps-${ex.id}', this.value)">
                            </div>
                        </div>

                        <div class="timer-wrapper">
                            <div class="timer-controls">${timerControls}</div>
                            <div class="timer-display" id="${timerId}">02:00</div>
                        </div>
                    `;
                    container.appendChild(card);
                });
            });
        }

        function saveLog(key, value) {
            localStorage.setItem(key, value);
        }

        function openTab(tabName) {
            document.querySelectorAll('.tab-content').forEach(c => c.classList.remove('active'));
            document.querySelectorAll('.tab-btn').forEach(b => b.classList.remove('active'));

            document.getElementById(tabName).classList.add('active');
            event.currentTarget.classList.add('active');

            if (tabName === 'dage') renderTrainingCalendar();
            if (tabName === 'vaegt') renderWeightCalendar();
        }

        function loadMedia(event, containerId) {
            const file = event.target.files[0];
            if (!file) return;

            const container = document.getElementById(containerId);
            container.innerHTML = '';
            const fileURL = URL.createObjectURL(file);

            if (file.type.startsWith('video/')) {
                const video = document.createElement('video');
                video.src = fileURL;
                video.controls = true;
                container.appendChild(video);
            } else {
                const img = document.createElement('img');
                img.src = fileURL;
                container.appendChild(img);
            }
        }

        let activeTimers = {};
        let timerTimeLeft = {};

        function playDingSound() {
            const ctx = new (window.AudioContext || window.webkitAudioContext)();
            const osc = ctx.createOscillator();
            const gain = ctx.createGain();

            osc.type = 'sine';
            osc.frequency.setValueAtTime(880, ctx.currentTime);
            gain.gain.setValueAtTime(1, ctx.currentTime);
            gain.gain.exponentialRampToValueAtTime(0.001, ctx.currentTime + 1.2);

            osc.connect(gain);
            gain.connect(ctx.destination);

            osc.start();
            osc.stop(ctx.currentTime + 1.2);
        }

        function startCustomTimer(timerId) {
            const seconds = parseInt(document.getElementById(`select-${timerId}`).value);
            startTimer(timerId, seconds);
        }

        function startTimer(timerId, durationSeconds) {
            if (activeTimers[timerId]) clearInterval(activeTimers[timerId]);

            timerTimeLeft[timerId] = durationSeconds;
            const display = document.getElementById(timerId);

            updateDisplay(display, timerTimeLeft[timerId]);

            activeTimers[timerId] = setInterval(() => {
                timerTimeLeft[timerId]--;
                updateDisplay(display, timerTimeLeft[timerId]);

                if (timerTimeLeft[timerId] <= 0) {
                    clearInterval(activeTimers[timerId]);
                    playDingSound();
                }
            }, 1000);
        }

        function stopTimer(timerId) {
            if (activeTimers[timerId]) {
                clearInterval(activeTimers[timerId]);
                activeTimers[timerId] = null;
            }
        }

        function updateDisplay(element, seconds) {
            const m = Math.floor(seconds / 60).toString().padStart(2, '0');
            const s = (seconds % 60).toString().padStart(2, '0');
            element.innerText = `${m}:${s}`;
        }

        function renderTrainingCalendar() {
            const grid = document.getElementById('training-calendar-days');
            grid.innerHTML = '';

            const now = new Date();
            const year = now.getFullYear();
            const month = now.getMonth();
            const daysInMonth = new Date(year, month + 1, 0).getDate();

            for (let day = 1; day <= daysInMonth; day++) {
                const dateKey = `train-${year}-${month + 1}-${day}`;
                const isTrained = localStorage.getItem(dateKey) === 'true';

                const cell = document.createElement('div');
                cell.className = `day-cell ${isTrained ? 'trained' : ''}`;
                cell.innerHTML = `<span>${day}</span>${isTrained ? '<span class="check-mark">✓</span>' : ''}`;

                cell.onclick = () => {
                    const newState = !isTrained;
                    localStorage.setItem(dateKey, newState);
                    renderTrainingCalendar();
                };

                grid.appendChild(cell);
            }
        }

        function renderWeightCalendar() {
            const grid = document.getElementById('weight-calendar-days');
            grid.innerHTML = '';

            const now = new Date();
            const year = now.getFullYear();
            const month = now.getMonth();
            const daysInMonth = new Date(year, month + 1, 0).getDate();

            for (let day = 1; day <= daysInMonth; day++) {
                const dateKey = `weight-${year}-${month + 1}-${day}`;
                const savedWeight = localStorage.getItem(dateKey) || '';

                const cell = document.createElement('div');
                cell.className = 'day-cell';
                
                let content = `<span>${day}</span>`;
                if (savedWeight) content += `<span class="weight-tag">${savedWeight} kg</span>`;
                cell.innerHTML = content;

                const btn = document.createElement('button');
                btn.className = 'cal-btn';
                btn.innerText = 'Vægt';
                btn.onclick = (e) => {
                    e.stopPropagation();
                    const input = prompt(`Indtast vægt for d. ${day}/${month + 1}:`, savedWeight);
                    if (input !== null) {
                        localStorage.setItem(dateKey, input.trim());
                        renderWeightCalendar();
                    }
                };

                cell.appendChild(btn);
                grid.appendChild(cell);
            }
        }

        renderProgram();
    </script>
</body>
</html>
