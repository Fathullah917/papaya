<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Papaya Coffee - KKN Dames Damai</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            line-height: 1.6;
            color: #333;
            /* Mengubah latar belakang menjadi gradasi biru */
            background: linear-gradient(to right, #e0f2f7, #bbdefb); /* Gradasi biru muda */
        }

        .container {
            max-width: 960px;
            margin: auto;
            overflow: hidden;
            padding: 0 20px;
        }

        header {
            /* Nilai 0.8 membuat latar belakang jauh lebih gelap */
            background: linear-gradient(rgba(96, 94, 107, 0.8), rgba(28, 26, 34, 0.8)), url('bb.jpg') no-repeat center center/cover;
            color: #fff;
            text-align: center;
            padding: 120px 0;
            position: relative;
            overflow: hidden;
            animation: fadeIn 1.5s ease-in-out;
        }
        .header-border {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 100px;
            background-color: #f7f9fc; /* Sesuaikan dengan warna latar belakang section berikutnya */
            border-top-left-radius: 50% 100%;
            border-top-right-radius: 50% 100%;
        }

        header h1 {
            font-size: 3rem;
            margin: 0;
        }

        .slogan {
            font-size: 1.2rem;
            font-weight: 400;
        }

        /* Bagian-bagian Konten */
        section {
            padding: 60px 0;
        }

        .section-tentang-kami, .section-manfaat, .section-kontak {
            background: #fff; /* Tetap putih untuk konten utama */
            border-radius: 10px;
            margin-bottom: 30px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }

        .section-produk, .section-testimoni {
            background: #e3f2fd; /* Biru muda untuk bagian ini */
            border-radius: 10px;
            margin-bottom: 30px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
        }

        h2 {
            text-align: center;
            color: #2196F3; /* Warna biru untuk judul */
            margin-bottom: 40px;
            font-size: 2.2rem;
        }

        .about-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 30px;
            text-align: center;
        }

        .about-image {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .product-item {
            text-align: center;
            background: #fff;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .product-image {
            max-width: 80%;
            height: auto;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .product-price {
            font-size: 1.5rem;
            font-weight: 600;
            color: #4CAF50;
            margin: 10px 0;
        }

        .button {
            display: inline-block;
            background: #2196F3; /* Warna biru untuk tombol */
            color: #fff;
            padding: 12px 25px;
            text-decoration: none;
            border-radius: 5px;
            font-weight: 600;
            transition: background-color 0.3s;
        }

        .button:hover {
            background-color: #1976D2; /* Biru lebih gelap saat hover */
        }

        .manfaat-grid, .testimoni-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
        }

        .manfaat-item, .testimoni-item {
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .manfaat-item ul {
            list-style-type: none;
            padding: 0;
            text-align: left;
        }

        .manfaat-item li::before {
            content: '✅ ';
            color: #4CAF50;
            margin-right: 8px;
        }

        .disclaimer {
            margin-top: 20px;
            font-style: italic;
            font-size: 0.9em;
            text-align: center;
            color: #666;
        }

        .section-kontak {
            text-align: center;
        }

        .social-icons a {
            font-size: 3em; /* Ukuran ikon lebih besar */
            margin: 0 15px;
            color: #2196F3; /* Warna ikon biru */
            transition: color 0.3s;
        }

        .social-icons a:hover {
            color: #1976D2; /* Warna ikon saat hover */
        }
        
        .social-icons p {
            margin-top: 20px;
            font-weight: 600;
        }


        footer {
            background: #2196F3; /* Biru untuk footer */
            color: #fff;
            text-align: center;
            padding: 20px 0;
        }

        /* Responsif untuk layar lebih besar */
        @media (min-width: 768px) {
            .about-content {
                flex-direction: row;
                text-align: left;
            }
            .about-image {
                max-width: 40%; /* Sedikit lebih kecil agar teks lebih dominan */
            }
            .manfaat-grid {
                grid-template-columns: 1fr 1fr;
            }
            .testimoni-grid {
                grid-template-columns: repeat(3, 1fr);
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="container">
            <h1>PAPAYA COFFEE</h1>
            <p class="slogan">Inovasi Mahasiswa, Kenikmatan Tiada Duanya.</p>
        </div>
    </header>

    <main>
        <section id="tentang-kami" class="section-tentang-kami">
            <div class="container">
                <h2>Tentang Kami</h2>
                <div class="about-content">
                    <img src="gambar-proses-kopi.jpg" alt="Proses pembuatan kopi biji pepaya" class="about-image">
                    <div>
                        <p>Papaya Coffee adalah inovasi produk dari mahasiswa KKN Dames Damai. Berawal dari keinginan untuk memanfaatkan limbah biji pepaya yang sering terbuang, kami melihat potensi besar untuk mengubahnya menjadi minuman alternatif yang tidak hanya unik, tetapi juga menyehatkan.</p>
                        <p>Kopi biji pepaya kami dibuat melalui proses seleksi biji yang ketat, pengeringan alami, sangrai dengan suhu terkontrol untuk menghasilkan aroma dan rasa terbaik, hingga penggilingan halus. Kami berkomitmen untuk menyajikan produk berkualitas tinggi dengan cita rasa otentik yang aman untuk dinikmati siapa saja.</p>
                    </div>
                </div>
            </div>
        </section>
        
        <section id="produk" class="section-produk">
            <div class="container">
                <h2>Produk Kami</h2>
                <div class="product-item">
                    <img src="gambar-produk-kopi.jpg" alt="Kemasan Kopi Biji Pepaya" class="product-image">
                    <h3>Papaya Coffee Original</h3>
                    <p class="product-description">Nikmati sensasi rasa unik dari Papaya Coffee Original. Aroma khas yang lembut berpadu dengan sentuhan rasa nutty, memberikan pengalaman minum kopi yang berbeda. Bebas kafein, aman untuk lambung, dan kaya manfaat kesehatan.</p>
                    <p class="product-price">Rp 15.000</p>
                    <p class="product-weight">Berat Bersih: 100gr</p>
                    <p class="product-serving">Cara Penyajian: Seduh 1-2 sendok teh bubuk kopi dengan 200ml air panas. Tambahkan gula atau krimer sesuai selera.</p>
                    <a href="https://wa.me/087859548565" target="_blank" class="button">Beli Sekarang</a>
                </div>
            </div>
        </section>
        
        <section id="manfaat" class="section-manfaat">
            <div class="container">
                <h2>Manfaat & Perhatian</h2>
                <div class="manfaat-grid">
                    <div class="manfaat-item">
                        <h3>Manfaat Papaya Coffee</h3>
                        <ul>
                            <li>Kaya Antioksidan untuk melindungi sel tubuh</li>
                            <li>Bebas Kafein, cocok untuk penderita asam lambung</li>
                            <li>Membantu Detoksifikasi & Kesehatan Pencernaan</li>
                            <li>Berpotensi Membantu Menurunkan Kolesterol</li>
                        </ul>
                    </div>
                    <div class="manfaat-item">
                        <h3>Perhatian (Tidak Dianjurkan Untuk)</h3>
                        <ul>
                            <li>Ibu Hamil dan Menyusui (konsultasi dokter)</li>
                            <li>Orang dengan Gangguan Pencernaan Akut</li>
                            <li>Pria yang Sedang dalam Program Hamil (konsultasi dokter)</li>
                        </ul>
                    </div>
                </div>
                <p class="disclaimer">*Konsultasikan dengan ahli kesehatan atau dokter jika Anda memiliki kondisi medis tertentu sebelum mengonsumsi produk ini.</p>
            </div>
        </section>

        <section id="testimoni" class="section-testimoni">
            <div class="container">
                <h2>Apa Kata Mereka?</h2>
                <div class="testimoni-grid">
                    <div class="testimoni-item">
                        <p>"Rasanya enak, seperti kopi beneran tapi lebih ringan di perut. Cocok untuk saya yang sensitif kafein!"</p>
                        <p><strong>- Sekdes Dames Damai</strong></p>
                    </div>
                    <div class="testimoni-item">
                        <p>"Produk unik dan menyehatkan. Aroma dan rasanya luar biasa. Pasti akan beli lagi!"</p>
                        <p><strong>- Ibu Nurlaila (Warga Lokal)</strong></p>
                    </div>
                    <div class="testimoni-item">
                        <p>"Sangat mudah diseduh dan tidak bikin kembung. Produk lokal inovatif yang patut diacungi jempol!"</p>
                        <p><strong>- Bapak Budi (Pemerhati UMKM)</strong></p>
                    </div>
                </div>
            </div>
        </section>

        <section id="kontak" class="section-kontak">
            <div class="container">
                <h2>Hubungi Kami</h2>
                <p>Terima kasih telah tertarik dengan Papaya Coffee. Kami siap melayani Anda!</p>
                <div class="social-icons">
                    <a href="https://wa.me/087859548565" target="_blank" aria-label="WhatsApp"><i class="fab fa-whatsapp"></i></a>
                    <a href="https://instagram.com/_ahmdfthllh_" target="_blank" aria-label="Instagram"><i class="fab fa-instagram"></i></a>
                </div>
                <p>Atau hubungi kami di Kantor Desa Dames Damai</p>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2024 Papaya Coffee KKN Dames Damai. Hak Cipta Dilindungi.</p>
        </div>
    </footer>

</body>
</html>
