<!DOCTYPE html>
<html lang="tk">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#070707">

<title>MUKAM UC — PUBG UC Top-Up</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,Helvetica,sans-serif;
}

body{
    background:
      radial-gradient(circle at top,#222 0%,#090909 38%,#030303 100%);
    color:#fff;
    min-height:100vh;
}

header{
    padding:20px;
    text-align:center;
    border-bottom:1px solid #292929;
    background:rgba(0,0,0,.75);
    position:sticky;
    top:0;
    z-index:10;
    backdrop-filter:blur(10px);
}

.logo{
    font-size:28px;
    font-weight:900;
    letter-spacing:3px;
    color:#f5c400;
    text-shadow:0 0 15px rgba(245,196,0,.35);
}

.subtitle{
    margin-top:5px;
    color:#999;
    font-size:12px;
    letter-spacing:1px;
}

.container{
    width:min(700px,94%);
    margin:25px auto 50px;
}

.hero{
    text-align:center;
    padding:25px 15px;
}

.hero h1{
    font-size:32px;
    margin-bottom:8px;
}

.hero h1 span{
    color:#f5c400;
}

.hero p{
    color:#aaa;
    line-height:1.5;
}

.card{
    background:linear-gradient(145deg,#151515,#0b0b0b);
    border:1px solid #292929;
    border-radius:18px;
    padding:20px;
    margin-top:18px;
    box-shadow:0 10px 35px rgba(0,0,0,.35);
}

.card h2{
    font-size:19px;
    margin-bottom:18px;
}

label{
    display:block;
    color:#aaa;
    font-size:13px;
    margin-bottom:7px;
}

input,select{
    width:100%;
    padding:14px;
    background:#080808;
    color:white;
    border:1px solid #333;
    border-radius:11px;
    outline:none;
    font-size:15px;
    margin-bottom:15px;
}

input:focus,select:focus{
    border-color:#f5c400;
    box-shadow:0 0 0 2px rgba(245,196,0,.08);
}

.uc-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:10px;
}

.uc-btn{
    background:#111;
    border:1px solid #333;
    color:#fff;
    padding:14px 8px;
    border-radius:12px;
    cursor:pointer;
    font-weight:bold;
    transition:.2s;
}

.uc-btn:hover,
.uc-btn.active{
    border-color:#f5c400;
    background:#201d08;
    color:#f5c400;
}

.price{
    margin-top:15px;
    padding:16px;
    background:#0a0a0a;
    border-radius:12px;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.price strong{
    color:#f5c400;
    font-size:22px;
}

.main-btn{
    width:100%;
    border:0;
    background:#f5c400;
    color:#000;
    font-weight:900;
    padding:16px;
    border-radius:12px;
    cursor:pointer;
    font-size:16px;
    margin-top:15px;
}

.main-btn:hover{
    background:#ffd83d;
}

.info{
    color:#888;
    font-size:12px;
    line-height:1.5;
    margin-top:12px;
}

.order{
    border:1px solid #292929;
    background:#0b0b0b;
    border-radius:14px;
    padding:15px;
    margin-top:12px;
}

.order-top{
    display:flex;
    justify-content:space-between;
    gap:10px;
}

.order-id{
    color:#f5c400;
    font-weight:bold;
}

.status{
    display:inline-block;
    margin-top:10px;
    padding:6px 10px;
    border-radius:20px;
    background:#302900;
    color:#f5c400;
    font-size:11px;
}

.empty{
    color:#777;
    text-align:center;
    padding:15px;
}

.socials{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:10px;
}

.social{
    text-decoration:none;
    color:#fff;
    padding:13px;
    border:1px solid #292929;
    border-radius:11px;
    text-align:center;
    background:#101010;
}

.social:hover{
    border-color:#f5c400;
}

footer{
    text-align:center;
    padding:30px 15px;
    color:#666;
    font-size:12px;
}

.success{
    display:none;
    padding:15px;
    border-radius:12px;
    background:#0d2415;
    border:1px solid #1c6331;
    color:#7df09b;
    margin-top:15px;
}

@media(max-width:500px){
    .logo{font-size:23px}
    .hero h1{font-size:26px}
    .uc-grid{grid-template-columns:1fr 1fr}
}
</style>
</head>

<body>

<header>
    <div class="logo">MUKAM UC</div>
    <div class="subtitle">PUBG MOBILE • UC TOP-UP</div>
</header>

<div class="container">

    <section class="hero">
        <h1>PUBG <span>UC</span> TOP-UP</h1>
        <p>
            PUBG Mobile UC sargydyňy döred.
            Töleg barlanandan soň sargyt işlenilýär.
        </p>
    </section>

    <div class="card">

        <h2>🎮 Sargyt döret</h2>

        <label>PUBG Player ID</label>
        <input
            id="playerId"
            type="text"
            placeholder="Mysal: 51234567890"
            maxlength="20"
        >

        <label>UC mukdary</label>

        <div class="uc-grid">

            <button class="uc-btn" onclick="selectUC(60,this)">
                60 UC
            </button>

            <button class="uc-btn" onclick="selectUC(325,this)">
                325 UC
            </button>

            <button class="uc-btn" onclick="selectUC(660,this)">
                660 UC
            </button>

            <button class="uc-btn" onclick="selectUC(1800,this)">
                1800 UC
            </button>

            <button class="uc-btn" onclick="selectUC(3850,this)">
                3850 UC
            </button>

            <button class="uc-btn" onclick="selectUC(8100,this)">
                8100 UC
            </button>

        </div>

        <input
            id="customUC"
            type="number"
            placeholder="Ýa-da öz UC mukdaryňy ýaz"
            oninput="customSelected()"
        >

        <div class="price">
            <span>Saýlanan UC</span>
            <strong id="selectedUC">0 UC</strong>
        </div>

        <label style="margin-top:18px;">
            Töleg usuly
        </label>

        <select id="payment">
            <option value="">Saýla</option>
            <option>Kaspi</option>
            <option>Halyk</option>
            <option>Bank transfer</option>
            <option>Başga</option>
        </select>

        <label>
            Töleg barada goşmaça maglumat
        </label>

        <input
            id="paymentInfo"
            type="text"
            placeholder="Mysal: töleg wagty ýa-da tranzaksiýa ID"
        >

        <button class="main-btn" onclick="createOrder()">
            🚀 SARGYT DÖRET
        </button>

        <div class="success" id="successBox"></div>

        <div class="info">
            🔐 Howpsuzlyk: MUKAM UC hiç haçan PUBG parolyňy,
            email parolyňy ýa-da SMS/2FA koduňy soramaýar.
        </div>

    </div>


    <div class="card">

        <h2>📦 Meniň sargytlarym</h2>

        <div id="orders">
            <div class="empty">
                Häzirlikçe sargyt ýok.
            </div>
        </div>

    </div>


    <div class="card">

        <h2>👤 MUKAM_PROVOCATIVE</h2>

        <p style="color:#aaa;line-height:1.6">
            PUBG ID: <b style="color:#f5c400">MkmPROVOCATIVE</b>
        </p>

        <div class="socials" style="margin-top:15px">

            <a
                class="social"
                href="https://www.tiktok.com/@mukam_provocative_"
                target="_blank"
            >
                TikTok
            </a>

            <a
                class="social"
                href="https://www.instagram.com/mukam_provocative"
                target="_blank"
            >
                Instagram
            </a>

            <a
                class="social"
                href="https://www.youtube.com/@mukam_provocative"
                target="_blank"
            >
                YouTube
            </a>

            <a
                class="social"
                href="https://t.me/Mkm_provocative_01"
                target="_blank"
            >
                Telegram
            </a>

        </div>

    </div>

</div>

<footer>
    © 2026 MUKAM UC • MUKAM_PROVOCATIVE
</footer>


<script>

let selectedUC = 0;


// UC saýlamak
function selectUC(amount, button){

    selectedUC = amount;

    document.getElementById("selectedUC").textContent =
        amount + " UC";

    document.getElementById("customUC").value = "";

    document.querySelectorAll(".uc-btn").forEach(btn=>{
        btn.classList.remove("active");
    });

    button.classList.add("active");
}


// Öz UC mukdary
function customSelected(){

    let value =
        parseInt(document.getElementById("customUC").value);

    if(!isNaN(value) && value > 0){

        selectedUC = value;

        document.getElementById("selectedUC").textContent =
            value + " UC";

        document.querySelectorAll(".uc-btn").forEach(btn=>{
            btn.classList.remove("active");
        });

    }
}


// Sargyt döretmek
function createOrder(){

    const playerId =
        document.getElementById("playerId").value.trim();

    const payment =
        document.getElementById("payment").value;

    const paymentInfo =
        document.getElementById("paymentInfo").value.trim();

    if(!playerId){

        alert("PUBG Player ID ýaz!");

        return;
    }

    if(selectedUC <= 0){

        alert("UC mukdaryny saýla!");

        return;
    }

    if(!payment){

        alert("Töleg usulyny saýla!");

        return;
    }


    const order = {

        id:
            "MUK" +
            Date.now().toString().slice(-7),

        playerId: playerId,

        uc: selectedUC,

        payment: payment,

        paymentInfo: paymentInfo,

        status: "Garaşylýar",

        date:
            new Date().toLocaleString()

    };


    let orders =
        JSON.parse(localStorage.getItem("mukamOrders")) || [];

    orders.unshift(order);

    localStorage.setItem(
        "mukamOrders",
        JSON.stringify(orders)
    );


    document.getElementById("successBox").style.display =
        "block";

    document.getElementById("successBox").innerHTML =
        "✅ Sargyt döredildi!<br>" +
        "Sargyt belgisi: <b>" +
        order.id +
        "</b>";


    document.getElementById("playerId").value = "";

    document.getElementById("customUC").value = "";

    document.getElementById("paymentInfo").value = "";

    document.getElementById("payment").value = "";

    selectedUC = 0;

    document.getElementById("selectedUC").textContent =
        "0 UC";

    document.querySelectorAll(".uc-btn").forEach(btn=>{
        btn.classList.remove("active");
    });


    showOrders();

}


// Sargytlary görkezmek
function showOrders(){

    const container =
        document.getElementById("orders");

    let orders =
        JSON.parse(localStorage.getItem("mukamOrders")) || [];


    if(orders.length === 0){

        container.innerHTML =
            '<div class="empty">Häzirlikçe sargyt ýok.</div>';

        return;
    }


    container.innerHTML = "";


    orders.forEach(order=>{

        const div =
            document.createElement("div");

        div.className = "order";


        div.innerHTML = `

            <div class="order-top">

                <div>
                    <div class="order-id">
                        ${order.id}
                    </div>

                    <div style="margin-top:7px;color:#aaa">
                        PUBG ID:
                        <b style="color:white">
                            ${escapeHTML(order.playerId)}
                        </b>
                    </div>
                </div>

                <strong style="color:#f5c400">
                    ${order.uc} UC
                </strong>

            </div>

            <div class="status">
                ${order.status}
            </div>

            <div style="
                margin-top:10px;
                color:#666;
                font-size:11px;
            ">
                ${order.date}
            </div>

        `;


        container.appendChild(div);

    });

}


// HTML howpsuzlygy
function escapeHTML(text){

    return text
        .replace(/&/g,"&amp;")
        .replace(/</g,"&lt;")
        .replace(/>/g,"&gt;")
        .replace(/"/g,"&quot;")
        .replace(/'/g,"&#039;");

}


// Sahypa açylanda
showOrders();

</script>

</body>
</html>
