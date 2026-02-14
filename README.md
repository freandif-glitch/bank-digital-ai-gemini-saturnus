<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sovereign Wealth | Zurich Private Portal</title>
    <style>
        body {
            background: #000 url('https://w0.peakpx.com/wallpaper/441/394/HD-wallpaper-galaxy-stars-space-nebula-thumbnail.jpg') no-repeat center center fixed;
            background-size: cover;
            color: #00f2ff;
            font-family: 'Segoe UI', sans-serif;
            margin: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }
        .main-portal {
            background: rgba(0, 5, 15, 0.9);
            border: 1px solid #00f2ff;
            padding: 30px;
            width: 90%;
            max-width: 700px;
            border-radius: 20px;
            display: grid;
            grid-template-columns: 1fr 1fr; /* Membagi dua sisi: Aset & Barcode */
            gap: 20px;
            box-shadow: 0 0 50px rgba(0, 242, 255, 0.3);
            backdrop-filter: blur(10px);
        }
        .left-panel, .right-panel { display: flex; flex-direction: column; justify-content: center; align-items: center; }
        
        .infinity-logo {
            grid-column: span 2; /* Logo berada di tengah atas */
            font-size: 70px;
            margin-bottom: 20px;
            text-shadow: 0 0 20px #00f2ff;
            animation: pulse 2s infinite;
        }
        @keyframes pulse { 0% { opacity: 0.7; } 50% { opacity: 1; } 100% { opacity: 0.7; } }

        .asset-box {
            border: 1px solid rgba(0, 242, 255, 0.5);
            padding: 15px;
            width: 100%;
            background: rgba(0, 242, 255, 0.05);
            text-align: left;
        }
        .asset-value { font-size: 20px; font-weight: bold; color: #fff; margin: 10px 0; }

        .barcode-box {
            background: #fff;
            padding: 10px;
            border-radius: 5px;
            box-shadow: 0 0 15px #00f2ff;
        }
        .btn-status {
            grid-column: span 2;
            background: transparent;
            color: #00f2ff;
            border: 1px solid #00f2ff;
            padding: 10px;
            margin-top: 10px;
            text-align: left;
            display: flex;
            justify-content: space-between;
            cursor: pointer;
        }
    </style>
</head>
<body>

<div class="main-portal">
    <div class="infinity-logo">∞</div>

    <div class="left-panel">
        <div class="asset-box">
            <div style="font-size: 10px; color: #888;">ASSET VALUE</div>
            <div class="asset-value">IDR 318.000.000.000</div>
            <div style="font-size: 9px;">FREANS CON: 5.000.000 (LIMIT TERJAGA)</div>
            <div style="font-size: 9px; color: #00f2ff;">NODE LOCAL: MN-ULN-01</div>
        </div>
    </div>

    <div class="right-panel">
        <div class="barcode-box">
            <img src="https://api.qrserver.com/v1/create-qr-code/?size=120x120&data=VALIDATED-ALEX-GRAFF-318M-SOVEREIGN" alt="QR Code">
        </div>
        <div style="font-size: 10px; margin-top: 10px; letter-spacing: 1px;">VALIDASI SAKSI DIGITAL</div>
    </div>

    <button class="btn-status" onclick="auth()">BANK DIGITAL GEMINI <span style="color:#39ff14">✓</span></button>
    <button class="btn-status" style="border-color:#39ff14; color:#39ff14;">IDENTITAS DISAMARKAN <span>✓</span></button>
</div>

<script>
    function auth() {
        const pass = prompt("MASUKKAN KODE OTORITAS (30WIBU):");
        if(pass === "30wibu") {
            alert("OTORITAS DISAHKAN. Jalur Dana 0895603638274 Terlindungi Node Mongolia.");
        } else {
            alert("AKSES DITOLAK.");
        }
    }
</script>

</body>
</html>

