<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Sowrov এর ড্যাশবোর্ড</title>
  <style>
    body, html {
      margin: 0;
      padding: 0;
      font-family: 'Segoe UI', Tahoma, sans-serif;
      background: #f1f5f9;
    }

    #dashboardLayout {
      display: flex;
      min-height: 100vh;
    }

    .sidebar {
      width: 220px;
      background: linear-gradient(135deg, #2563eb, #1e40af);
      color: #fff;
      padding: 20px 10px;
      box-shadow: 3px 0 10px rgba(0,0,0,0.2);
      display: flex;
      flex-direction: column;
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
      flex: 1;
      padding: 20px;
      overflow-y: auto;
    }

    header {
      display: flex;
      align-items: center;
      gap: 10px;
      margin-bottom: 15px;
    }

    .logo {
      width: 50px;
      height: 50px;
      background: radial-gradient(circle at top left, #3b82f6, #1e40af);
      border-radius: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      font-size: 1.8rem;
      font-weight: 700;
    }

    marquee {
      background: #bfdbfe;
      color: #1e3a8a;
      padding: 8px;
      border-radius: 8px;
      margin-bottom: 15px;
      font-weight: 600;
    }

    section {
      display: none;
      background: #fff;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
      margin-bottom: 20px;
    }

    section.active {
      display: block;
    }

    section h2 {
      color: #1d4ed8;
      border-bottom: 2px solid #60a5fa;
      padding-bottom: 5px;
      margin-bottom: 10px;
      font-size: 1.6rem;
    }

    #home p, #content p, #contact p {
      font-size: 1.1rem;
      color: #334155;
      margin-bottom: 8px;
    }

    #contact p {
      font-weight: 600;
    }

    #contact a {
      color: #2563eb;
      text-decoration: none;
    }

    #contact a:hover {
      text-decoration: underline;
    }

    #home img {
      max-width: 320px;
      border-radius: 12px;
      margin-top: 15px;
      box-shadow: 0 6px 20px rgba(30,64,175,0.3);
    }

    #footerImage {
      max-width: 100%;
      border-radius: 12px;
      margin-top: 20px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.25);
    }

    @media (max-width: 768px) {
      #dashboardLayout {
        flex-direction: column;
      }
      .sidebar {
        width: 100%;
        flex-direction: row;
        overflow-x: auto;
      }
      .sidebar a {
        flex: 1;
        text-align: center;
        padding: 10px;
      }
      main {
        padding: 10px;
      }
      .logo {
        width: 40px;
        height: 40px;
        font-size: 1.2rem;
      }
      #home img {
        max-width: 100%;
      }
    }
  </style>
</head>
<body>

  <div id="dashboardLayout">
    <div class="sidebar">
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
        <p><strong>স্বাগতম!</strong> এই ড্যাশবোর্ডে তুমি আমার ব্যক্তিগত তথ্য, লেখা ও যোগাযোগের উপায় খুঁজে পাবে।</p>
        <p>👉 উপরের মেনু থেকে যে কোনো সেকশন বেছে নাও।</p>
        <p>আমি Sowrov। বাড়ি: মোহনগঞ্জ, নেত্রকোনা।</p>
        <p>আমি নেত্রকোনা সরকারি কলেজের বিজ্ঞান বিভাগের ছাত্র।</p>
        <img src="https://uploads.onecompiler.io/43nf3b8nx/43pjmdvq2/3875.jpg" alt="Sowrov এর ছবি">
      </section>

      <section id="content">
        <h2>কনটেন্ট</h2>
        <p><strong>এখানে আমার সময় নিয়ে কিছু ভাবনা:</strong></p>
        <p>১️⃣ সময় বলতে কিছু না — পৃথিবীর আহ্নিক এবং বার্ষিক গতির ফলে অতিবাহিত মধ্যবর্তী স্থানটিকে সময় বলে।</p>
        <p>২️⃣ সময় মূলত জীবনের জন্ম-মৃত্যুর ধারাবাহিকতা।</p>
        <p>৩️⃣ পৃথিবীর দিন-রাত্রির ক্রমই সময়।</p>
        <p>৪️⃣ "অপেক্ষা" শব্দটি পুরোপুরি সময়ের উপর নির্ভরশীল।</p>
        <p>৫️⃣ মানুষের রক্ত সঞ্চালনও সময়ের প্রকাশ।</p>
        <p>👉 উপরের মেনু ব্যবহার করে অন্য সেকশন দেখো।</p>
      </section>

      <section id="contact">
        <h2>যোগাযোগ</h2>
        <p>আমার সাথে যোগাযোগ করতে নিচের তথ্য ব্যবহার করো:</p>
        <p>📞 ফোন: <a href="tel:+8801606672228">01606672228</a></p>
        <p>🌐 Facebook: <a href="https://www.facebook.com/shurovkhan.82" target="_blank">facebook.com/shurovkhan.82</a></p>
        <p>🏠 ঠিকানা: মোহনগঞ্জ, নেত্রকোনা</p>
        <p>🎓 কলেজ: নেত্রকোনা সরকারি কলেজ (বিজ্ঞান বিভাগ)</p>
        <p>👉 কোনো মতামত থাকলে জানাতে দ্বিধা কোরো না।</p>
      </section>

      <img id="footerImage" src="https://uploads.onecompiler.io/43nf3b8nx/43pjtxkqb/952.jpg" alt="Footer Image" />

    </main>
  </div>

  <script>
    const links = document.querySelectorAll('.sidebar a');
    const sections = document.querySelectorAll('section');

    links.forEach(link => {
      link.addEventListener('click', () => {
        links.forEach(l => l.classList.remove('active'));
        link.classList.add('active');

        const target = link.getAttribute('data-target');
        sections.forEach(sec => {
          sec.classList.toggle('active', sec.id === target);
        });
      });
    });
  </script>

</body>
</html>
