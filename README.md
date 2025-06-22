<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Surat Untuk Kamu 🌸</title>
    <style>
        body {
            font-family: 'Georgia', serif;
            background: #fff5f5;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }
        .surat {
            width: 90%;
            max-width: 600px;
            background: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 25px rgba(255, 105, 180, 0.2);
            position: relative;
            line-height: 1.8;
            color: #555;
        }
        .surat::before {
            content: "";
            position: absolute;
            top: 0;
            left: 30px;
            right: 30px;
            height: 3px;
            background: linear-gradient(to right, #ffb6c1, #ff69b4, #ffb6c1);
        }
        .kepala-surat {
            text-align: center;
            margin-bottom: 30px;
        }
        .kepala-surat h1 {
            color: #ff1493;
            font-size: 28px;
            margin-bottom: 5px;
        }
        .kepala-surat p {
            color: #888;
            font-style: italic;
        }
        .isi-surat p {
            margin-bottom: 20px;
            text-align: justify;
        }
        .tanda-tangan {
            margin-top: 40px;
            text-align: right;
            font-style: italic;
        }
        .tanda-tangan .nama {
            font-weight: bold;
            color: #ff1493;
            font-size: 18px;
        }
        .sticker {
            position: absolute;
            opacity: 0.1;
            z-index: 0;
        }
        .sticker-1 {
            top: 20px;
            right: 20px;
            font-size: 60px;
            transform: rotate(15deg);
        }
        .sticker-2 {
            bottom: 10px;
            left: 20px;
            font-size: 50px;
            transform: rotate(-10deg);
        }
        .btn-kirim {
            background: #ff69b4;
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 50px;
            font-size: 16px;
            cursor: pointer;
            margin: 30px auto 0;
            display: block;
            transition: all 0.3s;
        }
        .btn-kirim:hover {
            background: #ff1493;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(255, 105, 180, 0.4);
        }
    </style>
</head>
<body>
    <div class="surat">
        <!-- Sticker hati transparan -->
        <div class="sticker sticker-1">💖</div>
        <div class="sticker sticker-2">💌</div>
        
        <div class="kepala-surat">
            <h1>Untuk Kamu yang Spesial</h1>
            <p>Surat ini kubuat dengan hati, bukan dengan AI</p>
        </div>
        
        <div class="isi-surat">
            <p>Haloo sayang...</p>
            
            <p>Aku nggak pernah jago merangkai kata-kata indah kayak di novel atau film. Tapi hari ini, aku pengen mencoba menuliskan apa yang sering susah kuucapin langsung.</p>
            
            <p>Setiap hari bersamamu itu kayak hadiah yang nggak pernah aku duga. Kamu datang tiba-tiba, lalu mengubah semua standarku tentang "kebahagiaan". Aku yang biasanya pendiem, sekarang jadi sering senyum-senyum sendiri inget kelakuan kamu.</p>
            
            <p>Aku suka cara kamu...</p>
            <ul>
                <li>Peduli sama hal kecil yang bahkan aku sendiri nggak notice</li>
                <li>Ngasih semangat waktu aku lagi down, tanpa judgement</li>
                <li>Bikin hal-hal sederhana jadi berkesan</li>
            </ul>
            
            <p>Yang paling aku syukurin? Kamu nerima aku apa adanya. Nggak maksa aku berubah, nggak bandingin aku dengan orang lain.</p>
            
            <p>Maaf kalau kadang aku...</p>
            <ul>
                <li>Jarang ngungkapin perasaan kayak gini</li>
                <li>Terlalu fokus kerja sampai lupa waktu</li>
                <li>Nggak bisa baca pikiran kamu (aku berusaha kok!)</li>
            </ul>
            
            <p>Tapi yang pasti, aku pengen terus belajar jadi lebih baik buat kita. Karena kamu itu worth it.</p>
            
            <p>Nggak perlu langsung jawab atau bilang balik. Aku cuma pengen kamu tau aja kalau...</p>
            
            <p style="text-align: center; font-size: 20px; color: #ff1493; margin: 30px 0;">
                <b>Aku bersyukur banget punya kamu di hidup aku. ❤️</b>
            </p>
        </div>
        
        <div class="tanda-tangan">
            <p>Yang selalu berusaha memahami kamu,</p>
            <div class="nama">[Nama Kamu]</div>
        </div>
        
        <button class="btn-kirim" onclick="kirimSurat()">Kirim Perasaan Ini</button>
    </div>

    <script>
        function kirimSurat() {
            alert("Surat cinta terkirim! 💌 \n\nAku yakin doi akan tersentuh baca ini...");
            
            // Animasi hati
            for(let i = 0; i < 20; i++) {
                setTimeout(() => {
                    const heart = document.createElement('div');
                    heart.innerHTML = '❤️';
                    heart.style.position = 'fixed';
                    heart.style.left = Math.random() * 100 + 'vw';
                    heart.style.top = Math.random() * 100 + 'vh';
                    heart.style.fontSize = Math.random() * 30 + 10 + 'px';
                    heart.style.animation = `float ${Math.random() * 3 + 2}s ease-in-out infinite`;
                    document.body.appendChild(heart);
                }, i * 100);
            }
        }
        
        // Tambahkan style animasi
        const style = document.createElement('style');
        style.innerHTML = `
            @keyframes float {
                0%, 100% { transform: translateY(0) rotate(0deg); }
                50% { transform: translateY(-20px) rotate(10deg); }
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>
