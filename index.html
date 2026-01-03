<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Obsession Elite - Hardcore Expansion</title>
    <style>
        :root {
            --bg: #000;
            --primary: #f00;
            --secondary: #600;
            --card-bg: #0a0a0a;
            --border: #300;
        }

        body {
            background: var(--bg);
            color: #fff;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: flex-start;
            min-height: 100vh;
            overflow-x: hidden;
            touch-action: manipulation;
        }

        .container {
            width: 100%;
            max-width: 450px;
            padding: 20px;
            box-sizing: border-box;
        }

        header { margin-bottom: 25px; }

        h1 {
            color: var(--primary);
            font-style: italic;
            font-size: 2.8em;
            margin: 0;
            text-transform: uppercase;
            text-shadow: 0 0 15px rgba(255,0,0,0.5);
        }

        .sub {
            font-size: 11px;
            letter-spacing: 4px;
            color: var(--secondary);
            text-transform: uppercase;
            margin-top: -5px;
        }

        .mode-selector {
            display: flex;
            justify-content: center;
            gap: 8px;
            margin: 20px 0;
        }

        .m-btn {
            padding: 8px 16px;
            font-size: 11px;
            border: 1px solid #333;
            border-radius: 20px;
            color: #777;
            background: rgba(255,255,255,0.05);
            cursor: pointer;
            transition: all 0.3s;
            font-weight: bold;
        }

        .m-btn.active {
            background: var(--primary);
            color: #fff;
            border-color: var(--primary);
            box-shadow: 0 0 10px var(--primary);
        }

        .btn {
            background: #111;
            border: 1px solid var(--border);
            color: #fff;
            padding: 18px;
            width: 100%;
            border-radius: 12px;
            margin-bottom: 12px;
            font-weight: bold;
            font-size: 16px;
            cursor: pointer;
            transition: transform 0.1s, background 0.3s;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }

        .btn:active { transform: scale(0.98); }
        .btn-red { background: var(--primary); border: none; color: white; }

        .view-box { animation: fadeIn 0.4s ease; }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

        .wheel-container {
            position: relative;
            width: 300px;
            height: 300px;
            margin: 20px auto;
        }

        #canvas {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            border: 4px solid #222;
            transition: transform 4s cubic-bezier(0.15, 0, 0.15, 1);
            box-shadow: 0 0 30px rgba(255,0,0,0.2);
        }

        .arrow {
            position: absolute;
            top: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 0; height: 0;
            border-left: 15px solid transparent;
            border-right: 15px solid transparent;
            border-top: 30px solid var(--primary);
            z-index: 10;
        }

        .card {
            background: var(--card-bg);
            border: 2px solid var(--border);
            border-radius: 25px;
            padding: 40px 20px;
            min-height: 220px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            margin-bottom: 25px;
        }

        #txt {
            font-style: italic;
            font-size: 1.3em;
            line-height: 1.4;
            color: #eee;
        }

        .timer {
            font-size: 48px;
            color: var(--primary);
            font-weight: 800;
            margin-top: 20px;
            font-family: monospace;
        }

        .hidden { display: none !important; }

        #wheel-res {
            font-size: 1.2em;
            color: var(--primary);
            font-weight: bold;
            margin: 15px 0;
            min-height: 1.5em;
            text-transform: uppercase;
        }

        .footer-btns {
            display: flex;
            flex-direction: column;
            gap: 10px;
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>Obsession</h1>
        <div class="sub">Elite Intimacy</div>
        
        <div class="mode-selector">
            <button onclick="setLvl(1)" id="l1" class="m-btn">SOFT</button>
            <button onclick="setLvl(2)" id="l2" class="m-btn">SPICY</button>
            <button onclick="setLvl(3)" id="l3" class="m-btn active">HARDCORE</button>
        </div>
    </header>

    <div id="menu">
        <button class="btn" onclick="go('wheel')">🎡 RULETA PERVERSĂ</button>
        <button class="btn" onclick="go('cards')">🔞 ADEVĂR / PĂCAT</button>
        <button class="btn" onclick="go('role')">🎭 ROLEPLAY ELITE</button>
    </div>

    <div id="view-wheel" class="view-box hidden">
        <div class="wheel-container">
            <div class="arrow"></div>
            <canvas id="canvas" width="500" height="500"></canvas>
        </div>
        <div id="wheel-res"></div>
        <button class="btn btn-red" id="spinBtn" onclick="spin()">ROTEȘTE ACUM</button>
        <button class="btn" onclick="go('menu')">ÎNAPOI</button>
    </div>

    <div id="view-cards" class="view-box hidden">
        <div class="card">
            <div id="txt">Pregătește-te...</div>
            <div id="timer-box" class="timer hidden">03:00</div>
        </div>
        
        <div id="game-btns" class="footer-btns">
            <button class="btn" onclick="draw('truth')">EXTRAGE ADEVĂR</button>
            <button class="btn btn-red" onclick="draw('sin')">EXTRAGE PĂCAT</button>
        </div>
        
        <div id="role-btns" class="footer-btns hidden">
            <button class="btn btn-red" onclick="draw('role')">ALT SCENARIU</button>
        </div>
        
        <button class="btn" style="margin-top: 20px;" onclick="go('menu')">ÎNAPOI</button>
    </div>
</div>

<script>
    let lvl = 3;
    let rotation = 0;
    let timerInterval;

    const options = {
        1: ["Sărut Gât", "Masaj Umeri", "Mângâiere", "Șoaptă", "Îmbrățișare", "Sărut Mână"],
        2: ["Sărut Francez", "Mușcă Buza", "Linge Gâtul", "Sărut Sâni", "Mângâie Coapsa", "Spate Gol"],
        3: ["🔞 Sex Oral", "💦 Spermă pe Față", "⛓️ Dominare", "🍑 Mușcă Fundul", "🥒 Jucării", "🌋 Orgasm Forțat", "🥛 Linge-mă tot", "👠 Fetiș Picioare", "🍼 Regresie", "🎭 Mask Play", "🤐 Bondage", "🕯️ Wax Play"]
    };

    const modifiers = [" (legat la ochi)", " (fără mâini)", " (foarte lent)", " (privindu-ne în ochi)", " (cu forță)", " (cu multă salivă)", " (în timp ce gemi)", " (în genunchi)"];

    const db = {
        truth: {
            1: ["Care e trăsătura mea cea mai sexy?", "Ce te-a atras prima dată la mine?", "Unde îți place să fii sărutat(ă)?"],
            2: ["Care e locul cel mai ciudat unde ai făcut-o?", "Ce lenjerie preferi să port?", "Ai fantezii cu alte persoane?"],
            3: [
                "Care e cea mai murdară fantezie pe care nu mi-ai spus-o încă?",
                "Ți-ar plăcea să fim priviți în timp ce o facem?",
                "Ai accepta să fiu cu altcineva în timp ce tu privești?",
                "Ce mărime e ideală pentru tine și de ce?",
                "Te-ai masturbat vreodată cu o poză de-a mea în ultimele 24h?",
                "Care e fetișul tău cel mai 'bolnav'?",
                "Dacă am face un trio, ai vrea încă un bărbat sau o femeie?",
                "Îți place să înghiți sau să fii spermeat(ă) pe față?",
                "Ai încercat vreodată sexul anal? Dacă nu, ai vrea?",
                "Ce obiect din casă ai folosit pe post de jucărie sexuală?",
                "Ai făcut-o vreodată într-un loc public unde puteai fi prins(ă)?",
                "Care e cel mai lung maraton sexual pe care l-ai avut?",
                "Ești mai degrabă dominant sau submisiv?"
            ]
        },
        sin: {
            1: ["Sărută-mă pe gât timp de 30 de secunde.", "Mângâie-mi părul senzual.", "Dă-mi un masaj scurt la umeri."],
            2: ["Dezbracă-mă folosind doar dinții.", "Șoptește-mi ce vrei să-mi faci.", "Linge-mă de la încheietură până la cot."],
            3: [
                "Linge-mi degetele de la picioare unul câte unul, cu pasiune.",
                "Fă-mi sex oral fără să te oprești timp de 5 minute.",
                "Stai în genunchi și cere-mi permisiunea să mă atingi.",
                "Folosește gheață sau ceva rece pe organele mele intime.",
                "Linge-mă peste tot acolo jos până când te opresc eu.",
                "Mângâie-te în fața mea în timp ce mă privești fix în ochi.",
                "Dă-ți jos chiloții și pune-i pe fața mea.",
                "Linge-mi sfârcurile și mușcă-le ușor timp de 3 minute.",
                "Domină-mă agresiv: pune-mă la perete și sărută-mă cu forță.",
                "Folosește o curea sau ceva să-mi legi mâinile la spate.",
                "Linge-mi fundul în timp ce mă penetrezi/mă atingi.",
                "Pune-mă să-mi cer iertare pentru că am fost 'rău/rea'.",
                "Toarnă-ți băutura pe corp și lasă-mă să o ling.",
                "Fă-mi un masaj erotic folosind mult ulei peste tot."
            ]
        },
        role: {
            1: ["Străini la un bar.", "Prima noastră întâlnire."],
            2: ["Secretara și Boss-ul.", "Maseurul pervers."],
            3: [
                "Polițistul și Infractoarea: Mă arestezi și mă perchezizi corporal total.",
                "Doctorul și Pacienta: O examinare intimă foarte amănunțită.",
                "Stăpân și Sclav: Timp de 15 minute execuți orice ordin fără comentarii.",
                "Livratorul și Casnica: 'Nu am bani de pizza, cum pot să plătesc?'",
                "Profesorul și Eleva: Am luat o notă mică, merit o pedeapsă severă.",
                "Fotograful și Modelul: Pozează-mi provocator în timp ce eu te dirijez.",
                "Răpitorul: M-ai capturat și mă ții ostatic(ă) pentru plăcerea ta.",
                "Călătorii în tren: Suntem străini într-un compartiment gol.",
                "Supraveghetorul de noapte: M-ai prins făcând ceva interzis în birou."
            ]
        }
    };

    function setLvl(n) {
        lvl = n;
        document.querySelectorAll('.m-btn').forEach(b => b.classList.remove('active'));
        document.getElementById('l' + n).classList.add('active');
        if(!document.getElementById('view-wheel').classList.contains('hidden')) drawWheel();
    }

    function go(view) {
        document.getElementById('menu').classList.add('hidden');
        document.getElementById('view-wheel').classList.add('hidden');
        document.getElementById('view-cards').classList.add('hidden');
        clearInterval(timerInterval);
        document.getElementById('timer-box').classList.add('hidden');

        if(view === 'menu') document.getElementById('menu').classList.remove('hidden');
        else if(view === 'wheel') {
            document.getElementById('view-wheel').classList.remove('hidden');
            drawWheel();
        } else if(view === 'cards') {
            document.getElementById('view-cards').classList.remove('hidden');
            document.getElementById('game-btns').classList.remove('hidden');
            document.getElementById('role-btns').classList.add('hidden');
            document.getElementById('txt').innerText = "Alege-ți soarta...";
        } else if(view === 'role') {
            document.getElementById('view-cards').classList.remove('hidden');
            document.getElementById('game-btns').classList.add('hidden');
            document.getElementById('role-btns').classList.remove('hidden');
            draw('role');
        }
    }

    function drawWheel() {
        const c = document.getElementById('canvas');
        const ctx = c.getContext('2d');
        const opts = options[lvl];
        const slice = (Math.PI * 2) / opts.length;
        ctx.clearRect(0,0,500,500);
        opts.forEach((t, i) => {
            ctx.beginPath();
            ctx.fillStyle = i % 2 === 0 ? '#1a0000' : '#450000';
            ctx.moveTo(250, 250);
            ctx.arc(250, 250, 240, i * slice, (i + 1) * slice);
            ctx.fill();
            ctx.strokeStyle = '#800';
            ctx.lineWidth = 2;
            ctx.stroke();
            ctx.save();
            ctx.translate(250, 250);
            ctx.rotate(i * slice + slice / 2);
            ctx.fillStyle = "#fff";
            ctx.font = "bold 16px sans-serif";
            ctx.textAlign = "right";
            ctx.fillText(t, 225, 5);
            ctx.restore();
        });
        ctx.beginPath();
        ctx.arc(250,250,15,0,Math.PI*2);
        ctx.fillStyle = '#f00';
        ctx.fill();
    }

    function spin() {
        const btn = document.getElementById('spinBtn');
        const canvas = document.getElementById('canvas');
        btn.disabled = true;
        document.getElementById('wheel-res').innerText = "SORTEZ...";
        const extra = Math.floor(Math.random() * 360);
        rotation += (2160 + extra);
        canvas.style.transform = `rotate(${rotation}deg)`;
        setTimeout(() => {
            btn.disabled = false;
            const actual = rotation % 360;
            const arc = 360 / options[lvl].length;
            const idx = Math.floor(((360 - actual + 270) % 360) / arc);
            let res = options[lvl][idx % options[lvl].length];
            if(lvl === 3) res += modifiers[Math.floor(Math.random()*modifiers.length)];
            document.getElementById('wheel-res').innerText = res;
        }, 4000);
    }

    function draw(type) {
        const list = db[type][lvl];
        let res = list[Math.floor(Math.random() * list.length)];
        if(lvl === 3 && type === 'sin') res += modifiers[Math.floor(Math.random()*modifiers.length)];
        document.getElementById('txt').innerText = res;
        if(type === 'sin') startTimer(lvl === 3 ? 300 : 180);
        else {
            document.getElementById('timer-box').classList.add('hidden');
            clearInterval(timerInterval);
        }
    }

    function startTimer(seconds) {
        const box = document.getElementById('timer-box');
        box.classList.remove('hidden');
        let timeLeft = seconds;
        clearInterval(timerInterval);
        timerInterval = setInterval(() => {
            let m = Math.floor(timeLeft / 60);
            let s = timeLeft % 60;
            box.innerText = `${m}:${s < 10 ? '0' + s : s}`;
            if(timeLeft <= 0) {
                clearInterval(timerInterval);
                document.getElementById('txt').innerText = "TIMP EXPIRAT! NU MAI AȘTEPTA!";
            }
            timeLeft--;
        }, 1000);
    }

    window.onload = () => drawWheel();
</script>

</body>
</html>

