<!doctype html>
<html lang="id">

<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width,initial-scale=1">
    <meta name="description" content="Website resmi SMA Negeri Nusantara">
    <title>SMA ARM LUSTER NUSANTARA</title>
    <style>
        :root {
            --ink: #20252b;
            --muted: #64707d;
            --line: #d9dee5;
            --soft: #f4f6f8;
            --blue: #173d67;
            --blue2: #245887;
            --white: #fff;
            --radius: 14px;
            --shadow: 0 8px 28px rgba(25, 40, 60, .08)
        }

        * {
            box-sizing: border-box
        }

        html {
            scroll-behavior: smooth
        }

        body {
            margin: 0;
            font-family: Arial, Helvetica, sans-serif;
            color: var(--ink);
            background: #f7f8fa;
            line-height: 1.55
        }

        button,
        input,
        select,
        textarea {
            font: inherit
        }

        button,
        a {
            -webkit-tap-highlight-color: transparent
        }

        a {
            color: inherit;
            text-decoration: none
        }

        .container {
            width: min(1120px, calc(100% - 36px));
            margin: auto
        }

        header {
            background: #fff;
            border-bottom: 1px solid var(--line);
            position: sticky;
            top: 0;
            z-index: 20
        }

        .head {
            height: 76px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 18px
        }

        .brand {
            display: flex;
            align-items: center;
            gap: 12px;
            font-weight: 800;
            letter-spacing: .2px
        }

        .logo {
            height: 44px;
            width: 44px;
            border: 2px solid var(--blue);
            border-radius: 50%;
            display: grid;
            place-items: center;
            color: var(--blue);
            font-size: 11px;
            font-weight: 900;
            line-height: 1.05;
            text-align: center
        }

        .brand small {
            display: block;
            color: var(--muted);
            font-size: 11px;
            font-weight: 500;
            letter-spacing: 1px
        }

        .login-btn,
        .primary {
            border: 0;
            border-radius: 8px;
            background: var(--blue);
            color: #fff;
            padding: 11px 17px;
            font-weight: 700;
            cursor: pointer
        }

        .login-btn:hover,
        .primary:hover {
            background: var(--blue2)
        }

        nav {
            border-top: 1px solid #eef0f3
        }

        .nav-inner {
            display: flex;
            align-items: center;
            gap: 4px;
            min-height: 46px
        }

        .nav-inner a {
            padding: 12px 14px;
            color: #394552;
            font-size: 14px;
            font-weight: 600;
            border-radius: 7px
        }

        .nav-inner a:hover,
        .nav-inner a.active {
            background: #edf2f7;
            color: var(--blue)
        }

        .menu {
            display: none;
            background: none;
            border: 1px solid var(--line);
            border-radius: 8px;
            padding: 8px 11px
        }

        main {
            min-height: 70vh
        }

        .hero {
            padding: 28px 0 20px
        }

        .slider {
            height: 310px;
            border-radius: 18px;
            overflow: hidden;
            position: relative;
            background: linear-gradient(115deg, #173d67, #547da4);
            color: white;
            box-shadow: var(--shadow)
        }

        .slide {
            position: absolute;
            inset: 0;
            display: none;
            align-items: center;
            justify-content: space-between;
            padding: 42px 8%;
            gap: 25px;
            background: linear-gradient(110deg, rgba(12, 34, 59, .94), rgba(26, 76, 119, .72))
        }

        .slide.active {
            display: flex
        }

        .slide h1 {
            font-size: clamp(28px, 4vw, 46px);
            line-height: 1.12;
            margin: 0 0 14px;
            max-width: 540px
        }

        .slide p {
            max-width: 520px;
            color: #e5edf5;
            margin: 0 0 22px
        }

        .slide-art {
            width: 34%;
            height: 190px;
            border: 1px solid rgba(255, 255, 255, .5);
            border-radius: 16px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2)
        }

        .slide-art img {
            width: 100%;
            height: 100%;
            object-fit: cover
        }

        .slider-arrow {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            border: 1px solid #ffffff80;
            background: #ffffff20;
            color: white;
            border-radius: 50%;
            width: 38px;
            height: 38px;
            cursor: pointer;
            font-size: 22px
        }

        .prev {
            left: 14px
        }

        .next {
            right: 14px
        }

        .dots {
            position: absolute;
            bottom: 14px;
            left: 0;
            right: 0;
            display: flex;
            justify-content: center;
            gap: 7px
        }

        .dots button {
            width: 8px;
            height: 8px;
            border: 0;
            border-radius: 50%;
            background: #ffffff70;
            padding: 0;
            cursor: pointer
        }

        .dots button.active {
            background: white;
            width: 22px;
            border-radius: 9px
        }

        .section {
            padding: 26px 0
        }

        .section-title {
            display: flex;
            align-items: end;
            justify-content: space-between;
            gap: 12px;
            margin-bottom: 17px
        }

        .section-title h2 {
            margin: 0;
            font-size: 25px
        }

        .eyebrow {
            color: var(--blue2);
            font-size: 11px;
            font-weight: 800;
            letter-spacing: 1.5px;
            text-transform: uppercase
        }

        .welcome {
            display: grid;
            grid-template-columns: 160px 1fr;
            gap: 22px;
            align-items: center;
            background: white;
            padding: 24px;
            border: 1px solid var(--line);
            border-radius: var(--radius)
        }

        .principal {
            height: 142px;
            border-radius: 12px;
            overflow: hidden;
            background: #e8edf2;
        }

        .principal img {
            width: 100%;
            height: 100%;
            object-fit: cover
        }

        .welcome h2 {
            margin: 2px 0 8px
        }

        .welcome p {
            margin: 0;
            color: var(--muted)
        }

        .cards {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 16px
        }

        .card {
            background: white;
            border: 1px solid var(--line);
            border-radius: 13px;
            overflow: hidden;
            box-shadow: 0 3px 14px #172b4308
        }

        .thumb {
            height: 140px;
            background: linear-gradient(135deg, #dfe7ef, #f1f4f7);
            overflow: hidden;
        }

        .thumb img {
            width: 100%;
            height: 100%;
            object-fit: cover
        }

        .card-body {
            padding: 16px
        }

        .card h3 {
            font-size: 16px;
            margin: 0 0 7px
        }

        .card p {
            font-size: 13px;
            color: var(--muted);
            margin: 0 0 12px
        }

        .read {
            color: var(--blue2);
            font-size: 13px;
            font-weight: 700
        }

        .two-col {
            display: grid;
            grid-template-columns: 1.2fr .8fr;
            gap: 18px
        }

        .panel {
            background: #fff;
            border: 1px solid var(--line);
            border-radius: var(--radius);
            padding: 21px
        }

        .panel h2 {
            font-size: 21px;
            margin: 0 0 15px
        }

        .event {
            display: flex;
            gap: 13px;
            padding: 12px 0;
            border-bottom: 1px solid #edf0f3
        }

        .event:last-child {
            border: 0
        }

        .event-icon {
            width: 38px;
            height: 38px;
            border-radius: 10px;
            background: #edf2f7;
            display: grid;
            place-items: center
        }

        .event strong {
            display: block
        }

        .event small {
            color: var(--muted)
        }

        .quicklinks {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 9px
        }

        .quicklinks a {
            padding: 12px;
            background: #f3f6f9;
            border-radius: 9px;
            font-size: 13px;
            font-weight: 700;
            color: var(--blue)
        }

        footer {
            margin-top: 36px;
            background: #152e49;
            color: #eaf0f6;
            padding: 32px 0
        }

        .foot {
            display: flex;
            justify-content: space-between;
            gap: 25px;
            flex-wrap: wrap
        }

        .foot p {
            color: #c5d0dc;
            font-size: 13px;
            margin: 7px 0
        }

        .page {
            padding: 34px 0 50px
        }

        .crumb {
            color: var(--muted);
            font-size: 13px;
            margin-bottom: 8px
        }

        .page h1 {
            font-size: 32px;
            margin: 0 0 8px
        }

        .lead {
            color: var(--muted);
            margin: 0 0 24px
        }

        .content-box {
            background: white;
            border: 1px solid var(--line);
            border-radius: var(--radius);
            padding: 24px;
            margin-bottom: 18px
        }

        .content-box h2 {
            margin: 0 0 14px;
            font-size: 21px
        }

        .grid2 {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 14px
        }

        .info {
            padding: 17px;
            background: #f4f6f8;
            border-radius: 10px
        }

        .info h3 {
            margin: 0 0 6px;
            font-size: 16px
        }

        .info p {
            margin: 0;
            color: var(--muted);
            font-size: 14px
        }

        .org {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 14px
        }

        .org-top,
        .org-node {
            padding: 10px 18px;
            background: #edf2f7;
            border: 1px solid #cad5e0;
            border-radius: 8px;
            font-weight: 700
        }

        .org-branches {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 15px;
            width: 100%;
            text-align: center
        }

        .teacher-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 14px
        }

        .teacher {
            background: #f4f6f8;
            border-radius: 10px;
            padding: 18px;
            text-align: center
        }

        .avatar {
            width: 70px;
            height: 70px;
            border-radius: 50%;
            background: #dce5ee;
            margin: 0 auto 9px;
            overflow: hidden;
        }

        .avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover
        }

        .teacher small {
            display: block;
            color: var(--muted)
        }

        .steps {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 12px;
            margin: 18px 0
        }

        .step {
            padding: 17px 12px;
            text-align: center;
            background: #f1f5f8;
            border-radius: 10px;
            font-weight: 700
        }

        .step b {
            display: block;
            margin: auto auto 8px;
            width: 28px;
            height: 28px;
            border-radius: 50%;
            background: var(--blue);
            color: white;
            line-height: 28px
        }

        .form-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 14px
        }

        .field {
            display: flex;
            flex-direction: column;
            gap: 6px
        }

        .field.full {
            grid-column: 1/-1
        }

        .field label {
            font-size: 13px;
            font-weight: 700
        }

        .field input,
        .field select,
        .field textarea {
            border: 1px solid #ccd4dd;
            border-radius: 8px;
            padding: 11px;
            background: white;
            min-width: 0
        }

        .field input:focus,
        .field select:focus,
        .field textarea:focus {
            outline: 2px solid #a9c4df;
            border-color: var(--blue2)
        }

        .notice {
            display: none;
            padding: 12px;
            border-radius: 8px;
            background: #e9f6ed;
            color: #206039;
            margin-top: 14px
        }

        .schedule {
            width: 100%;
            border-collapse: collapse
        }

        .schedule th,
        .schedule td {
            border: 1px solid var(--line);
            padding: 11px;
            text-align: left
        }

        .schedule th {
            background: #edf2f7
        }

        .portal-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 14px
        }

        .portal-tile {
            padding: 20px;
            background: #f4f6f8;
            border-radius: 10px
        }

        .portal-tile strong {
            display: block;
            font-size: 18px
        }

        .modal {
            position: fixed;
            inset: 0;
            background: #0b1b2dcc;
            display: none;
            place-items: center;
            padding: 20px;
            z-index: 50
        }

        .modal.show {
            display: grid
        }

        .modal-card {
            background: white;
            border-radius: 14px;
            padding: 25px;
            width: min(420px, 100%);
            position: relative
        }

        .close {
            position: absolute;
            right: 14px;
            top: 10px;
            border: 0;
            background: none;
            font-size: 25px;
            cursor: pointer
        }

        .modal-card h2 {
            margin: 0 0 6px
        }

        .modal-card p {
            color: var(--muted);
            font-size: 13px;
            margin: 0 0 18px
        }

        @media(max-width:760px) {
            .head {
                height: 68px
            }

            .menu {
                display: block
            }

            .nav-inner {
                display: none;
                flex-direction: column;
                align-items: stretch;
                padding: 8px 0
            }

            .nav-inner.open {
                display: flex
            }

            .nav-inner a {
                padding: 10px
            }

            .login-btn {
                padding: 9px 11px
            }

            .brand {
                font-size: 13px
            }

            .logo {
                width: 39px;
                height: 39px
            }

            .slider {
                height: 340px
            }

            .slide {
                padding: 35px 48px;
                align-items: flex-start;
                justify-content: center;
                flex-direction: column
            }

            .slide-art {
                display: none
            }

            .cards {
                grid-template-columns: 1fr 1fr
            }

            .two-col {
                grid-template-columns: 1fr
            }

            .welcome {
                grid-template-columns: 100px 1fr;
                padding: 17px
            }

            .principal {
                height: 105px;
            }

            .section-title h2 {
                font-size: 21px
            }

            .teacher-grid {
                grid-template-columns: repeat(2, 1fr)
            }
        }

        @media(max-width:480px) {
            .container {
                width: min(100% - 24px, 1120px)
            }

            .cards {
                grid-template-columns: 1fr
            }

            .grid2,
            .form-grid,
            .portal-grid {
                grid-template-columns: 1fr
            }

            .field.full {
                grid-column: auto
            }

            .welcome {
                grid-template-columns: 1fr
            }

            .principal {
                height: 180px
            }

            .steps {
                grid-template-columns: 1fr
            }

            .org-branches {
                grid-template-columns: 1fr
            }

            .page h1 {
                font-size: 27px
            }

            .slide h1 {
                font-size: 30px
            }

            .slider {
                height: 355px
            }

            .teacher-grid {
                grid-template-columns: 1fr 1fr
            }
        }
    </style>
