[my_account.html](https://github.com/user-attachments/files/32445138/my_account.html)
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>حسين الراوي | حساباتي وروابط التواصل</title>
  <meta name="description" content="مرحباً بكم في صفحتي الرسمية! يسعدني تواصلكم ومتابعتكم لجديدي عبر منصات التواصل الاجتماعي أدناه.">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Alexandria:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-gradient: radial-gradient(circle at 50% 0%, #1e1e24 0%, #0c0d10 100%);
      --card-bg: rgba(255, 255, 255, 0.04);
      --card-border: rgba(255, 255, 255, 0.08);
      --card-hover-border: rgba(255, 255, 255, 0.22);
      --text-main: #f8fafc;
      --text-muted: #94a3b8;
      --accent: #f59e0b;
      --accent-glow: rgba(245, 158, 11, 0.2);
    }
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body {
      font-family: 'Alexandria', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
      background: #0c0d10;
      background-image: var(--bg-gradient);
      color: var(--text-main);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 40px 16px 60px;
      line-height: 1.6;
    }
    .container {
      width: 100%;
      max-width: 600px;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    /* Profile Header */
    .profile-header {
      text-align: center;
      margin-bottom: 32px;
      display: flex;
      flex-direction: column;
      align-items: center;
      width: 100%;
    }
    .avatar-wrapper {
      position: relative;
      margin-bottom: 20px;
    }
    .avatar-img {
      width: 104px;
      height: 104px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid rgba(255, 255, 255, 0.15);
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.5);
    }
    .verified-badge {
      position: absolute;
      bottom: 4px;
      left: 4px;
      background: #3b82f6;
      color: white;
      border-radius: 50%;
      width: 26px;
      height: 26px;
      display: flex;
      align-items: center;
      justify-content: center;
      border: 2px solid #0c0d10;
    }
    .profile-name {
      font-size: 1.65rem;
      font-weight: 700;
      letter-spacing: -0.5px;
      color: #ffffff;
      margin-bottom: 6px;
    }
    .profile-title {
      font-size: 0.95rem;
      color: var(--accent);
      font-weight: 600;
      margin-bottom: 12px;
    }
    .profile-bio {
      font-size: 0.9rem;
      color: var(--text-muted);
      max-width: 480px;
      margin: 0 auto 16px;
      line-height: 1.6;
    }
    .location-tag {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(255, 255, 255, 0.08);
      padding: 4px 14px;
      border-radius: 9999px;
      font-size: 0.8rem;
      color: #cbd5e1;
    }
    /* Links Container */
    .links-list {
      width: 100%;
      display: flex;
      flex-direction: column;
      gap: 14px;
      margin-bottom: 40px;
    }
    .social-card {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 14px 18px;
      background: var(--card-bg);
      border: 1px solid var(--card-border);
      border-radius: 16px;
      text-decoration: none;
      color: inherit;
      transition: all 0.25s cubic-bezier(0.4, 0, 0.2, 1);
      backdrop-filter: blur(8px);
    }
    .social-card:hover {
      background: rgba(255, 255, 255, 0.08);
      border-color: var(--card-hover-border);
      transform: translateY(-2px);
      box-shadow: 0 12px 24px rgba(0, 0, 0, 0.3);
    }
    .card-start {
      display: flex;
      align-items: center;
      gap: 16px;
    }
    .icon-wrap {
      width: 46px;
      height: 46px;
      border-radius: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 10px;
      color: #ffffff;
      flex-shrink: 0;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
    }
    .text-content {
      display: flex;
      flex-direction: column;
      gap: 2px;
    }
    .card-title-row {
      display: flex;
      align-items: center;
      gap: 8px;
      flex-wrap: wrap;
    }
    .card-title {
      font-size: 0.98rem;
      font-weight: 600;
      color: #ffffff;
    }
    .card-handle {
      font-size: 0.82rem;
      color: var(--text-muted);
      direction: ltr;
      text-align: right;
    }
    .link-badge {
      font-size: 0.7rem;
      font-weight: 600;
      padding: 2px 8px;
      border-radius: 9999px;
      background: rgba(245, 158, 11, 0.15);
      color: #fbbf24;
      border: 1px solid rgba(245, 158, 11, 0.3);
    }
    .card-arrow {
      color: var(--text-muted);
      display: flex;
      align-items: center;
      justify-content: center;
      transition: transform 0.2s ease;
    }
    .social-card:hover .card-arrow {
      color: #ffffff;
      transform: translateX(-4px);
    }
    /* Footer */
    footer {
      text-align: center;
      font-size: 0.8rem;
      color: #64748b;
      margin-top: auto;
      padding-top: 24px;
    }
    @media (max-width: 480px) {
      body {
        padding: 24px 12px 40px;
      }
      .avatar-img {
        width: 90px;
        height: 90px;
      }
      .profile-name {
        font-size: 1.4rem;
      }
      .social-card {
        padding: 12px 14px;
      }
      .icon-wrap {
        width: 40px;
        height: 40px;
        padding: 9px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <header class="profile-header">
      <div class="avatar-wrapper">
        <img src="https://p16-common-sign.tiktokcdn.com/tos-alisg-avt-0068/f8f33f7262033dde3772ae394095b742~tplv-tiktokx-cropcenter:1080:1080.jpeg?dr=14579&refresh_token=6f54fbac&x-expires=1790100000&x-signature=PdMOi0CGvVw77wJnCrgnWuQQ36Y%3D&t=4d5b0474&ps=13740610&shp=a5d48078&shcp=81f88b70&idc=my2"  class="avatar-img">
        <div class="verified-badge" title="حساب موثق">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round">
            <polyline points="20 6 9 17 4 12"></polyline>
          </svg>
        </div>
      </div>
      <h1 class="profile-name">حسين الراوي</h1>
      <p class="profile-title">صانع محتوى </p>
      <p class="profile-bio">مرحباً بكم في صفحتي الرسمية! يسعدني تواصلكم ومتابعتكم لجديدي عبر منصات التواصل الاجتماعي أدناه.</p>
      
      
          <circle cx="12" cy="10" r="3"></circle>
        </svg>
      </div>
    </header>

    <main class="links-list">
      
      <!-- إنستغرام -->
      <a href="https://www.instagram.com/hzx_rawi?stkn=eDBldDNwMXdza3Jz" target="_blank" rel="noopener noreferrer" class="social-card">
        <div class="card-start">
          <div class="icon-wrap" style="background: #E1306C;">
            <svg viewBox="0 0 24 24" fill="currentColor" class="w-full h-full"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/></svg>
          </div>
          <div class="text-content">
            <div class="card-title-row">
              <span class="card-title">إنستغرام </span>
            </div>
            <span class="card-handle">@hzx_rawi</span>
          </div>
        </div>
        <div class="card-arrow">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="15 18 9 12 15 6"></polyline></svg>
        </div>
      </a>

      <!-- تيك توك -->
      <a href="https://www.tiktok.com/@hzx_rawi?_r=1&_t=ZS-99tejnspR7E" target="_blank" rel="noopener noreferrer" class="social-card">
        <div class="card-start">
          <div class="icon-wrap" style="background: #000000; border: 1px solid rgba(255,255,255,0.2);">
            <svg viewBox="0 0 24 24" fill="currentColor" class="w-full h-full"><path d="M12.525.02c1.31-.02 2.61-.01 3.91-.02.08 1.53.63 3.09 1.75 4.17 1.12 1.11 2.7 1.62 4.24 1.79v4.03c-1.44-.05-2.89-.35-4.2-.97-.57-.26-1.1-.59-1.62-.93-.01 2.92.01 5.84-.02 8.75-.08 1.4-.54 2.79-1.35 3.94-1.31 1.92-3.58 3.17-5.91 3.21-1.43.08-2.86-.31-4.08-1.03-2.02-1.19-3.44-3.37-3.65-5.71-.02-.5-.03-1-.01-1.49.18-1.9 1.12-3.72 2.58-4.96 1.66-1.44 3.98-2.13 6.15-1.72.02 1.48-.04 2.96-.04 4.44-.99-.32-2.15-.23-3.02.37-.63.41-1.11 1.04-1.36 1.75-.21.51-.24 1.07-.14 1.61.24 1.64 1.82 3.02 3.5 2.87 1.12-.01 2.19-.66 2.77-1.61.19-.33.4-.67.41-1.06.1-1.79.06-3.57.07-5.36.01-4.03-.01-8.05.02-12.07z"/></svg>
          </div>
          <div class="text-content">
            <div class="card-title-row">
              <span class="card-title">تيك توك </span>
            </div>
            <span class="card-handle">@hzx_rawi</span>
          </div>
        </div>
        <div class="card-arrow">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="15 18 9 12 15 6"></polyline></svg>
        </div>
      </a>

      <!-- تيليجرام -->
      <a href="https://t.me/hzx_rawi" target="_blank" rel="noopener noreferrer" class="social-card">
        <div class="card-start">
          <div class="icon-wrap" style="background: #26A5E4;">
            <svg viewBox="0 0 24 24" fill="currentColor" class="w-full h-full"><path d="M11.944 0A12 12 0 0 0 0 12a12 12 0 0 0 12 12 12 12 0 0 0 12-12A12 12 0 0 0 12 0a12 12 0 0 0-.056 0zm4.962 7.224c.1-.002.321.023.465.14a.506.506 0 0 1 .171.325c.016.093.036.306.02.472-.18 1.898-.962 6.502-1.36 8.627-.168.9-.499 1.201-.82 1.23-.696.065-1.225-.46-1.9-.902-1.056-.693-1.653-1.124-2.678-1.8-1.185-.78-.417-1.21.258-1.91.177-.184 3.247-2.977 3.307-3.23.007-.032.014-.15-.056-.212s-.174-.041-.249-.024c-.106.024-1.793 1.14-5.061 3.345-.48.33-.913.49-1.302.48-.428-.008-1.252-.241-1.865-.44-.752-.245-1.349-.374-1.297-.789.027-.216.325-.437.893-.663 3.498-1.524 5.83-2.529 6.998-3.014 3.332-1.386 4.025-1.627 4.476-1.635z"/></svg>
          </div>
          <div class="text-content">
            <div class="card-title-row">
              <span class="card-title">حساب التيليجرام</span>
            </div>
            <span class="card-handle">@hzx_rawi</span>
          </div>
        </div>
        <div class="card-arrow">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="15 18 9 12 15 6"></polyline></svg>
        </div>
      </a>
      
    </main>
  </div>
</body>
</html>
