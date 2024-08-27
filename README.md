<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>9-G CLASS</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <style>
        /* Reset default styles */
        body, h1, h2, h3, p {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
        }
        body {
            background: #f0f4f8;
            color: #333;
            padding: 0;
            margin: 0;
        }
        header {
            background: linear-gradient(135deg, #004d99, #003366);
            color: #fff;
            padding: 20px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            position: fixed;
            width: 100%;
            top: 0;
            left: 0;
            z-index: 1000;
        }
        header h1 {
            margin: 0;
        }
        nav {
            margin-top: 10px;
        }
        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 15px;
            font-size: 1.1rem;
            padding: 10px 15px;
            display: inline-block;
            border-radius: 5px;
            transition: background-color 0.3s ease, color 0.3s ease;
        }
        nav a:hover {
            background-color: rgba(255, 255, 255, 0.2);
            color: #ffddc1;
        }
        .hero {
            background: rgba(0, 0, 0, 0.5)
            color: #fff;
            text-align: center;
            padding: 100px 20px;
            background-blur: 10px;
            margin-top: 60px; /* Adjusted for fixed header */
        }
        .hero h2 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            animation: fadeIn 2s ease-in;
        }
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 20px;
        }
        .button-primary {
            background: #007bff;
            color: #fff;
            padding: 15px 25px;
            border-radius: 5px;
            text-decoration: none;
            font-size: 1.1rem;
            display: inline-block;
            transition: background 0.3s ease, transform 0.3s ease, box-shadow 0.3s ease;
        }
        .button-primary:hover {
            background: #0056b3;
            transform: scale(1.05);
            box-shadow: 0 6px 12px rgba(0,0,0,0.3);
        }
        .container {
            padding: 20px;
            margin-top: 20px; /* Add space to avoid overlap with fixed header */
        }
        section {
            margin-bottom: 40px;
        }
        h2 {
            border-bottom: 2px solid #007bff;
            padding-bottom: 10px;
            margin-bottom: 20px;
            position: relative;
        }
        h2::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            height: 5px;
            width: 50px;
            background: #007bff;
        }
        .carousel-container {
            position: relative;
            overflow: hidden;
            width: 100%;
            max-width: 800px;
            margin: 0 auto;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        }
        .carousel-images {
            display: flex;
            transition: transform 0.5s ease;
        }
        .carousel-images img {
            width: 100%;
            height: auto;
            flex-shrink: 0;
        }
        .carousel-controls {
            position: absolute;
            top: 50%;
            width: 100%;
            display: flex;
            justify-content: space-between;
            transform: translateY(-50%);
        }
        .carousel-controls button {
            background: rgba(0, 0, 0, 0.5);
            border: none;
            color: #fff;
            padding: 10px;
            border-radius: 50%;
            cursor: pointer;
            font-size: 1.5rem;
            transition: background 0.3s ease;
        }
        .carousel-controls button:hover {
            background: rgba(0, 0, 0, 0.7);
        }
        .gallery-item {
            margin-bottom: 20px;
            border-radius: 10px;
            overflow: hidden;
            background: #fff;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        }
        .gallery-item img {
            width: 100%;
            height: auto;
            transition: transform 0.3s ease;
        }
        .gallery-item img:hover {
            transform: scale(1.05);
        }
        .teacher, .student {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
            background: #fff;
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        }
        .teacher img, .student img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            margin-right: 15px;
            border: 2px solid #007bff;
        }
        .teacher-info, .student-info {
            max-width: 500px;
        }
        .student-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            justify-content: center;
        }
        .student-card {
            background: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            padding: 10px;
            text-align: center;
            width: calc(25% - 25px);
            transition: transform 0.3s ease;
        }
        .student-card img {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            margin-bottom: 5px;
            border: 2px solid #007bff;
        }
        .student-card:hover {
            transform: scale(1.05);
        }
        footer {
            background: #003366;
            color: #fff;
            text-align: center;
            padding: 15px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .icon-green{
            font-size: 24px;
            color: greenyellow;
        }
        .icon-red{
            font-size: 24px;
            color: red;
        }
    </style>
</head>
<body>
    <header>
        <h1>9-G CLASS</h1>
        <nav>
            <a href="#home">Beranda</a>
            <a href="https://9-g2023.github.io/Gallery-9G/" target="_blank">Full Gallery</a>
            <a href="#gallery">Gallery</a>
            <a href="#teachers">Wali Kelas</a>
            <a href="#students">Siswa-Siswi</a>
            <a href="https://www.instagram.com/sembilanntuujuh?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==" target="_blank"><i class="bi bi-instagram icon-red"></i></a>
            <a href="https://www.tiktok.com/@sembilanntuujuh_?is_from_webapp=1&sender_device=pc" target="_blank"><i class="bi bi-tiktok icon-black"></i></a>
        </nav>
    </header>
    <div class="hero" id="home">
        <h2>WELCOME TO 9-G CLASS</h2>
        <p>9-G CLASS Tahun Ajaran 2023-2024</p>
        <a href="#about" class="button-primary">Pelajari Lebih Lanjut</a>
    </div> 
    <div class="container">
        <section id="about">
            <h2>9G CLASS</h2>
            <img src="image/newwww.webp" alt="Tentang Kelas 9-G">
        </section>
        <section id="gallery">
            <h2>Galeri Kelas</h2>
            <div class="carousel-container">
                <div class="carousel-images">
                    <img src="image/448207003_7643637229052243_5760121963997977542_n.webp" alt="Galeri 1">
                    <img src="image/aja.webp" alt="Galeri 2">
                    <img src="image/366146358_255700773987015_2705461868856523935_n.webp" alt="Galeri 3">
                    <img src="image/IMG-20240825-WA0018.jpg" alt="Galeri 4">
                    <img src="image/IMG-20240825-WA0019.jpg" alt="Galeri 5">
                    <img src="image/IMG-20240825-WA0020.jpg" alt="Galeri 6">
                    <img src="image/IMG-20240825-WA0021.jpg" alt="Galeri 7">
                    <img src="image/IMG-20240825-WA0022.jpg" alt="Galeri 8">
                </div>
                <div class="carousel-controls">
                    <button class="prev">&#10094;</button>
                    <button class="next">&#10095;</button>
                </div>
            </div>
        </section>
        <section id="teachers">
            <h2>Wali Kelas</h2>
            <div class="teacher">
                <img src="image/DSC_0594.JPG" alt="Foto Guru">
                <div class="teacher-info">
                    <h3>Hj.Yeti Irawatie, S.Pd</h3>
                    <p>Wali Kelas</p>
                    <p>Di setiap perjalanan pendidikan, ada sosok yang mengubah hidup dan meninggalkan jejak yang mendalam—itulah Bu Yeti. Dengan kebijaksanaan dan dedikasi yang luar biasa, beliau tidak hanya mengajarkan mata pelajaran, tetapi juga membentuk karakter dan inspirasi bagi setiap siswa yang dia ajar. Bu Yeti adalah pelita yang menerangi jalan menuju pengetahuan dan perkembangan pribadi, mengajarkan lebih dari sekadar kurikulum.</p>
                </div>
            </div>
        </section>
        <section id="students">
            <h2>Identitas Siswa</h2>
            <div class="student-list">
                <div class="student-card">
                    <img src="image/ANGGI REFLI (1).JPG" alt="Siswa 1">
                    <p>Anggi Refli A</p>
                </div>
                <div class="student-card">
                    <img src="image/ARI HADI (1).JPG" alt="Siswa 2">
                    <p>Ari Hadi W</p>
                </div>
                <div class="student-card">
                    <img src="image/ARISSA FARRAS (1).JPG" alt="Siswa 1">
                    <p>Arissa Farras E</p>
                </div>
                <div class="student-card">
                    <img src="image/ARSISYA (1).JPG" alt="Siswa 1">
                    <p>Arsisya Fardila P</p>
                </div>
                <div class="student-card">
                    <img src="image/ASMIRA PUANDINI (1).JPG" alt="Siswa 1">
                    <p>Asmira Puandini</p>
                </div>
                <div class="student-card">
                    <img src="image/AUDYA RACHMA (1).JPG" alt="Siswa 1">
                    <p>Audya Rachma R</p>
                </div>
                <div class="student-card">
                    <img src="image/AURA ANNASTASYA (1).JPG" alt="Siswa 1">
                    <p>Aura Annastasya K</p>
                </div>
                <div class="student-card">
                    <img src="image/BIAN QANITAH (1).JPG" alt="Siswa 1">
                    <p>Bian Qonitah</p>
                </div>
                <div class="student-card">
                    <img src="image/BILQIS (1).JPG" alt="Siswa 1">
                    <p>Bilqis Azizatushalihah</p>
                </div>
                <div class="student-card">
                    <img src="image/DAVA BINTANG (1).JPG" alt="Siswa 1">
                    <p>Dava Bintang A</p>
                </div>
                <div class="student-card">
                    <img src="image/DESTIYA SARAH (1).JPG" alt="Siswa 1">
                    <p>Destiya Sarah</p>
                </div>
                <div class="student-card">
                    <img src="image/ELLA NUR (1).JPG" alt="Siswa 1">
                    <p>Ella Nurhandayani</p>
                </div>
                <div class="student-card">
                    <img src="image/ELSA ARYANI (1).JPG" alt="Siswa 1">
                    <p>Elsa Aryani</p>
                </div>
                <div class="student-card">
                    <img src="image/FARID BAHAR (1).JPG" alt="Siswa 1">
                    <a href="https://9-g2023.github.io/Profil-Farid-Bahar-M/" target="_blank"><p>Farid Bahar M</p></a>
                </div>
                <div class="student-card">
                    <img src="image/GRECIA VALENTINE (1).JPG" alt="Siswa 1">
                    <p>Grecia Valentine</p>
                </div>
                <div class="student-card">
                    <img src="image/HAFSHOH RAIHANAH (1).JPG" alt="Siswa 1">
                    <p>Hafshoh Raihanah K</p>
                </div>
                <div class="student-card">
                    <img src="image/KENT ATHURA (1).JPG" alt="Siswa 1">
                    <p>Kent Athuura S</p>
                </div>
                <div class="student-card">
                    <img src="image/KIRANA SAFITRI (1).JPG" alt="Siswa 1">
                    <p>Kirana Safitri</p>
                </div>
                <div class="student-card">
                    <img src="image/LAILA PUTRI (1).JPG" alt="Siswa 1">
                    <p>Laila Putri N</p>
                </div>
                <div class="student-card">
                    <img src="image/LINGGO ADITYA (1).JPG" alt="Siswa 1">
                    <p>Linggo Aditya</p>
                </div>
                <div class="student-card">
                    <img src="image/M ALFIAN DWI (1).JPG" alt="Siswa 1">
                    <p>Muhamad Alfian Dwi J</p>
                </div>
                <div class="student-card">
                    <img src="image/MUHAMMAD NAZRIL (1).JPG" alt="Siswa 1">
                    <p>Muhammad Nazril F</p>
                </div>
                <div class="student-card">
                    <img src="image/MUHAMMAD QILMAN (1).JPG" alt="Siswa 1">
                    <p>Muhamad Qilman H</p>
                </div>
                <div class="student-card">
                    <img src="image/NADIA AMANDAR (1).JPG" alt="Siswa 1">
                    <p>Nadia Amandar</p>
                </div>
                <div class="student-card">
                    <img src="image/NURUL WAHIDAH (1).JPG" alt="Siswa 1">
                    <p>Nurul Wahidah</p>
                </div>
                <div class="student-card">
                    <img src="image/PARISKA ZAHRA (1).JPG" alt="Siswa 1">
                    <p>Pariska Zahra</p>
                </div>
                <div class="student-card">
                    <img src="image/RAFA KURNIA (1).JPG" alt="Siswa 1">
                    <p>Rafa Kurnia F</p>
                </div>
                <div class="student-card">
                    <img src="image/RAFA OKTAVIAN (1).JPG" alt="Siswa 1">
                    <p>Rafa Oktavian F</p>
                </div>
                <div class="student-card">
                    <img src="image/RAMMY (1).JPG" alt="Siswa 1">
                    <p>Rammy Munira El-Esami R</p>
                </div>
                <div class="student-card">
                    <img src="image/riyadhi.jpg" alt="Siswa 1">
                    <p>Riyadhi Akbar</p>
                </div>
                <div class="student-card">
                    <img src="image/RIVAL (1).JPG" alt="Siswa 1">
                    <p>Rival Agatha R</p>
                </div>
                <div class="student-card">
                    <img src="image/SARAH NUR AZIZAH (1).JPG" alt="Siswa 1">
                    <p>Sarah Nur Azizah</p>
                </div>
                <div class="student-card">
                    <img src="image/SAZKIA NOUREEN (1).JPG" alt="Siswa 1">
                    <p>Sazkia Noureen A</p>
                </div>
                <div class="student-card">
                    <img src="image/SUCI RAMADHANI (1).JPG" alt="Siswa 1">
                    <p>Suci Ramadhani</p>
                </div>
                <div class="student-card">
                    <img src="image/SYALOM (1).JPG" alt="Siswa 1">
                    <p>Syallom Yadrastirani A D</p>
                </div>
                <div class="student-card">
                    <img src="image/ZHROTUL AINI (1).JPG" alt="Siswa 1">
                    <p>Zahrotul Aini</p>
                </div>
            </div>
        </section>
    </div>
    <footer>
        &copy; 2024 Website Kelas 9-G. All rights reserved.
    </footer>
    <script>
        const prevButton = document.querySelector('.prev');
        const nextButton = document.querySelector('.next');
        const carouselImages = document.querySelector('.carousel-images');
        let currentIndex = 0;

        function showImage(index) {
            const totalImages = carouselImages.children.length;
            if (index >= totalImages) {
                currentIndex = 0;
            } else if (index < 0) {
                currentIndex = totalImages - 1;
            } else {
                currentIndex = index;
            }
            carouselImages.style.transform = `translateX(-${currentIndex * 100}%)`;
        }

        prevButton.addEventListener('click', () => {
            showImage(currentIndex - 1);
        });

        nextButton.addEventListener('click', () => {
            showImage(currentIndex + 1);
        });

        // Optional: auto-slide every 8 seconds
        setInterval(() => {
            showImage(currentIndex + 1);
        }, 3000);
    </script>
</body>
</html>
