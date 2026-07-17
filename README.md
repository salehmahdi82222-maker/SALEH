<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover" />
    <title>استودیو پرامپت | گرافیت پلاس</title>
    <link href="https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Vazirmatn-font-face.css" rel="stylesheet" type="text/css" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root { --bg-color: #fff7ed; --text-color: #333; --card-bg: #ffffff; --primary-color: #f97316; --border-color: #fed7aa; --secondary-bg: #fff7ed; }
        [data-theme="dark"] { --bg-color: #121212; --text-color: #e0e0e0; --card-bg: #1e1e1e; --primary-color: #fb923c; --border-color: #333; --secondary-bg: #252525; }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Vazirmatn', sans-serif; transition: background-color 0.3s, color 0.3s, border-color 0.3s; -webkit-tap-highlight-color: transparent; -webkit-touch-callout: none; }
        
        /* رفع کامل باگ اسکرول و سایز در گوشی‌های موبایل */
        html { overflow-x: hidden; -webkit-overflow-scrolling: touch; width: 100%; }
        body { 
            background-color: var(--bg-color); 
            color: var(--text-color); 
            margin: 0; padding: 0; width: 100%;
            min-height: 100vh; min-height: 100dvh; 
            position: relative;
            padding-top: 80px; 
            padding-bottom: 50px; 
            overflow-x: hidden;
            word-wrap: break-word;
            overflow-wrap: break-word;
        }
        
        .top-bar { 
            position: fixed; top: 10px; left: 10px; right: 10px; 
            background: var(--card-bg); border-radius: 50px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); 
            padding: 8px 15px; display: flex; flex-wrap: nowrap; overflow-x: auto; white-space: nowrap; 
            z-index: 1000; border: 1px solid var(--border-color); gap: 15px; scrollbar-width: none; 
            justify-content: center; width: auto; max-width: calc(100% - 20px); box-sizing: border-box;
            margin: 0 auto;
        }
        .top-bar::-webkit-scrollbar { display: none; } 
        .top-bar button { background: none; border: none; color: var(--text-color); cursor: pointer; font-size: 14px; display: flex; align-items: center; gap: 6px; font-weight: bold; flex-shrink: 0; }
        .top-bar button:hover { color: var(--primary-color); }

        .toast-container { position: fixed; top: 80px; left: 0; right: 0; z-index: 9999; display: flex; flex-direction: column; gap: 10px; align-items: center; pointer-events: none; padding: 0 15px; box-sizing: border-box; }
        .toast { padding: 10px 20px; border-radius: 8px; color: #fff; font-weight: bold; box-shadow: 0 4px 12px rgba(0,0,0,0.15); opacity: 0; transform: translateY(-20px); transition: all 0.3s ease; max-width: 100%; word-wrap: break-word; text-align: center; font-size: 14px; }
        .toast.show { opacity: 1; transform: translateY(0); }
        .toast-success { background-color: #10b981; } .toast-error { background-color: #ef4444; } .toast-info { background-color: var(--primary-color); }
        .btn { padding: 10px 15px; border-radius: 10px; border: none; cursor: pointer; font-weight: bold; display: inline-flex; align-items: center; justify-content: center; gap: 8px; color: #fff; position: relative; overflow: hidden; font-size: 14px; touch-action: manipulation; }
        .btn::after { content: ''; position: absolute; top: 50%; left: 50%; width: 5px; height: 5px; background: rgba(255,255,255,0.5); opacity: 0; border-radius: 100%; transform: scale(1, 1) translate(-50%, -50%); transform-origin: 50% 50%; }
        .btn:focus:not(:active)::after { animation: ripple 1s ease-out; }
        @keyframes ripple { 0% { transform: scale(0, 0); opacity: 0.5; } 100% { transform: scale(40, 40); opacity: 0; } }
        .btn-primary { background: var(--primary-color); } .btn-success { background: #10b981; } .btn-danger { background: #ef4444; } .btn-warning { background: #f59e0b; } .btn-secondary { background: #6b7280; }
        .btn:hover { opacity: 0.9; transform: translateY(-2px); box-shadow: 0 4px 10px rgba(0,0,0,0.2); }
        .btn-custom { background: var(--primary-color); } .btn-random { background: #10b981; } .btn-select { background: #f59e0b; } .btn-clear { background: #ef4444; }
        .view { display: none; animation: fadeIn 0.5s; } .view.active { display: block; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }
        .auth-container { max-width: 400px; margin: 20px auto; background: var(--card-bg); padding: 20px; border-radius: 20px; box-shadow: 0 4px 20px rgba(0,0,0,0.05); }
        .auth-tabs { display: flex; margin-bottom: 15px; border-bottom: 2px solid var(--border-color); }
        .auth-tabs button { flex: 1; padding: 8px; background: none; border: none; font-size: 16px; cursor: pointer; color: var(--text-color); font-weight: bold; }
        .auth-tabs button.active { color: var(--primary-color); border-bottom: 3px solid var(--primary-color); }
        .form-group { margin-bottom: 12px; }
        .form-group label { display: block; margin-bottom: 5px; font-size: 13px; }
        .form-group .hint { font-size: 11px; color: #888; margin-bottom: 5px; }
        .form-group .hint-warn { font-size: 11px; color: var(--primary-color); margin-top: 5px; text-align: center; font-weight: bold; }
        .form-group input, .form-group select, .form-group textarea { width: 100%; padding: 10px; border-radius: 10px; border: 1px solid var(--border-color); background: var(--secondary-bg); color: var(--text-color); font-family: inherit; font-size: 15px; }
        .form-group textarea { resize: vertical; min-height: 60px; }
        .error-msg { color: #ef4444; font-size: 12px; margin-top: 5px; display: none; }
        .password-wrapper { position: relative; width: 100%; }
        .password-wrapper input { padding-left: 40px; width: 100%; }
        .password-toggle { position: absolute; left: 15px; top: 50%; transform: translateY(-50%); cursor: pointer; color: #888; font-size: 16px; z-index: 2; }
        .dashboard { display: grid; grid-template-columns: minmax(300px, 1fr) minmax(300px, 2fr); gap: 15px; max-width: 1400px; margin: 15px auto; padding: 0 15px; }
        .card { background: var(--card-bg); border-radius: 15px; padding: 15px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); margin-bottom: 15px; max-width: 100%; }
        .card h3 { margin-bottom: 12px; border-bottom: 1px solid var(--border-color); padding-bottom: 8px; font-size: 18px; }
        .profile-info p { margin-bottom: 12px; display: flex; align-items: center; gap: 8px; flex-wrap: wrap; font-size: 14px; }
        .profile-info input { flex: 1; min-width: 100px; padding: 8px; border-radius: 5px; border: 1px solid var(--border-color); background: var(--secondary-bg); color: var(--text-color); font-size: 14px; }
        .profile-info .password-wrapper { flex: 1; min-width: 100px; }
        .profile-info .password-wrapper input { padding: 8px 8px 8px 30px; }
        .live-preview-box-h { width: 100%; aspect-ratio: 16/9; background: #000; border-radius: 15px; overflow: hidden; position: relative; border: 2px dotted var(--primary-color); margin-bottom: 10px; box-shadow: 0 0 15px rgba(249, 115, 22, 0.4); }
        .live-preview-box-v { width: 100%; max-width: 300px; height: 380px; margin: 0 auto 10px auto; background: #000; border-radius: 15px; overflow: hidden; position: relative; border: 2px dotted var(--primary-color); box-shadow: 0 0 15px rgba(249, 115, 22, 0.4); }
        .preview-btn { width: 100%; margin-top: 5px; }
        .categories-bar { display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 15px; }
        .cat-btn { padding: 6px 12px; border-radius: 20px; border: 1px solid var(--border-color); background: transparent; color: var(--text-color); cursor: pointer; font-size: 13px; transition: all 0.2s; }
        .cat-btn:hover { transform: translateY(-2px); border-color: var(--primary-color); }
        .cat-btn.active { background: var(--primary-color); color: #fff; border-color: var(--primary-color); box-shadow: 0 4px 10px rgba(249, 115, 22, 0.3); }
        .hidden-initial { display: none !important; }
        .words-container { display: flex; flex-wrap: wrap; gap: 6px; min-height: 50px; padding: 10px; background: var(--secondary-bg); border-radius: 10px; margin-bottom: 15px; border: 1px dashed var(--border-color); animation: fadeIn 0.3s; }
        .word-chip { padding: 5px 10px; background: #ffedd5; color: #c2410c; border-radius: 8px; cursor: pointer; font-size: 12px; transition: transform 0.1s; }
        [data-theme="dark"] .word-chip { background: #c2410c; color: #ffedd5; }
        .word-chip:hover { transform: scale(1.05); }
        .word-chip.selected { opacity: 0.5; border: 1px solid var(--primary-color); background: var(--secondary-bg); }
        .selected-words-bar { background: var(--secondary-bg); border: 1px solid var(--border-color); border-radius: 10px; padding: 8px; margin-bottom: 15px; min-height: 50px; display: flex; flex-wrap: wrap; gap: 8px; align-items: center; animation: fadeIn 0.3s; }
        .selected-chip { background: var(--primary-color); color: #fff; padding: 5px 10px; border-radius: 20px; font-size: 12px; display: flex; align-items: center; gap: 8px; animation: slideIn 0.3s; }
        @keyframes slideIn { from { transform: scale(0); } to { transform: scale(1); } }
        .selected-chip i { cursor: pointer; font-size: 12px; }
        .actions-bar { display: flex; flex-wrap: wrap; justify-content: flex-end; gap: 8px; margin-bottom: 10px; }
        .powered-by { text-align: center; font-size: 11px; color: #888; margin-bottom: 15px; }
        .powered-by a { color: var(--primary-color); text-decoration: none; font-weight: bold; }
        .custom-form { display: none; margin-bottom: 15px; padding: 15px; background: var(--secondary-bg); border-radius: 10px; border: 1px solid var(--border-color); }
        .custom-form.active { display: block; animation: fadeIn 0.3s; }
        .grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; }
        .prompt-output { background: #1e293b; color: #e2e8f0; padding: 15px; border-radius: 10px; font-family: 'Vazirmatn', sans-serif; font-size: 14px; min-height: 120px; margin-bottom: 10px; direction: ltr; text-align: left; line-height: 1.6; border: 1px solid #334155; white-space: pre-wrap; word-break: break-word; overflow-wrap: break-word; display: flex; align-items: center; }
        .copy-btn { width: 100%; margin-bottom: 10px; }
        .chatgpt-btn { width: 100%; background: #10a37f; }
        
        .history-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 12px; flex-wrap: wrap; gap: 8px; }
        .search-box { padding: 8px 12px; border-radius: 8px; border: 1px solid var(--border-color); background: var(--secondary-bg); color: var(--text-color); min-width: 150px; font-size: 14px; }
        
        .history-item { background: var(--secondary-bg); padding: 12px; border-radius: 10px; margin-bottom: 8px; border-left: 4px solid var(--primary-color); position: relative; word-wrap: break-word; }
        .history-item .meta { font-size: 11px; color: #888; margin-bottom: 5px; }
        .history-item .topic { font-weight: bold; margin-bottom: 5px; color: var(--primary-color); font-size: 14px; }
        .history-item .text { font-family: 'Vazirmatn', sans-serif; font-size: 13px; color: var(--text-color); white-space: nowrap; overflow: hidden; text-overflow: ellipsis; direction: ltr; text-align: left; }
        .history-item .actions { margin-top: 8px; display: flex; gap: 8px; }
        
        .pagination-container { margin-top: 15px; display: flex; justify-content: center; align-items: center; gap: 6px; flex-wrap: wrap; }
        .page-btn { padding: 6px 12px; border-radius: 8px; border: 1px solid var(--border-color); background: var(--secondary-bg); cursor: pointer; font-weight: bold; color: var(--text-color); transition: all 0.2s; display: flex; align-items: center; gap: 5px; font-size: 13px; }
        .page-btn:hover:not(:disabled) { border-color: var(--primary-color); color: var(--primary-color); }
        .page-btn.active { background: var(--primary-color); color: #fff; border-color: var(--primary-color); }
        .page-btn:disabled { opacity: 0.5; cursor: not-allowed; }
        .page-dots { padding: 6px 5px; color: #888; font-weight: bold; }

        .gallery-filter-bar { margin-bottom: 15px; text-align: center; }
        .gallery-filter-bar select { padding: 8px 12px; border-radius: 10px; border: 1px solid var(--border-color); background: var(--secondary-bg); color: var(--text-color); font-family: inherit; font-size: 13px; min-width: 200px; }

        .gallery-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 15px; }
        .gallery-item { background: var(--card-bg); border-radius: 15px; overflow: hidden; box-shadow: 0 2px 10px rgba(0,0,0,0.05); border: 1px solid var(--border-color); }
        .gallery-item .content { padding: 12px; }
        .gallery-item img { width: 100%; border-radius: 10px; margin-bottom: 8px; height: 180px; object-fit: cover; }
        .gallery-item .title { font-weight: bold; margin-bottom: 5px; font-size: 15px; }
        .gallery-item .meta-tags { display: flex; gap: 8px; margin-bottom: 8px; flex-wrap: wrap; }
        .gallery-item .tag { font-size: 10px; padding: 4px 8px; border-radius: 5px; background: var(--secondary-bg); color: var(--primary-color); border: 1px solid var(--border-color); }
        .gallery-item .desc { font-family: 'Vazirmatn', sans-serif; font-size: 12px; background: var(--secondary-bg); padding: 8px; border-radius: 5px; color: #888; word-break: break-word; direction: ltr; text-align: left; max-height: 80px; overflow-y: auto; }
        
        .main-footer { text-align: center; padding: 15px; font-size: 11px; color: #888; border-top: 1px solid var(--border-color); margin-top: 30px; }
        .main-footer a { color: var(--primary-color); text-decoration: none; font-weight: bold; }
        .fab-container { position: fixed; bottom: 15px; z-index: 900; display: flex; flex-direction: column; gap: 10px; }
        .fab-right { right: 15px; }
        .fab-pill { position: fixed; bottom: 15px; left: 15px; background: var(--primary-color); color: #fff; padding: 10px 15px; border-radius: 30px; border: none; cursor: pointer; font-weight: bold; display: flex; align-items: center; gap: 8px; box-shadow: 0 4px 10px rgba(0,0,0,0.3); z-index: 900; font-size: 13px; transition: transform 0.2s; }
        .fab-pill:hover { transform: scale(1.05); background: #ea580c; }
        .fab { width: 45px; height: 45px; border-radius: 50%; background: #ef4444; color: #fff; border: none; cursor: pointer; font-size: 18px; box-shadow: 0 4px 10px rgba(0,0,0,0.3); display: flex; align-items: center; justify-content: center; transition: transform 0.2s; }
        .fab:hover { transform: scale(1.1) rotate(10deg); }
        .modal-overlay { position: fixed; top: 0; left: 0; right: 0; bottom: 0; background: rgba(0,0,0,0.6); z-index: 2000; display: none; align-items: center; justify-content: center; padding: 20px; }
        .modal-overlay.active { display: flex; animation: fadeIn 0.3s; }
        .modal-box { background: var(--card-bg); padding: 20px; border-radius: 20px; max-width: 400px; width: 100%; text-align: center; box-shadow: 0 10px 30px rgba(0,0,0,0.3); animation: slideUp 0.4s ease; }
        @keyframes slideUp { from { transform: translateY(50px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
        .modal-box h3 { margin-bottom: 12px; }
        .modal-box p { margin-bottom: 15px; line-height: 1.6; }
        .size-options { display: grid; grid-template-columns: 1fr 1fr; gap: 8px; margin: 15px 0; }
        .size-option { padding: 8px; border: 1px solid var(--border-color); border-radius: 8px; cursor: pointer; background: var(--secondary-bg); text-align: center; font-size: 12px; }
        .size-option:hover { border-color: var(--primary-color); color: var(--primary-color); }
        .hidden { display: none !important; }

        /* استایل لودینگ و تایپ زنده */
        .spinner-box { display: flex; flex-direction: column; align-items: center; justify-content: center; width: 100%; }
        .spinner { border: 4px solid rgba(255, 255, 255, 0.1); border-radius: 50%; border-top: 4px solid var(--primary-color); width: 40px; height: 40px; animation: spin 1s linear infinite; }
        @keyframes spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
        .loading-text { margin-top: 15px; color: #888; font-size: 14px; }
        .typed-text { width: 100%; }

        @media (max-width: 900px) { .dashboard { grid-template-columns: 1fr; } }
        @media (max-width: 1200px) and (min-width: 901px) { .dashboard { grid-template-columns: 1fr; max-width: 700px; } }
        @media (max-width: 1200px) {
            /* ترتیب نمایش در صفحه کوچک: استودیو پرامپت -> پروفایل کاربر -> سایت گرافیت پلاس -> کانال گرافیک ترنج */
            .left-col, .right-col { display: contents; }
            .right-col .card:nth-child(1) { order: 1; } /* استودیو پرامپت */
            .left-col .card:nth-child(1) { order: 2; }  /* پروفایل کاربر */
            .left-col .card:nth-child(2) { order: 3; }  /* سایت گرافیت پلاس */
            .left-col .card:nth-child(3) { order: 4; }  /* کانال گرافیک ترنج */
            .right-col .card:nth-child(2) { order: 5; } /* تاریخچه پرامپت‌ها */
        }
        @media (max-width: 500px) { 
            .grid-2 { grid-template-columns: 1fr; }
            .top-bar button span { display: none; } /* مخفی کردن متن دکمه‌ها در گوشی بسیار کوچک */
            .top-bar button { font-size: 16px; }
            .top-bar button i { margin: 0; }
            .gallery-grid { grid-template-columns: 1fr; }
        }

        /* بهینه‌سازی تکمیلی برای نمایش صحیح روی گوشی و مانیتورهای مختلف - بدون حذف قوانین قبلی */
        @media (max-width: 768px) {
            body { padding-top: 70px; padding-bottom: 40px; }
            .dashboard { padding: 0 10px; gap: 12px; margin: 10px auto; }
            .card { padding: 12px; border-radius: 12px; }
            .auth-container { padding: 15px; margin: 15px auto; border-radius: 15px; }
            .size-options { grid-template-columns: 1fr; }
            .history-header { justify-content: center; text-align: center; }
            .search-box { width: 100%; min-width: 0; }
            .gallery-filter-bar select { width: 100%; max-width: 100%; min-width: 0; }
            .actions-bar { justify-content: center; }
            .categories-bar { justify-content: center; }
        }
        @media (max-width: 480px) {
            .top-bar { padding: 6px 10px; gap: 10px; top: 6px; left: 6px; right: 6px; }
            .card h3 { font-size: 16px; }
            .btn { font-size: 13px; padding: 9px 12px; }
            .prompt-output { font-size: 13px; padding: 12px; }
            .live-preview-box-v { max-width: 100%; height: 320px; }
            .gallery-item img { height: 150px; }
            .modal-box { padding: 15px; border-radius: 15px; }
            .form-group input, .form-group select, .form-group textarea { font-size: 14px; padding: 9px; }
        }
        @media (max-width: 360px) {
            .top-bar { gap: 6px; padding: 6px 8px; }
            .top-bar button { font-size: 15px; }
            .card { padding: 10px; }
            .auth-container { padding: 12px; }
        }
        @media (min-width: 1600px) {
            .dashboard { max-width: 1600px; }
        }
    </style>
</head>
<body>
    <div class="toast-container" id="toastContainer"></div>
    <div class="top-bar">
        <button id="backToStudioBtn" class="hidden" onclick="switchView('studioView')"><i class="fas fa-arrow-right"></i> <span>بازگشت</span></button>
        <button id="exitBtn" class="hidden" onclick="logout()"><i class="fas fa-right-from-bracket"></i> <span>خروج</span></button>
        <button onclick="window.open('https://graphit-plus.ir', '_blank')"><i class="fas fa-globe"></i> <span>سایت گرافیت پلاس</span></button>
        <button id="themeBtn" onclick="toggleTheme()"><i class="fas fa-moon"></i> <span>تم</span></button>
    </div>

    <div id="authView" class="view active">
        <div class="auth-container">
            <div class="auth-tabs">
                <button id="tabLogin" class="active" onclick="switchTab('login')">ورود</button>
                <button id="tabRegister" onclick="switchTab('register')">ثبت نام</button>
            </div>
            <form id="loginForm" onsubmit="handleLogin(event)">
                <div class="form-group"><label>نام کاربری یا شماره تلفن</label><input type="text" id="loginIdentifier" required></div>
                <div class="form-group"><label>رمز عبور</label><div class="password-wrapper"><input type="password" id="loginPassword" required><i class="fas fa-eye password-toggle" onclick="togglePass('loginPassword', this)"></i></div></div>
                <button type="submit" class="btn btn-primary" style="width:100%">ورود</button>
            </form>
            <form id="registerForm" class="hidden" onsubmit="handleRegister(event)">
                <div class="form-group"><label>نام</label><input type="text" id="regFirstName" required></div>
                <div class="form-group"><label>نام خانوادگی</label><input type="text" id="regLastName" required></div>
                <div class="form-group"><label>نام کاربری</label><div class="hint">فقط حروف انگلیسی و عدد مجاز است.</div><input type="text" id="regUsername" required pattern="[a-zA-Z0-9]+"><div class="error-msg" id="userError">نام کاربری تکراری است یا فرمت اشتباه است.</div></div>
                <div class="form-group"><label>شماره تلفن</label><div class="hint">باید 11 رقم باشد و با 09 شروع شود (فقط عدد).</div><input type="tel" id="regPhone" required pattern="09[0-9]{9}" maxlength="11" oninput="this.value=this.value.replace(/[^0-9]/g,'')"><div class="error-msg" id="phoneError">فرمت شماره تلفن اشتباه است.</div></div>
                <div class="form-group"><label>رمز عبور</label><div class="password-wrapper"><input type="password" id="regPassword" required><i class="fas fa-eye password-toggle" onclick="togglePass('regPassword', this)"></i></div></div>
                <button type="submit" class="btn btn-success" style="width:100%">ثبت نام</button>
            </form>
        </div>
    </div>

    <div id="studioView" class="view">
        <div class="dashboard">
            <div class="left-col">
                <div class="card profile-info">
                    <h3>پروفایل کاربر</h3>
                    <p>نام: <input type="text" id="profFirstName"></p>
                    <p>نام خانوادگی: <input type="text" id="profLastName"></p>
                    <p>نام کاربری: <strong id="profUsername"></strong></p>
                    <p>شماره تلفن: <strong id="profPhone"></strong></p>
                    <button class="btn btn-primary" style="width:100%; margin-top:10px" onclick="updateProfile()">ذخیره تغییرات</button>
                    <button class="btn btn-warning" style="width:100%; margin-top:10px;" onclick="openPasswordModal()"><i class="fas fa-key"></i> ویرایش رمز عبور</button>
                </div>
                <div class="card">
                    <h3>سایت گرافیت پلاس</h3>
                    <div class="live-preview-box-h"><iframe src="https://graphit-plus.ir" style="width:100%; height:100%; border:none;" title="Graphit Plus"></iframe></div>
                    <button class="btn btn-primary preview-btn" onclick="window.open('https://graphit-plus.ir', '_blank')"><i class="fas fa-arrow-up-right-from-square"></i> ورود به سایت</button>
                </div>
                <div class="card">
                    <h3>کانال گرافیک ترنج</h3>
                    <div class="live-preview-box-v"><iframe src="https://eitaa.com/graphic_toranj" style="width:100%; height:100%; border:none;" title="Graphic Toranj"></iframe></div>
                    <button class="btn btn-success preview-btn" onclick="window.open('https://eitaa.com/graphic_toranj', '_blank')"><i class="fab fa-telegram"></i> ورود به کانال</button>
                </div>
            </div>
            <div class="right-col">
                <div class="card">
                    <h3>استودیو پرامپت</h3>
                    <div class="categories-bar" id="categoriesBar"></div>
                    <div class="words-container hidden-initial" id="wordsContainer"></div>
                    <div class="selected-words-bar hidden-initial" id="selectedWordsBar"></div>
                    <div class="actions-bar">
                        <button class="btn btn-clear" onclick="clearAll()"><i class="fas fa-trash"></i> پاک سازی</button>
                        <button class="btn btn-select" onclick="openSizeModal()"><i class="fas fa-list-check"></i> از انتخاب ها</button>
                        <button class="btn btn-random" onclick="generateRandom()"><i class="fas fa-dice"></i> تصادفی</button>
                        <button class="btn btn-custom" onclick="toggleCustomForm()"><i class="fas fa-sliders"></i> سفارشی</button>
                    </div>
                    <div class="powered-by">قدرت گرفته از <a href="https://chatgpt.com/" target="_blank">ChatGPT</a></div>
                    <div class="custom-form" id="customForm">
                        <div class="form-group"><label>موضوع (Subject)</label><input type="text" id="customTopic" placeholder="مثال: گرافیک ترنج منبع تمام ابزار ها"></div>
                        <div class="form-group"><label>توضیح بیشتر (Description)</label><textarea id="customDesc" rows="3" placeholder="مثال: یک صفحه کانال که مطالب کانال در مورد گرافیک باشد،پکیج-ابزار-آموزش"></textarea></div>
                        <div class="grid-2">
                            <div class="form-group"><label>ابعاد تصویر (Size)</label><select id="customSize"></select></div>
                            <div class="form-group"><label>سبک تصویر (Style)</label><select id="customStyle"></select></div>
                            <div class="form-group"><label>نورپردازی (Lighting)</label><select id="customLighting"></select></div>
                            <div class="form-group"><label>زاویه دوربین (Camera Angle)</label><select id="customCamera"></select></div>
                        </div>
                        <div class="grid-2">
                            <div class="form-group"><label>متن روی تصویر (Text on Image)</label><select id="textOnImg" onchange="toggleTextLang()"><option value="no">خیر (No)</option><option value="yes">بله (Yes)</option></select></div>
                            <div class="form-group hidden-initial" id="textLangBox"><label>زبان متن (Text Language)</label><select id="textLang"><option value="Persian">فارسی (Persian)</option><option value="English">انگلیسی (English)</option><option value="Hebrew">عبری (Hebrew)</option><option value="Arabic">عربی (Arabic)</option></select></div>
                        </div>
                        <div class="form-group hidden-initial" id="textContentBox"><label>متن پیشنهادی برای روی تصویر (Text Content)</label><input type="text" id="textContent" placeholder="مثلا: Graphit Plus"></div>
                        <div class="form-group">
                            <label>ارسال به کدام هوش مصنوعی؟ (AI Target)</label>
                            <select id="aiTarget"></select>
                            <div class="hint-warn">برای تحویل پرامپت متناسب دقت داشته باشید</div>
                        </div>
                        <button class="btn btn-primary" style="width:100%" onclick="generateCustomPrompt()"><i class="fas fa-magic-wand-sparkles"></i> تولید پرامپت</button>
                    </div>
                    <div class="prompt-output" id="promptOutput"><div class="typed-text">Prompt will be generated here...</div></div>
                    <button class="btn btn-secondary copy-btn" onclick="copyPrompt()"><i class="fas fa-copy"></i> کپی پرامپت</button>
                    <button class="btn chatgpt-btn" onclick="sendToChatGPT()"><i class="fas fa-robot"></i> ارسال به ChatGPT</button>
                </div>
                <div class="card">
                    <div class="history-header">
                        <h3 style="border:none; margin:0; padding:0;">تاریخچه پرامپت‌ها</h3>
                        <input type="text" class="search-box" id="historySearch" oninput="searchHistory()" placeholder="جستجو...">
                    </div>
                    <div id="historyContainer"><p style="color:#888; text-align:center;">هنوز پرامپتی تولید نشده است.</p></div>
                    <div id="historyPagination" class="pagination-container"></div>
                </div>
            </div>
        </div>
    </div>

    <div id="galleryView" class="view">
        <div class="dashboard" style="grid-template-columns: 1fr;">
            <div class="card">
                <h3>گالری پرامپت کاربران</h3>
                <button class="btn btn-success" onclick="toggleUploadForm()" style="margin-bottom:15px;"><i class="fas fa-upload"></i> بارگذاری پرامپت جدید</button>
                
                <div class="gallery-filter-bar">
                    <select id="galleryFilter" onchange="changeGalleryFilter(this.value)">
                        <option value="all">همه دسته‌ها</option>
                    </select>
                </div>

                <div class="custom-form" id="uploadForm" style="margin-bottom: 15px;">
                    <div class="form-group"><label>عنوان پرامپت (Title)</label><input type="text" id="galleryTitle"></div>
                    <div class="grid-2">
                        <div class="form-group">
                            <label>دسته‌بندی (Category)</label>
                            <select id="galleryCategory"></select>
                        </div>
                        <div class="form-group">
                            <label>هوش مصنوعی (AI Target)</label>
                            <select id="galleryAI" onchange="toggleCustomAI(this.value)">
                                <option value="Midjourney">Midjourney</option>
                                <option value="DALL-E 3">DALL-E 3</option>
                                <option value="Stable Diffusion">Stable Diffusion</option>
                                <option value="ChatGPT">ChatGPT</option>
                                <option value="Nano Banana">Nano Banana</option>
                                <option value="custom">سایر (دلخواه)</option>
                            </select>
                        </div>
                    </div>
                    <div class="form-group hidden-initial" id="customAIBox">
                        <label>نام هوش مصنوعی دلخواه</label>
                        <input type="text" id="galleryCustomAI" placeholder="نام هوش مصنوعی را وارد کنید">
                    </div>
                    <div class="form-group"><label>متن پرامپت (Prompt Text)</label><textarea id="galleryText" rows="4" style="width:100%; padding:10px; border-radius:8px; border:1px solid var(--border-color); background:var(--secondary-bg); color:var(--text-color);"></textarea></div>
                    <div class="form-group"><label>تصویر نمونه (Sample Image - حداکثر 2 مگابایت)</label><input type="file" id="galleryImage" accept="image/*" style="padding:10px;"></div>
                    <button class="btn btn-primary" onclick="uploadPrompt()" id="gallerySubmitBtn"><i class="fas fa-check"></i> ثبت در گالری</button>
                    <button class="btn btn-danger hidden" onclick="cancelEditGallery()" id="galleryCancelBtn" style="margin-top:10px;"><i class="fas fa-times"></i> انصراف</button>
                </div>

                <div class="gallery-grid" id="galleryGrid"></div>
                <div id="galleryPagination" class="pagination-container"></div>
            </div>
        </div>
    </div>

    <button class="fab-pill" onclick="goToGallery()" title="گالری پرامپت"><i class="fas fa-images"></i> گالری پرامپت</button>
    <div class="fab-container fab-right"><button class="fab" onclick="openSupportModal()" title="پشتیبانی"><i class="fas fa-headset"></i></button></div>

    <div class="modal-overlay" id="sizeModal"><div class="modal-box"><h3>انتخاب ابعاد تصویر (Select Size)</h3><p>لطفاً سایز مورد نظر برای فضای مجازی را انتخاب کنید:</p><div class="size-options" id="sizeOptionsGrid"></div><button class="btn btn-danger" onclick="closeModal('sizeModal')">انصراف</button></div></div>
    <div class="modal-overlay" id="supportModal"><div class="modal-box"><h3>ارتباط با پشتیبانی</h3><p>در صورت هر گونه مشکل از سایت <a href="https://graphit-plus.ir" target="_blank" style="color:var(--primary-color);">گرافیت پلاس</a> تیکت ثبت کنید.</p><button class="btn btn-primary" onclick="closeModal('supportModal')"><i class="fas fa-check"></i> تایید</button></div></div>
    <div class="modal-overlay" id="deleteModal"><div class="modal-box"><h3><i class="fas fa-triangle-exclamation" style="color: #ef4444;"></i> تایید حذف</h3><p>آیا از حذف این پرامپت اطمینان دارید؟</p><button class="btn btn-danger" onclick="confirmDeleteGallery()"><i class="fas fa-trash"></i> بله، حذف شود</button><button class="btn btn-secondary" style="margin-top:10px;" onclick="closeModal('deleteModal')">انصراف</button></div></div>
    
    <div class="modal-overlay" id="passwordModal">
        <div class="modal-box">
            <h3>تغییر رمز عبور</h3>
            <div class="form-group" style="text-align:right;">
                <label>رمز عبور جدید</label>
                <input type="password" id="newPassword" placeholder="رمز جدید">
            </div>
            <div class="form-group" style="text-align:right;">
                <label>تکرار رمز عبور جدید</label>
                <input type="password" id="confirmNewPassword" placeholder="تکرار رمز">
            </div>
            <button class="btn btn-primary" onclick="updatePassword()"><i class="fas fa-check"></i> ثبت رمز جدید</button>
            <button class="btn btn-danger" style="margin-top:10px;" onclick="closeModal('passwordModal')">انصراف</button>
        </div>
    </div>

    <footer class="main-footer">برای رایگان بودن این پنل، در کانال <a href="https://eitaa.com/graphic_toranj" target="_blank">گرافیک ترنج</a> عضو شوید.</footer>

    <script>
        function getUsers() { try { return JSON.parse(localStorage.getItem('users') || '{}'); } catch (e) { return {}; } }
        function saveUsers(users) { try { localStorage.setItem('users', JSON.stringify(users)); } catch (e) { showToast('خطا در ذخیره‌سازی', 'error'); } }
        function togglePass(id, icon) { const input = document.getElementById(id); if (input.type === 'password') { input.type = 'text'; icon.classList.replace('fa-eye','fa-eye-slash'); } else { input.type = 'password'; icon.classList.replace('fa-eye-slash','fa-eye'); } }

        const categories = {
            "طبیعت": ["جنگل", "کوهستان", "اقیانوس", "آسمان", "رودخانه", "صحرا", "دشت", "آبشار", "غروب", "طلوع", "باران", "برف", "پاییز", "بهار", "تابستان", "زمستان", "گل", "درخت", "ابر", "رعد", "طوفان", "جزیره", "خلیج", "چشمه", "غار", "دره", "صخره", "شن", "ماسه", "مرتع", "کویر", "دریاچه", "برکه", "یخچال", "تالاب", "طبیعت بکر", "جنگل کاج", "صخره‌های مرجانی", "آب‌های فیروزه‌ای", "رود یخ‌زده", "شکوفه‌های بهاری", "خزان پاییزی", "کویر بی‌انتها", "دشت ستاره‌ها", "غار زیرآبی", "نسیم ملایم", "باد شدید", "گردباد", "تگرگ", "مه غلیظ", "شبنم", "باران موسمی", "برف سنگین", "کولاک", "رنگین‌کمان", "آسمان پرستاره", "ماه کامل", "خورشیدگرفتگی", "ماه‌گرفتگی", "ساحل مرجانی", "جنگل انبوه", "دشت گل‌های وحشی", "کوه‌های برفی", "دریاچه نمک", "غار یخی", "آتشفشان خاموش", "چشمه آب گرم", "آبشار یخ‌زده", "تپه", "دامنه", "قله", "مرداب", "چشمه آب معدنی", "سنگ آذرین", "سنگ دگرگونی", "سنگ رسوبی", "آبگینه", "بلور", "کریستال"],
            "فانتزی": ["اژدها", "قصر", "جادوگر", "الف", "کوتوله", "جنگجو", "شمشیر", "سپر", "تاج", "نیروی جادویی", "جنگل تاریک", "پری", "اهریمن", "فرشته", "قهرمان", "گنج", "نقشه قدیمی", "معبد", "طلسم", "معجزه", "روح", "خفاش", "گرگ", "کلاغ", "کتاب جادو", "پیامرسان", "سوارکار", "اسب بالدار", "ساحره", "غول", "گوبلین", "قوی سیاه", "پری دریایی", "سنگ جادو", "الف تاریک", "جادوگر خبیث", "شهریار اژدها", "شهر گمشده", "شمشیر نور", "سپر آهنین", "معبد طلایی", "پری مه‌انگار", "گرگینه", "خفاش غول‌پیکر", "چشم شیطانی", "اونیکورن", "گریفین", "مینوتور", "کراکن", "زامبی", "مومیایی", "خون‌آشام", "اسکلت", "جن", "دیو", "پری آتش", "شوالیه تاریکی", "جنگجوی نور", "آینه جادویی", "تخت طلایی", "عصای جادو", "کلاه جادوگر", "شنل نامرئی", "کفش بالدار", "زره اژدها", "کمان نور", "تیر برق‌آسا", "سپر الماس", "گردنبند جاودانگی", "حلقه قدرت", "کتاب اسرار", "طلسم جاودانگی", "غار گنج", "جزیره مرموز", "آسمان جادویی", "دروازه ابدیت", "فونیکس", "پگاسوس", "اژدهای آتش‌آفرین", "روباه نه‌دم", "سندباد", "علاءالدین", "جینی", "دزد دریایی", "کابوی"],
            "تکنولوژی": ["ربات", "کامپیوتر", "کابل", "هولوگرام", "شهر هوشمند", "ماشین پرواز", "لیزر", "چیپ", "هوش مصنوعی", "واقعیت مجازی", "فضاپیما", "موتور", "برق", "باتری", "مانیتور", "کیبورد", "موشواره", "ایستگاه فضایی", "پهپاد", "میکروچیپ", "شبکه", "سرور", "داده", "کد", "مدار", "ترانزیستور", "آنتن", "ماهواره", "رباتیک", "پرینتر سه‌بعدی", "واقعیت افزوده", "بلاکچین", "متاورس", "نورون مصنوعی", "کابل نوری", "سرور رک", "چیپ کوانتومی", "گجت پوشیدنی", "نانوبات", "هولوگرام سه‌بعدی", "موتور مغناطیسی", "شهر سایبری", "ایستگاه مداری", "دوربین چتری", "هوش عمومی", "متالورژی پیشرفته", "اسکنر عنبیه", "پروتز هوشمند", "دستکش واقعیت مجازی", "هدفون سه‌بعدی", "صفحه لمسی", "پنل خورشیدی", "توربین بادی", "باتری هسته‌ای", "رایانه کوانتومی", "سیستم دفاعی", "رادار پیشرفته", "پایگاه داده ابری", "الگوریتم پیچیده", "ربات انسان‌نما", "سگ رباتیک", "پرنده مصنوعی", "ماهی رباتیک", "دوربین مداربسته هوشمند", "سنسور", "مدار چاپی", "پردازنده", "حافظه فلش", "درایو", "هارد دیسک", "رم", "سی پی یو", "جی پی یو"],
            "فضایی": ["کهکشان", "سیاره", "ستاره", "ماه", "خورشید", "سوراخ سیاه", "شهاب", "دنباله‌دار", "فضانورد", "کاشف", "مدار", "جرم آسمانی", "نور", "تاریکی", "بعد", "زمان", "جهان", "ملکوتی", "فرازمینی", "مدارگرد", "پرتاب", "سوخت", "ایستگاه فضایی", "مریخ", "زهره", "مشتری", "زحل", "اورانوس", "نپتون", "عطارد", "ستاره دنباله‌دار", "سحابی", "اخترشناس", "تلسکوپ فضایی", "کهکشان مارپیچ", "سیاره سرخ", "کمربند سیارکی", "سحابی اسب سر", "حلقه زحل", "کره خورشیدی", "انفجار گامایی", "ماده تاریک", "کرم‌چاله", "زمان نسبی", "ابر خوشه", "اجرام دور", "ستاره نوترونی", "سیاهچاله کلان‌جرم", "انفجار بزرگ", "جهان موازی", "سفر در زمان", "کاوشگر فضایی", "موشک فضایی", "فضاپیمای سرنشین‌دار", "ایستگاه فضایی بین‌المللی", "کهکشان بیضوی", "کهکشان نامنظم", "ستاره کوتوله", "ابرنواختر", "پلاسمای کیهانی", "تابش زمینه", "سیاره فراخورشیدی", "ماه یخی", "بارش شهابی", "سیاره گازی", "سیاره سنگی", "فضای بی‌نهایت", "منظومه شمسی", "سیارک", "ستاره قطبی", "صورت فلکی", "کهکشان آندرومدا"],
            "شهرنشینی": ["آسمانخراش", "خیابان", "ماشین", "ترافیک", "پارک", "مترو", "پل", "بندر", "کافه", "رستوران", "فروشگاه", "چراغ راهنما", "پیاده‌رو", "دوربین", "تبلیغات", "مردم", "شلوغ", "شب", "روز", "باران شهری", "حومه", "مرکز شهر", "بازار", "میدان", "ایستگاه اتوبوس", "اتوبان", "کوچه", "ساختمان اداری", "مسکن", "بیلبورد", "تاکسی", "اتوبوس", "ایستگاه قطار", "دوربین مداربسته", "چراغ‌های نئونی", "بن‌بست", "خیابان سنگ‌فرش", "پله برقی", "پل عابر", "میدان بزرگ", "ساعت دیواری", "باغ شهری", "منطقه صنعتی", "مسیر دوچرخه", "ایستگاه تاکسی", "فروشگاه زنجیره‌ای", "برج مسکونی", "مجتمع تجاری", "پیاده‌رو سایه‌دار", "نیمکت پارک", "آبنمای شهری", "مجسمه میدان", "سطل زباله", "چراغ خیابان", "تابلو راهنما", "دکه روزنامه", "دستگاه بلیط", "اسکیت‌بورد", "دوچرخه اشتراکی", "خودرو برقی", "ایستگاه شارژ", "خانه تاریخی", "ساختمان مدرن", "معماری قدیمی", "تراموا", "اتوبوس دوطبقه", "موتورسیکلت", "چراغ راهنمایی", "خط عابر پیاده", "پارکینگ طبقاتی", "مجسمه شهری"],
            "پرتره": ["چهره مرد", "چهره زن", "کودک", "سالمند", "هنرمند", "نگاه عمیق", "خنده", "غصه", "آرامش", "عصبانیت", "چشم", "لب", "موی بلند", "موی کوتاه", "ریش", "کلاه", "عینک", "آرایش", "طبیعی", "استودیو", "پس‌زمینه", "نور طبیعی", "نیم‌رخ", "تمام قد", "محیط کار", "رسمی", "اسپرت", "خالکوبی", "پیرسینگ", "گریم", "مدل", "بازیگر", "خواننده", "ورزشکار", "نویسنده", "نگاه کناری", "چشم‌های آبی", "لب‌های پر", "چهره رنگ‌پریده", "خالکوبی صورت", "کلاه لبه‌دار", "عینک آفتابی", "آرایش تیره", "آرایش ملایم", "موهای فرفری", "ریش بلند", "پیرمرد چروک", "نوجوان", "چهره خندان", "چهره غمگین", "چهره متفکر", "چشم‌های درشت", "ابروهای کلفت", "گونه‌های برجسته", "فک محکم", "پیشانی بلند", "لبخند ملایم", "نگاه خشمگین", "نگاه عاشقانه", "نگاه خیره", "پوست روشن", "پوست تیره", "موی مجعد", "موی صاف", "کک و مک", "خال صورت", "چشم‌های قهوه‌ای", "چشم‌های سبز", "ریش کوتاه", "سبیل", "گریم سینمایی", "چهره آراسته", "چهره خسته", "چهره شاداب"],
            "حیوانات": ["شیر", "ببر", "گرگ", "کفتار", "اسب", "گوزن", "عقاب", "شاهین", "گربه", "سگ", "خرس", "فیل", "ماهی", "کوسه", "نهنگ", "دلفین", "لاکپشت", "مار", "کروکودیل", "پرنده", "مرغ", "اردک", "خرگوش", "موش", "میمون", "گوریل", "حشره", "زرافه", "گورخر", "کرگدن", "کنگورو", "پاندا", "ببر سفید", "یوزپلنگ", "روباه", "جغد", "کبوتر", "طاووس", "طوطی", "مار گرمسیری", "قورباغه شاخ‌دار", "پلنگ برفی", "گربه وحشی", "ماهی مرکب", "هشت‌پا", "عقاب دریایی", "کرکور", "لاک‌پشت غول‌پیکر", "فلامینگو", "پنگوئن", "خرس قطبی", "گوزن شمالی", "سمور آبی", "اردک وحشی", "غاز", "قو", "لک‌لک", "کرکس", "خفاش", "سنجاب", "موش صحرایی", "جوجه‌تیغی", "گورکن", "خرگوش صحرایی", "شتر", "لاما", "آلپاکا", "گاومیش", "گاو", "گوسفند", "بز", "بز کوهی", "آهو", "گوزن زرد", "خرگوش قطبی", "روباه قطبی", "سمندر", "ایگوانا", "آفتاب‌پرست", "جغد برفی", "عقاب طلایی"],
            "خوراکی": ["همبرگر", "پیتزا", "سالاد", "میوه", "سیب", "موز", "انار", "انگور", "کیک", "شکلات", "بستنی", "قهوه", "چای", "آب", "نوشابه", "پاستا", "برنج", "گوشت", "مرغ", "ماهی سرخ شده", "سوپ", "نان", "پنیر", "تخم مرغ", "سوسیس", "کباب", "دسر", "شیرینی", "کلوچه", "پاپ کورن", "پنکیک", "وافل", "نودل", "سوشی", "کاپوچینو", "لاته", "چای سبز", "آب‌میوه", "خربوزه", "هندوانه", "گیلاس", "توت‌فرنگی", "دیزی", "حلیم", "فسنجان", "قرمه‌سبزی", "زرشک پلو", "ماهی قزل‌آلا", "میگو", "سالاد الویه", "ماست", "دوغ", "آب دوغ خیار", "نعنا", "جعفری", "گوجه", "خیار", "هویج", "سبزیجات", "کاهو", "کلم", "بروکلی", "قارچ", "فلفل دلمه‌ای", "پیاز", "سیر", "زعفران", "زرشک", "گردو", "پسته", "بادام", "فندق", "کشمش", "خرما", "انجیر", "آلو", "هلو", "شلیل", "کیوی", "آناناس", "انبه", "کباب برگ", "جوجه کباب", "چلوکباب", "ته‌چین", "آبگوشت", "کله‌پاچه", "سیرابی", "دلمه", "فالوده", "شربت", "عرق نعنا", "عرق بیدمشک"],
            "وسایل نقلیه": ["ماشین مسابقه", "ماشین کلاسیک", "ماشین شاسی‌بلند", "موتور سیکلت", "کامیون", "اتوبوس", "هواپیما", "هلیکوپتر", "قایق", "کشتی", "دوچرخه", "واگن", "قطار", "تراموا", "مترو", "کشنده", "تانک", "خودرو زرهی", "آمبولانس", "ماشین پلیس", "ماشین آتش‌نشانی", "بیل مکانیکی", "لودر", "جرثقیل", "تراکتور", "گاری", "زیردریایی", "جت جنگنده", "بالگرد", "هاورکرافت", "کالسکه اسب", "کشتی بادبانی", "گلایدر", "کایاک", "ماشین شاسی‌کوتاه", "ماشین کروک", "ماشین دست‌ساز", "ماشین بخار", "قطار سریع‌السیر", "قطار باری", "کشتی نفت‌کش", "زیردریایی اتمی", "جنگنده رادارگریز", "بالگرد تجاری", "پهپاد نظامی", "ماشین برقی", "خودرو هیبرید", "خودروی خودران", "ون", "مینی‌بوس", "تریلر", "قایق موتوری", "قایق بادی", "موتور جت", "موشک", "فضاپیمای مسافرتی", "ماشین مسابقه‌ای فرمول یک", "ماشین رالی", "جیپ", "خودرو سافاری", "ماشین اسپورت", "اسکوتر", "پله‌برقی متحرک", "سورتمه", "گاری اسبی", "کالسکه شاهانه"],
            "تاریخ": ["شاهنشاه", "سلطان", "شوالیه", "جنگجو", "معبد", "قلعه", "شمشیر", "سپر", "تیر", "کمان", "زره", "صلیب", "تاج", "تخت", "سکه", "پیمان", "نقشه", "جنگ", "صلح", "پادشاهی", "امپراتوری", "جمهوری", "باستانی", "عتیقه", "سند", "خط میخی", "هیروگلیف", "یونان باستان", "روم باستان", "پارس", "مصر باستان", "چین باستان", "ژاپن فئودال", "سپاه جاویدان", "ارتش روم", "گلادیاتور", "سامورایی", "وایکینگ", "کاوبوی", "دزدان دریایی", "قلعه متروک", "خرابه‌های روم", "معبد یونانی", "اهرام مصر", "دیوار چین", "تاج‌وتخت", "فرعون", "کلئوپاترا", "اسکندر کبیر", "جنگ‌های صلیبی", "شوالیه‌های معبد", "امپراتوری عثمانی", "صفویان", "هخامنشیان", "ساسانیان", "اشکانیان", "تمدن ایلام", "تمدن مایا", "تمدن آزتک", "تمدن اینکا", "تمدن بین‌النهرین", "سنگ‌نبشته", "کتیبه", "غار باستانی", "شهر سوخته", "زیگورات", "آرامگاه کوروش", "تخت جمشید", "آتشکده", "معبد آناهیتا", "پل تاریخی", "کاروانسرا", "آثار باستانی", "کاوش باستان‌شناسی"],
            "هنر": ["نقاشی", "مجسمه", "گرافیتی", "طرح", "آبرنگ", "رنگ روغن", "مداد", "ذغال", "خاک رس", "سفال", "صنایع دستی", "فرش", "موزاییک", "شیشه", "چوب", "فلز", "طلا", "نقره", "برنز", "سنگ", "مرمر", "کلاژ", "خوشنویسی", "تذهیب", "مینیاتور", "نقاشی دیواری", "تندیس", "مجسمه‌سازی", "طراحی صنعتی", "گرافیک", "تایپوگرافی", "طراحی پوستر", "کارت پستال", "طراحی لوگو", "طرح دست‌ساز", "نقاشی دیجیتال", "طراحی سه‌بعدی", "مجسمه برنزی", "آهنگری", "شیشه‌گری", "چوب‌بری", "فرش دستباف", "طراحی داخلی", "طراحی لباس", "نقاشی چهره", "پیکرتراشی", "حکاکی", "کنده‌کاری", "خراطی", "معرق", "خاتم‌کاری", "میناکاری", "قلمزنی", "مسگری", "سفال‌گری", "کاشی‌کاری", "آینه‌کاری", "گچ‌بری", "تراش سنگ", "مجسمه مدرن", "نقاشی انتزاعی", "نقاشی سورئال", "نقاشی امپرسیونیست", "پاستل", "گواش", "مداد رنگی", "مرکب", "سیاه‌قلم", "طراحی مانکن", "طراحی صحنه", "طراحی گرافیک", "نقاشی رنگ روغن", "نقاشی اکریلیک"],
            "علمی": ["آزمایشگاه", "میکروسکوپ", "تلسکوپ", "شیمی", "فیزیک", "زیست‌شناسی", "DNA", "مولکول", "اتم", "الکترون", "جرم", "انرژی", "موج", "نور", "صوت", "الکتریسیته", "آهنربا", "گرما", "سرما", "فشار", "شعاع", "اشعه", "لیزر", "پلاسما", "گاز", "مایع", "جامد", "واکنش شیمیایی", "فرمول", "ریاضیات", "هندسه", "جبر", "آمار", "اخترفیزیک", "نانوتکنولوژی", "زیست‌شناسی مولکولی", "شیمی آلی", "فیزیک کوانتوم", "گرانش", "نسبیت", "سیاه‌چاله", "ستاره نوترونی", "ژنتیک", "سلول بنیادی", "ویروس", "باکتری", "واکسن", "آنتی‌بیوتیک", "پادتن", "کروموزوم", "پروتئین", "آنزیم", "متابولیسم", "فتوسنتز", "تنفس سلولی", "انرژی هسته‌ای", "واکنش زنجیره‌ای", "شکافت هسته‌ای", "همجوشی هسته‌ای", "ذرات بنیادین", "بوزون هیگز", "میدان مغناطیسی", "طیف‌نمایی", "بلورشناسی", "نانوذرات", "حسگرهای زیستی", "بیوتکنولوژی", "مهندسی ژنتیک", "کلونینگ", "سلول", "بافت", "ارگانیسم"],
            "احساسات": ["شادی", "غم", "عشق", "ترس", "خشم", "آرامش", "استرس", "امید", "ناامیدی", "تنهایی", "رنجش", "سوگواری", "خنده", "گریه", "تعجب", "شرم", "افتخار", "حسادت", "راستی", "دروغ", "وفاداری", "خیانت", "شجاعت", "جسارت", "مهربانی", "دشمنی", "مهر", "اشتیاق", "بی‌حوصلگی", "خستگی", "تمنا", "حسرت", "خداحافظی", "آغوش", "سکوت", "خشم کور", "شوق", "ترس و لرز", "عشق افلاطونی", "دلتنگی", "پشیمانی", "بی‌تفاوتی", "اعتماد به نفس", "ضعف", "سرخوردگی", "وحشت", "خلسه", "دوستی", "محبت", "لطافت", "خشونت", "بغض", "اشک", "حیرت", "انزجار", "علاقه", "بیزاری", "عطوفت", "دلسوزی", "غمگینی", "شادابی", "نگرانی", "دلهره", "اضطراب", "افسردگی", "شور", "حرارت", "سردی", "بی‌تفاوتی"],
            "ورزش": ["فوتبال", "بسکتبال", "والیبال", "تنیس", "شنا", "دویدن", "کوهنوردی", "دوچرخه‌سواری", "شمشیربازی", "بوکس", "کاراته", "جودو", "وزنه‌برداری", "کشتی", "هاکی", "بیسبال", "گلف", "اسکی", "اسنوبورد", "سوارکاری", "تیراندازی", "قایق‌رانی", "موج‌سواری", "غواصی", "ژیمناستیک", "والیبال ساحلی", "رقص", "یوگا", "پیاده‌روی", "پارکور", "اسکیت", "ویندسرف", "پرش با چتر", "پرش ارتفاع", "دو میدانی", "ماراتن", "دو سرعت", "شنای سینکرون", "پرش سه‌گام", "پرتاب نیزه", "پرتاب دیسک", "هاکی روی یخ", "کرلینگ", "بدمینتون", "تنیس روی میز", "راگبی", "کریکت", "اسنوکر", "بیلیارد", "بولینگ", "دارت", "شطرنج", "تیراندازی با کمان", "سه‌گانه", "واترپلو", "کبدی", "کشتی فرنگی", "کشتی آزاد", "تکواندو", "ووشو", "کیک‌بوکسینگ", "ژیمناستیک ریتمیک", "پرش با نیزه", "پرتاب چکش", "ده‌گانه", "ورزش سوارکاری", "اسلالوم"],
            "آب و هوا": ["باران", "برف", "طوفان", "گرم", "سرد", "بهار", "تابستان", "پاییز", "زمستان", "رعد", "برق", "ابر", "مه", "خاک", "گرد و غبار", "سیل", "خشکسالی", "تگرگ", "یخ", "دود", "ماسه", "طوفان شن", "طوفان برف", "ابرهای سیاه", "آسمان صاف", "آسمان ابری", "رنگ پاییزی", "سرمای شدید", "گرمای شدید", "رعد و برق شدید", "نسیم ملایم", "باد شدید", "گردباد", "توفان گرمسیری", "باران اسیدی", "شبنم", "یخبندان", "برفک", "باران سیل‌آسا", "تگرگ بزرگ", "رعد و برق درخشان", "آسمان ارغوانی", "غروب آتشین", "طلوع طلایی", "مه صبحگاهی", "باد موسمی", "طوفان دریایی", "گرد و غبار کویری", "بارش برف سنگین", "کولاک", "رگبار", "نم نم باران", "آفتاب سوزان", "آسمان تاریک", "ابری شدن ناگهانی"],
            "موسیقی": ["پیانو", "گیتار", "ویولن", "نی", "تار", "سه‌تار", "دهل", "طبل", "سنتور", "قانون", "فلوت", "کلارینت", "کنسرت", "ارکستر", "نوازنده", "خواننده", "نت", "ریتم", "ملودی", "هارمونی", "موسیقی سنتی", "موسیقی پاپ", "موسیقی راک", "موسیقی جاز", "موسیقی کلاسیک", "موسیقی الکترونیک", "رپ", "موسیقی محلی", "بیس", "ساز زنده", "میکروفون", "آمپلی‌فایر", "هدفون", "صفحه گرامافون", "دی‌جی", "گیتار بیس", "درامز", "ساز کوبه‌ای", "ساز بادی", "سمفونی", "اپرا", "تک‌نوازی", "هم‌نوازی", "استودیو ضبط", "میکسر", "کابل صدا", "کنسول دی‌جی", "سازهای زهی", "سازهای بادی چوبی", "سازهای برنجی", "سازهای کوبه‌ای", "آکاردئون", "ارگ", "هارپ", "ماندولین", "بنجو", "ساکسیفون", "ترومپت", "ترومبون", "هورن", "ابوا", "فاگوت", "ویولن‌سل", "کنترباس", "فلوت پیکولو", "کمانچه", "دوتار", "تنبور", "دف", "تمبک", "ساز دهنی"],
            "فرهنگ و آیین": ["عروسی", "عید", "مذهبی", "رقص محلی", "لباس سنتی", "غذا", "سنت", "زبان", "لهجه", "افسانه", "ضرب‌المثل", "بازی", "عروسک", "نمایش", "تئاتر", "سینما", "فیلم", "ادبیات", "شعر", "داستان", "رمان", "کتاب", "کتابخانه", "موزه", "گالری", "نمایشگاه", "جشنواره", "بازار محلی", "رقص محلی", "لباس سنتی", "نقاب سنتی", "سفره هفت‌سین", "شب یلدا", "هالووین", "کریسمس", "نوروز", "سیزده‌به‌در", "چهارشنبه‌سوری", "جشن مهرگان", "جشن سده", "سال نو", "عید فطر", "عید قربان", "ماه رمضان", "شب قدر", "اعتکاف", "نماز جمعه", "مسجد", "حسینیه", "تکیه", "مراسم خواستگاری", "عقدکنان", "دید و بازدید", "عیدی دادن", "سبزه‌سبز کردن", "فال حافظ", "فال کوفی", "نخل‌گردانی", "علم‌گردانی"],
            "معماری": ["ساختمان", "خانه", "ویلا", "آپارتمان", "پل", "برج", "کلیسا", "مسجد", "کنیسه", "معبد", "قلعه", "دژ", "ارگ", "شهر باستانی", "خرابه", "کاخ", "تالار", "ایوان", "حیاط", "بام", "درگاه", "پنجره", "در", "ستون", "طاق", "گنبد", "آرامگاه", "بنای تاریخی", "آسمانخراش", "خانه‌های سنتی", "عمارت", "بارگاه", "ایستگاه قطار", "فرودگاه", "استادیوم", "مجتمع تجاری", "برج دوقلو", "برج میلاد", "برج ایفل", "دیوار بزرگ", "باغ معلق", "خانه شیشه‌ای", "بتن مسلح", "طرح مدرن", "طرح کلاسیک", "آجرنما", "سنگ‌نما", "گنبد طلایی", "مناره", "شبستان", "حرم", "ضریح", "ایوان بزرگ", "تالار آیینه", "پل معلق", "ساختمان سبز", "طراحی پایدار", "سازه فلزی", "قوس‌های رومی", "ستون‌های یونانی", "معماری گوتیک", "معماری رنسانس", "معماری اسلامی", "معماری ایرانی", "معماری هخامنشی", "معماری ساسانی"],
            "لباس": ["پیراهن", "شلوار", "دامن", "کت", "پالتو", "بافت", "تیشرت", "کلاه", "کفش", "بوت", "صندل", "روسری", "مانتو", "چادر", "عبا", "کیف", "کمربند", "دستکش", "شال", "گرمه", "عینک", "آویز", "گوشواره", "انگشتر", "ساعت", "پاپیون", "کراوات", "شلوار جین", "شورت", "لباس خواب", "مایو", "لباس عروس", "لباس نظامی", "روپوش", "جلیقه", "کت‌وشلوار", "دستکش چرمی", "کفش پاشنه‌دار", "کفش کتونی", "کلاه لبه‌دار", "کلاه نمدی", "شال گردن", "پالتو چرمی", "بافت یقه اسکی", "لباس زیر", "جوراب", "دامن تا زانو", "شلوارک", "بارانی", "لباس مجلسی", "پوشش صورت", "ماسک", "دستمال گردن", "کیف کمری", "کوله‌پشتی", "جوراب شلواری", "لباس ورزشی", "لباس کار", "لباس اداری", "لباس سنتی", "چادر شب", "روپوش طبی", "تیپار", "سارافون", "شلوار پلنگی", "کت خز"],
            "حشرات": ["زنبور", "مورچه", "پروانه", "سوسک", "مگس", "پشه", "کک", "شپش", "هزارپا", "موریانه", "عقرب", "رتیل", "مارمولک", "قورباغه", "وزغ", "حلزون", "کرم", "لارو", "پیله", "شاخک", "بال", "چشم", "دهان", "سم", "گزش", "نیش", "سوسک کرگدنی", "شب‌پره", "مگس سرکه", "کفشدوزک", "زنبور عسل", "پروانه ملوانی", "عقرب سیاه", "رتیل پرنده", "کرم ابریشم", "مگس گند", "پشه خون‌آشام", "شپش سر", "هزارپای غول‌پیکر", "سنجاقک", "آسیابک", "کرم شب‌تاب", "زنبور وحشی", "سوسک شاخدار", "پروانه دم‌چلچله‌ای", "پروانه شب", "کرم برگ‌خوار", "شته", "کنه", "عنکبوت", "مگس اسب", "سوسک آبی", "پروانه مونارک", "زنبور گرده‌آور", "مورچه قرمز", "موریانه چوب‌خوار"],
            "سینما و فیلم": ["فیلم سینمایی", "سریال", "مستند", "انیمیشن", "فیلم کوتاه", "فیلمنامه", "کارگردان", "تهیه‌کننده", "بازیگر", "بدلکار", "فیلمبردار", "تدوینگر", "صدابردار", "طراحی صحنه", "طراحی لباس", "گریم", "جلوه‌های ویژه", "موسیقی متن", "آهنگساز", "فیلمنامه‌نویس", "داستان", "دیالوگ", "نقش", "شخصیت", "قهرمان", "ضدقهرمان", "تعلیق", "هیجان", "اکشن", "درام", "کمدی", "ترسناک", "وحشت", "علمی-تخیلی", "فانتزی", "تاریخی", "عاشقانه", "جنایی", "معمایی", "پلیسی", "جنگی", "خانوادگی", "موزیکال", "فیلم مستقل", "فیلم خارجی", "فیلم ایرانی", "جشنواره فیلم", "اکران", "بلیت", "سینما", "نقد فیلم", "جایزه اسکار", "جشنواره کن", "جشنواره ونیز", "جشنواره برلین", "جشنواره فجر", "سیمرغ بلورین", "فیلم کلاسیک", "فیلم پرفروش", "اکران ویژه", "دوبله", "زیرنویس", "تیزر", "تریلر", "پوستر فیلم", "فیلمبرداری", "نورپردازی", "نما", "سکانس", "پلان", "برداشت", "مونتاژ", "صداگذاری", "لوکیشن", "صحنه", "پشت صحنه", "فیلم‌سازی", "سینمای ایران", "سینمای هالیوود", "سینمای اروپا", "سینمای هند", "سینمای کره", "سینمای ژاپن", "انیمیشن سه‌بعدی"],
            "اسب و کالسکه": ["اسب", "اسب سفید", "اسب سیاه", "کالسکه", "زین", "افسار", "لقمه", "مهار", "دام", "سم", "دم", "یال", "چرم", "فلز", "چوب", "طلا", "نقره", "شوالیه", "شاهزاده", "پرنسس", "ملکه", "پادشاه", "سوارکار", "تیرانداز", "کماندار", "شمشیرزن", "نعل", "چرخ", "گاری", "اسب‌سواری", "مسابقه اسب", "اسب چوبی", "اسب سواری جنگی", "کره‌ای", "اسب عربی", "اسب وحشی", "اسب قهوه‌ای", "کالسکه سلطنتی", "گاری چوبی", "زین چرمی", "لگام نقره", "چرم زین", "تازیانه", "پالان", "پیشانی‌بند", "گام", "یورتمه", "تاخت", "چهارنعل", "پرش اسب", "اصطبل", "علفخوار", "اسب نریان", "مادیان", "کره اسب", "اسب مسابقه", "اسب آموزش‌دیده", "اسب بارکش", "کالسکه عروس"],
            "شخصیت‌های خیالی": ["تک‌شاخ", "گریفین", "پرنده مگس‌خوار", "اسب بالدار", "اژدها", "غول", "کوتوله", "الف", "پری", "ساحره", "جادوگر", "شیطان", "فرشته", "روح", "خون‌آشام", "مومیایی", "زامبی", "اسکلت", "گوژپشت", "گرگینه", "مینوتور", "سیندرلا", "سفیدبرفی", "رابین‌هود", "بتمن", "سوپرمن", "مرد عنکبوتی", "کاپیتان آمریکا", "آیرون‌من", "ثور", "هالک", "وندر وومن", "فلش", "آکوامن", "پیکاچو", "ماریو", "لینک", "سونیک", "دونکی کنگ", "لوفی", "ناروتو", "گوكو", "علاءالدین", "سندباد", "شهرزاد", "علی‌بابا", "کلاغ سیاه", "فونیکس", "پگاسوس", "سانتا", "دزد دریایی", "کابوی", "جادوگر سفید", "جنگجوی سیاه", "شاهزاده جادوگر", "دختر پری", "پسر گرگ", "سوارکار شب"],
            "عناصر طبیعی": ["آتش", "آب", "خاک", "هوا", "برف", "یخ", "باران", "تگرگ", "مه", "دود", "گرد و غبار", "ماسه", "گل", "سنگ", "صخره", "کانی", "کوه", "دره", "دریا", "اقیانوس", "چشمه", "آبشار", "دریاچه", "برکه", "جنگل", "بیابان", "مرتع", "کویر", "رودخانه", "نهر", "چشمه آب گرم", "حوزه آبریز", "کوهستان آتشفشانی", "غار زمستانی", "سرداب یخی", "جنگل بارانی", "سنگ‌زار", "تپه شنی", "صخره مرجانی", "کویر نمکی", "آتشفشان فعال", "چشمه گوگردی", "غار سنگی", "رودخانه زیرزمینی", "یخچال طبیعی", "تالاب آب شیرین", "گرداب", "تپه", "دامنه", "قله", "دریاچه نمک", "مرداب", "چشمه آب معدنی", "آهک", "گچ", "رس", "سنگ آذرین", "سنگ دگرگونی", "سنگ رسوبی", "کانی فلزی", "کانی غیرفلزی", "گوه", "دره عمیق"],
            "حرفه‌ها": ["پزشک", "مهندس", "معلم", "نظامی", "پلیس", "آتش‌نشان", "خلبان", "ملوان", "راننده", "آشپز", "نوازنده", "نقاش", "نویسنده", "شاعر", "بازیگر", "کارگردان", "عکاس", "روزنامه‌نگار", "وکیل", "قاضی", "کارگر", "کارمند", "مدیر", "رئیس", "کارآفرین", "فروشنده", "کشاورز", "نجار", "آهنگر", "خیاط", "قصاب", "نانوا", "قناد", "کافی‌شاپ‌دار", "باغبان", "جراح", "روانشناس", "معمار", "شهرساز", "برنامه‌نویس", "تحلیلگر", "حسابدار", "مربی", "مترجم", "دیپلمات", "سفیر", "روحانی", "خطیب", "منجم", "زمین‌شناس", "زیست‌شناس", "شیمیدان", "فیزیکدان", "ریاضی‌دان", "ستاره‌شناس", "دامپزشک", "داروساز", "متخصص", "رادیولوژیست", "پرستار"],
            "مناسبت‌ها": ["عاشورا", "محرم", "تعزیه", "سینه‌زنی", "خیمه", "پرچم سیاه", "شب یلدا", "سفره هفت‌سین", "نوروز", "رمضان", "افطاری", "کریسمس", "عید فطر", "عزاداری", "روضه", "علم", "بیرق", "مولودی", "سفره", "شمع", "مسجد", "حسینیه", "امامزاده", "چله", "نخل", "علم‌گردانی", "عروسی", "سالگرد", "تولد", "فستیوال", "هالووین", "ولنتاین", "سیزده‌به‌در", "چهارشنبه‌سوری", "جشن مهرگان", "جشن سده", "شب قدر", "اعتکاف", "عید قربان", "عید غدیر", "تاسوعا", "اربعین", "پیاده‌روی اربعین", "مراسم تحویل سال", "دید و بازدید", "عیدی دادن", "سبزه‌سبز کردن", "فال حافظ", "شب عید", "سفره افطار", "قرائت قرآن", "دعای کمیل", "دعای ندبه", "جشنواره نوروزی", "آتش‌بازی", "جشن تولد", "مراسم خواستگاری", "عقد و ازدواج"]
        };

        const dict = {
            "و":"and","با":"with","در":"in","روی":"on","زیر":"under","بکنار":"next to","كنار":"next to","برای":"for","از":"from","به":"to","تا":"until","که":"that","اما":"but","یا":"or","چون":"because","اگر":"if","همچنین":"also","هم":"also","نه":"no","بله":"yes","بدون":"without","درباره":"about","مثل":"like","مانند":"like","بهترین":"best",
            "من":"I","تو":"you","او":"he/she","ما":"we","شما":"you","آنها":"they","این":"this","آن":"that","خود":"self",
            "است":"is","هست":"is","بود":"was","شد":"became","دارد":"has","داشته":"has","ایستاده":"standing","نشسته":"sitting","خوابیده":"lying","می‌دود":"running","پرواز می‌کند":"flying","نگاه می‌کند":"looking","می‌خندد":"laughing","گریه می‌کند":"crying","می‌خورد":"eating","می‌نوشد":"drinking","می‌برد":"carrying","نگه می‌دارد":"holding","می‌سازد":"building","ویران شده":"destroyed","در حال شکستن":"breaking","در حال افتادن":"falling","در حال پریدن":"jumping","در حال شنا کردن":"swimming","در حال نبرد":"fighting","محافظت می‌کند":"protecting","حمله می‌کند":"attacking","فرار می‌کند":"escaping","پنهان شده":"hidden","پیدا شده":"found","می‌بالد":"flying","می‌خزد":"crawling","راه می‌رود":"walking","می‌خوابد":"sleeping",
            "زیبا":"beautiful","زشت":"ugly","بزرگ":"big","کوچک":"small","عظیم":"huge","غول‌پیکر":"giant","کوتاه":"short","بلند":"tall","پهن":"wide","باریک":"narrow","ضخیم":"thick","نازک":"thin","سنگین":"heavy","سبک":"light","تیز":"sharp","کند":"blunt","تازه":"fresh","کهنه":"old","جدید":"new","باستانی":"ancient","مدرن":"modern","سنتی":"traditional","ساده":"simple","پیچیده":"complex","تمیز":"clean","کثیف":"dirty","خالی":"empty","پر":"full","روشن":"bright","تاریک":"dark","شفاف":"transparent","تار":"blurry","واضح":"clear","دقیق":"precise","مبهم":"ambiguous","سریع":"fast","قوی":"strong","ضعیف":"weak","قدرتمند":"powerful","خسته":"tired","پرانرژی":"energetic","آرام":"calm","خشن":"rough","ملایم":"gentle","خشک":"dry","خیس":"wet","سرد":"cold","گرم":"warm","داغ":"hot","یخ":"ice","جذاب":"attractive","ترسناک":"scary","هولناک":"terrifying","عجیب":"strange","غریب":"weird","معمولی":"normal","خاص":"special","منحصر به فرد":"unique","افسانه‌ای":"legendary","جادویی":"magical","وهم‌انگیز":"hallucinatory","سورئال":"surreal","هیجان‌انگیز":"exciting","حرفه‌ای":"professional","آماتور":"amateur","دوست‌داشتنی":"lovely","تنفرآور":"disgusting",
            "قرمز":"red","آبی":"blue","سبز":"green","زرد":"yellow","مشکی":"black","سفید":"white","نارنجی":"orange","بنفش":"purple","صورتی":"pink","قهوه‌ای":"brown","طوسی":"gray","نقره‌ای":"silver","طلایی":"golden","برنزی":"bronze","شفاف":"transparent","رنگارنگ":"colorful",
            "چوب":"wood","فلز":"metal","آهن":"iron","طلا":"gold","نقره":"silver","برنز":"bronze","سنگ":"stone","مرمر":"marble","شیشه":"glass","پلاستیک":"plastic","خاک رس":"clay","بتن":"concrete","آجر":"brick","پارچه":"fabric","ابریشم":"silk","پشم":"wool","چرم":"leather","مخمل":"velvet","خشن":"rough","نرم":"soft","صاف":"smooth","براق":"shiny","مات":"matte",
            "نقاشی":"painting","مجسمه":"sculpture","طرح":"design","آبرنگ":"watercolor","رنگ روغن":"oil paint","نورپردازی":"lighting","نور":"light","سایه":"shadow","تبادل نور":"chiaroscuro","جلوه نور":"glow","درخشش":"shimmer","انعکاس":"reflection","پرتو":"beam","حجمی":"volumetric","نئونی":"neon","طبیعی":"natural","محراب":"studio",
            "انسان":"human","مرد":"man","زن":"woman","پسر":"boy","دختر":"girl","کودک":"child","نوزاد":"baby","خانواده":"family","دوست":"friend","دشمن":"enemy","پادشاه":"king","ملکه":"queen","شاهزاده":"prince","شاهزاده خانم":"princess","سرباز":"soldier","فرمانده":"commander","پزشک":"doctor","معلم":"teacher","هنرمند":"artist","نویسنده":"writer","خواننده":"singer","نوازنده":"musician","سارق":"thief","قاتل":"killer","قهرمان":"hero","جادوگر":"wizard","جنگجو":"warrior","شکارچی":"hunter","ماهیگیر":"fisherman","کشاورز":"farmer","کارگر":"worker","تاجر":"merchant","مسافر":"traveler",
            "سر":"head","مو":"hair","چشم":"eye","گوش":"ear","بینی":"nose","دهان":"mouth","لب":"lip","دندان":"tooth","زبان":"tongue","گردن":"neck","شانه":"shoulder","بازو":"arm","دست":"hand","انگشت":"finger","سینه":"chest","شکم":"stomach","پشت":"back","کمر":"waist","پا":"leg/foot","زانو":"knee","مچ":"ankle","پاشنه":"heel",
            "زمان":"time","مکان":"place","فضا":"space","امروز":"today","فردا":"tomorrow","دیروز":"yesterday","حال":"present","گذشته":"past","آینده":"future","صبح":"morning","ظهر":"noon","عصر":"evening","شب":"night","بامداد":"dawn","سال":"year","ماه":"month","هفته":"week","روز":"day","ساعت":"hour","دقیقه":"minute","ثانیه":"second","راست":"right","چپ":"left","بالا":"up","پایین":"down","جلو":"front","عقب":"back","داخل":"inside","بیرون":"outside",
            "جنگل":"forest","کوهستان":"mountain","اقیانوس":"ocean","آسمان":"sky","رودخانه":"river","صحرا":"desert","دشت":"plain","آبشار":"waterfall","غروب":"sunset","طلوع":"sunrise","باران":"rain","برف":"snow","پاییز":"autumn","بهار":"spring","تابستان":"summer","زمستان":"winter","گل":"flower","درخت":"tree","ابر":"cloud","رعد":"thunder","طوفان":"storm","جزیره":"island","خلیج":"gulf","چشمه":"spring","غار":"cave","دره":"valley","صخره":"rock","شن":"sand","ماسه":"sand","مرتع":"meadow","کویر":"desert","دریاچه":"lake","برکه":"pond","یخچال":"glacier","تالاب":"wetland","طبیعت بکر":"pristine nature","جنگل کاج":"pine forest","صخره‌های مرجانی":"coral reefs","آب‌های فیروزه‌ای":"turquoise waters","رود یخ‌زده":"frozen river","شکوفه‌های بهاری":"spring blossoms","خزان پاییزی":"autumn foliage","کویر بی‌انتها":"endless desert","دشت ستاره‌ها":"starry plain","غار زیرآبی":"underwater cave",
            "اژدها":"dragon","قصر":"castle","جادوگر":"wizard","الف":"elf","کوتوله":"dwarf","جنگجو":"warrior","شمشیر":"sword","سپر":"shield","تاج":"crown","نیروی جادویی":"magic power","جنگل تاریک":"dark forest","پری":"fairy","اهریمن":"demon","فرشته":"angel","قهرمان":"hero","گنج":"treasure","نقشه قدیمی":"old map","معبد":"temple","طلسم":"spell","معجزه":"miracle","روح":"ghost","خفاش":"bat","گرگ":"wolf","کلاغ":"crow","کتاب جادو":"spellbook","پیامرسان":"messenger","سوارکار":"rider","اسب بالدار":"winged horse","قنادیس":"qandis","ساحره":"witch","غول":"giant","گoblin":"goblin","قوی سیاه":"black swan","پری دریایی":"mermaid","سنگ جادو":"magic stone","الف تاریک":"dark elf","جادوگر خبیث":"wicked wizard","شهریار اژدها":"dragon lord","شهر گمشده":"lost city","شمشیر نور":"sword of light","سپر آهنین":"iron shield","معبد طلایی":"golden temple","پری مه‌انگار":"mist fairy","گرگینه":"werewolf","خفاش غول‌پیکر":"giant bat","قطره خون":"drop of blood","چشم شیطانی":"demonic eye",
            "ربات":"robot","کامپیوتر":"computer","کابل":"cable","هولوگرام":"hologram","شهر هوشمند":"smart city","ماشین پرواز":"flying car","لیزر":"laser","چیپ":"chip","هوش مصنوعی":"artificial intelligence","واقعیت مجازی":"virtual reality","فضاپیما":"spaceship","موتور":"engine","برق":"electricity","باتری":"battery","مانیتور":"monitor","کیبورد":"keyboard","موشواره":"mouse","ایستگاه فضایی":"space station","پهپاد":"drone","میکروچیپ":"microchip","شبکه":"network","سرور":"server","داده":"data","کد":"code","مدار":"circuit","ترانزیستور":"transistor","آنتن":"antenna","ماهواره":"satellite","رباتیک":"robotics","آرما":"arma","پرینتر سه‌بعدی":"3d printer","واقعیت افزوده":"augmented reality","بلاکچین":"blockchain","متاورس":"metaverse","نورون مصنوعی":"artificial neuron","کابل نوری":"optical cable","سرور رک":"rack server","چیپ کوانتومی":"quantum chip","گجت پوشیدنی":"wearable gadget","نانوبات":"nanobot","هولوگرام سه‌بعدی":"3d hologram","موتور مغناطیسی":"magnetic engine","شهر سایبری":"cyber city","ایستگاه مداری":"orbital station","دوربین چتری":"umbrella camera","هوش عمومی":"general intelligence","متالورژی پیشرفته":"advanced metallurgy",
            "کهکشان":"galaxy","سیاره":"planet","ستاره":"star","ماه":"moon","خورشید":"sun","سوراخ سیاه":"black hole","شهاب":"meteor","مذنب":"comet","فضانورد":"astronaut","کاشف":"explorer","جرم":"mass","نور":"light","تاریکی":"darkness","بعد":"dimension","زمان":"time","جهان":"universe","ملکوتی":"celestial","فرازمینی":"extraterrestrial","مدارگرد":"orbiter","پرتاب":"launch","سوخت":"fuel","ایستگاه":"station","رقاص":"pendulum","مریخ":"mars","زهره":"venus","مشتری":"jupiter","زحل":"saturn","اورانوس":"uranus","نپتون":"neptune","عطارد":"mercury","ستاره دنباله‌دار":"comet","سحابی":"nebula","اخترشناس":"astronomer","تلسکوپ فضایی":"space telescope","کهکشان مارپیچ":"spiral galaxy","سیاره سرخ":"red planet","کمربند سیارکی":"asteroid belt","سحابی اسب سر":"horsehead nebula","حلقه زحل":"rings of saturn","کره خورشیدی":"solar globe","انفجار گامارای":"gamma ray burst","ماده تاریک":"dark matter","کرم‌چاله":"wormhole","زمان نسبی":"relative time","ابر خوشه":"supercluster","اجرام دور":"distant objects",
            "آسمانخراش":"skyscraper","خیابان":"street","ماشین":"car","ترافیک":"traffic","پارک":"park","مترو":"subway","پل":"bridge","بندر":"port","کافه":"cafe","رستوران":"restaurant","فروشگاه":"shop","چراغ راهنما":"traffic light","پیاده‌رو":"sidewalk","دوربین":"camera","تبلیغات":"advertisements","مردم":"people","شلوغ":"crowded","شب":"night","روز":"day","باران شهری":"city rain","حومه":"suburb","مرکز":"center","بازار":"market","میدان":"square","اتوبان":"highway","کوچه":"alley","ساختمان اداری":"office building","مسکن":"housing","بیلبورد":"billboard","تاکسی":"taxi","اتوبوس":"bus","ایستگاه قطار":"train station","دوربین مداربسته":"cctv","چراغ‌های نئونی":"neon lights","بن‌بست":"dead end","خیابان سنگ‌فرش":"cobblestone street","پله برقی":"escalator","پل عابر":"pedestrian bridge","میدان بزرگ":"grand square","ساعت سنتی":"traditional clock","باغ شهری":"city garden","حومه صنعتی":"industrial suburb","مسیر دوچرخه":"bicycle path","ایستگاه تاکسی":"taxi stand","فروشگاه زنجیره‌ای":"chain store",
            "چهره مرد":"male face","چهره زن":"female face","کودک":"child","سالمند":"elderly","هنرمند":"artist","نگاه عمیق":"deep gaze","خنده":"laughter","غصه":"sorrow","آرامش":"peace","عصبانیت":"anger","چشم":"eye","لب":"lip","موی بلند":"long hair","موی کوتاه":"short hair","ریش":"beard","کلاه":"hat","عینک":"glasses","آرایش":"makeup","طبیعی":"natural","استودیو":"studio","پس‌زمینه":"background","نور طبیعی":"natural light","نیم‌رخ":"profile","تمام قد":"full body","محیط کار":"work environment","رسمی":"formal","اسپرت":"sporty","خالکوبی":"tattoo","پیرسینگ":"piercing","گریم":"makeup","مدل":"model","بازیگر":"actor","خواننده":"singer","ورزشکار":"athlete","نویسنده":"writer","نگاه کناری":"side glance","چشم‌های آبی":"blue eyes","لب‌های پر":"full lips","چهره رنگ‌پریده":"pale face","خالکوبی صورت":"face tattoo","کلاه لبه‌دار":"brimmed hat","عینک آفتابی":"sunglasses","آرایش تیره":"dark makeup","آرایش ملایم":"soft makeup","موهای فرفری":"curly hair","ریش بلند":"long beard","پیرمرد چروک":"wrinkled old man",
            "شیر":"lion","ببر":"tiger","گرگ":"wolf","کفتار":"hyena","اسب":"horse","گوزن":"deer","عقاب":"eagle","شاهین":"falcon","گربه":"cat","سگ":"dog","خرس":"bear","فیل":"elephant","ماهی":"fish","کوسه":"shark","نهنگ":"whale","دلفین":"dolphin","لاکپشت":"turtle","مار":"snake","کروکودیل":"crocodile","پرنده":"bird","مرغ":"chicken","اردک":"duck","خرگوش":"rabbit","موش":"mouse","میمون":"monkey","گوریل":"gorilla","حشره":"insect","زرافه":"giraffe","گورخر":"zebra","کرگدن":"rhinoceros","کنگورو":"kangaroo","پاندا":"panda","ببر سفید":"white tiger","یوزپلنگ":"cheetah","روباه":"fox","جغد":"owl","کبوتر":"pigeon","طاووس":"peacock","طوطی":"parrot","مار گرمسیری":"tropical snake","قورباغه شاخ‌دار":"horned frog","پلنگ برفی":"snow leopard","گربه وحشی":"wildcat","ماهی مرکب":"squid","هشت‌پا":"octopus","عقاب دریایی":"sea eagle","کرکور":"vulture","لاک‌پشت غول‌پیکر":"giant turtle",
            "همبرگر":"hamburger","پیتزا":"pizza","سالاد":"salad","میوه":"fruit","سیب":"apple","موز":"banana","انار":"pomegranate","انگور":"grape","کیک":"cake","شکلات":"chocolate","بستنی":"ice cream","قهوه":"coffee","چای":"tea","آب":"water","نوشابه":"soda","پاستا":"pasta","برنج":"rice","گوشت":"meat","مرغ":"chicken","ماهی سرخ شده":"fried fish","سوپ":"soup","نان":"bread","پنیر":"cheese","تخم مرغ":"egg","سوسیس":"sausage","کباب":"kebab","دسر":"dessert","شیرینی":"sweet","کلوچه":"cookie","پاپ کورن":"popcorn","پنکیک":"pancake","وافل":"waffle","بشمک":"cupcake","نودل":"noodle","سوشی":"sushi","کاپوچینو":"cappuccino","لاته":"latte","چای سبز":"green tea","آب‌میوه":"juice","خربوزه":"melon","هندوانه":"watermelon","گیلاس":"cherry","توت‌فرنگی":"strawberry","کله‌پاچه":"kale pache","دیزی":"dizi","حلیم":"haleem","فسنجان":"fesenjan",
            "ماشین مسابقه":"racing car","ماشین کلاسیک":"classic car","ماشین شاسی‌بلند":"suv","موتور سیکلت":"motorcycle","کامیون":"truck","اتوبوس":"bus","هواپیما":"airplane","هلیکوپتر":"helicopter","قایب":"boat","کشتی":"ship","دوچرخه":"bicycle","واگن":"wagon","قطار":"train","تراموا":"tram","کشنده":"trailer","تانک":"tank","زرهی":"armored","آمبولانس":"ambulance","پلیس":"police car","آتش‌نشانی":"fire truck","بیل مکانیکی":"excavator","لودر":"loader","جرثقیل":"crane","تراکتور":"tractor","گاری":"cart","زیردریایی":"submarine","جت":"jet","بالگرد":"helicopter","هاواناو":"hovercraft","ماشین اسب‌بازی":"toy car","کالسکه اسب":"horse carriage","کشتی بادبانی":"sailing ship","گلایدر":"glider","کایاک":"kayak","ماشین پلیس":"police car","ماشین شاسی‌کوتاه":"low chassis car","ماشین کروک":"convertible","ماشین دست‌ساز":"handmade car","ماشین بخار":"steam car","قطار سریع‌السیر":"express train","قطار باری":"freight train","کشتی نفت‌کش":"oil tanker","زیردریایی اتمی":"nuclear submarine","جنگنده رادارگریز":"stealth fighter","بالگرد تجاری":"commercial helicopter","پهپاد نظامی":"military drone",
            "شاهنشاه":"emperor","سلطان":"sultan","شوالیه":"knight","معبد":"temple","قلعه":"castle","اسلحه":"weapon","شمشیر":"sword","سپر":"shield","تیر":"arrow","کمان":"bow","زره":"armor","صلیب":"cross","تاج":"crown","تخت":"throne","سکه":"coin","پیمان":"covenant","نقشه":"map","جنگ":"war","صلح":"peace","پادشاهی":"kingdom","امپراتوری":"empire","جمهوری":"republic","سنتی":"traditional","باستانی":"ancient","عتیقه":"antique","سند":"document","خط میخی":"cuneiform","هیروگلیف":"hieroglyph","یونان":"greece","رم":"rome","پارس":"persia","مصر":"egypt","چین باستان":"ancient china","ژاپن فئودال":"feudal japan","سپاه جاویدان":"immortal army","ارتش روم":"roman army","گلادیاتور":"gladiator","سامورایی":"samurai","وایکینگ":"viking","کاوبوی":"cowboy","دزدان دریایی":"pirates","قلعه متروک":"abandoned castle","خرابه‌های روم":"roman ruins","معبد یونانی":"greek temple","اهرام مصر":"egyptian pyramids","دیوار چین":"great wall of china","تاج‌وتخت":"throne",
            "نقاشی":"painting","مجسمه":"sculpture","گرافیتی":"graffiti","طرح":"design","آبرنگ":"watercolor","رنگ روغن":"oil paint","مداد":"pencil","ذغال":"charcoal","خاک رس":"clay","سفال":"pottery","کار دست":"handicraft","فرش":"carpet","موزاییک":"mosaic","شیشه":"glass","چوب":"wood","فلز":"metal","آهن":"iron","طلا":"gold","نقره":"silver","برنز":"bronze","سنگ":"stone","مرمر":"marble","کلاژ":"collage","خوشنویسی":"calligraphy","تذهیب":"illumination","مینیاتور":"miniature","نقاشی دیواری":"mural","تندیس":"statue","مجسمه‌سازی":"sculpting","طراحی صنعتی":"industrial design","گرافیک":"graphic","تایپوگرافی":"typography","طراحی پوستر":"poster design","کارت پستال":"postcard","طراحی لوگو":"logo design","طرح دست‌ساز":"handmade design","نقاشی دیجیتال":"digital painting","طراحی سه‌بعدی":"3d design","مجسمه برنزی":"bronze statue","آهنگری فلز":"metal forging","شیشه‌گری":"glassblowing","چوب‌بری":"woodcarving","فرش دستباف":"handwoven carpet","طراحی داخلی":"interior design","طراحی لباس":"fashion design","نقاشی چهره":"portrait painting","پیکرتراشی":"sculpture",
            "آزمایشگاه":"laboratory","میکروسکوپ":"microscope","تلسکوپ":"telescope","شیمی":"chemistry","فیزیک":"physics","بیولوژی":"biology","مولکول":"molecule","اتم":"atom","الکترون":"electron","انرژی":"energy","موج":"wave","صوت":"sound","الکتریسیته":"electricity","مگنت":"magnet","گرما":"heat","سرما":"cold","فشار":"pressure","شعاع":"ray","اشعه":"radiation","لایز":"laser","پلاسما":"plasma","گاز":"gas","مایع":"liquid","جامد":"solid","واکنش":"reaction","فرمول":"formula","ریاضیات":"mathematics","هندسه":"geometry","جبر":"algebra","آمار":"statistics","اخترفیزیک":"astrophysics","نانوتکنولوژی":"nanotechnology","بیولوژی مولکولی":"molecular biology","شیمی آلی":"organic chemistry","کوانتوم":"quantum","گرانش":"gravity","نسبیت":"relativity","سیاه‌چاله":"black hole","ستاره نوترونی":"neutron star","ژنتیک":"genetics","سلول بنیادی":"stem cell","ویروس":"virus","باکتری":"bacteria","واکسن":"vaccine",
            "شادی":"happiness","غم":"sadness","عشق":"love","ترس":"fear","خشم":"anger","استرس":"stress","امید":"hope","ناامیدی":"despair","تنهایی":"loneliness","رنجش":"resentment","سوگواری":"mourning","خنده":"laughter","گریه":"crying","تعجب":"surprise","شرم":"shame","افتخار":"pride","حسادت":"jealousy","راستی":"truth","دروغ":"lie","وفاداری":"loyalty","خیانت":"betrayal","شجاعت":"courage","جسارت":"audacity","مهربانی":"kindness","دشمنی":"enmity","مهر":"affection","اشتیاق":"eagerness","بی‌حوصلگی":"impatience","خستگی":"fatigue","تمنا":"desire","حسرت":"regret","خداحافظی":"farewell","آغوش":"hug","سکوت":"silence","خشم کور":"blind rage","شوق":"excitement","ترس و لرز":"fear and trembling","عشق افلاطونی":"platonic love","دلتنگی":"nostalgia","پشیمانی":"remorse","بی‌تفاوتی":"apathy","اعتماد به نفس":"self-confidence","ضعف":"weakness","سرخوردگی":"frustration","وحشت":"horror","خلسه":"trance",
            "فوتبال":"football","بسکتبال":"basketball","والیبال":"volleyball","تنیس":"tennis","شنا":"swimming","دویدن":"running","کوهنوردی":"climbing","دوچرخه سواری":"cycling","شمشیربازی":"fencing","بوکس":"boxing","کاراته":"karate","جودو":"judo","وزنه برداری":"weightlifting","کشتی":"wrestling","هاکی":"hockey","بیسبال":"baseball","گلف":"golf","اسکی":"skiing","اسنوبورد":"snowboarding","سوارکاری":"equestrian","تیراندازی":"shooting","قایق سواری":"boating","موج سواری":"surfing","غواصی":"diving","ژیمناستیک":"gymnastics","بالی":"ballet","رقص":"dance","یوگا":"yoga","پیاده روی":"walking","پارکور":"parkour","اسکیت":"skating","ویندسرف":"windsurfing","پرش با چتر":"skydiving","پرش ارتفاع":"high jump","دو میدانی":"track and field","ماراتن":"marathon","دو سرعت":"sprint","شنای سینکروناید":"synchronized swimming","پرش سه‌گام":"triple jump","پرتاب نیزه":"javelin throw","پرتاب دیسک":"discus throw","هاکی روی یخ":"ice hockey","کرلینگ":"curling","بدمینتون":"badminton","تنیس روی میز":"table tennis","راگبی":"rugby","کریکت":"cricket",
            "هندسی":"geometric","موج":"wave","دایره":"circle","مربع":"square","مثلث":"triangle","خط":"line","نقطه":"point","فضا":"space","بعد":"dimension","زمان":"time","حرکت":"motion","سکون":"stillness","نور":"light","تاریکی":"darkness","رنگ":"color","تضاد":"contrast","هماهنگی":"harmony","آشوب":"chaos","نظم":"order","بازی":"play","توهم":"illusion","انعکاس":"reflection","سایه":"shadow","حجم":"volume","پوچی":"emptiness","معنی":"meaning","نماد":"symbol","تجرد":"abstraction","تجسم":"embodiment","فلسفه":"philosophy","فراکتال":"fractal","مینیمال":"minimal","سورئال":"surreal","مایع":"liquid","ذرات":"particles","نقاب":"mask","مکعب":"cube","بی‌نهایت":"infinity","پیچش":"twist","گره":"knot","خطوط موازی":"parallel lines","خطوط متقاطع":"intersecting lines","طیف رنگ":"color spectrum","تار و پود":"warp and weft","اسپیرال":"spiral","چرخه":"cycle","فضای سفید":"white space",
            "تگرگ":"hail","یخ":"ice","مه":"fog","دود":"smoke","گرد و غبار":"dust","گل":"mud","کانی":"mineral","دریا":"sea","برکه":"pond","بیابان":"desert","مرتع":"meadow","نهر":"stream","چشمه آب گرم":"hot spring","حوزه آبریز":"watershed","کوهستان آتشفشانی":"volcanic mountain","غار زمستانی":"winter cave","سرداب یخی":"ice crypt","جنگل بارانی":"rainforest",
            "پیانو":"piano","گیتار":"guitar","ویولن":"violin","نی":"ney","تار":"tar","سه‌تار":"setar","دهل":"dohol","طبل":"drum","سنتور":"santur","قانون":"qanun","فلوت":"flute","کلارینت":"clarinet","کنسرت":"concert","ارکستر":"orchestra","نوازنده":"musician","خواننده":"singer","نت":"note","ریتم":"rhythm","ملودی":"melody","هارمونی":"harmony","موسیقی سنتی":"traditional music","پاپ":"pop","راک":"rock","جاز":"jazz","کلاسیک":"classical","الکترونیک":"electronic","رپ":"rap","محلی":"local","بیس":"bass","ساز زنده":"live instrument","میکروفون":"microphone","آمپلی‌فایر":"amplifier","هدفون":"headphones","صفحه گرامافون":"vinyl record","دی جی":"dj","گیتار بیس":"bass guitar","درامز":"drums","ساز کوبه‌ای":"percussion instrument","ساز بادی":"wind instrument","سمفونی":"symphony","اپرا":"opera","تک‌نوازی":"solo","هم‌نوازی":"ensemble","استودیو ضبط":"recording studio","میکسر":"mixer","کابل صدا":"audio cable","کنسول دی‌جی":"dj console",
            "عروسی":"wedding","عید":"eid","مذهبی":"religious","رقص":"dance","پوشش":"clothing","غذا":"food","سنت":"tradition","زبان":"language","لهجه":"accent","افسانه":"legend","ضرب‌المثل":"proverb","بازی":"game","عروسک":"doll","نمایش":"show","تئاتر":"theater","سینما":"cinema","فیلم":"film","ادبیات":"literature","شعر":"poetry","داستان":"story","رمان":"novel","مقاله":"article","کتاب":"book","کتابخانه":"library","موزه":"museum","گالری":"gallery","نمایشگاه":"exhibition","جشنواره":"festival","همایش":"congress","وبینار":"webinar","سفارت":"embassy","گذرنامه":"passport","ویزا":"visa","مراسم":"ceremony","بازار محلی":"local market","رقص محلی":"local dance","لباس سنتی":"traditional clothing","نقاب سنتی":"traditional mask","سفره هفت‌سین":"haft-sin table","شب یلدا":"yalda night","مراسم عاشورا":"ashura ceremony","هالووین":"halloween","کریسمس":"christmas","عید فطر":"eid al-fitr","رمضان":"ramadan","آیین مذهبی":"religious ritual","تشریق":"tashriq",
            "ساختمان":"building","خانه":"house","ویلا":"villa","آپارتمان":"apartment","پل":"bridge","برج":"tower","کلیسا":"church","مسجد":"mosque","کنیسه":"synagogue","دژ":"fortress","ارگ":"citadel","شهر باستانی":"ancient city","خرابه":"ruin","کاخ":"palace","تالار":"hall","ایوان":"ivan","حیاط":"courtyard","بام":"roof","درگاه":"portal","پنجره":"window","در":"door","ستون":"column","طاق":"arch","گنبد":"dome","آرامگاه":"tomb","بنای تاریخی":"historical monument","آسمانخراش":"skyscraper","خانه‌های سنتی":"traditional houses","عمارت":"mansion","بارگاه":"court","ایستگاه قطار":"train station","فرودگاه":"airport","استادیوم":"stadium","مجتمع تجاری":"shopping mall","برج دوقلو":"twin towers","برج میلاد":"milad tower","برج ایفل":"eiffel tower","دیوار بزرگ":"great wall","باغ معلق":"hanging garden","خانه شیشه‌ای":"glass house","فلز مذاب":"molten metal","بتن مسلح":"reinforced concrete","طرح مدرن":"modern design","طرح کلاسیک":"classic design","آجرنما":"brick facade","سنگ‌نما":"stone facade",
            "تفنگ":"gun","کلت":"colt","مینی‌تان":"mini-tank","توپ":"cannon","موشک":"missile","نارنجک":"grenade","چاقو":"knife","خنجر":"dagger","زوبین":"javelin","تبر":"axe","گرز":"mace","نیزه":"spear","چماق":"club","اسلحه سرد":"cold weapon","اسلحه گرم":"firearm","مسلسل":"machine gun","کلاشنیکف":"kalashnikov","کاتانا":"katana","سامورایی":"samurai","تپانچه":"pistol","دسته‌گلوله":"hand grenade","بمب":"bomb","مین":"mine","ناپالم":"napalm","سلاح لیزری":"laser weapon","تفنگ ساچمه‌ای":"shotgun","اسلحه کمری":"handgun","قفل ماشین":"car lock","دودبار":"smoke grenade","تفنگ تک‌تیرانداز":"sniper rifle","مسلسل دستی":"submachine gun","نارنجک‌انداز":"grenade launcher","خمپاره‌انداز":"mortar","موشک‌انداز":"rocket launcher","ماگنوم":"magnum","شمشیر دولبه":"double-edged sword","خنجر زهرآگین":"poisoned dagger","سپر بالستیک":"ballistic shield","کلاهخود":"helmet","زره ضدگلوله":"bulletproof vest","گانشپ":"gunship",
            "پیراهن":"shirt","شلوار":"pants","دامن":"skirt","کت":"coat","پالتو":"overcoat","بافت":"sweater","تیشرت":"t-shirt","کفش":"shoes","بوت":"boots","صندل":"sandals","روسری":"scarf","مانتو":"manteau","چادر":"chador","عبای":"abaya","کیف":"bag","کمربند":"belt","دستکش":"gloves","شال":"shawl","گرمه":"geree","آویز":"pendant","گوشواره":"earrings","انگشتر":"ring","ساعت":"watch","پاپیون":"bowtie","کراوات":"tie","شلوار جین":"jeans","شورت":"shorts","لباس خواب":"pajamas","مایو":"swimsuit","لباس عروس":"wedding dress","لباس نظامی":"military uniform","روپوش":"lab coat","کاور":"cover","جلیقه":"vest","کت‌وشلوار":"suit","دستکش چرمی":"leather gloves","کفش پاشنه‌دار":"high heels","کفش کتونی":"sneakers","کلاه لبه‌دار":"brimmed hat","کلاه نمدی":"felt hat","شال گردن":"scarf","پالتو چرمی":"leather coat","بافت یقه اسکی":"turtleneck sweater","لباس زیر":"underwear","جوراب":"socks","دامن تا زانو":"knee-length skirt",
            "زنبور":"bee","مورچه":"ant","پروانه":"butterfly","سوسک":"beetle","مگس":"fly","پشه":"mosquito","کک":"flea","شپش":"lice","هزارپا":"centipede","موریانه":"termite","عقرب":"scorpion","رتیل":"tarantula","مارمولک":"lizard","قورباغه":"frog","وزغ":"toad","حلزون":"snail","کرم":"worm","لارو":"larva","تخم":"egg","پیله":"cocoon","کرک":"fleece","شاخک":"antenna","بال":"wing","پا":"leg","چشم":"eye","دهان":"mouth","سم":"venom","گزش":"bite","نیش":"sting","سوسک کرگدنی":"rhinoceros beetle","شب‌پره":"moth","مگس سرکه":"fruit fly","سوسک هندوانه":"watermelon beetle","كفشدوزك":"ladybug","پیرگوش":"earwig","زنبور عسل":"honeybee","مورچه گوله‌ای":"bullet ant","پروانه ملوانی":"monarch butterfly","سوسك گورخری":"tiger beetle","عقرب سیاه":"black scorpion","رتیل پرنده":"flying tarantula","كرم ابریشم":"silkworm","مگس گند":"carrion fly","پشه خون‌آشام":"bloodsucking mosquito","كك انسان":"human flea","شپش سر":"head lice","هزارپای غول‌پیکر":"giant centipede",
            "اسب سفید":"white horse","اسب سیاه":"black horse","كالسکه":"carriage","زین":"saddle","افسر":"bridle","لقمه":"bit","مهار":"harness","دام":"mare","سم":"hoof","دُم":"tail","یال":"mane","چرم":"leather","طلا":"gold","نقره":"silver","شاهزاده":"prince","پرنسس":"princess","ملكه":"queen","پادشاه":"king","تیرانداز":"archer","كماندار":"bowman","شمشیرزن":"swordsman","نعل":"horseshoe","چرخ":"wheel","گاری":"cart","اسب سواری":"horseback riding","مسابقه اسب":"horse race","اسب چوبی":"wooden horse","تله اسب":"horse trap","اسباب‌بازی":"toy","اسب سواری جنگی":"warhorse riding","اسب كره‌ای":"arabian horse","اسب عربی":"arabian horse","اسب وحشی":"wild horse","اسب قهوه‌ای":"brown horse","كالسکه سلطنتی":"royal carriage","گاری چوبی":"wooden cart","زین چرمی":"leather saddle","طناب پنجه":"lead rope","لگام نقره":"silver reins","چرم زین":"saddle leather",
            "اونیکورن":"unicorn","گریفین":"griffin","مرغ مگس‌خوار":"hummingbird","خون‌آشام":"vampire","مومیایی":"mummy","زامبی":"zombie","اسكلت":"skeleton","گوژپشت":"hunchback","مرد گرگ":"werewolf","مرد حشره":"insect man","مرد آهنی":"iron man","مرد شنی":"sand man","قطره‌ماهی":"blobfish","كراكن":"kraken","مینوتور":"minotaur","سیندرلا":"cinderella","سفیدبرفی":"snow white","رابین‌هود":"robin hood","بتمن":"batman","سوپرمن":"superman","مرد عنكبوتی":"spider-man","كاپیتان آمریکا":"captain america","آیرون‌من":"ironman","ثور":"thor","هالک":"hulk","ووندر وومن":"wonder woman","فلش":"flash","آكوامن":"aquaman","پیکاچو":"pikachu","مریو":"mario","لینك":"link","كراش":"crash","سونیک":"sonic","مگا من":"mega man","ریو":"rio",
            "آتش":"fire","هوا":"air","خاك":"soil","تگرگ":"hail","چشمه آب گرم":"hot spring","كوهستان آتشفشانی":"volcanic mountain","غار زمستانی":"winter cave","سرداب یخی":"ice crypt","جنگل بارانی":"rainforest",
            "پزشك":"doctor","مهندس":"engineer","معلم":"teacher","نظامی":"military","پلیس":"police","آتش‌نشان":"firefighter","خلبان":"pilot","ملوان":"sailor","راننده":"driver","آشپز":"chef","نقاص":"painter","شاعر":"poet","بازیگر":"actor","كارگردان":"director","عكاس":"photographer","روزنامه‌نگار":"journalist","وکیل":"lawyer","قاضی":"judge","كارگر":"worker","كارمند":"employee","مدیر":"manager","رئیس":"boss","كارآفرین":"entrepreneur","فروشنده":"seller","كشاورز":"farmer","گلدان":"florist","نجار":"carpenter","آهنگر":"blacksmith","خیاط":"tailor","قصاب":"butcher","نانوا":"baker","قناد":"confectioner","كافی‌شاپ‌دار":"cafe owner","باغبان":"gardener",
            "عاشورا":"Ashura commemoration","محرم":"Muharram mourning","تعزیه":"Ta'zieh passion play","سینه‌زنی":"rhythmic chest beating ritual","خیمه":"black mourning tent","پرچم سیاه":"black mourning flag","شب یلدا":"Yalda night winter festival","هفت‌سین":"traditional Haft-Sin table","نوروز":"Nowruz Persian New Year","افطاری":"Iftar fast-breaking meal","عید فطر":"Eid al-Fitr festival","عزاداری":"religious mourning ceremony","روضه":"religious eulogy gathering","علم":"religious ceremonial banner","بیرق":"religious black standard","مولودی":"religious birth celebration","شمع":"candlelight","مسجد":"mosque","حسینیه":"Hosseiniyeh congregation hall","امامزاده":"Imamzadeh shrine","کابل نورانی":"luminous cables","پرده":"religious curtain","چله":"Chelleh winter solstice","زار":"Zar ritual","نخل":"Nakhel palm structure","علم‌گردانی":"Alam-bearing ceremony"
        };

        const persianToLatinMap = {
            'آ': 'aa', 'ا': 'a', 'ب': 'b', 'پ': 'p', 'ت': 't', 'ث': 's',
            'ج': 'j', 'چ': 'ch', 'ح': 'h', 'خ': 'kh', 'د': 'd', 'ذ': 'z',
            'ر': 'r', 'ز': 'z', 'ژ': 'zh', 'س': 's', 'ش': 'sh', 'ص': 's',
            'ض': 'z', 'ط': 't', 'ظ': 'z', 'ع': 'a', 'غ': 'gh', 'ف': 'f',
            'ق': 'gh', 'ک': 'k', 'گ': 'g', 'ل': 'l', 'م': 'm', 'ن': 'n',
            'و': 'v', 'ه': 'h', 'ی': 'y', 'ئ': 'y',
            'َ': 'a', 'ُ': 'o', 'ِ': 'e', 'ّ': '', 'ً': 'an', 'ٌ': 'on', 'ٍ': 'en',
            ' ': ' ', '.': '.', ',': ',', '!': '!', '?': '?', '-': '-', '_': '_'
        };

        function toFinglish(text) {
            if (!text) return "";
            let result = "";
            for (let i = 0; i < text.length; i++) {
                let char = text[i];
                let mapped = persianToLatinMap[char];
                if (mapped !== undefined) {
                    result += mapped;
                } else if (/[a-zA-Z0-9\s.,!?]/.test(char)) {
                    result += char; 
                }
            }
            return result.replace(/\s+/g, ' ').trim();
        }

        let selectedWords = [];
        let history = [];
        let gallery = [];
        let editingGalleryId = null;
        let deleteTargetId = null;
        let historyPage = 1;
        let galleryPage = 1;
        let galleryFilter = 'all';
        let historySearchQuery = '';
        let isTyping = false;
        const itemsPerPage = 8;
        const galleryPerPage = 18;

        try { history = JSON.parse(localStorage.getItem('promptHistory') || '[]'); gallery = JSON.parse(localStorage.getItem('promptGallery') || '[]'); } catch (e) { history = []; gallery = []; }
        if(gallery.length === 0) {
            gallery = [
                {id: "1", title: "Cyberpunk City", text: "A cyberpunk city at night with neon lights, flying cars, rain, cinematic lighting, 8k, highly detailed", author: "Admin", image: null, category: "شهرنشینی", aiTarget: "Midjourney"},
                {id: "2", title: "Fantasy Warrior", text: "A fantasy warrior princess with silver armor and fire sword, standing in a dark forest, volumetric lighting", author: "Admin", image: null, category: "فانتزی", aiTarget: "DALL-E 3"}
            ];
            try { localStorage.setItem('promptGallery', JSON.stringify(gallery)); } catch (e) {}
        }

        const sizes = [
            "1:1 (1080x1080) - پست اینستاگرام",
            "9:16 (1080x1920) - استوری/ریلز",
            "16:9 (1920x1080) - ویدیو یوتیوب",
            "4:5 (1080x1350) - پرتره اینستاگرام",
            "1.91:1 (1200x628) - پست توییتر/لینکدین",
            "3:4 (1080x1440) - پین پینترست",
            "2:3 (1080x1620) - پرتره فیسبوک",
            "16:9 (1280x720) - هدر توییتر",
            "8:1 (5120x640) - بنر توییتر",
            "3:1 (1200x400) - هدر وب‌سایت",
            "1:2 (1080x2160) - تبلیغ اسنپ‌چت",
            "9:1 (5120x576) - بنر یوتیوب",
            "4:3 (1024x768) - صفحه نمایش استاندارد",
            "21:9 (2560x1080) - مانیتور اولترا واید",
            "5:4 (1080x864) - پست عکس تلگرام"
        ];
        const styles = [
            "Photorealistic - واقع‌گرایانه", "Cinematic - سینمایی", "Anime - انیمه", "3D Render - رندر سه‌بعدی", 
            "Watercolor - آبرنگ", "Oil Painting - نقاشی رنگ روغن", "Cyberpunk - سایبرپانک", "Steampunk - استیم‌پانک", 
            "Minimalist - مینیمال", "Pop Art - پاپ آرت", "Fantasy Art - هنر فانتزی", "Sci-Fi - علمی-تخیلی", 
            "Noir - نوآر", "Pixel Art - پیکسل آرت", "Concept Art - کانسپت آرت", "Abstract - انتزاعی", 
            "Surrealism - سورئالیسم", "Impressionism - امپرسیونیسم", "Gothic - گوتیک", "Vintage - وینتیج"
        ];
        const lightings = [
            "Soft Light - نور نرم", "Hard Light - نور سخت", "Golden Hour - ساعت طلایی", "Blue Hour - ساعت آبی", 
            "Studio Lighting - نور استودیویی", "Volumetric Lighting - نور حجمی", "Neon Lighting - نور نئونی", 
            "Backlit - نور پس‌زمینه", "Rim Light - نور حاشیه", "Natural Light - نور طبیعی", 
            "Cinematic Lighting - نورپردازی سینمایی", "Chiaroscuro - روشن و تاریک", "Bioluminescence - زیست‌تابی", 
            "Fluorescent - فلورسنت", "Candlelight - نور شمع"
        ];
        const cameras = [
            "Close-up - کلوزآپ", "Wide Angle - زاویه باز", "Aerial View - نمای هوایی", "Drone Shot - شات پهپاد", 
            "Macro - ماکرو", "Eye Level - سطح چشم", "High Angle - زاویه بالا", "Low Angle - زاویه پایین", 
            "Over the Shoulder - روی شانه", "Dutch Angle - زاویه هلندی", "Fisheye - فیش‌آی", 
            "Telephoto - تله‌فوتو", "First Person View - نمای اول شخص", "Bird's Eye View - نمای پرنده", 
            "Worm's Eye View - نمای کرم"
        ];
        const aiTargets = [
            "Midjourney - میدجورنی", "DALL-E 3 - دال-ای ۳", "Stable Diffusion - استیبل دیفیوژن", 
            "ChatGPT - چت‌جی‌پی‌تی", "Nano Banana - نانو بنانا"
        ];

        function showToast(message, type = 'info') { const container = document.getElementById('toastContainer'); const toast = document.createElement('div'); toast.className = `toast toast-${type}`; toast.innerText = message; container.appendChild(toast); setTimeout(() => toast.classList.add('show'), 10); setTimeout(() => { toast.classList.remove('show'); setTimeout(() => toast.remove(), 300); }, 3000); }
        function toggleTheme() { const currentTheme = document.documentElement.getAttribute('data-theme'); const newTheme = currentTheme === 'dark' ? 'light' : 'dark'; document.documentElement.setAttribute('data-theme', newTheme); try { localStorage.setItem('theme', newTheme); } catch (e) {} document.getElementById('themeBtn').innerHTML = newTheme === 'dark' ? '<i class="fas fa-sun"></i> <span>تم</span>' : '<i class="fas fa-moon"></i> <span>تم</span>'; }
        function loadTheme() { let savedTheme = 'light'; try { savedTheme = localStorage.getItem('theme') || 'light'; } catch (e) {} document.documentElement.setAttribute('data-theme', savedTheme); document.getElementById('themeBtn').innerHTML = savedTheme === 'dark' ? '<i class="fas fa-sun"></i> <span>تم</span>' : '<i class="fas fa-moon"></i> <span>تم</span>'; }
        function switchView(viewId) { document.querySelectorAll('.view').forEach(v => v.classList.remove('active')); document.getElementById(viewId).classList.add('active'); if(viewId === 'galleryView') { document.getElementById('backToStudioBtn').classList.remove('hidden'); renderGallery(); } else { document.getElementById('backToStudioBtn').classList.add('hidden'); } }
        function switchTab(tab) { if (tab === 'login') { document.getElementById('loginForm').classList.remove('hidden'); document.getElementById('registerForm').classList.add('hidden'); document.getElementById('tabLogin').classList.add('active'); document.getElementById('tabRegister').classList.remove('active'); } else { document.getElementById('loginForm').classList.add('hidden'); document.getElementById('registerForm').classList.remove('hidden'); document.getElementById('tabLogin').classList.remove('active'); document.getElementById('tabRegister').classList.add('active'); } }
        function handleRegister(e) { e.preventDefault(); const fname = document.getElementById('regFirstName').value; const lname = document.getElementById('regLastName').value; const user = document.getElementById('regUsername').value; const phone = document.getElementById('regPhone').value; const pass = document.getElementById('regPassword').value; document.getElementById('userError').style.display = 'none'; document.getElementById('phoneError').style.display = 'none'; if (!/^[a-zA-Z0-9]+$/.test(user)) { document.getElementById('userError').style.display = 'block'; showToast('فرمت نام کاربری اشتباه است', 'error'); return; } if (!/^09[0-9]{9}$/.test(phone)) { document.getElementById('phoneError').style.display = 'block'; showToast('فرمت شماره تلفن اشتباه است', 'error'); return; } let users = getUsers(); let userExists = Object.keys(users).some(k => k.toLowerCase() === user.toLowerCase()); if (userExists) { document.getElementById('userError').style.display = 'block'; showToast('نام کاربری تکراری است', 'error'); return; } users[user] = { fname, lname, phone, pass }; saveUsers(users); showToast('ثبت نام با موفقیت انجام شد! وارد شوید.', 'success'); document.getElementById('regFirstName').value = ''; document.getElementById('regLastName').value = ''; document.getElementById('regUsername').value = ''; document.getElementById('regPhone').value = ''; document.getElementById('regPassword').value = ''; switchTab('login'); document.getElementById('loginIdentifier').value = user; }
        function handleLogin(e) { e.preventDefault(); const identifier = document.getElementById('loginIdentifier').value.trim(); const pass = document.getElementById('loginPassword').value; let users = getUsers(); let foundUser = null; let userKey = null; for (let key in users) { if (key.toLowerCase() === identifier.toLowerCase() || users[key].phone === identifier) { if (users[key].pass === pass) { foundUser = users[key]; userKey = key; } break; } } if (foundUser) { try { localStorage.setItem('currentUser', userKey); } catch (e) {} showToast('ورود با موفقیت انجام شد', 'success'); enterDashboard(userKey, foundUser); } else { showToast('کاربر یافت نشد یا رمز عبور اشتباه است', 'error'); } }
        function enterDashboard(username, userData) { switchView('studioView'); document.getElementById('exitBtn').classList.remove('hidden'); document.getElementById('profFirstName').value = userData.fname; document.getElementById('profLastName').value = userData.lname; document.getElementById('profUsername').innerText = username; document.getElementById('profPhone').innerText = userData.phone; renderHistory(); }
        function logout() { try { localStorage.removeItem('currentUser'); } catch (e) {} document.getElementById('exitBtn').classList.add('hidden'); switchView('authView'); document.getElementById('loginIdentifier').value = ''; document.getElementById('loginPassword').value = ''; showToast('با موفقیت خارج شدید', 'info'); }
        function updateProfile() { const username = document.getElementById('profUsername').innerText; let users = getUsers(); if (users[username]) { users[username].fname = document.getElementById('profFirstName').value; users[username].lname = document.getElementById('profLastName').value; saveUsers(users); showToast('پروفایل با موفقیت بروزرسانی شد', 'success'); } else { showToast('خطا در یافتن کاربر', 'error'); } }
        function openPasswordModal() { document.getElementById('newPassword').value = ''; document.getElementById('confirmNewPassword').value = ''; document.getElementById('passwordModal').classList.add('active'); }
        function updatePassword() { const p1 = document.getElementById('newPassword').value; const p2 = document.getElementById('confirmNewPassword').value; if (p1 !== p2 || p1.trim() === '') { showToast('رمزها یکسان نیستند یا خالی است', 'error'); return; } const username = document.getElementById('profUsername').innerText; let users = getUsers(); if (users[username]) { users[username].pass = p1; saveUsers(users); showToast('رمز عبور با موفقیت تغییر کرد', 'success'); closeModal('passwordModal'); } else { showToast('خطا در یافتن کاربر', 'error'); } }
        
        function initDropdowns() {
            const fillDropdown = (id, arr) => {
                const sel = document.getElementById(id);
                sel.innerHTML = '';
                arr.forEach(item => {
                    let opt = document.createElement('option');
                    opt.value = item;
                    opt.innerText = item;
                    sel.appendChild(opt);
                });
            };
            fillDropdown('customSize', sizes);
            fillDropdown('customStyle', styles);
            fillDropdown('customLighting', lightings);
            fillDropdown('customCamera', cameras);
            fillDropdown('aiTarget', aiTargets);

            const filterSel = document.getElementById('galleryFilter');
            const uploadCatSel = document.getElementById('galleryCategory');
            Object.keys(categories).forEach(cat => {
                let opt1 = document.createElement('option'); opt1.value = cat; opt1.innerText = cat; filterSel.appendChild(opt1);
                let opt2 = document.createElement('option'); opt2.value = cat; opt2.innerText = cat; uploadCatSel.appendChild(opt2);
            });
        }
        
        function initCategories() { const bar = document.getElementById('categoriesBar'); bar.innerHTML = ''; Object.keys(categories).forEach(cat => { let btn = document.createElement('button'); btn.className = 'cat-btn'; btn.innerText = cat; btn.onclick = () => showWords(cat, btn); bar.appendChild(btn); }); }
        function showWords(cat, btn) { document.querySelectorAll('.cat-btn').forEach(b => b.classList.remove('active')); btn.classList.add('active'); const container = document.getElementById('wordsContainer'); container.classList.remove('hidden-initial'); container.innerHTML = ''; categories[cat].forEach(word => { let chip = document.createElement('div'); chip.className = 'word-chip'; chip.innerText = word; chip.onclick = () => addSelectedWord(word, chip); container.appendChild(chip); }); }
        function addSelectedWord(word, chipElem) { if (selectedWords.includes(word)) { showToast('این مورد قبلا انتخاب شده است', 'info'); return; } selectedWords.push(word); chipElem.classList.add('selected'); const bar = document.getElementById('selectedWordsBar'); bar.classList.remove('hidden-initial'); renderSelectedWords(); }
        function removeSelectedWord(word) { selectedWords = selectedWords.filter(w => w !== word); renderSelectedWords(); document.querySelectorAll('.word-chip').forEach(c => { if(c.innerText === word) c.classList.remove('selected'); }); if(selectedWords.length === 0) { document.getElementById('selectedWordsBar').classList.add('hidden-initial'); } }
        function renderSelectedWords() { const bar = document.getElementById('selectedWordsBar'); if(selectedWords.length === 0) return; bar.innerHTML = ''; selectedWords.forEach(word => { let chip = document.createElement('div'); chip.className = 'selected-chip'; chip.innerHTML = `${word} <i class="fas fa-times" onclick="removeSelectedWord('${word}')"></i>`; bar.appendChild(chip); }); }
        
        function resetCustomForm() {
            const form = document.getElementById('customForm');
            form.removeAttribute('data-edit-id');
            document.getElementById('customTopic').value = '';
            document.getElementById('customDesc').value = '';
            
            const selects = ['customSize', 'customStyle', 'customLighting', 'customCamera', 'aiTarget'];
            selects.forEach(id => {
                const sel = document.getElementById(id);
                if (sel.options.length > 0) sel.selectedIndex = 0;
            });
            
            document.getElementById('textOnImg').value = 'no';
            toggleTextLang(); 
            document.getElementById('textContent').value = '';
        }

        function toggleCustomForm(id = 'customForm') { 
            const form = document.getElementById(id);
            if (!form.classList.contains('active')) {
                resetCustomForm();
            }
            form.classList.toggle('active'); 
        }
        
        function toggleTextLang() { const val = document.getElementById('textOnImg').value; const isYes = val === 'yes'; document.getElementById('textLangBox').classList.toggle('hidden-initial', !isYes); document.getElementById('textContentBox').classList.toggle('hidden-initial', !isYes); }
        function toggleCustomAI(val) { document.getElementById('customAIBox').classList.toggle('hidden-initial', val !== 'custom'); }
        
        // ترجمه به انگلیسی با حفظ تمامی کلمات (تبدیل ناشناخته‌ها به فینگلیش)
        function translateTextToEnglish(text) {
            if (!text) return "";
            if (!/[\u0600-\u06FF\u0750-\u077F\uFB50-\uFDFF\uFE70-\uFEFF]/.test(text)) return text;
            let cleanText = text.replace(/\n/g, '. ');
            let words = cleanText.split(/\s+/);
            let translatedWords = words.map(word => {
                let cleanWord = word.replace(/[.,\/#!$%\^&\*;:{}=\-_`~()،؟]/g, "");
                let engWord = dict[cleanWord];
                if (engWord) return engWord;
                // تبدیل کلمات ناشناخته به فینگلیش
                if (/[\u0600-\u06FF\u0750-\u077F\uFB50-\uFDFF\uFE70-\uFEFF]/.test(cleanWord)) {
                    return toFinglish(cleanWord);
                }
                return word;
            });
            return translatedWords.join(" ");
        }

        // ==========================================
        // 2. موتور پرامپت ساز با افکت تایپ زنده و لودینگ
        // ==========================================
        const NVIDIA_API_KEY = "کلید_شما_اینجا"; // کلید API نvidia خود را اینجا بگذارید

        function generateLocalPrompt(subject, desc, isTextActive, userText, style, lighting, camera, aiTarget) {
            const modifiers = ["hyper-detailed", "intricate textures", "volumetric lighting", "cinematic atmosphere", "vibrant color palette", "dramatic shadows", "high contrast", "octane render", "Unreal Engine 5", "ray tracing", "subsurface scattering", "hyper-realistic", "masterpiece", "aesthetically pleasing", "sharp focus", "8k resolution", "evocative composition", "dynamic angle", "breathtaking environment"];
            let selectedModifiers = [];
            for(let i=0; i<5; i++) {
                let rand = modifiers[Math.floor(Math.random() * modifiers.length)];
                if(!selectedModifiers.includes(rand)) selectedModifiers.push(rand);
            }
            
            let textPart = "";
            if (isTextActive) {
                if (userText && userText.trim() !== "") {
                    textPart = `. The image prominently features the exact text "${userText}" seamlessly integrated into the scene using glowing neon typography or natural elements like clouds or shadows`;
                } else {
                    textPart = `. The image includes a highly aesthetic and fitting typographic overlay that perfectly complements the main subject`;
                }
            }
            
            const structures = [
                `Create a ${selectedModifiers.join(", ")} ${style} masterpiece of ${subject}. The scene vividly portrays ${desc}${textPart}. The lighting is meticulously designed using ${lighting}, casting dynamic shadows. Captured from a ${camera} perspective, emphasizing the scale and depth. Highly optimized for ${aiTarget}.`,
                `An exceptionally ${selectedModifiers[0]} and ${selectedModifiers[1]} ${style} depiction of ${subject}. It features ${desc}${textPart}. Rendered with ${lighting} and shot from a ${camera} angle. Details include ${selectedModifiers[2]}, ${selectedModifiers[3]}, and ${selectedModifiers[4]}. Perfect for ${aiTarget}.`,
                `Visualize ${subject} in a ${style} style, where ${desc}${textPart}. The environment is brought to life with ${lighting} and captured via ${camera}. The scene boasts ${selectedModifiers.join(", ")}. Tailored for ${aiTarget}.`
            ];
            
            return structures[Math.floor(Math.random() * structures.length)];
        }

        async function generateAIPrompt(subject, desc, isTextOnImageActive, userText, style, lighting, camera, aiTarget) {
            const baseUrl = "https://integrate.api.nvidia.com/v1/chat/completions";
            
            const antiFilterProxies = [
                "", 
                "https://corsproxy.io/?url=", 
                "https://api.allorigins.win/raw?url=" 
            ];

            let systemPrompt = "You are an expert AI image prompt engineer. First, accurately translate any Persian/Farsi words in the Subject and Description into their closest English meanings. Then, create a highly detailed, vivid, and optimized prompt for image generation based on the translated English text. IMPORTANT: Generate a completely unique and varied prompt every single time. Use random descriptive words, alter sentence structure, and vary artistic interpretations. Do NOT include any programming code or technical parameters (like --ar or --v). Only provide descriptive English text.";
            let finalUserContent = "";

            if (isTextOnImageActive) {
                if (userText && userText.trim() !== "") {
                    systemPrompt += " The user wants specific text on an image. Enhance the visual details around this text while keeping the exact text intact. The text MUST be in the final prompt.";
                    finalUserContent = `Subject: ${subject}\nDescription: ${desc}\nText to put on image: "${userText}"\nStyle: ${style}\nLighting: ${lighting}\nCamera: ${camera}\nAI Target: ${aiTarget}\nUnique Variation ID: ${Math.floor(Math.random() * 1000000)}\nGenerate a detailed prompt that incorporates this exact text seamlessly into the image.`;
                } else {
                    systemPrompt += " The user wants an image with text, but didn't provide text. Generate a suitable, short, and meaningful text based on the subject.";
                    finalUserContent = `Subject: ${subject}\nDescription: ${desc}\nStyle: ${style}\nLighting: ${lighting}\nCamera: ${camera}\nAI Target: ${aiTarget}\nUnique Variation ID: ${Math.floor(Math.random() * 1000000)}\nGenerate a detailed prompt for an image that includes a fitting text overlay related to the subject.`;
                }
            } else {
                finalUserContent = `Subject: ${subject}\nDescription: ${desc}\nStyle: ${style}\nLighting: ${lighting}\nCamera: ${camera}\nAI Target: ${aiTarget}\nUnique Variation ID: ${Math.floor(Math.random() * 1000000)}\nGenerate a highly detailed image prompt. Make it unique and creative.`;
            }

            const requestBody = {
                model: "openai/gpt-oss-120b",
                messages: [
                    { role: "system", content: systemPrompt },
                    { role: "user", content: finalUserContent }
                ],
                temperature: 1, 
                top_p: 1,
                max_tokens: 4096,
                stream: false
            };

            for (let i = 0; i < antiFilterProxies.length; i++) {
                const proxy = antiFilterProxies[i];
                const targetUrl = proxy === "" ? baseUrl : proxy + encodeURIComponent(baseUrl);
                
                try {
                    const response = await fetch(targetUrl, {
                        method: 'POST',
                        headers: {
                            'Content-Type': 'application/json',
                            'Authorization': `Bearer ${NVIDIA_API_KEY}`
                        },
                        body: JSON.stringify(requestBody)
                    });

                    if (response.ok) {
                        const data = await response.json();
                        const message = data.choices[0].message;
                        const reasoning = message.reasoning_content || null;
                        let finalResult = "";
                        if (reasoning) {
                            finalResult += reasoning + "\n\n";
                        }
                        finalResult += message.content;
                        return finalResult; 
                    }
                } catch (error) {
                    console.warn(`اتصال ناموفق. تلاش بعدی یا استفاده از موتور آفلاین...`);
                }
            }
            return null; 
        }

        function typeWriter(text, element, callback) {
            isTyping = true;
            element.innerHTML = '<div class="typed-text"></div>';
            const typedTextElement = element.querySelector('.typed-text');
            let words = text.split(' ');
            let i = 0;

            function type() {
                if (i < words.length) {
                    typedTextElement.innerHTML += (i === 0 ? '' : ' ') + words[i];
                    i++;
                    // سرعت تایپ کلمه به کلمه
                    setTimeout(type, Math.floor(Math.random() * 50) + 30); 
                } else {
                    isTyping = false;
                    if (callback) callback();
                }
            }
            type();
        }

        async function generateCustomPrompt() {
            if (isTyping) return;
            
            const editId = document.getElementById('customForm').getAttribute('data-edit-id');
            const topic = document.getElementById('customTopic').value;
            if(!topic) { showToast('لطفا موضوع را وارد کنید', 'error'); return; }
            const desc = document.getElementById('customDesc').value;
            const style = document.getElementById('customStyle').value.split(' - ')[0];
            const lighting = document.getElementById('customLighting').value.split(' - ')[0];
            const camera = document.getElementById('customCamera').value.split(' - ')[0];
            const ai = document.getElementById('aiTarget').value.split(' - ')[0];
            
            let isTextActive = document.getElementById('textOnImg').value === "yes";
            let userText = document.getElementById('textContent').value;
            if(isTextActive && userText) {
                userText = translateTextToEnglish(userText);
            }

            // نمایش انیمیشن لودینگ
            const output = document.getElementById('promptOutput');
            output.innerHTML = '<div class="spinner-box"><div class="spinner"></div><div class="loading-text">در حال نوشتن پرامپت با هوش مصنوعی...</div></div>';
            showToast('در حال ارسال درخواست...', 'info');

            let finalPrompt = await generateAIPrompt(topic, desc, isTextActive, userText, style, lighting, camera, ai);
            
            if (!finalPrompt) {
                finalPrompt = generateLocalPrompt(translateTextToEnglish(topic), translateTextToEnglish(desc), isTextActive, userText, style, lighting, camera, ai);
                showToast('حالت آفلاین: پرامپت متفاوت با موتور پیشرفته داخلی ساخته شد.', 'info');
            } else {
                showToast('پرامپت متفاوت با هوش مصنوعی ساخته شد', 'success');
            }
            
            // اجرای افکت تایپ زنده
            typeWriter(finalPrompt, output, () => {
                document.getElementById('customForm').classList.remove('active');
                const formData = { topic: topic, desc: desc, size: document.getElementById('customSize').value, style: document.getElementById('customStyle').value, lighting: document.getElementById('customLighting').value, camera: document.getElementById('customCamera').value, textOnImg: document.getElementById('textOnImg').value, textLang: document.getElementById('textLang').value, textContent: document.getElementById('textContent').value, aiTarget: document.getElementById('aiTarget').value };
                historyPage = 1; 
                saveHistory(finalPrompt, 'custom', topic, editId, formData);
                if (editId) document.getElementById('customForm').removeAttribute('data-edit-id');
            });
        }

        function generateRandom() {
            if (isTyping) return;
            if (history.length === 0) {
                showToast('برای ساخت پرامپت تصادفی ترکیبی، ابتدا یک پرامپت بسازید', 'error');
                return;
            }
            
            const numToCombine = Math.min(history.length, Math.floor(Math.random() * 2) + 2);
            let shuffledHistory = [...history].sort(() => 0.5 - Math.random());
            let combinedTopics = [];
            
            for (let i = 0; i < numToCombine; i++) {
                if (shuffledHistory[i].topic && !combinedTopics.includes(shuffledHistory[i].topic)) {
                    combinedTopics.push(shuffledHistory[i].topic);
                }
            }
            
            if (combinedTopics.length === 0 || combinedTopics.every(t => t === "Random Prompt" || t === "Random Combined Prompt")) {
                let words = [];
                for (let i = 0; i < numToCombine; i++) {
                    let text = shuffledHistory[i].text;
                    let splitText = text.split(/[\s,]+/).filter(w => w.length > 4 && !w.startsWith('--'));
                    if(splitText.length > 0) words.push(splitText[Math.floor(Math.random() * splitText.length)]);
                }
                combinedTopics = words;
            }

            const finalSubject = combinedTopics.length > 0 ? combinedTopics.join(" mixed with ") : "a mysterious and captivating entity";
            
            const styles = ["Cinematic", "Anime", "3D Render", "Photorealistic", "Concept Art", "Cyberpunk", "Surrealism"];
            const lightings = ["Golden Hour", "Neon Lighting", "Studio Lighting", "Volumetric Lighting", "Bioluminescence"];
            const cameras = ["Wide Angle", "Close-up", "Aerial View", "Macro", "Dutch Angle"];
            
            const randStyle = styles[Math.floor(Math.random() * styles.length)];
            const randLighting = lightings[Math.floor(Math.random() * lightings.length)];
            const randCamera = cameras[Math.floor(Math.random() * cameras.length)];
            
            const p = `A highly detailed and visually stunning ${randStyle} composition blending elements of ${finalSubject}. The scene is illuminated with ${randLighting}, creating a dramatic and immersive atmosphere. Captured from a ${randCamera} perspective. Rendered in 8k resolution, masterpiece, ultra-detailed, sharp focus, ray tracing, volumetric lighting, vivid colors, cinematic post-processing.`;
            
            const output = document.getElementById('promptOutput');
            typeWriter(p, output, () => {
                showToast('پرامپت تصادفی ترکیبی از تاریخچه ساخته شد', 'success');
                historyPage = 1;
                saveHistory(p, 'random', "Random Combined Prompt", null, null);
            });
        }

        function openSizeModal() {
            if(selectedWords.length === 0) { showToast('لطفا ابتدا از دسته بندی‌ها کلماتی را انتخاب کنید', 'error'); return; }
            const grid = document.getElementById('sizeOptionsGrid');
            grid.innerHTML = '';
            sizes.forEach(size => { 
                let div = document.createElement('div'); 
                div.className = 'size-option'; 
                div.innerText = size; 
                div.onclick = () => { 
                    const engSize = size.split(' - ')[0].split(' ')[0]; 
                    generateFromSelection(engSize); 
                    closeModal('sizeModal'); 
                }; 
                grid.appendChild(div); 
            });
            document.getElementById('sizeModal').classList.add('active');
        }

        function generateFromSelection(size) {
            if (isTyping) return;
            const engWords = selectedWords.map(w => translateTextToEnglish(w)).join(", ");
            
            const details = ["intricate textures", "hyper-realistic details", "cinematic atmosphere", "dramatic lighting", "volumetric fog", "ray tracing", "subsurface scattering", "8k resolution", "masterpiece composition", "vibrant color grading", "ethereal mood", "sharp focus", "octane render"];
            const environments = ["in a mystical setting", "in a bustling city", "in an ancient temple", "in a vast desert", "in a futuristic landscape", "under a starry sky", "in a serene forest", "in an abandoned ruins"];
            const moods = ["evoking a sense of wonder", "creating a dramatic tension", "with a peaceful and calm aura", "with an intense and mysterious vibe"];
            
            let chosenDetails = [];
            for(let i=0; i<3; i++) {
                let rand = details[Math.floor(Math.random() * details.length)];
                if(!chosenDetails.includes(rand)) chosenDetails.push(rand);
            }
            let chosenEnv = environments[Math.floor(Math.random() * environments.length)];
            let chosenMood = moods[Math.floor(Math.random() * moods.length)];
            
            const structures = [
                `A visually spectacular image featuring ${engWords}, set ${chosenEnv}. The composition is enhanced with ${chosenDetails.join(", ")}, ${chosenMood}. Highly detailed, aesthetically pleasing. Aspect ratio: ${size}.`,
                `Visualize ${engWords} ${chosenEnv}. This masterpiece includes ${chosenDetails.join(", ")}, creating a breathtaking and immersive scene. The mood is ${chosenMood}. Aspect ratio: ${size}.`,
                `An ultra-detailed scene showcasing ${engWords} ${chosenEnv}. Rendered with ${chosenDetails.join(", ")}. ${chosenMood}. Cinematic and hyper-realistic. Aspect ratio: ${size}.`
            ];
            
            const p = structures[Math.floor(Math.random() * structures.length)];
            const output = document.getElementById('promptOutput');
            typeWriter(p, output, () => {
                showToast('پرامپت غنی و متفاوت از روی انتخاب‌های شما ساخته شد', 'success');
                historyPage = 1;
                saveHistory(p, 'selection', selectedWords.join(", "), null, null);
            });
        }

        function copyPrompt() { const text = document.getElementById('promptOutput').innerText; if(text.includes("Prompt will be generated") || text.includes("در حال نوشتن")) { showToast('ابتدا یک پرامپت تولید کنید', 'error'); return; } navigator.clipboard.writeText(text).then(() => { showToast('پرامپت با موفقیت کپی شد', 'success'); }); }
        function sendToChatGPT() { const text = document.getElementById('promptOutput').innerText; if(text.includes("Prompt will be generated") || text.includes("در حال نوشتن")) { showToast('ابتدا یک پرامپت تولید کنید', 'error'); return; } const chatGptUrl = `https://chatgpt.com/?q=Please%20generate%20an%20image%20based%20on%20this%20prompt:%20${encodeURIComponent(text)}`; window.open(chatGptUrl, '_blank'); }
        function clearAll() { selectedWords = []; renderSelectedWords(); document.getElementById('selectedWordsBar').classList.add('hidden-initial'); document.getElementById('wordsContainer').classList.add('hidden-initial'); document.querySelectorAll('.cat-btn').forEach(b => b.classList.remove('active')); document.getElementById('promptOutput').innerHTML = '<div class="typed-text">Prompt will be generated here...</div>'; document.getElementById('customForm').classList.remove('active'); showToast('صفحه پاکسازی شد', 'info'); }

        function saveHistory(promptText, type, topic, editId = null, formData = null) {
            if(editId) { const idx = history.findIndex(h => h.id === editId); if(idx !== -1) { history[idx].text = promptText; history[idx].topic = topic; if(formData) history[idx].formData = formData; } showToast('پرامپت ویرایش شد', 'success'); }
            else { history.unshift({ id: Date.now().toString(), text: promptText, type: type, topic: topic, date: new Date().toLocaleString('fa-IR'), formData: type === 'custom' ? formData : null }); }
            try { localStorage.setItem('promptHistory', JSON.stringify(history)); } catch (e) {}
            renderHistory();
        }
        
        function searchHistory() {
            historySearchQuery = document.getElementById('historySearch').value.toLowerCase();
            historyPage = 1;
            renderHistory();
        }

        function renderHistory() {
            const container = document.getElementById('historyContainer');
            const paginationContainer = document.getElementById('historyPagination');
            
            let filteredHistory = history;
            if (historySearchQuery) {
                filteredHistory = history.filter(item => item.topic && item.topic.toLowerCase().includes(historySearchQuery));
            }

            const totalPages = Math.ceil(filteredHistory.length / itemsPerPage);
            if (totalPages > 0 && historyPage > totalPages) historyPage = totalPages;
            if (historyPage < 1) historyPage = 1;

            if (filteredHistory.length === 0) {
                container.innerHTML = '<p style="color:#888; text-align:center;">پرامپتی یافت نشد.</p>';
                paginationContainer.innerHTML = '';
                return;
            }

            const start = (historyPage - 1) * itemsPerPage;
            const end = start + itemsPerPage;
            const pageItems = filteredHistory.slice(start, end);

            container.innerHTML = '';
            pageItems.forEach(item => {
                const div = document.createElement('div');
                div.className = 'history-item';
                div.innerHTML = `<div class="meta">${item.date} | نوع: ${item.type}</div><div class="topic">موضوع: ${item.topic || 'بدون موضوع'}</div><div class="text" title="${item.text}">${item.text}</div><div class="actions"><button class="btn btn-secondary" style="padding:5px 10px; font-size:12px;" onclick="copyText('${item.id}')"><i class="fas fa-copy"></i> کپی</button>${item.type === 'custom' ? `<button class="btn btn-warning" style="padding:5px 10px; font-size:12px;" onclick="editPrompt('${item.id}')"><i class="fas fa-edit"></i> ویرایش</button>` : ''}</div>`;
                container.appendChild(div);
            });

            renderPagination(paginationContainer, totalPages, historyPage, 'historyPage', renderHistory);
        }
        
        function copyText(id) { const item = history.find(h => h.id === id); navigator.clipboard.writeText(item.text); showToast('متن کپی شد', 'success'); }
        function editPrompt(id) { 
            const item = history.find(h => h.id === id); 
            if(!item || !item.formData) { showToast('امکان ویرایش این پرامپت وجود ندارد', 'error'); return; } 
            document.getElementById('customForm').classList.add('active'); 
            document.getElementById('customForm').setAttribute('data-edit-id', id); 
            document.getElementById('customTopic').value = item.formData.topic || ''; 
            document.getElementById('customDesc').value = item.formData.desc || ''; 
            document.getElementById('customSize').value = item.formData.size || ''; 
            document.getElementById('customStyle').value = item.formData.style || ''; 
            document.getElementById('customLighting').value = item.formData.lighting || ''; 
            document.getElementById('customCamera').value = item.formData.camera || ''; 
            document.getElementById('textOnImg').value = item.formData.textOnImg || 'no'; 
            toggleTextLang(); 
            if(item.formData.textLang) document.getElementById('textLang').value = item.formData.textLang; 
            document.getElementById('textContent').value = item.formData.textContent || ''; 
            document.getElementById('aiTarget').value = item.formData.aiTarget || ''; 
            document.getElementById('promptOutput').innerHTML = `<div class="typed-text">${item.text}</div>`; 
            showToast('تنظیمات قبلی بارگذاری شد. ویرایش را انجام داده و دوباره تولید کنید.', 'info'); 
            document.getElementById('customForm').scrollIntoView({behavior: "smooth", block: "start"}); 
        }

        function goToGallery() { let currentUser = null; try { currentUser = localStorage.getItem('currentUser'); } catch (e) {} if (!currentUser) { showToast('برای مشاهده گالری پرامپت باید وارد حساب کاربری شوید', 'error'); switchView('authView'); return; } switchView('galleryView'); }
        function toggleUploadForm() { cancelEditGallery(); document.getElementById('uploadForm').classList.toggle('active'); }
        function uploadPrompt() {
            const title = document.getElementById('galleryTitle').value; 
            const text = document.getElementById('galleryText').value; 
            const imageFile = document.getElementById('galleryImage').files[0];
            const category = document.getElementById('galleryCategory').value;
            let aiTarget = document.getElementById('galleryAI').value;
            if (aiTarget === 'custom') {
                aiTarget = document.getElementById('galleryCustomAI').value || 'Unknown AI';
            }
            
            if(!title || !text) { showToast('عنوان و متن الزامی است', 'error'); return; }
            let user = 'Guest'; try { user = localStorage.getItem('currentUser') || 'Guest'; } catch (e) {}
            const processImageAndSave = (imageData = null) => {
                if (editingGalleryId) { const idx = gallery.findIndex(g => g.id === editingGalleryId); if (idx !== -1) { gallery[idx].title = title; gallery[idx].text = text; gallery[idx].category = category; gallery[idx].aiTarget = aiTarget; if(imageData) gallery[idx].image = imageData; } showToast('پرامپت با موفقیت ویرایش شد', 'success'); cancelEditGallery(); }
                else { gallery.unshift({ id: Date.now().toString(), title, text, author: user, image: imageData, category: category, aiTarget: aiTarget }); showToast('پرامپت در گالری بارگذاری شد', 'success'); document.getElementById('uploadForm').classList.remove('active'); }
                try { localStorage.setItem('promptGallery', JSON.stringify(gallery)); } catch (e) { showToast('خطا در ذخیره‌سازی (احتمالا حجم عکس زیاد است)', 'error'); }
                document.getElementById('galleryTitle').value = ''; document.getElementById('galleryText').value = ''; document.getElementById('galleryImage').value = ''; document.getElementById('galleryCustomAI').value = ''; renderGallery();
            };
            if (imageFile) {
                if (imageFile.size > 2 * 1024 * 1024) { showToast('حجم تصویر باید کمتر از 2 مگابایت باشد', 'error'); return; }
                const reader = new FileReader(); reader.onload = function(e) { processImageAndSave(e.target.result); }; reader.readAsDataURL(imageFile);
            } else { if (editingGalleryId) { const oldItem = gallery.find(g => g.id === editingGalleryId); processImageAndSave(oldItem ? oldItem.image : null); } else { processImageAndSave(null); } }
        }
        function editGalleryPrompt(id) { const item = gallery.find(g => g.id === id); if(!item) return; editingGalleryId = id; document.getElementById('uploadForm').classList.add('active'); document.getElementById('galleryTitle').value = item.title; document.getElementById('galleryText').value = item.text; document.getElementById('galleryImage').value = ''; document.getElementById('galleryCategory').value = item.category || 'طبیعت'; 
            let aiFound = false;
            for(let opt of document.getElementById('galleryAI').options) { if(opt.value === item.aiTarget) { document.getElementById('galleryAI').value = item.aiTarget; aiFound = true; break; } }
            if(!aiFound) { document.getElementById('galleryAI').value = 'custom'; toggleCustomAI('custom'); document.getElementById('galleryCustomAI').value = item.aiTarget; } else { toggleCustomAI(document.getElementById('galleryAI').value); }
            document.getElementById('gallerySubmitBtn').innerHTML = '<i class="fas fa-check"></i> بروزرسانی پرامپت'; document.getElementById('galleryCancelBtn').classList.remove('hidden'); document.getElementById('uploadForm').scrollIntoView({behavior: "smooth", block: "start"}); showToast('حالت ویرایش فعال شد.', 'info'); }
        function deleteGalleryPrompt(id) { deleteTargetId = id; document.getElementById('deleteModal').classList.add('active'); }
        function confirmDeleteGallery() { if (deleteTargetId) { gallery = gallery.filter(g => g.id !== deleteTargetId); try { localStorage.setItem('promptGallery', JSON.stringify(gallery)); } catch (e) {} renderGallery(); showToast('پرامپت با موفقیت حذف شد', 'success'); deleteTargetId = null; } closeModal('deleteModal'); }
        function cancelEditGallery() { editingGalleryId = null; document.getElementById('gallerySubmitBtn').innerHTML = '<i class="fas fa-check"></i> ثبت در گالری'; document.getElementById('galleryCancelBtn').classList.add('hidden'); document.getElementById('galleryTitle').value = ''; document.getElementById('galleryText').value = ''; document.getElementById('galleryImage').value = ''; document.getElementById('galleryCustomAI').value = ''; }
        
        function changeGalleryFilter(val) { galleryFilter = val; galleryPage = 1; renderGallery(); }

        function renderGallery() {
            const grid = document.getElementById('galleryGrid');
            const paginationContainer = document.getElementById('galleryPagination');
            let currentUser = 'Guest';
            try { currentUser = localStorage.getItem('currentUser') || 'Guest'; } catch (e) {}

            let filteredGallery = gallery;
            if (galleryFilter !== 'all') {
                filteredGallery = gallery.filter(item => item.category === galleryFilter);
            }

            const totalPages = Math.ceil(filteredGallery.length / galleryPerPage);
            if (totalPages > 0 && galleryPage > totalPages) galleryPage = totalPages;
            if (galleryPage < 1) galleryPage = 1;

            if (filteredGallery.length === 0) {
                grid.innerHTML = '<p style="color:#888; text-align:center; grid-column: 1/-1;">هیچ پرامپتی در این دسته یافت نشد.</p>';
                paginationContainer.innerHTML = '';
                return;
            }

            const start = (galleryPage - 1) * galleryPerPage;
            const end = start + galleryPerPage;
            const pageItems = filteredGallery.slice(start, end);

            grid.innerHTML = '';
            pageItems.forEach(item => {
                const isOwner = item.author === currentUser;
                const div = document.createElement('div');
                div.className = 'gallery-item';
                div.innerHTML = `<div class="content">
                    <div class="title">${item.title} <span style="font-size:11px; color:#888;">(توسط: ${item.author})</span></div>
                    <div class="meta-tags">
                        ${item.category ? `<span class="tag"><i class="fas fa-folder"></i> ${item.category}</span>` : ''}
                        ${item.aiTarget ? `<span class="tag"><i class="fas fa-robot"></i> ${item.aiTarget}</span>` : ''}
                    </div>
                    ${item.image ? `<img src="${item.image}" alt="Sample Image">` : ''}
                    <div class="desc">${item.text}</div>
                    ${isOwner ? `<div style="margin-top:15px; display:flex; gap:10px;"><button class="btn btn-warning" style="flex:1; padding:8px; font-size:13px;" onclick="editGalleryPrompt('${item.id}')"><i class="fas fa-edit"></i> ویرایش</button><button class="btn btn-danger" style="flex:1; padding:8px; font-size:13px;" onclick="deleteGalleryPrompt('${item.id}')"><i class="fas fa-trash"></i> حذف</button></div>` : ''}
                </div>`;
                grid.appendChild(div);
            });

            renderPagination(paginationContainer, totalPages, galleryPage, 'galleryPage', renderGallery, true);
        }

        function renderPagination(container, totalPages, currentPage, pageVarName, renderFunc, showAllPages) {
            container.innerHTML = '';
            if (totalPages <= 1) return;

            let prevBtn = document.createElement('button');
            prevBtn.className = 'page-btn';
            prevBtn.innerHTML = '<i class="fas fa-chevron-right"></i> قبلی';
            prevBtn.disabled = currentPage === 1;
            prevBtn.onclick = () => { 
                if (pageVarName === 'historyPage') { historyPage--; renderHistory(); } 
                else if (pageVarName === 'galleryPage') { galleryPage--; renderGallery(); }
            };
            container.appendChild(prevBtn);

            let pages = [];
            if (showAllPages) {
                for(let i=1; i<=totalPages; i++) pages.push(i);
            } else if (totalPages <= 3) {
                for(let i=1; i<=totalPages; i++) pages.push(i);
            } else {
                if (currentPage <= 3) {
                    pages = [1, 2, 3, '...', totalPages];
                } else if (currentPage >= totalPages - 2) {
                    pages = [1, '...', totalPages-2, totalPages-1, totalPages];
                } else {
                    pages = [1, '...', currentPage, '...', totalPages];
                }
            }

            pages.forEach(p => {
                if (p === '...') {
                    let span = document.createElement('span');
                    span.innerText = '...';
                    span.className = 'page-dots';
                    container.appendChild(span);
                } else {
                    let btn = document.createElement('button');
                    btn.innerText = p;
                    btn.className = 'page-btn' + (p === currentPage ? ' active' : '');
                    btn.onclick = () => { 
                        if (pageVarName === 'historyPage') { historyPage = p; renderHistory(); } 
                        else if (pageVarName === 'galleryPage') { galleryPage = p; renderGallery(); }
                    };
                    container.appendChild(btn);
                }
            });

            let nextBtn = document.createElement('button');
            nextBtn.className = 'page-btn';
            nextBtn.innerHTML = 'بعدی <i class="fas fa-chevron-left"></i>';
            nextBtn.disabled = currentPage === totalPages;
            nextBtn.onclick = () => { 
                if (pageVarName === 'historyPage') { historyPage++; renderHistory(); } 
                else if (pageVarName === 'galleryPage') { galleryPage++; renderGallery(); }
            };
            container.appendChild(nextBtn);
        }

        function closeModal(id) { document.getElementById(id).classList.remove('active'); }
        function openSupportModal() { document.getElementById('supportModal').classList.add('active'); }

        window.onload = () => {
            loadTheme(); initDropdowns(); initCategories();
            let currentUser = null;
            try { currentUser = localStorage.getItem('currentUser'); } catch (e) {}
            if (currentUser) { let users = getUsers(); if (users[currentUser]) { enterDashboard(currentUser, users[currentUser]); } else { try { localStorage.removeItem('currentUser'); } catch (e) {} } }
        }
    </script>
</body>
</html>