</head>

<body>
    <header>
        <div class="container head">
            <a class="brand" href="#beranda" aria-label="SMA ARM LUSTER NUSANTARA beranda"><span
                    class="logo">SMA<br>ALN</span><span>SMA ARM LUSTER NUSANTARA<small>UNGGUL • BERKARAKTER •
                        BERPRESTASI</small></span></a>
            <div style="display:flex;gap:9px;align-items:center"><button class="login-btn" id="openLogin">Login
                    Portal</button><button class="menu" id="menuBtn" aria-label="Buka menu">☰</button></div>
        </div>
        <nav>
            <div class="container nav-inner" id="nav">
                <a href="#beranda" data-page="beranda">Beranda</a><a href="#profil" data-page="profil">Profil</a><a
                    href="#akademik" data-page="akademik">Akademik</a><a href="#kesiswaan"
                    data-page="kesiswaan">Kesiswaan</a><a href="#ppdb" data-page="ppdb">PPDB</a><a href="#berita"
                    data-page="berita">Berita</a><a href="#kontak" data-page="kontak">Kontak</a>
            </div>
        </nav>
    </header>
    <main id="app"></main>
    <footer>
        <div class="container foot">
            <div>
                <div class="brand" style="color:white"><span class="logo"
                        style="border-color:white;color:white">SMA<br>ALN</span><span>SMA ARM LUSTER NUSANTARA</span>
                </div>
                <p>Mewujudkan generasi cerdas, berkarakter, dan siap menghadapi masa depan.</p>
            </div>
            <div><strong>Alamat & Kontak</strong>
                <p>Jl. Purbalingga No. 1, Jawa Tengah</p>
                <p>Email: info@smalusternusantara.sch.id</p>
                <p>Telepon: 0858-5637-1154</p>
            </div>
            <div><strong>Tautan Penting</strong>
                <p><a href="#akademik">Akademik</a> · <a href="#ppdb">PPDB</a> · <a href="#kesiswaan">Kesiswaan</a></p>
                <p>© <span id="year"></span> SMA ARM LUSTER NUSANTARA</p>
            </div>
        </div>
    </footer>
    <div class="modal" id="loginModal" role="dialog" aria-modal="true" aria-labelledby="loginTitle">
        <div class="modal-card"><button class="close" id="closeLogin" aria-label="Tutup">×</button>
            <h2 id="loginTitle">Login Portal Akademik</h2>
            <p>Masuk menggunakan akun siswa atau guru.</p>
            <form id="loginForm">
                <div class="field"><label for="user">NIS / Username</label><input id="user" required
                        placeholder="Masukkan username"></div>
                <div class="field" style="margin-top:12px"><label for="pass">Password</label><input id="pass"
                        type="password" required placeholder="Masukkan password"></div><button class="primary"
                    style="width:100%;margin-top:17px">Masuk</button>
                <div class="notice" id="loginNotice"></div>
            </form>
        </div>
    </div>
    <script>
        const app = document.getElementById('app');
        const pages = {
            beranda: () => `<div class="container hero"><section class="slider" aria-label="Banner utama">
 <div class="slide active"><div><div class="eyebrow" style="color:#c9e1f8">Selamat datang</div><h1>Membangun Masa Depan, Meraih Prestasi</h1><p>SMA ARM LUSTER NUSANTARA menjadi tempat tumbuhnya generasi unggul, kreatif, dan berkarakter.</p><a class="primary" href="#profil">Kenali Sekolah Kami</a></div><div class="slide-art"><img src="https://images.unsplash.com/photo-1523240795612-9a054b0db644?auto=format&fit=crop&w=600&q=80" alt="Siswa Belajar"></div></div>
 <div class="slide"><div><div class="eyebrow" style="color:#c9e1f8">Prestasi siswa</div><h1>Bangga Berkarya dan Berprestasi</h1><p>Dukung potensi dan bakat setiap peserta didik melalui kegiatan akademik maupun nonakademik.</p><a class="primary" href="#berita">Lihat Berita</a></div><div class="slide-art"><img src="https://images.unsplash.com/photo-1577896851231-70ef18881754?auto=format&fit=crop&w=600&q=80" alt="Prestasi Siswa"></div></div>
 <div class="slide"><div><div class="eyebrow" style="color:#c9e1f8">Fasilitas sekolah</div><h1>Lingkungan Belajar yang Mendukung</h1><p>Fasilitas pendidikan untuk pengalaman belajar yang aktif, aman, dan menyenangkan.</p><a class="primary" href="#profil">Lihat Profil</a></div><div class="slide-art"><img src="https://images.unsplash.com/photo-1562774053-701939374585?auto=format&fit=crop&w=600&q=80" alt="Gedung Sekolah"></div></div>
 <button class="slider-arrow prev" aria-label="Slide sebelumnya">‹</button><button class="slider-arrow next" aria-label="Slide berikutnya">›</button><div class="dots"><button class="active" aria-label="Slide 1"></button><button aria-label="Slide 2"></button><button aria-label="Slide 3"></button></div></section></div>
 <section class="container section"><div class="welcome"><div class="principal"><img src="https://images.unsplash.com/photo-1560250097-0b93528c311a?auto=format&fit=crop&w=400&q=80" alt="Kepala Sekolah"></div><div><div class="eyebrow">Sambutan kepala sekolah</div><h2>Selamat Datang di SMA ARM LUSTER NUSANTARA</h2><p>Assalamu’alaikum warahmatullahi wabarakatuh. Kami berkomitmen menghadirkan pendidikan berkualitas yang mengembangkan ilmu pengetahuan, karakter, kreativitas, dan kepedulian. Mari bersama membangun lingkungan belajar yang inspiratif.</p><p style="margin-top:9px"><b>Kepala Sekolah</b>, SMA ARM LUSTER NUSANTARA</p></div></div></section>
 <section class="container section"><div class="section-title"><div><div class="eyebrow">Informasi sekolah</div><h2>Berita Terbaru</h2></div><a class="read" href="#berita">Semua berita →</a></div><div class="cards">
 ${newsCards()}</div></section>
 <section class="container section"><div class="two-col"><div class="panel"><div class="eyebrow">Agenda sekolah</div><h2>Kegiatan Mendatang</h2><div class="event"><span class="event-icon">🎯</span><div><strong>Ekstrakurikuler</strong><small>Pengembangan minat dan bakat siswa</small></div></div><div class="event"><span class="event-icon">🏅</span><div><strong>Kegiatan OSIS</strong><small>Organisasi dan kepemimpinan siswa</small></div></div><div class="event"><span class="event-icon">📅</span><div><strong>Kalender Akademik</strong><small>Informasi agenda pembelajaran</small></div></div></div><div class="panel"><div class="eyebrow">Akses cepat</div><h2>Tautan Penting</h2><div class="quicklinks"><a href="#akademik">📘 Akademik</a><a href="#ppdb">📝 PPDB Online</a><a href="#kesiswaan">🎓 Kesiswaan</a><a href="#portal">🔐 Portal Siswa</a></div></div></div></section>`,
            profil: () => `<div class="container page"><div class="crumb">Beranda / Profil</div><h1>Profil Sekolah</h1><p class="lead">Mengenal visi, misi, dan lingkungan SMA ARM LUSTER NUSANTARA.</p><div class="content-box"><h2>Visi & Misi</h2><div class="grid2"><div class="info"><h3>Visi</h3><p>Menjadi sekolah unggul dalam prestasi, berkarakter, berwawasan lingkungan, dan berdaya saing global.</p></div><div class="info"><h3>Misi</h3><p>Menyelenggarakan pembelajaran berkualitas, membangun karakter, serta mengembangkan potensi dan kreativitas peserta didik.</p></div><div class="info"><h3>Tujuan Pendidikan</h3><p>Menghasilkan lulusan yang kompeten, mandiri, bertanggung jawab, dan peduli terhadap sesama.</p></div><div class="info"><h3>Nilai Sekolah</h3><p>Integritas, disiplin, gotong royong, rasa ingin tahu, dan semangat berprestasi.</p></div></div></div><div class="content-box"><h2>Struktur Organisasi</h2><div class="org"><div class="org-top">Kepala Sekolah</div><div style="height:18px;border-left:2px solid #cad5e0"></div><div class="org-branches"><div><div class="org-node">Wakil Kurikulum</div><p>Guru & Wali Kelas</p></div><div><div class="org-node">Wakil Kesiswaan</div><p>OSIS & Ekstrakurikuler</p></div><div><div class="org-node">Wakil Sarpras</div><p>Laboratorium & Perpustakaan</p></div></div></div></div></div>`,
            akademik: () => `<div class="container page"><div class="crumb">Beranda / Akademik</div><h1>Halaman Akademik</h1><p class="lead">Informasi kurikulum, tenaga pendidik, dan kegiatan pembelajaran.</p><div class="content-box"><h2>Kurikulum</h2><p>SMA ARM LUSTER NUSANTARA menyelenggarakan pembelajaran sesuai kurikulum yang berlaku, dengan penguatan literasi, numerasi, karakter, dan pembelajaran berbasis proyek.</p><div class="grid2"><div class="info"><h3>Program Pembelajaran</h3><p>Pembelajaran intrakurikuler, kokurikuler, dan pengembangan minat.</p></div><div class="info"><h3>Penilaian</h3><p>Penilaian proses dan hasil belajar secara berkala dan transparan.</p></div></div></div><div class="content-box"><h2>Daftar Guru</h2><div class="teacher-grid">${teachersCards()}</div></div></div>`,
            kesiswaan: () => `<div class="container page"><div class="crumb">Beranda / Kesiswaan</div><h1>Halaman Kesiswaan</h1><p class="lead">Informasi kegiatan, organisasi, dan layanan peserta didik.</p><div class="content-box"><h2>Organisasi & Ekstrakurikuler</h2><div class="grid2"><div class="info"><h3>OSIS</h3><p>Wadah belajar kepemimpinan, kerja sama, dan tanggung jawab.</p></div><div class="info"><h3>Pramuka</h3><p>Mengembangkan kemandirian, kedisiplinan, dan kepedulian.</p></div><div class="info"><h3>Olahraga</h3><p>Futsal, bola voli, basket, dan kegiatan kebugaran.</p></div><div class="info"><h3>Seni & Sains</h3><p>Musik, seni rupa, klub sains, dan teknologi.</p></div></div></div><div class="content-box"><h2>Layanan Siswa</h2><p>Hubungi wali kelas atau bagian kesiswaan untuk konsultasi, informasi kegiatan, dan layanan administrasi peserta didik.</p></div></div>`,
            ppdb: () => `<div class="container page"><div class="crumb">Beranda / PPDB</div><h1>Penerimaan Peserta Didik Baru</h1><p class="lead">Ikuti alur pendaftaran dan lengkapi formulir pendaftaran online.</p><div class="content-box"><h2>Alur Pendaftaran</h2><div class="steps"><div class="step"><b>1</b>Isi Formulir</div><div class="step"><b>2</b>Verifikasi Data</div><div class="step"><b>3</b>Pengumuman</div></div><h2>Persyaratan</h2><ul><li>Ijazah atau surat keterangan lulus.</li><li>Kartu keluarga dan akta kelahiran.</li><li>Pas foto terbaru.</li><li>Dokumen pendukung sesuai ketentuan sekolah.</li></ul><p style="color:var(--muted);font-size:13px">Catatan: persyaratan dan jadwal resmi mengikuti pengumuman sekolah.</p></div><div class="content-box"><h2>Formulir Online</h2><form id="ppdbForm" class="form-grid"><div class="field"><label for="nama">Nama lengkap *</label><input id="nama" required placeholder="Nama sesuai dokumen"></div><div class="field"><label for="lahir">Tanggal lahir *</label><input id="lahir" type="date" required></div><div class="field"><label for="email">Email *</label><input id="email" type="email" required placeholder="nama@email.com"></div><div class="field"><label for="hp">Nomor telepon *</label><input id="hp" type="tel" required placeholder="08xxxxxxxxxx"></div><div class="field full"><label for="alamat">Alamat lengkap *</label><textarea id="alamat" rows="3" required placeholder="Alamat tempat tinggal"></textarea></div><div class="field"><label for="asal">Asal sekolah *</label><input id="asal" required></div><div class="field"><label for="jurusan">Pilihan program *</label><select id="jurusan" required><option value="">Pilih program</option><option>Program Reguler</option><option>Program Sains</option><option>Program Sosial</option></select></div><div class="field full"><button class="primary">Kirim Pendaftaran</button><div class="notice" id="ppdbNotice"></div></div></form></div></div>`,
            berita: () => `<div class="container page"><div class="crumb">Beranda / Berita</div><h1>Berita Terbaru</h1><p class="lead">Kabar, informasi, dan dokumentasi kegiatan SMA ARM LUSTER NUSANTARA.</p><div class="cards">${newsCards()}</div></div>`,
            kontak: () => `<div class="container page"><div class="crumb">Beranda / Kontak</div><h1>Alamat & Kontak</h1><p class="lead">Silakan hubungi sekolah untuk informasi lebih lanjut.</p><div class="grid2"><div class="content-box"><h2>Informasi Sekolah</h2><p><b>Alamat</b><br>Jl. Purbalingga No. 1, Jawa Tengah</p><p><b>Email</b><br>info@smalusternusantara.sch.id</p><p><b>Telepon</b><br>0858-5637-1154</p><p><b>Jam layanan</b><br>Senin–Jumat, 07.00–15.00</p></div><div class="content-box"><h2>Kirim Pesan</h2><form id="contactForm"><div class="field"><label>Nama</label><input required></div><div class="field" style="margin-top:12px"><label>Email</label><input type="email" required></div><div class="field" style="margin-top:12px"><label>Pesan</label><textarea rows="4" required></textarea></div><button class="primary" style="margin-top:14px">Kirim Pesan</button><div class="notice" id="contactNotice">Pesan berhasil disiapkan. Hubungkan formulir ke server/email untuk pengiriman sungguhan.</div></form></div></div></div>`,
            portal: () => `<div class="container page"><div class="crumb">Beranda / Portal Akademik</div><h1>Portal Akademik</h1><p class="lead">Contoh tampilan portal setelah login. Data di bawah merupakan data demo.</p><div class="content-box"><h2>Selamat datang, Siswa</h2><div class="portal-grid"><div class="portal-tile">📅<strong>Jadwal Pelajaran</strong><small>Senin–Jumat · Kelas X</small></div><div class="portal-tile">📊<strong>Nilai Rapor</strong><small>Semester berjalan · Data demo</small></div><div class="portal-tile">🗓️<strong>Absensi</strong><small>Rekap kehadiran</small></div><div class="portal-tile">📢<strong>Pengumuman Guru</strong><small>Informasi kelas terbaru</small></div></div></div><div class="content-box"><h2>Jadwal Pelajaran</h2><table class="schedule"><thead><tr><th>Hari</th><th>07.30–09.00</th><th>09.30–11.00</th></tr></thead><tbody><tr><td>Senin</td><td>Matematika</td><td>Bahasa Indonesia</td></tr><tr><td>Selasa</td><td>Bahasa Inggris</td><td>Informatika</td></tr><tr><td>Rabu</td><td>Biologi</td><td>Sejarah</td></tr></tbody></table></div></div>`
        };

        function newsCards() {
            return `
            <article class="card">
                <div class="thumb"><img src="https://images.unsplash.com/photo-1546410531-bb4caa6b424d?auto=format&fit=crop&w=500&q=80" alt="Kompetisi"></div>
                <div class="card-body"><h3>Prestasi Siswa di Ajang Kompetisi</h3><p>Apresiasi untuk siswa yang terus mengembangkan potensi dan meraih prestasi.</p><a class="read" href="#berita"></a></div>
            </article>
            <article class="card">
                <div class="thumb"><img src="https://images.unsplash.com/photo-1532094349884-543bc11b234d?auto=format&fit=crop&w=500&q=80" alt="Eksperimen"></div>
                <div class="card-body"><h3>Kegiatan Pembelajaran Berbasis Proyek</h3><p>Siswa berkolaborasi, bereksperimen, dan menghasilkan karya inovatif.</p><a class="read" href="#berita"></a></div>
            </article>
            <article class="card">
                <div class="thumb"><img src="https://images.unsplash.com/photo-1542601906990-b4d3fb778b09?auto=format&fit=crop&w=500&q=80" alt="Lingkungan"></div>
                <div class="card-body"><h3>Gerakan Sekolah Peduli Lingkungan</h3><p>Membangun kebiasaan menjaga kebersihan dan kelestarian lingkungan.</p><a class="read" href="#berita"></a></div>
            </article>`
        }

        function teachersCards() {
            const list = [
                { name: 'Ibu Ratna, S.Pd.', subject: 'Bahasa Indonesia', img: 'https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?auto=format&fit=crop&w=200&q=80' },
                { name: 'Ibu Dina, S.Pd.', subject: 'Matematika', img: 'https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=200&q=80' },
                { name: 'Ibu Sari, S.Pd.', subject: 'Bahasa Inggris', img: 'https://images.unsplash.com/photo-1544717305-2782549b5136?auto=format&fit=crop&w=200&q=80' },
                { name: 'Bapak Andi, S.Pd.', subject: 'IPA', img: 'https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?auto=format&fit=crop&w=200&q=80' },
                { name: 'Ibu Maya, S.Pd.', subject: 'IPS', img: 'https://images.unsplash.com/photo-1544005313-94ddf0286df2?auto=format&fit=crop&w=200&q=80' },
                { name: 'Bapak Deni, S.Kom.', subject: 'Informatika', img: 'https://images.unsplash.com/photo-1500648767791-00dcc994a43e?auto=format&fit=crop&w=200&q=80' }
            ];
            return list.map(t => `
                <div class="teacher">
                    <div class="avatar"><img src="${t.img}" alt="${t.name}"></div>
                    <b>${t.name}</b>
                    <small>${t.subject}</small>
                </div>
            `).join('');
        }

        function render() {
            let key = location.hash.replace('#', '') || 'beranda';
            if (key === 'portal' && !sessionStorage.getItem('demoLogin')) {
                key = 'beranda';
                location.hash = 'beranda';
                openLogin();
                return;
            }
            if (!pages[key]) key = 'beranda';
            app.innerHTML = pages[key]();
            document.querySelectorAll('[data-page]').forEach(a => a.classList.toggle('active', a.dataset.page === key));
            document.getElementById('nav').classList.remove('open');
            wirePage(key);
        }

        function wirePage(key) {
            if (key === 'beranda') {
                let slides = [...document.querySelectorAll('.slide')],
                    dots = [...document.querySelectorAll('.dots button')],
                    idx = 0;
                function show(n) {
                    idx = (n + slides.length) % slides.length;
                    slides.forEach((s, i) => s.classList.toggle('active', i === idx));
                    dots.forEach((d, i) => d.classList.toggle('active', i === idx));
                }
                document.querySelector('.next').onclick = () => show(idx + 1);
                document.querySelector('.prev').onclick = () => show(idx - 1);
                dots.forEach((d, i) => d.onclick = () => show(i));
                if (window.slideTimer) clearInterval(window.slideTimer);
                window.slideTimer = setInterval(() => show(idx + 1), 6000);
            }
            let pf = document.getElementById('ppdbForm');
            if (pf) pf.onsubmit = e => {
                e.preventDefault();
                document.getElementById('ppdbNotice').style.display = 'block';
                document.getElementById('ppdbNotice').textContent = 'Pendaftaran demo berhasil divalidasi. Untuk menyimpan data sungguhan, hubungkan formulir ini ke backend.';
                pf.reset();
            };
            let cf = document.getElementById('contactForm');
            if (cf) cf.onsubmit = e => {
                e.preventDefault();
                document.getElementById('contactNotice').style.display = 'block';
                cf.reset();
            };
        }

        const modal = document.getElementById('loginModal');
        function openLogin() {
            modal.classList.add('show');
            document.getElementById('user').focus();
        }
        document.getElementById('openLogin').onclick = openLogin;
        document.getElementById('closeLogin').onclick = () => modal.classList.remove('show');
        modal.addEventListener('click', e => { if (e.target === modal) modal.classList.remove('show'); });
        document.addEventListener('keydown', e => { if (e.key === 'Escape') modal.classList.remove('show'); });
        document.getElementById('loginForm').onsubmit = e => {
            e.preventDefault();
            sessionStorage.setItem('demoLogin', '1');
            modal.classList.remove('show');
            location.hash = 'portal';
            document.getElementById('loginNotice').style.display = 'none';
        };
        document.getElementById('menuBtn').onclick = () => document.getElementById('nav').classList.toggle('open');
        window.addEventListener('hashchange', render);
        document.getElementById('year').textContent = new Date().getFullYear();
        render();
    </script>
</body>

</html>
