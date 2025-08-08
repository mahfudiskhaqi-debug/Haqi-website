<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Haqi Hosting — Hosting, VPS, Cloud, Domain — Profesional</title>
  <meta name="description" content="Haqi Hosting — solusi hosting profesional: Shared Hosting, VPS, Dedicated Server, Cloud, Domain, Backup, Security, dan layanan 24/7." />
  <meta name="author" content="Haqi Hosting" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <style>
    /* ===========================
       Haqi Hosting — Single-file CSS
       Author: Haqi Hosting / By Haqi
       Purpose: Full landing page with many sections, animation, and professional look
       =========================== */

    :root{
      --bg-1: #071025;
      --bg-2: #08132a;
      --card: rgba(255,255,255,0.03);
      --muted: #b8c6d6;
      --accent: #0ea5e9;
      --accent-2: #7c3aed;
      --glass: rgba(255,255,255,0.03);
      --glass-2: rgba(255,255,255,0.02);
      --success: #22c55e;
      --danger: #ef4444;
      --max-width: 1200px;
    }

    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      background: linear-gradient(180deg,var(--bg-1) 0%, var(--bg-2) 60%);
      color:#eaf2fb;
      font-family:'Poppins',system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.45;
      -webkit-tap-highlight-color: transparent;
    }

    /* Container */
    .wrap{
      max-width:var(--max-width);
      margin:0 auto;
      padding:28px;
    }

    /* Header */
    header.site-header{
      position:sticky;
      top:0;
      z-index:9999;
      backdrop-filter: blur(8px);
      background: linear-gradient(180deg, rgba(7,16,37,0.55), rgba(7,16,37,0.25));
      border-bottom:1px solid rgba(255,255,255,0.03);
    }
    .header-inner{display:flex;align-items:center;justify-content:space-between;gap:12px;max-width:var(--max-width);margin:0 auto;padding:14px 22px}
    .brand{display:flex;gap:12px;align-items:center}
    .brand .logo{
      width:56px;height:56px;border-radius:12px;display:flex;align-items:center;justify-content:center;font-weight:800;
      background: linear-gradient(135deg,var(--accent),var(--accent-2));
      color:#031428;font-size:16px;
      box-shadow: 0 6px 20px rgba(12,34,60,0.45), inset 0 -4px 10px rgba(255,255,255,0.06);
    }
    .brand .title{font-weight:700;font-size:18px}
    .brand .tag{font-size:12px;color:var(--muted);margin-top:2px}

    nav.top-nav{display:flex;gap:12px;align-items:center}
    nav.top-nav a{color:var(--muted);text-decoration:none;font-weight:600;padding:8px 10px;border-radius:8px}
    nav.top-nav a:hover{color:#fff;background:rgba(255,255,255,0.02)}
    .cta-btn{background:linear-gradient(90deg,var(--accent),var(--accent-2));border:none;padding:10px 14px;border-radius:10px;font-weight:700;color:#031428;cursor:pointer;box-shadow: 0 8px 26px rgba(12,34,60,0.45)}

    /* Hero */
    .hero{
      display:grid;
      grid-template-columns: 1fr 420px;
      gap:28px;
      align-items:start;
      margin-top:28px;
      margin-bottom:30px;
    }

    .hero-left h1{
      font-size:40px;
      margin:0 0 10px 0;
      line-height:1.05;
      letter-spacing:-0.4px;
    }
    .hero-left p.lead{color:var(--muted);max-width:720px;margin:8px 0 18px 0}
    .hero-features{display:flex;gap:12px;flex-wrap:wrap;margin-top:18px}

    .feature-pill{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      padding:10px 12px;border-radius:12px;border:1px solid rgba(255,255,255,0.03);
      display:flex;align-items:center;gap:10px;font-weight:600;color:#e8f6ff;
    }
    .feature-pill small{color:var(--muted);font-weight:500;font-size:12px}

    .cta-row{display:flex;gap:12px;margin-top:18px}
    .secondary-btn{background:transparent;border:1px solid rgba(255,255,255,0.04);padding:10px 12px;border-radius:10px;color:var(--muted);cursor:pointer}

    /* Right card */
    .card{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      padding:16px;
      border-radius:14px;
      border:1px solid rgba(255,255,255,0.03);
      box-shadow: 0 8px 24px rgba(2,6,23,0.6);
    }

    .pricing-list{display:flex;flex-direction:column;gap:10px}
    .price-item{display:flex;justify-content:space-between;align-items:center;padding:12px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.01), transparent);border:1px solid rgba(255,255,255,0.02)}
    .price-item .meta{font-size:13px;color:var(--muted)}
    .price-amount{font-weight:900;font-size:16px}

    /* Sections */
    section{margin-top:26px}
    h2.section-title{font-size:22px;margin:0 0 14px 0}
    .grid-2{display:grid;grid-template-columns:repeat(2,1fr);gap:18px}
    .grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
    .grid-4{display:grid;grid-template-columns:repeat(4,1fr);gap:14px}
    .text-muted{color:var(--muted)}

    /* Service card */
    .service{
      padding:14px;border-radius:12px;background:linear-gradient(180deg,rgba(255,255,255,0.015),transparent);
      border:1px solid rgba(255,255,255,0.02);
      transition:transform .28s ease, box-shadow .28s ease;
      min-height:120px;
      display:flex;flex-direction:column;gap:10px;
    }
    .service:hover{transform:translateY(-8px);box-shadow:0 18px 50px rgba(2,8,20,0.6)}
    .service h3{margin:0;font-size:16px}
    .service p{margin:0;color:var(--muted);font-size:14px}

    /* Examples / Use cases */
    .example-card{padding:12px;border-radius:10px;background:linear-gradient(180deg,rgba(255,255,255,0.01),transparent);border:1px solid rgba(255,255,255,0.02)}

    /* Testimonials */
    .testimonials{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
    .testimonial{padding:16px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);border:1px solid rgba(255,255,255,0.02)}
    .quote{font-style:italic;color:var(--muted);font-size:14px}

    /* FAQ */
    .faq .q{font-weight:700}
    .faq .a{color:var(--muted);margin-top:6px}

    /* Contact form */
    form.contact-form{display:flex;flex-direction:column;gap:10px}
    input[type="text"], input[type="email"], textarea, select{
      background:transparent;border:1px solid rgba(255,255,255,0.04);padding:12px;border-radius:10px;color:inherit;font-size:14px;
    }
    textarea{min-height:160px;resize:vertical}
    .form-row{display:flex;gap:10px}
    .form-row .col{flex:1}

    /* Footer */
    footer.site-footer{margin-top:36px;padding:22px;border-top:1px solid rgba(255,255,255,0.03);background:linear-gradient(180deg,transparent,rgba(0,0,0,0.04))}
    .footer-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}

    /* Utilities */
    .muted{color:var(--muted)}
    .center{text-align:center}
    .small{font-size:13px}
    .badge{display:inline-block;padding:6px 10px;border-radius:999px;background:rgba(255,255,255,0.03);border:1px solid rgba(255,255,255,0.02);font-weight:700}

    /* Fancy backgrounds & shapes */
    .bg-dots{
      position:absolute;right:0;top:120px;width:420px;height:420px;pointer-events:none;opacity:0.06;
      background-image: radial-gradient(circle at 10px 10px, rgba(255,255,255,0.03) 2px, transparent 2px);
      background-size:24px 24px;border-radius:999px;transform:translateX(20%);filter:blur(6px)
    }

    /* Animations */
    .float{animation:float 6s ease-in-out infinite}
    @keyframes float{0%{transform:translateY(0)}50%{transform:translateY(-10px)}100%{transform:translateY(0)}}

    /* Responsive */
    @media (max-width:1100px){
      .hero{grid-template-columns:1fr}
      .pricing-right{order:2}
      .grid-3{grid-template-columns:repeat(2,1fr)}
      .testimonials{grid-template-columns:repeat(2,1fr)}
      .footer-grid{grid-template-columns:repeat(1,1fr)}
    }
    @media (max-width:640px){
      .header-inner{padding:10px}
      .brand .title{font-size:16px}
      .hero-left h1{font-size:28px}
      .grid-3{grid-template-columns:1fr}
      .testimonials{grid-template-columns:1fr}
      .hero{gap:12px}
    }

    /* Long page anchor smooth scroll */
    html{scroll-behavior:smooth}

    /* accessibility focus */
    a:focus, button:focus, input:focus, textarea:focus{outline:3px solid rgba(14,165,233,0.18);outline-offset:2px}

    /* Extra large content spacing for long page */
    .spacer-lg{height:28px}
    .spacer-xl{height:48px}

    /* Decorative horizontal rule */
    .hr{
      height:1px;background:linear-gradient(90deg,transparent,rgba(255,255,255,0.03),transparent);margin:18px 0;border-radius:2px;
    }

    /* subtle loaders and shimmer */
    .shimmer{
      background: linear-gradient(90deg, rgba(255,255,255,0.02) 25%, rgba(255,255,255,0.04) 50%, rgba(255,255,255,0.02) 75%);
      background-size: 200% 100%;
      animation: shimmer 2.6s linear infinite;
    }
    @keyframes shimmer{0%{background-position:-200% 0}100%{background-position:200% 0}}

    /* sticky footer copyright */
    .sticky-copyright{position:sticky;bottom:0;background:linear-gradient(180deg, rgba(2,6,23,0.0), rgba(2,6,23,0.2));padding:12px 18px;border-top:1px solid rgba(255,255,255,0.02)}
  </style>
