<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<title>Hacker System Pro</title>

<style>
body {
    background: black;
    color: #00ff00;
    font-family: "Courier New", monospace;
}

.box {
    width: 420px;
    margin: 40px auto;
    border: 1px solid #00ff00;
    padding: 15px;
    box-shadow: 0 0 15px #00ff00;
}

input, button {
    width: 100%;
    padding: 8px;
    margin-top: 10px;
    background: black;
    color: #00ff00;
    border: 1px solid #00ff00;
}

button:hover {
    background: #00ff00;
    color: black;
    cursor: pointer;
}

.terminal {
    margin-top: 10px;
    height: 160px;
    overflow-y: auto;
    border: 1px solid #00ff00;
    padding: 10px;
    font-size: 13px;
}

.hidden {
    display: none;
}

.line {
    opacity: 0;
    transform: translateY(10px);
    animation: fadeIn 0.3s forwards;
}

@keyframes fadeIn {
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Countdown */
.countdown {
    margin-top: 10px;
    font-size: 14px;
    border: 1px solid #00ff00;
    padding: 5px;
    text-align: center;
}
</style>
</head>

<body>

<!-- PAGE 1 -->
<div class="box" id="page1">
    <h3>> SYSTEM ACCESS</h3>

    <input type="email" id="email" placeholder="Nhập Gmail">

    <button onclick="startHack()">INITIATE</button>
    <button onclick="goSpamPage()">SPAM LOGIN</button>

    <div class="terminal" id="terminal"></div>
</div>

<!-- PAGE 2 -->
<div class="box hidden" id="page2">
    <h3>> SPAM LOGIN PANEL</h3>

    <input type="email" id="checkEmail" placeholder="Nhập lại Gmail">
    <input type="text" id="checkCode" placeholder="Nhập mã bảo mật">

    <input type="number" id="days" placeholder="Ngày (0)" min="0">
    <input type="number" id="hours" placeholder="Giờ (0)" min="0">
    <input type="number" id="minutes" placeholder="Phút (0)" min="0">

    <button onclick="startSpam()">START SPAM</button>
    <button onclick="stopSpam()">STOP SPAM</button>
    <button onclick="back()">BACK</button>

    <div class="countdown" id="countdown">Time Left: 00d 00h 00m 00s</div>

    <div class="terminal" id="spamTerminal"></div>
</div>

<script>
let savedEmail = "";
let savedCode = "";
let spamInterval = null;
let spamTimeout = null;
let countdownInterval = null;
let endTime = 0;

/* RANDOM CODE */
function randomCode() {
    return Math.floor(100000 + Math.random() * 900000);
}

/* FORMAT TIME */
function formatTime(ms) {
    let totalSec = Math.floor(ms / 1000);

    let d = Math.floor(totalSec / 86400);
    let h = Math.floor((totalSec % 86400) / 3600);
    let m = Math.floor((totalSec % 3600) / 60);
    let s = totalSec % 60;

    return `${String(d).padStart(2,"0")}d ${String(h).padStart(2,"0")}h ${String(m).padStart(2,"0")}m ${String(s).padStart(2,"0")}s`;
}

/* ADD LINE */
function addLine(id, text) {
    let box = document.getElementById(id);

    let div = document.createElement("div");
    div.className = "line";
    div.innerText = text;

    box.appendChild(div);
    box.scrollTop = box.scrollHeight;
}

/* HACK */
function startHack() {
    let terminal = document.getElementById("terminal");
    terminal.innerHTML = "";

    let email = document.getElementById("email").value;
    savedEmail = email;

    addLine("terminal", "> Initializing...");
    setTimeout(() => addLine("terminal", "> Connecting to " + email), 800);
    setTimeout(() => addLine("terminal", "> Bypassing firewall..."), 1600);

    setTimeout(() => {
        savedCode = randomCode();
        addLine("terminal", "> Security Code: " + savedCode);
    }, 2400);

    setTimeout(() => addLine("terminal", "> DONE"), 3200);
}

/* PAGE SWITCH */
function goSpamPage() {
    document.getElementById("page1").classList.add("hidden");
    document.getElementById("page2").classList.remove("hidden");
}

function back() {
    stopSpam();
    document.getElementById("page2").classList.add("hidden");
    document.getElementById("page1").classList.remove("hidden");
}

/* START SPAM */
function startSpam() {
    let email = document.getElementById("checkEmail").value;
    let code = document.getElementById("checkCode").value;

    let days = parseInt(document.getElementById("days").value) || 0;
    let hours = parseInt(document.getElementById("hours").value) || 0;
    let minutes = parseInt(document.getElementById("minutes").value) || 0;

    let totalTime = (days*86400 + hours*3600 + minutes*60) * 1000;

    let terminal = document.getElementById("spamTerminal");
    terminal.innerHTML = "";

    if (email !== savedEmail || code != savedCode) {
        addLine("spamTerminal", "> ERROR: INVALID CREDENTIALS");
        return;
    }

    if (totalTime <= 0) {
        addLine("spamTerminal", "> ERROR: INVALID TIME");
        return;
    }

    addLine("spamTerminal", "> Access Granted...");
    addLine("spamTerminal", "> Spam started...");

    let count = 0;
    endTime = Date.now() + totalTime;

    /* spam */
    spamInterval = setInterval(() => {
        count++;
        addLine("spamTerminal", "> Sending login request #" + count);

        if (count % 5 === 0) {
            addLine("spamTerminal", "> Bypass attempt OK");
        }
    }, 250);

    /* countdown */
    countdownInterval = setInterval(() => {
        let remaining = endTime - Date.now();

        if (remaining <= 0) {
            stopSpam(true);
            return;
        }

        document.getElementById("countdown").innerText =
            "Time Left: " + formatTime(remaining);

    }, 1000);

    /* auto stop */
    spamTimeout = setTimeout(() => {
        stopSpam(true);
    }, totalTime);
}

/* STOP */
function stopSpam(auto = false) {
    if (spamInterval) clearInterval(spamInterval);
    if (spamTimeout) clearTimeout(spamTimeout);
    if (countdownInterval) clearInterval(countdownInterval);

    spamInterval = null;
    spamTimeout = null;
    countdownInterval = null;

    let text = auto ? "> TIME EXPIRED - STOPPED" : "> STOPPED BY USER";
    addLine("spamTerminal", text);

    document.getElementById("countdown").innerText =
        "Time Left: 00d 00h 00m 00s";
}
</script>

</body>
</html>
