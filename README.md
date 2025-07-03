<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Sowrov এর ড্যাশবোর্ড</title>
  <style>
    body, html {
      margin: 0; padding: 0;
      height: 100%;
      font-family: 'Segoe UI', Tahoma, sans-serif;
      background: #f1f5f9;
      transition: all 0.3s ease;
    }

    #startScreen {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #2563eb, #1e40af);
      color: white;
      font-size: 4rem;
      font-weight: 900;
      cursor: pointer;
      user-select: none;
      letter-spacing: 5px;
    }

    #dashboardLayout {
      display: none;
      height: 100vh;
      display: flex;
    }

    .sidebar {
      width: 220px;
      background: linear-gradient(135deg, #2563eb, #1e40af);
      color: #fff;
      padding: 20px 10px;
      box-shadow: 3px 0 10px rgba(0,0,0,0.2);
      display: flex;
      flex-direction: column;
      height: 100vh;
      position: fixed;
      top: 0; left: 0;
    }
    .sidebar h2 {
      text-align: center;
      margin-bottom: 30px;
      font-size: 1.8rem;
      font-weight: 900;
      letter-spacing: 2px;
    }
    .sidebar a {
      display: block;
      color: #cbd5e1;
      padding: 12px 15px;
      text-decoration: none;
      margin-bottom: 10px;
      border-radius: 8px;
      font-weight: 600;
      cursor: pointer;
    }
    .sidebar a:hover, .sidebar a.active {
      background: #1d4ed8;
      color: #fff;
    }

    main {
      margin-left: 220px;
      padding: 30px;
      flex: 1;
      overflow-y: auto;
      height: 100vh;
      background: #f1f5f9;
    }

    header {
      display: flex;
      align-items: center;
      gap: 15px;
      margin-bottom: 20px;
    }
    .logo {
      width: 60px;
      height: 60px;
      border-radius: 50%;
      background: radial-gradient(circle at top left, #3b82f6, #1e40af);
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      font-size: 2rem;
      font-weight: 900;
      box-shadow: 0 4px 10px rgba(59,130,246,0.5);
    }

    marquee {
      display: block;
      background: #bfdbfe;
      color: #1e3a8a;
      padding: 10px;
      border-radius: 10px;
      margin-bottom: 20px;
      font-weight: bold;
    }

    section {
      background: #fff;
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      margin-bottom: 20px;
      display: none; /* সেকশনগুলো লুকানো থাকবে */
    }
    section.active {
      display: block; /* active সেকশন দেখাবে */
    }
    section h2 {
      font-size: 1.8rem;
      color: #1d4ed8;
      border-bottom: 2px solid #93c5fd;
      padding-bottom: 8px;
      margin-bottom: 15px;
    }
    section p {
      font-size: 1.1rem;
      color: #334155;
      line-height: 1.6;
    }
    .contact-info p {
      margin: 6px 0;
    }
    .contact-info a {
      color: #2563eb;
      text-decoration: none;
      font-weight: 600;
    }
    .contact-info a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>

  <div id="startScreen" title="Click to enter dashboard">ড্যাশবোর্ড</div>

  <div id="dashboardLayout">
    <div class="sidebar">
      <h2>ড্যাশবোর্ড</h2>
      <a data-target="home" class="active">হোম</a>
      <a data-target="content">কনটেন্ট</a>
      <a data-target="contact">যোগাযোগ</a>
    </div>

    <main>
      <header>
        <div class="logo">S</div>
        <h1>Sowrov</h1>
      </header>

      <marquee scrollamount="5">আমার প্রথম ওয়েবসাইটে স্বাগতম — Sowrov এর ব্যক্তিগত ড্যাশবোর্ড</marquee>

      <section id="home" class="active">
        <h2>হোম</h2>
        <p>এটা হলো ড্যাশবোর্ডের প্রথম পেজ।</p>
        <p>মোহনগঞ্জ, নেত্রকোনা বাসিন্দা। নেত্রকোনা সরকারি কলেজের বিজ্ঞান বিভাগের ছাত্র।</p>
      </section>

      <section id="content">
        <h2>কনটেন্ট</h2>
        <p>সময় সম্পর্কে আমার নিজের লেখা শেয়ার করা হয়েছে।</p>
        <p>(১) সময় বলতে কিছু না-- (যা একটি শব্দ) -- {পৃথিবীর আহ্নিক এবং বার্ষিক গতির ফলে অতিবাহিত মধ্যবর্তী স্থানটিকে সময় বলে}</p>
        <p>(২) সময় মূলত জীবনের (জন্ম-মৃত্যু) ধারাবাহিকতা।</p>
        <p>(৩) পৃথিবীর দিন রাত্রি হওয়ার ক্রমান্বয় টা হচ্ছে সময়।</p>
        <p>(৪) "অপেক্ষা" শব্দটি সম্পূর্ণ ভাবে নির্ভর করে সময়ের উপর।</p>
        <p>(৫) এভাবে বলা যায় মানুষের রক্ত সঞ্চালনটাই সময়।</p>
      </section>

      <section id="contact">
        <h2>যোগাযোগ</h2>
        <div class="contact-info">
          <p>ফোন: <a href="tel:+8801606672228">01606672228</a></p>
          <p>Facebook: <a href="https://www.facebook.com/shurovkhan.82" target="_blank">facebook.com/shurovkhan.82</a></p>
          <p>বাড়ি: মোহনগঞ্জ, নেত্রকোনা</p>
          <p>কলেজ: নেত্রকোনা সরকারি কলেজ (বিজ্ঞান বিভাগ)</p>
        </div>
      </section>
    </main>
  </div>

  <script>
    const startScreen = document.getElementById('startScreen');
    const dashboardLayout = document.getElementById('dashboardLayout');
    const links = document.querySelectorAll('.sidebar a');
    const sections = document.querySelectorAll('section');

    startScreen.addEventListener('click', () => {
      startScreen.style.display = 'none';
      dashboardLayout.style.display = 'flex';
    });

    links.forEach(link => {
      link.addEventListener('click', () => {
        // active ক্লাস বদলানো
        links.forEach(l => l.classList.remove('active'));
        link.classList.add('active');

        // সেকশন লুকানো এবং active সেকশন দেখানো
        const target = link.getAttribute('data-target');
        sections.forEach(sec => {
          if (sec.id === target) {
            sec.classList.add('active');
          } else {
            sec.classList.remove('active');
          }
        });
      });
    });
  </script>

</body>
</html>