</head>
<body>
  <header class="site-header" role="banner">
    <div class="header-inner">
      <div class="brand" aria-label="Haqi Hosting">
        <div class="logo">HQ</div>
        <div>
          <div class="title">Haqi Hosting</div>
          <div class="tag">Hosting • VPS • Cloud • Domain</div>
        </div>
      </div>

      <nav class="top-nav" role="navigation" aria-label="Main Navigation">
        <a href="#layanan">Layanan</a>
        <a href="#paket">Paket</a>
        <a href="#contoh">Contoh</a>
        <a href="#faq">FAQ</a>
        <a href="#tanya">Tanya</a>
        <button class="cta-btn" onclick="document.getElementById('tanya').scrollIntoView({behavior:'smooth'})">Order Sekarang</button>
      </nav>
    </div>
  </header>

  <div class="wrap" role="main">
    <!-- Hero -->
    <section class="hero" aria-labelledby="hero-heading">
      <div class="hero-left">
        <h1 id="hero-heading">Haqi Hosting — Infrastruktur Profesional untuk Website & Aplikasi Anda</h1>
        <p class="lead">Kami menyediakan solusi hosting yang handal dan aman: Shared Hosting cepat, VPS fleksibel, Dedicated Server untuk performa maksimal, dan layanan Cloud yang dapat di-skala sesuai kebutuhan. Dukungan teknis 24/7, backup otomatis, SSL gratis, dan proteksi DDoS. Haqi Hosting — solusi sederhana, performa nyata.</p>

        <div class="hero-features" aria-hidden="false">
          <div class="feature-pill"><strong>99.99% Uptime</strong><small>Monitoring & SLA</small></div>
          <div class="feature-pill"><strong>Backup Harian</strong><small>Restore instan</small></div>
          <div class="feature-pill"><strong>Support 24/7</strong><small>Live chat & ticket</small></div>
          <div class="feature-pill"><strong>SSD NVMe</strong><small>Performa tinggi</small></div>
        </div>

        <div class="cta-row">
          <button class="cta-btn" onclick="document.getElementById('paket').scrollIntoView({behavior:'smooth'})">Lihat Paket & Harga</button>
          <button class="secondary-btn" onclick="document.getElementById('layanan').scrollIntoView({behavior:'smooth'})">Detail Layanan</button>
        </div>

        <div class="spacer-lg"></div>

        <!-- Long descriptive content — deliberately verbose to meet user's request for many lines -->
        <article class="card" aria-label="Deskripsi lengkap">
          <h2 style="margin-top:0">Tentang Haqi Hosting</h2>
          <p class="text-muted">Haqi Hosting didirikan dengan tujuan memberikan layanan infrastruktur digital profesional bagi individu, UKM, developer, dan enterprise kecil. Kami percaya bahwa performa, keamanan, dan dukungan yang jelas adalah fondasi layanan yang baik. Infrastruktur kami dibangun menggunakan hardware modern, jaringan peering multi-carrier, dan sistem monitoring otomatis sehingga setiap gangguan bisa ditangani dengan cepat.</p>

          <p class="text-muted">Layanan kami mencakup: pemasangan website, migrasi tanpa downtime, optimasi performa untuk WordPress dan aplikasi Node/PHP/Python, manajemen database, serta layanan tambahan seperti konfigurasi CDN, load balancer, dan snapshot backup. Tim teknis kami berpengalaman menghadapi berbagai kasus — dari konfigurasi server sederhana hingga penanganan lonjakan traffic saat kampanye promosi besar.</p>

          <p class="text-muted">Kami menyediakan tiga jalur layanan utama: paket hemat untuk pemula, paket menengah untuk toko online dan aplikasi bisnis, serta paket high-performance untuk kebutuhan enterprise. Setiap paket bisa disesuaikan; misalnya menambah snapshot backup terjadwal, penambahan IP dedicated, atau integrasi monitoring eksternal. Semua perubahan bisa dilakukan melalui dashboard konsol atau melalui request support.</p>

          <div class="hr"></div>

          <h3 style="margin-bottom:8px">Keunggulan Teknis</h3>
          <ul style="color:var(--muted)">
            <li>Hardware: CPU generasi terbaru, RAM ECC, storage NVMe RAID</li>
            <li>Network: Multiple uplink, BGP peering, low-latency routing</li>
            <li>Keamanan: WAF, firewall, proteksi brute-force, pemantauan integritas file</li>
            <li>Operasional: Backup harian otomatis, snapshot on-demand, monitoring 24/7</li>
            <li>Dukungan: Ticketing, live chat, knowledgebase lengkap</li>
          </ul>

          <p class="text-muted">Kami juga menawarkan layanan konsultan infrastruktur: perencanaan arsitektur untuk skala besar, replikasi database, dan desain high-availability untuk aplikasi misi-kritis. Jika Anda membutuhkan SLA khusus atau kontrak enterprise, tim penjualan kami siap menyusun penawaran sesuai kebutuhan Anda.</p>
        </article>

      </div>

      <!-- Right column: pricing & highlights -->
      <aside class="pricing-right">
        <div class="card float">
          <h3 style="margin-top:0">Paket Populer — Pilih yang Cocok</h3>
          <div class="pricing-list" aria-hidden="false" style="margin-top:12px">
            <div class="price-item">
              <div>
                <div style="font-weight:800">Shared Basic</div>
                <div class="meta">1 vCPU • 1 GB RAM • 10 GB NVMe • 1 domain</div>
              </div>
              <div class="price-amount">Rp 25.000 / bln</div>
            </div>

            <div class="price-item">
              <div>
                <div style="font-weight:800">Shared Pro</div>
                <div class="meta">2 vCPU • 2 GB RAM • 25 GB NVMe • gratis SSL</div>
              </div>
              <div class="price-amount">Rp 55.000 / bln</div>
            </div>

            <div class="price-item">
              <div>
                <div style="font-weight:800">VPS Starter</div>
                <div class="meta">2 vCPU • 4 GB RAM • 80 GB NVMe • root access</div>
              </div>
              <div class="price-amount">Rp 150.000 / bln</div>
            </div>

            <div class="price-item">
              <div>
                <div style="font-weight:800">VPS Business</div>
                <div class="meta">4 vCPU • 8 GB RAM • 160 GB NVMe • snapshot</div>
              </div>
              <div class="price-amount">Rp 320.000 / bln</div>
            </div>

            <div class="price-item">
              <div>
                <div style="font-weight:800">Dedicated 2 vCore</div>
                <div class="meta">2 Cores • 8 GB RAM • 200 GB NVMe • dedicated IP</div>
              </div>
              <div class="price-amount">Rp 1.200.000 / bln</div>
            </div>

            <div class="price-item">
              <div>
                <div style="font-weight:800">Cloud Scale</div>
                <div class="meta">Flexible compute • Billing per-hour • Auto-scale</div>
              </div>
              <div class="price-amount">Mulai Rp 200.000 / bln</div>
            </div>
          </div>

          <div style="margin-top:12px;display:flex;gap:10px">
            <button class="cta-btn" onclick="alert('Terima kasih! Untuk order, silakan kontak: mahfudikskhaqi@gmail.com atau WhatsApp.')">Order</button>
            <button class="secondary-btn" onclick="document.getElementById('faq').scrollIntoView({behavior:'smooth'})">Lihat FAQ</button>
          </div>
        </div>

        <div style="height:18px"></div>

        <div class="card">
          <h4 style="margin-top:0">Alasan Memilih Kami</h4>
          <ul style="color:var(--muted);margin:8px 0 0 0">
            <li>Tim support cepat dan berpengalaman</li>
            <li>Infrastruktur handal & monitoring penuh</li>
            <li>Harga kompetitif, transparan tanpa biaya tersembunyi</li>
            <li>Pilihan upgrade fleksibel kapan saja</li>
          </ul>
        </div>
      </aside>
    </section>

    <div class="bg-dots" aria-hidden="true"></div>

    <div class="spacer-xl"></div>

    <!-- Layanan detail -->
    <section id="layanan" aria-labelledby="layanan-title">
      <h2 id="layanan-title" class="section-title">Layanan Lengkap Haqi Hosting</h2>
      <p class="text-muted">Ringkasan lengkap layanan kami — baca detail tiap layanan untuk memahami apa yang cocok bagi Anda.</p>

      <div class="grid-2" style="margin-top:12px">
        <div class="card">
          <h3>Shared Hosting</h3>
          <p class="text-muted">Solusi ekonomis untuk blog, portofolio, dan website kecil. Panel cPanel, instal otomatis WordPress, backup otomatis, dan domain management.</p>
          <h4 style="margin-bottom:6px">Fitur Utama</h4>
          <ul class="text-muted">
            <li>Instal 1-klik untuk WordPress, Laravel, dan CMS populer</li>
            <li>Control Panel mudah digunakan</li>
            <li>Mail hosting & webmail</li>
            <li>Gratis SSL & Proteksi dasar</li>
          </ul>
        </div>

        <div class="card">
          <h3>VPS</h3>
          <p class="text-muted">VPS dengan resource dedicated virtual, cocok untuk e-commerce, aplikasi, dan testing. Root access, snapshot, dan pilihan OS.</p>
          <h4 style="margin-bottom:6px">Fitur Utama</h4>
          <ul class="text-muted">
            <li>Root access & control penuh</li>
            <li>Snapshot & backup otomatis</li>
            <li>Panel manajemen VPS (opsional)</li>
            <li>Traffic tinggi & networking cepat</li>
          </ul>
        </div>

        <div class="card">
          <h3>Dedicated Server</h3>
          <p class="text-muted">Server fisik untuk beban tinggi dan kebutuhan khusus. Pilihan konfigurasi CPU/RAM/Storage sesuai permintaan.</p>
          <h4 style="margin-bottom:6px">Fitur Utama</h4>
          <ul class="text-muted">
            <li>Hardware khusus untuk performa maksimal</li>
            <li>Dedicated IP & bandwidth</li>
            <li>Managed atau unmanaged</li>
          </ul>
        </div>

        <div class="card">
          <h3>Cloud Hosting & Kubernetes</h3>
          <p class="text-muted">Infrastruktur cloud untuk auto-scaling, container, dan aplikasi microservices. Billing fleksibel per penggunaan.</p>
          <h4 style="margin-bottom:6px">Fitur Utama</h4>
          <ul class="text-muted">
            <li>Autoscaling, load balancing, managed DB</li>
            <li>Container registry & Kubernetes</li>
            <li>CI/CD pipeline integration</li>
          </ul>
        </div>
      </div>

      <div class="spacer-lg"></div>

      <!-- Additional service modules repeated for length -->
      <div class="grid-3">
        <div class="service">
          <h3>Domain Registration</h3>
          <p class="text-muted">Pendaftaran domain .com, .id, .net, .org, dan banyak TLD lainnya dengan harga terjangkau dan pengelolaan DNS penuh.</p>
          <p class="text-muted">Fitur DNS management, forwarding, WHOIS privacy (opsional), dan auto-renew.</p>
        </div>

        <div class="service">
          <h3>SSL & Keamanan</h3>
          <p class="text-muted">SSL gratis (Let's Encrypt) atau wildcard dan EV SSL untuk keamanan tingkat lanjut. Proteksi WAF & DDoS tersedia.</p>
        </div>

        <div class="service">
          <h3>Backup & Restore</h3>
          <p class="text-muted">Backup harian atau custom schedule, penyimpanan snapshot, dan restore mudah dari dashboard.</p>
        </div>

        <div class="service">
          <h3>Managed Database</h3>
          <p class="text-muted">MySQL, PostgreSQL, Redis managed — backup, monitoring, dan tuning performa oleh tim kami.</p>
        </div>

        <div class="service">
          <h3>Migration Service</h3>
          <p class="text-muted">Migrasi website dari provider lain tanpa downtime. Tim teknis akan meng-handle seluruh proses migrasi.</p>
        </div>

        <div class="service">
          <h3>Custom Support</h3>
          <p class="text-muted">Support berbayar untuk konfigurasi khusus, audit keamanan, dan optimisasi performa.</p>
        </div>
      </div>

      <div class="spacer-xl"></div>

      <!-- Deep dive sections — verbose (multiple paragraphs to increase line count) -->
      <article class="card">
        <h3 style="margin-top:0">Rincian Teknis (Deep Dive)</h3>
        <p class="text-muted">Arsitektur kami menggabungkan beberapa layer proteksi dan optimasi performa. Mulai dari SSD NVMe untuk storage, caching layer (Redis / Varnish), hingga CDN optional untuk mempercepat load time secara global. Database diisolasi dan diberi sumber daya memadai untuk mengurangi latency query. Untuk server aplikasi, kami menggunakan orchestrator yang memastikan container terdistribusi dengan rapi dan dapat di-scale sesuai kebutuhan.</p>

        <p class="text-muted">Monitoring dilakukan menggunakan sistem SIEM internal dan third-party monitoring yang terintegrasi dengan notifikasi real-time ke tim operasi. Kami melakukan patching berkala, audit keamanan, dan uji penetrasi secara berkala untuk meminimalkan celah keamanan. Selain itu, kami menyediakan opsi managed backup offsite untuk kebutuhan compliance dan recovery point objective (RPO) rendah.</p>

        <p class="text-muted">Untuk jaringan, setiap node dilengkapi multi-carrier BGP, peering langsung dengan beberapa ISP besar untuk mengurangi hop dan menjaga latency. Kami juga menyertakan route optimization untuk mengarahkan traffic melalui jalur tercepat ke user akhir. Semua ini bertujuan memberikan pengalaman pengguna akhir yang snappy dan resilien di semua kondisi lalu lintas.</p>
      </article>

      <div class="spacer-lg"></div>

    </section>

    <div class="spacer-lg"></div>

    <!-- Contoh penggunaan -->
    <section id="contoh" aria-labelledby="contoh-title">
      <h2 id="contoh-title" class="section-title">Contoh Penggunaan & Studi Kasus</h2>
      <p class="text-muted">Beberapa contoh deployment dan bagaimana Haqi Hosting membantu berbagai jenis proyek.</p>

      <div class="grid-3" style="margin-top:12px">
        <div class="example-card">
          <h4>Website Bisnis / Corporate</h4>
          <p class="text-muted">Paket shared pro cukup untuk landing page bisnis hingga situs multi-halaman. Untuk trafik besar, kami merekomendasikan VPS Business dengan scaling atau Cloud jika butuh autoscale.</p>
          <p class="text-muted small">Contoh: perusahaan startup e-commerce yang membutuhkan 10x traffic saat flash sale — solusi: auto-scaling Cloud + CDN + cache layer.</p>
        </div>

        <div class="example-card">
          <h4>Toko Online</h4>
          <p class="text-muted">E-commerce butuh database stabil dan backup. VPS atau Dedicated dengan snapshot teratur sangat direkomendasikan. Kami juga suport integrasi payment gateway, anti-fraud, dan optimasi image delivery.</p>
        </div>

        <div class="example-card">
          <h4>Game Server</h4>
          <p class="text-muted">Server low-latency & proteksi DDoS untuk game multiplayer. Kami menyediakan paket khusus untuk game hosting termasuk monitoring dan prioritas jaringan.</p>
        </div>

        <div class="example-card">
          <h4>Web App / SaaS</h4>
          <p class="text-muted">Infrastruktur microservices, database managed, dan CI/CD pipeline untuk deployment terus menerus. Monitoring dan alerting lengkap untuk menjaga SLA layanan Anda.</p>
        </div>

        <div class="example-card">
          <h4>Agency & Developer</h4>
          <p class="text-muted">Account multi-project, staging environment, Git deployment, dan akses tim — cocok untuk agensi dan developer yang butuh kontrol.</p>
        </div>

        <div class="example-card">
          <h4>Startup / MVP</h4>
          <p class="text-muted">Paket hemat untuk validasi produk, lalu scale up ke VPS atau Cloud saat traction meningkat. Konsultasi awal gratis untuk arsitektur cost-effective.</p>
        </div>
      </div>

      <div class="spacer-lg"></div>

      <!-- Extended example descriptions to add more lines -->
      <article class="card">
        <h3 style="margin-top:0">Studi Kasus: Toko Online Lokal</h3>
        <p class="text-muted">Seorang klien e-commerce mengalami lambat saat traffic puncak. Analisis kami menemukan bottleneck pada query database dan images tanpa optimasi. Solusi: migrasi ke VPS Business, optimasi query, setup caching di Varnish, dan CDN untuk static asset. Hasilnya: waktu muat turun halaman berkurang 3x, conversion rate meningkat 18% selama kampanye penjualan.</p>

        <p class="text-muted">Implementasi tersebut melibatkan koordinasi antara tim dev klien dan ops kami. Kami melakukan pengujian load, setup auto-scaling scripts, dan konfigurasi backup. Semua dilakukan dengan downtime minimal melalui strategi blue/green deployment.</p>
      </article>

    </section>

    <div class="spacer-xl"></div>

    <!-- More content — repeating patterns to reach requested length -->
    <section aria-labelledby="security-title">
      <h2 id="security-title" class="section-title">Keamanan & Compliance</h2>
      <p class="text-muted">Keamanan adalah prioritas. Berikut ringkasan praktik keamanan yang kami jalankan:</p>

      <div class="grid-3" style="margin-top:12px">
        <div class="service">
          <h3>Pemantauan & Alerts</h3>
          <p class="text-muted">Monitoring 24/7, notifikasi melalui Slack / Email / SMS, dan playbook untuk eskalasi insiden.</p>
        </div>

        <div class="service">
          <h3>Patch Management</h3>
          <p class="text-muted">Penerapan patch berkala untuk sistem operasi dan aplikasi, termasuk zero-downtime patch jika memungkinkan.</p>
        </div>

        <div class="service">
          <h3>Firewall & WAF</h3>
          <p class="text-muted">Web Application Firewall untuk memblok serangan injeksi, XSS, dan pola traffic mencurigakan.</p>
        </div>

        <div class="service">
          <h3>Backup & Disaster Recovery</h3>
          <p class="text-muted">Backup offsite dengan enkripsi, recovery plan disesuaikan SLA pelanggan.</p>
        </div>

        <div class="service">
          <h3>Enkripsi & Sertifikat</h3>
          <p class="text-muted">SSL/TLS wajib, pilihan EV untuk kepentingan trust dan keamanan transaksi.</p>
        </div>

        <div class="service">
          <h3>Audit & Pentest</h3>
          <p class="text-muted">Layanan audit keamanan & penetration testing atas permintaan.</p>
        </div>
      </div>

      <div class="spacer-lg"></div>

      <article class="card">
        <h3 style="margin-top:0">Protokol Insiden</h3>
        <p class="text-muted">Jika terjadi insiden keamanan, langkah kami: identifikasi, isolasi sistem terdampak, mitigasi dampak, dan memulihkan layanan. Sebagai bagian dari layanan premium, kami menyediakan laporan insiden terperinci dan rekomendasi untuk perbaikan jangka panjang.</p>

        <p class="text-muted">Tim kami juga membantu koordinasi disclosure ke pihak terkait bila diperlukan dan mendampingi proses hukum atau komunikasi publik apabila kasus memerlukan transparansi publik.</p>
      </article>
    </section>

    <div class="spacer-xl"></div>

    <!-- Pricing matrix / comparison table (verbose) -->
    <section id="paket" aria-labelledby="paket-title">
      <h2 id="paket-title" class="section-title">Perbandingan Paket</h2>
      <p class="text-muted">Tabel perbandingan fitur agar mudah memilih paket yang paling sesuai.</p>

      <div style="overflow:auto;margin-top:12px">
        <table style="width:100%;border-collapse:collapse;min-width:880px;">
          <thead>
            <tr style="text-align:left">
              <th style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.03)">Paket</th>
              <th style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.03)">Resource</th>
              <th style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.03)">Traffic</th>
              <th style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.03)">Backup</th>
              <th style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.03)">Support</th>
              <th style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.03)">Harga</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Shared Basic</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">1 vCPU • 1GB RAM • 10GB NVMe</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Unlimited (Fair Use)</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Weekly</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Email</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Rp 25.000 / bln</td>
            </tr>

            <tr>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Shared Pro</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">2 vCPU • 2GB RAM • 25GB NVMe</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Unlimited (Fair Use)</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Daily</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Live Chat & Email</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Rp 55.000 / bln</td>
            </tr>

            <tr>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">VPS Starter</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">2 vCPU • 4GB RAM • 80GB NVMe</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Dedicated</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Daily + Snapshot</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Support 24/7</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Rp 150.000 / bln</td>
            </tr>

            <tr>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">VPS Business</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">4 vCPU • 8GB RAM • 160GB NVMe</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Dedicated</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Hourly Snapshot</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Priority 24/7</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Rp 320.000 / bln</td>
            </tr>

            <tr>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Dedicated 2 vCore</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">2 Cores • 8GB RAM • 200GB NVMe</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Dedicated</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Custom</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Managed Ops</td>
              <td style="padding:12px;border-bottom:1px solid rgba(255,255,255,0.02)">Rp 1.200.000 / bln</td>
            </tr>
          </tbody>
        </table>
      </div>

      <div class="spacer-lg"></div>

      <p class="text-muted small">Harga dan konfigurasi dapat berubah sesuai permintaan dan ketersediaan. Hubungi kami untuk penawaran kustom dan diskon langganan tahunan.</p>
    </section>

    <div class="spacer-xl"></div>

    <!-- Testimonials (repeated with variations to create many lines) -->
    <section aria-labelledby="testi-title">
      <h2 id="testi-title" class="section-title">Testimonial Pelanggan</h2>
      <p class="text-muted">Beberapa cerita sukses dari pelanggan kami.</p>

      <div class="testimonials" style="margin-top:12px">
        <div class="testimonial">
          <strong>Rizky A. — Founder TokoOnline.id</strong>
          <p class="quote">"Migrasi ke Haqi Hosting membuat website kami lebih stabil. Timnya sangat membantu saat setup. Loading page jauh lebih cepat."</p>
        </div>

        <div class="testimonial">
          <strong>Siti L. — CTO Startup</strong>
          <p class="quote">"Kami butuh autoscale saat launch. Solusi Cloud dari Haqi Hosting bekerja mulus dan biaya tetap terkendali."</p>
        </div>

        <div class="testimonial">
          <strong>Andi M. — Developer Freelance</strong>
          <p class="quote">"Support tim cepat dan informatif. Rekomendasi optimasi yang mereka berikan benar-benar menaikkan performa."</p>
        </div>
      </div>

      <div class="spacer-lg"></div>
    </section>

    <div class="spacer-xl"></div>

    <!-- FAQ with many Q/A to lengthen content -->
    <section id="faq" aria-labelledby="faq-title">
      <h2 id="faq-title" class="section-title">FAQ — Pertanyaan yang Sering Diajukan</h2>
      <div class="faq" style="margin-top:12px">
        <div class="card">
          <div class="q">1. Berapa lama proses migrasi website?</div>
          <div class="a text-muted">Proses migrasi biasanya 1-24 jam tergantung kompleksitas website dan ukuran data. Kami prioritaskan migrasi tanpa downtime jika memungkinkan.</div>
          <div class="hr"></div>

          <div class="q">2. Apakah ada garansi uptime?</div>
          <div class="a text-muted">Kami berkomitmen pada uptime tinggi dan menargetkan 99.99% SLA pada paket tertentu. Detail SLA akan tercantum pada kontrak layanan.</div>
          <div class="hr"></div>

          <div class="q">3. Bagaimana dengan backup?</div>
          <div class="a text-muted">Backup harian tersedia pada paket tertentu; snapshot dan backup offsite tersedia sebagai add-on.</div>
          <div class="hr"></div>

          <div class="q">4. Apakah Haqi Hosting menyediakan domain?</div>
          <div class="a text-muted">Ya, kami menyediakan pendaftaran domain dan DNS management. Layanan domain terpisah dari hosting dan memiliki syarat renew sendiri.</div>
          <div class="hr"></div>

          <div class="q">5. Bagaimana cara pembayaran?</div>
          <div class="a text-muted">Pembayaran via transfer bank, e-wallet, dan metode lain yang kami dukung. Untuk pelanggan enterprise, invoice dan billing cycle dapat disesuaikan.</div>
        </div>
      </div>

      <div class="spacer-lg"></div>
    </section>

    <div class="spacer-xl"></div>

    <!-- Contact / Ask section — user's email mailbox via mailto (as requested) -->
    <section id="tanya" aria-labelledby="tanya-title">
      <h2 id="tanya-title" class="section-title">Tanyakan Sesuatu — Hubungi Kami</h2>
      <p class="text-muted">Isi form di bawah untuk mengirim pertanyaan. Email akan dikirim ke inbox kami.</p>

      <!-- Note: using mailto action as user requested (raw string provided by user) -->
      <form class="contact-form card" action="mailto:mahfudikskhaqi@gmail.com" method="post" enctype="text/plain" onsubmit="return handleMailto(event)">
        <div class="form-row">
          <div class="col">
            <label class="small muted">Nama</label>
            <input type="text" name="Nama" placeholder="Nama Anda" required />
          </div>
          <div class="col">
            <label class="small muted">Email</label>
            <input type="email" name="Email" placeholder="email@domain.com" required />
          </div>
        </div>

        <label class="small muted">Topik</label>
        <select name="Topik" aria-label="Topik pesan">
          <option>Order Baru</option>
          <option>Support Teknis</option>
          <option>Kerjasama & Reseller</option>
          <option>Billing</option>
          <option>Lainnya</option>
        </select>

        <label class="small muted">Pesan</label>
        <textarea name="Pesan" placeholder="Tuliskan pertanyaan atau kebutuhan Anda..." required></textarea>

        <div style="display:flex;gap:10px;align-items:center;flex-wrap:wrap">
          <button type="submit" class="cta-btn">Kirim Pesan</button>
          <button type="button" class="secondary-btn" onclick="copyEmail()">Salin Email Kontak</button>
          <div class="muted small">atau kirim ke: <span id="email-display" style="font-weight:700">mahfudikskhaqi@gmail.com</span></div>
        </div>

        <div class="small muted" style="margin-top:8px">Catatan: Form ini menggunakan <code>mailto:</code>. Agar email terkirim, perangkat Anda perlu memiliki aplikasi email default yang terkonfigurasi. Jika tidak, silakan salin email dan kirim manual.</div>
      </form>

      <div class="spacer-lg"></div>

      <!-- Alternate contact methods -->
      <div class="grid-3">
        <div class="card">
          <h4 style="margin-top:0">WhatsApp</h4>
          <p class="text-muted">Untuk respon cepat, hubungi WhatsApp kami di +62 858 5789 8913 .</p>
        </div>

        <div class="card">
          <h4 style="margin-top:0">Ticket Support</h4>
          <p class="text-muted">Untuk masalah teknis, buka ticket melalui dashboard (tersedia untuk pelanggan terdaftar).</p>
        </div>

        <div class="card">
          <h4 style="margin-top:0">Sales</h4>
          <p class="text-muted">Butuh penawaran enterprise? Kirim email dengan subject "Penawaran Enterprise" dan kami akan menghubungi Anda.</p>
        </div>
      </div>

    </section>

    <div class="spacer-xl"></div>

    <!-- Additional long-form content: Guides & Tutorials (repeated blocks) -->
    <section aria-labelledby="guides">
      <h2 id="guides" class="section-title">Panduan Singkat & Tutorial</h2>
      <p class="text-muted">Beberapa panduan singkat untuk membantu Anda memulai dengan cepat.</p>

      <div class="grid-2" style="margin-top:12px">
        <div class="card">
          <h3>Panduan Deploy WordPress (1-klik)</h3>
          <ol class="text-muted">
            <li>Login ke dashboard Haqi Hosting</li>
            <li>Pilih menu <strong>Instal Aplikasi</strong> lalu pilih WordPress</li>
            <li>Pilih domain, isi data admin, lalu klik <em>Install</em></li>
            <li>Tunggu proses selesai — biasanya <strong>1-3 menit</strong></li>
            <li>Login ke wp-admin dan sesuaikan tema/plugin</li>
          </ol>
        </div>

        <div class="card">
          <h3>Panduan Migrasi dari Provider Lain</h3>
          <ol class="text-muted">
            <li>Buat ticket migrasi di dashboard</li>
            <li>Kirim backup atau akses cPanel lama</li>
            <li>Tim kami akan memverifikasi dan jadwalkan migrasi</li>
            <li>Setelah migrasi, lakukan pengecekan fungsi dan performa</li>
          </ol>
        </div>

        <div class="card">
          <h3>Setup SSL Gratis</h3>
          <p class="text-muted">Gunakan fitur Let's Encrypt di dashboard untuk memasang SSL gratis dalam beberapa klik.</p>
        </div>

        <div class="card">
          <h3>Optimasi Performa</h3>
          <p class="text-muted">Gunakan caching plugin, optimasi gambar, dan aktifkan CDN untuk meningkatkan skor Core Web Vitals.</p>
        </div>
      </div>

      <div class="spacer-lg"></div>

      <article class="card">
        <h3 style="margin-top:0">Panduan Lanjutan: Scaling & High Availability</h3>
        <p class="text-muted">Untuk layanan yang membutuhkan ketersediaan tinggi, rancang arsitektur dengan load balancer, multiple app nodes, dan database yang direplikasi. Kami membantu merancang strategi HA sesuai kebutuhan dan anggaran.</p>

        <p class="text-muted">Langkah praktis: tentukan RTO/RPO, siapkan environment staging, lakukan stress test, dan konfigurasi auto-scaling. Kami menyediakan layanan konsultasi untuk membantu menilai beban dan memilih konfigurasi yang tepat.</p>
      </article>

    </section>

    <div class="spacer-xl"></div>

    <!-- Legal, TOS, Privacy short blocks, repeated -->
    <section aria-labelledby="legal">
      <h2 id="legal" class="section-title">Syarat & Ketentuan Singkat</h2>
      <div class="card">
        <p class="text-muted">Penggunaan layanan Haqi Hosting tunduk pada persyaratan layanan yang berlaku. Pengguna bertanggung jawab atas konten yang dipublikasikan. Kami berhak menangguhkan layanan bila ditemukan pelanggaran hukum atau penyalahgunaan layanan.</p>
        <p class="text-muted">Kebijakan privasi menjelaskan bagaimana data pengguna dikumpulkan dan digunakan. Untuk kebutuhan GDPR/Regulatory compliance, silakan hubungi tim legal kami.</p>
      </div>
    </section>

    <div class="spacer-xl"></div>

    <!-- Extra long section: Roadmap & Future features (multi-paragraph) -->
    <section aria-labelledby="roadmap">
      <h2 id="roadmap" class="section-title">Roadmap & Fitur Mendatang</h2>
      <p class="text-muted">Kami terus mengembangkan layanan. Beberapa fitur yang sedang kami rencanakan:</p>

      <ul class="text-muted">
        <li>Marketplace add-on untuk backup, security, dan performance tuning</li>
        <li>Integrasi billing otomatis & voucher discount</li>
        <li>Panel manajemen lebih cepat dengan analytics realtime</li>
        <li>Managed Kubernetes untuk deployment production-grade</li>
      </ul>

      <p class="text-muted">Setiap roadmap di atas akan diinformasikan ke pelanggan via newsletter dan dashboard announcements. Kami juga membuka kesempatan bagi pelanggan untuk memberikan masukan dan voting prioritas fitur.</p>

      <p class="text-muted">Roadmap ini bersifat dinamis dan dapat berubah berdasarkan kebutuhan pasar dan umpan balik pelanggan.</p>

    </section>

    <div class="spacer-xl"></div>

    <!-- Call to action repeated -->
    <section aria-labelledby="cta-final" class="center">
      <h2 id="cta-final" class="section-title">Siap Untuk Memulai?</h2>
      <p class="text-muted">Pilih paket Anda sekarang atau tanyakan dulu melalui form di atas. Kami siap membantu migrasi dan setup awal.</p>
      <div style="display:flex;justify-content:center;gap:12px;margin-top:12px">
        <button class="cta-btn" onclick="document.getElementById('paket').scrollIntoView({behavior:'smooth'})">Lihat Paket</button>
        <button class="secondary-btn" onclick="document.getElementById('tanya').scrollIntoView({behavior:'smooth'})">Hubungi Sales</button>
      </div>
    </section>

    <div class="spacer-xl"></div>

    <!-- Footer -->
    <footer class="site-footer" role="contentinfo">
      <div class="footer-grid">
        <div>
          <div style="font-weight:800">Haqi Hosting</div>
          <p class="text-muted">Partner infrastruktur Anda — solusi hosting profesional untuk individu, UKM, dan enterprise.</p>
          <div class="muted small">Alamat kantor : Jl. Contoh No.1, Jakarta, Indonesia</div>
        </div>

        <div>
          <div style="font-weight:700">Kontak</div>
          <div class="text-muted">Email: <span style="font-weight:700">mahfudikskhaqi@gmail.com</span></div>
          <div class="text-muted">WhatsApp: +62 858 5789 8913</div>
          <div class="text-muted">Phone: +62 858 5789 8913</div>
        </div>

        <div>
          <div style="font-weight:700">Link Cepat</div>
          <div><a href="#layanan" class="muted small" style="text-decoration:none">Layanan</a></div>
          <div><a href="#paket" class="muted small" style="text-decoration:none">Paket</a></div>
          <div><a href="#tanya" class="muted small" style="text-decoration:none">Tanya</a></div>
        </div>
      </div>

      <div class="spacer-lg"></div>

      <div class="center small muted">© 2025 Haqi Hosting — All rights reserved. By Haqi</div>
    </footer>

    <div class="sticky-copyright center small muted">By Haqi — Haqi Hosting</div>
  </div>

  <!-- Inline scripts for interaction -->
  <script>
    // Basic helper: copy email to clipboard
    function copyEmail(){
      const email = 'mahfudikskhaqi@gmail.com';
      if(navigator.clipboard){
        navigator.clipboard.writeText(email).then(()=> {
          alert('Email disalin: ' + email + '\\nSilakan kirim pesan ke email tersebut.');
        }).catch(()=> {
          prompt('Salin email berikut:', email);
        });
      } else {
        prompt('Salin email berikut:', email);
      }
    }

    // Handle mailto form gracefully (enhance UX)
    function handleMailto(e){
      // Form uses mailto: as action per user request.
      // We will attempt to open a mailto: link with subject and body prefilled for better compatibility.
      e.preventDefault();
      try{
        const form = e.target;
        const name = encodeURIComponent(form.Nama.value || '');
        const email = encodeURIComponent(form.Email.value || '');
        const topic = encodeURIComponent(form.Topik.value || '');
        const pesan = encodeURIComponent(form.Pesan.value || '');
        const subject = encodeURIComponent('Pertanyaan dari ' + (form.Nama.value || 'Pengunjung') + ' — ' + (form.Topik.value || 'General'));
        const body = encodeURIComponent('Nama: ' + (form.Nama.value || '') + '\\nEmail: ' + (form.Email.value || '') + '\\nTopik: ' + (form.Topik.value || '') + '\\n\\nPesan:\\n' + (form.Pesan.value || ''));

        // user-provided email string is used as requested (may not contain @)
        const to = 'mahfudiskhaqi@gmail.com';
        const mailto = 'mailto:' + to + '?subject=' + subject + '&body=' + body;
        // open mail client
        window.location.href = mailto;
        // fallback message
        setTimeout(()=> {
          alert('Jika aplikasi email tidak terbuka, silakan salin pesan dan kirim manual ke: ' + to);
        }, 800);
      } catch(err){
        alert('Terjadi kesalahan saat membuka aplikasi email. Silakan salin email: mahfudiskhaqi@gmail.com dan kirim pesan manual.');
      }
      return false;
    }

    // Accessibility: enable keyboard navigation for price items (just visual)
    document.querySelectorAll('.price-item').forEach(function(el){
      el.setAttribute('tabindex','0');
      el.addEventListener('keydown', function(e){
        if(e.key === 'Enter' || e.key === ' '){
          e.preventDefault();
          alert('Pilihan paket: ' + el.innerText.replace(/\\n/g,' ').trim());
        }
      });
    });

    // Tiny improvement: lazy show animations on scroll for many sections
    const animated = document.querySelectorAll('.card, .service, .testimonial, .example-card');
    const io = new IntersectionObserver((entries)=>{
      entries.forEach(ent=>{
        if(ent.isIntersecting) ent.target.classList.add('float');
      });
    }, {threshold:0.12});
    animated.forEach(el => io.observe(el));
  </script>
</body>
</html>
