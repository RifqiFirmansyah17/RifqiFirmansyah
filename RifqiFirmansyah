<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rifqi Firmansyah - Profil Profesional</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts - Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        /* Base styles for body and font */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc; /* Tailwind: bg-slate-50 */
            color: #334155; /* Tailwind: text-slate-700 */
            scroll-behavior: smooth; /* Smooth scrolling for anchor links */
        }
        /* Custom shadow for cards and sections for depth */
        .card-shadow {
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1), 0 1px 3px rgba(0, 0, 0, 0.08);
        }
        /* Gradient background for primary buttons */
        .btn-gradient {
            background-image: linear-gradient(to right top, #6366f1, #8b5cf6, #a78bfa); /* Tailwind: from-indigo-500 to-purple-600 */
        }
        /* Darker gradient on hover for buttons */
        .btn-gradient:hover {
            background-image: linear-gradient(to right top, #4f46e5, #7c3aed, #9333ea);
        }

        /* --- Dramatic Background Animation (Subtle Gradient Movement) --- */
        .animated-gradient-bg {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, #6366f1, #8b5cf6, #a78bfa, #c4b5fd);
            background-size: 400% 400%; /* Make gradient larger than container */
            animation: gradientShift 15s ease infinite alternate; /* Smooth, looping animation */
            z-index: -1; /* Ensure it stays behind content */
            opacity: 0.8; /* Subtle transparency */
        }

        @keyframes gradientShift {
            0% { background-position: 0% 0%; }
            50% { background-position: 100% 100%; }
            100% { background-position: 0% 0%; }
        }

        /* --- Hero Section Text Animation --- */
        @keyframes fadeInScaleUp {
            from {
                opacity: 0;
                transform: scale(0.95);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
        .animate-fade-in-scale-up {
            animation: fadeInScaleUp 1s ease-out forwards;
            opacity: 0; /* Hidden before animation */
        }

        /* --- Section Header Animation --- */
        @keyframes slideInFromLeft {
            from {
                opacity: 0;
                transform: translateX(-50px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        /* This class will be added by Intersection Observer for scroll-triggered animation */
        .animate-on-scroll {
            opacity: 0;
        }
        .animate-on-scroll.is-visible {
            animation: slideInFromLeft 0.8s ease-out forwards;
        }

        /* --- Card Hover Effect --- */
        .hover-lift {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .hover-lift:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 25px -5px rgba(0, 0, 0, 0.15), 0 5px 10px -5px rgba(0, 0, 0, 0.08);
        }

        /* Parallax effect for hero background image */
        .parallax-hero {
            background-image: url('IMG_2517.jpg'); /* Your photo */
            background-size: cover;
            background-position: center;
            background-attachment: fixed; /* This creates the parallax effect */
            position: relative;
            z-index: 0;
        }
        /* Overlay for hero image to make text readable */
        .parallax-hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5); /* Dark overlay */
            z-index: 1;
        }
        .hero-content {
            position: relative;
            z-index: 2; /* Ensure content is above overlay */
        }
    </style>
</head>
<body>
    <!-- Header Section: Fixed at the top, includes site title and navigation -->
    <header class="bg-white shadow-sm py-4 px-6 md:px-8 lg:px-12 fixed w-full z-10 card-shadow">
        <nav class="container mx-auto flex justify-between items-center">
            <div class="flex items-center">
                <span class="text-2xl font-extrabold text-gray-900">Rifqi Firmansyah</span>
            </div>
            <!-- Desktop Navigation Links -->
            <ul class="hidden md:flex space-x-8">
                <li><a href="#hero" class="text-gray-700 hover:text-indigo-600 font-medium transition duration-300">Beranda</a></li>
                <li><a href="#about" class="text-gray-700 hover:text-indigo-600 font-medium transition duration-300">Tentang Saya</a></li>
                <li><a href="#skills" class="text-gray-700 hover:text-indigo-600 font-medium transition duration-300">Keahlian</a></li>
                <li><a href="#portfolio" class="text-gray-700 hover:text-indigo-600 font-medium transition duration-300">Portofolio</a></li>
                <li><a href="#contact" class="text-gray-700 hover:text-indigo-600 font-medium transition duration-300">Kontak</a></li>
            </ul>
            <!-- Mobile Menu Button: Shown only on small screens -->
            <button id="mobile-menu-button" class="md:hidden p-2 rounded-md text-gray-700 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-indigo-500">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                </svg>
            </button>
        </nav>
    </header>

    <!-- Mobile Menu Overlay: Hidden by default, appears when mobile menu button is clicked -->
    <div id="mobile-menu" class="hidden md:hidden fixed inset-0 bg-white bg-opacity-95 z-20 flex flex-col items-center justify-center space-y-8 text-2xl font-bold">
        <button id="close-mobile-menu" class="absolute top-6 right-6 p-2 rounded-md text-gray-700 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-indigo-500">
            <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
            </svg>
        </button>
        <a href="#hero" class="text-gray-800 hover:text-indigo-600 transition duration-300" onclick="document.getElementById('mobile-menu').classList.add('hidden');">Beranda</a>
        <a href="#about" class="text-gray-800 hover:text-indigo-600 transition duration-300" onclick="document.getElementById('mobile-menu').classList.add('hidden');">Tentang Saya</a>
        <a href="#skills" class="text-gray-800 hover:text-indigo-600 transition duration-300" onclick="document.getElementById('mobile-menu').classList.add('hidden');">Keahlian</a>
        <a href="#portfolio" class="text-gray-800 hover:text-indigo-600 transition duration-300" onclick="document.getElementById('mobile-menu').classList.add('hidden');">Portofolio</a>
        <a href="#contact" class="text-gray-800 hover:text-indigo-600 transition duration-300" onclick="document.getElementById('mobile-menu').classList.add('hidden');">Kontak</a>
    </div>

    <!-- Hero Section: Main introduction with your photo and dramatic background -->
    <section id="hero" class="parallax-hero relative text-white py-24 md:py-32 lg:py-40 flex items-center justify-center overflow-hidden pt-20 min-h-screen">
        <!-- Animated Gradient Background (behind parallax image) -->
        <div class="animated-gradient-bg"></div>

        <div class="container mx-auto text-center hero-content px-4">
            <!-- Your Profile Photo -->
            <img src="IMG_2517.jpg" alt="Foto Profil Rifqi Firmansyah" class="w-32 h-32 md:w-40 md:h-40 rounded-full object-cover mx-auto mb-6 border-4 border-white shadow-lg animate-fade-in-scale-up"
                 onerror="this.onerror=null;this.src='https://placehold.co/160x160/F0F0F0/000000?text=Rifqi'; console.error('Gagal memuat IMG_2517.jpg. Pastikan jalur sudah benar dan gambar di-hosting secara publik.');">
            <h1 class="text-4xl md:text-5xl lg:text-6xl font-extrabold leading-tight mb-4 animate-fade-in-scale-up">
                Rifqi Firmansyah
            </h1>
            <p class="text-lg md:text-xl lg:text-2xl font-light mb-10 max-w-3xl mx-auto animate-fade-in-scale-up" style="animation-delay: 0.2s;">
                Mewujudkan Ide Kreatif melalui Desain dan Teknologi.
            </p>
            <a href="#contact" class="inline-block btn-gradient text-white font-bold py-3 px-8 rounded-full shadow-lg hover:shadow-xl transition duration-300 ease-in-out transform hover:scale-105 animate-fade-in-scale-up" style="animation-delay: 0.4s;">
                Hubungi Saya
            </a>
        </div>
    </section>

    <!-- About Me Section -->
    <section id="about" class="py-16 md:py-24 bg-white">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl md:text-4xl font-extrabold text-gray-800 mb-12 animate-on-scroll">Tentang Saya</h2>
            <div class="max-w-4xl mx-auto text-lg text-gray-700 leading-relaxed">
                <p class="mb-4">
                    Halo! Saya Rifqi Firmansyah, seorang individu yang bersemangat dalam dunia desain dan teknologi.
                    Dengan latar belakang pendidikan di bidang IT dan minat yang mendalam pada estetika visual,
                    saya selalu mencari cara untuk menggabungkan fungsionalitas dengan keindahan dalam setiap proyek.
                </p>
                <p class="mb-4">
                    Saya percaya bahwa desain yang baik tidak hanya terlihat menarik, tetapi juga mampu memecahkan masalah
                    dan menciptakan pengalaman yang bermakna bagi pengguna. Saya terus belajar dan beradaptasi dengan
                    tren terbaru untuk memastikan setiap karya yang saya hasilkan relevan dan inovatif.
                </p>
                <p>
                    Di luar pekerjaan, saya menikmati eksplorasi ide-ide baru dan tantangan kreatif yang mendorong batas-batas
                    kemampuan saya. Mari berkolaborasi untuk mewujudkan visi Anda!
                </p>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-16 md:py-24 bg-slate-50">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl md:text-4xl font-extrabold text-gray-800 mb-12 animate-on-scroll">Keahlian Saya</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 max-w-5xl mx-auto">
                <!-- Skill Card 1: Graphic Design -->
                <div class="bg-white p-8 rounded-xl card-shadow transition duration-300 hover-lift">
                    <div class="mb-4 text-indigo-500">
                        <svg class="w-16 h-16 mx-auto" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z"></path>
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-800 mb-3">Desain Grafis</h3>
                    <p class="text-gray-600">
                        Menciptakan visual yang menarik dan efektif untuk berbagai media, dari branding hingga materi promosi.
                    </p>
                </div>

                <!-- Skill Card 2: Web Development (Frontend) -->
                <div class="bg-white p-8 rounded-xl card-shadow transition duration-300 hover-lift">
                    <div class="mb-4 text-purple-500">
                        <svg class="w-16 h-16 mx-auto" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"></path>
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-800 mb-3">Pengembangan Web (Frontend)</h3>
                    <p class="text-gray-600">
                        Membangun antarmuka pengguna yang responsif dan interaktif menggunakan HTML, CSS, dan JavaScript.
                    </p>
                </div>

                <!-- Skill Card 3: UI/UX Design Principles -->
                <div class="bg-white p-8 rounded-xl card-shadow transition duration-300 hover-lift">
                    <div class="mb-4 text-teal-500">
                        <svg class="w-16 h-16 mx-auto" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9.75 7.5a2.25 2.25 0 00-2.25-2.25h-1.5A2.25 2.25 0 003.75 7.5v9.75m16.5-7.5l-1.5-1.5m-3.75 3.75l-1.5 1.5M12 9l-1.5-1.5m-3.75 3.75l-1.5 1.5M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-800 mb-3">Prinsip UI/UX</h3>
                    <p class="text-gray-600">
                        Menerapkan prinsip desain pengalaman pengguna untuk menciptakan produk yang intuitif dan menyenangkan.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio/Projects Section (Dummy Content) -->
    <section id="portfolio" class="py-16 md:py-24 bg-white">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-3xl md:text-4xl font-extrabold text-gray-800 mb-12 animate-on-scroll">Portofolio & Proyek</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 max-w-6xl mx-auto">
                <!-- Project Item 1 -->
                <div class="bg-gray-50 rounded-xl overflow-hidden card-shadow group hover-lift">
                    <img src="https://placehold.co/600x400/9ca3af/ffffff?text=Proyek+Desain+Brand" alt="Proyek Desain Brand" class="w-full h-48 object-cover transition duration-300 group-hover:scale-110">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Desain Identitas Brand</h3>
                        <p class="text-gray-600 text-sm">Pengembangan logo dan panduan visual untuk startup teknologi.</p>
                        <a href="#" class="text-indigo-600 hover:underline text-sm mt-3 inline-block">Lihat Detail</a>
                    </div>
                </div>
                <!-- Project Item 2 -->
                <div class="bg-gray-50 rounded-xl overflow-hidden card-shadow group hover-lift">
                    <img src="https://placehold.co/600x400/9ca3af/ffffff?text=Landing+Page+Web" alt="Landing Page Web" class="w-full h-48 object-cover transition duration-300 group-hover:scale-110">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">Desain Landing Page</h3>
                        <p class="text-gray-600 text-sm">Perancangan dan implementasi landing page konversi tinggi.</p>
                        <a href="#" class="text-indigo-600 hover:underline text-sm mt-3 inline-block">Lihat Detail</a>
                    </div>
                </div>
                <!-- Project Item 3 -->
                <div class="bg-gray-50 rounded-xl overflow-hidden card-shadow group hover-lift">
                    <img src="https://placehold.co/600x400/9ca3af/ffffff?text=Aplikasi+Mobile+UI" alt="Aplikasi Mobile UI" class="w-full h-48 object-cover transition duration-300 group-hover:scale-110">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-gray-800 mb-2">UI Aplikasi Mobile</h3>
                        <p class="text-gray-600 text-sm">Desain antarmuka pengguna untuk aplikasi manajemen tugas.</p>
                        <a href="#" class="text-indigo-600 hover:underline text-sm mt-3 inline-block">Lihat Detail</a>
                    </div>
                </div>
            </div>
            <div class="mt-12">
                <a href="https://www.instagram.com/rifqii.firmansyah/" target="_blank" rel="noopener noreferrer" class="inline-block btn-gradient text-white font-bold py-3 px-8 rounded-full shadow-lg hover:shadow-xl transition duration-300 ease-in-out transform hover:scale-105">
                    Lihat Lebih Banyak di Instagram
                </a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 md:py-24 bg-slate-50">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl md:text-4xl font-extrabold text-gray-800 text-center mb-12 animate-on-scroll">Hubungi Saya</h2>
            <div class="flex flex-col lg:flex-row gap-12 items-center lg:items-start max-w-5xl mx-auto">
                <!-- Contact Information -->
                <div class="w-full lg:w-1/2 bg-white p-8 rounded-xl card-shadow flex flex-col justify-center items-center lg:items-start text-center lg:text-left hover-lift">
                    <h3 class="text-2xl font-bold text-gray-800 mb-4">Informasi Kontak</h3>
                    <p class="text-gray-600 mb-6">
                        Tertarik untuk berkolaborasi atau hanya ingin menyapa? Jangan ragu untuk menghubungi saya!
                    </p>
                    <ul class="space-y-4 text-gray-700">
                        <!-- WhatsApp Contact -->
                        <li class="flex items-center justify-center lg:justify-start">
                            <svg class="w-6 h-6 mr-3 text-indigo-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.158l-2.23 1.094a2 2 0 00-.773 2.016l.163.535a4.708 4.708 0 002.392 2.392l.535.163a2 2 0 002.016-.773l1.094-2.23a1 1 0 011.158-.502l4.493 1.498a1 1 0 01.684.948V19a2 2 0 01-2 2h-1C9.717 21 3 14.283 3 6V5z"></path></svg>
                            <span>WhatsApp: <a href="https://wa.me/6285213745965" target="_blank" rel="noopener noreferrer" class="text-indigo-600 hover:underline">0852-1374-5965</a></span>
                        </li>
                        <!-- Instagram Contact -->
                        <li class="flex items-center justify-center lg:justify-start">
                            <svg class="w-6 h-6 mr-3 text-indigo-500" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                                <path fill-rule="evenodd" d="M12.315 2c2.43 0 2.784.002 3.797.043 1.054.049 1.791.216 2.428.468.65.255 1.218.598 1.772 1.153a4.908 4.908 0 011.153 1.772c.252.637.42 1.374.468 2.427.04 1.013.043 1.373.043 3.797s-.003 2.783-.043 3.797c-.049 1.055-.216 1.79-.468 2.428a4.908 4.908 0 01-1.153 1.772c-.554.554-1.122.897-1.772 1.153-.637.252-1.373.42-2.428.468-1.013.04-1.373.043-3.797.043s-2.783-.003-3.797-.043c-1.055-.049-1.79-.216-2.428-.468a4.908 4.908 0 01-1.772-1.153 4.908 4.908 0 01-1.153-1.772c-.252-.637-.42-1.373-.468-2.428-.04-1.013-.043-1.373-.043-3.797s.003-2.783.043-3.797c.049-1.055.216-1.79.468-2.428a4.908 4.908 0 011.153-1.772A4.908 4.908 0 015.45 2.502c.637-.252 1.373-.42 2.428-.468C8.892 2.002 9.252 2 11.685 2h.63zm-.056 2.378c-2.07 0-2.327.008-3.132.042-.803.038-1.164.166-1.405.26a2.036 2.036 0 00-.916.63A2.035 2.035 0 004.24 8.78c-.095.241-.223.6-.26 1.405-.034.805-.042 1.062-.042 3.132s.008 2.327.042 3.132c.038.803.166 1.164.26 1.405a2.036 2.036 0 00.63.916 2.035 2.035 0 00.916.63c.241.095.6.223 1.405.26.805.034 1.062.042 3.132.042s2.327-.008 3.132-.042c.803-.038 1.164-.166 1.405-.26a2.036 2.036 0 00.916-.63 2.035 2.035 0 00.63-.916c.095-.241.223-.6.26-1.405-.034-.805-.042-1.062-.042-3.132s-.008-2.327-.042-3.132c-.038-.803-.166-1.164-.26-1.405a2.036 2.036 0 00-.63-.916 2.035 2.035 0 00-.916-.63c-.241-.095-.6-.223-1.405-.26-.805-.034-1.062-.042-3.132-.042zM12 7a5 5 0 100 10 5 5 0 000-10zm0 2a3 3 0 110 6 3 3 0 010-6zm6.5-3.5a1.25 1.25 0 11-2.5 0 1.25 1.25 0 012.5 0z" clip-rule="evenodd" />
                            </svg>
                            <span>Instagram: <a href="https://www.instagram.com/rifqii.firmansyah/" target="_blank" rel="noopener noreferrer" class="text-indigo-600 hover:underline">@rifqii.firmansyah</a></span>
                        </li>
                        <!-- Email (placeholder) -->
                        <li class="flex items-center justify-center lg:justify-start">
                            <svg class="w-6 h-6 mr-3 text-indigo-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                            <span>Email: <a href="mailto:rifqi.firmansyah@email.com" class="text-indigo-600 hover:underline">rifqi.firmansyah@email.com</a></span>
                        </li>
                    </ul>
                </div>

                <!-- Contact Form -->
                <div class="w-full lg:w-1/2 bg-white p-8 rounded-xl card-shadow hover-lift">
                    <h3 class="text-2xl font-bold text-gray-800 mb-4 text-center lg:text-left">Kirim Pesan</h3>
                    <p class="text-gray-600 mb-6 text-center lg:text-left">
                        Punya proyek menarik atau ingin berdiskusi lebih lanjut? Kirimkan pesan kepada saya.
                    </p>
                    <form id="contact-form" class="space-y-4">
                        <div>
                            <label for="contact-name" class="block text-sm font-medium text-gray-700">Nama Lengkap</label>
                            <input type="text" id="contact-name" name="name" required class="mt-1 block w-full p-3 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500">
                        </div>
                        <div>
                            <label for="contact-email" class="block text-sm font-medium text-gray-700">Email</label>
                            <input type="email" id="contact-email" name="email" required class="mt-1 block w-full p-3 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500">
                        </div>
                        <div>
                            <label for="contact-message" class="block text-sm font-medium text-gray-700">Pesan Anda</label>
                            <textarea id="contact-message" name="message" rows="4" required class="mt-1 block w-full p-3 border border-gray-300 rounded-md shadow-sm focus:ring-indigo-500 focus:border-indigo-500"></textarea>
                        </div>
                        <button type="submit" class="w-full btn-gradient text-white font-bold py-3 px-4 rounded-md shadow-lg hover:shadow-xl transition duration-300 ease-in-out transform hover:scale-105">
                            Kirim Pesan
                        </button>
                    </form>
                    <!-- Success/Error Message Container -->
                    <div id="form-message" class="mt-4 p-3 rounded-md text-center hidden"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer Section -->
    <footer class="bg-gray-800 text-white py-8">
        <div class="container mx-auto px-4 text-center">
            <p>&copy; <span id="current-year"></span> Rifqi Firmansyah. Hak Cipta Dilindungi.</p>
            <div class="flex justify-center space-x-4 mt-4">
                <a href="https://wa.me/6285213745965" target="_blank" rel="noopener noreferrer" class="text-gray-300 hover:text-white transition duration-300" title="WhatsApp Rifqi Firmansyah">
                    <!-- WhatsApp Icon (SVG) - simplified for common use -->
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M12.04 2C7.03 2 3 6.03 3 11.04c0 1.75.5 3.4 1.37 4.86L3.02 21.01l5.12-1.35c1.37.75 2.92 1.16 4.04 1.16 5.01 0 9.04-4.03 9.04-9.04C21.08 6.03 17.05 2 12.04 2zM17.5 15.3c-.23.12-.95.46-1.1.55-.15.09-.27.14-.38.07-.11-.07-.45-.17-.65-.2-.2-.03-.15-.03-.38.1-.23.14-.88.86-1.07.98-.19.12-.37.13-.69.02-.32-.11-1.37-.5-1.72-1.29-.35-.79-.04-1.12.23-1.39.2-.2.46-.35.6-.46.14-.12.07-.23-.02-.38-.09-.11-.38-.95-.52-1.28-.14-.32-.29-.27-.46-.28-.16-.01-.35-.01-.55-.01-.2 0-.52.07-.79.35-.27.28-1.04 1.01-1.04 2.47 0 1.46 1.07 2.85 1.22 3.05.15.2.29.32.6.46.3.14.61.18.88.1.27-.08 1.1-.42 1.36-.62.26-.2.45-.29.65-.35.2-.06.6-.26.86-.46.26-.2.32-.18.44-.1.12.07.78.37 1.49.73.71.36 1.27.56 1.42.63.15.07.28.1.38.1.11 0 .2-.01.3-.03.1-.02.23-.06.35-.13.12-.07.74-.36 1.07-.73.33-.37.33-.69.23-.86-.1-.17-.37-.26-.52-.33z"/>
                    </svg>
                </a>
                <a href="https://www.instagram.com/rifqii.firmansyah/" target="_blank" rel="noopener noreferrer" class="text-gray-300 hover:text-white transition duration-300" title="Instagram Rifqi Firmansyah">
                    <!-- Instagram Icon (SVG) -->
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                        <path fill-rule="evenodd" d="M12.315 2c2.43 0 2.784.002 3.797.043 1.054.049 1.791.216 2.428.468.65.255 1.218.598 1.772 1.153a4.908 4.908 0 011.153 1.772c.252.637.42 1.374.468 2.427.04 1.013.043 1.373.043 3.797s-.003 2.783-.043 3.797c-.049 1.055-.216 1.79-.468 2.428a4.908 4.908 0 01-1.153 1.772c-.554.554-1.122.897-1.772 1.153-.637.252-1.373.42-2.428.468-1.013.04-1.373.043-3.797.043s-2.783-.003-3.797-.043c-1.055-.049-1.79-.216-2.428-.468a4.908 4.908 0 01-1.772-1.153 4.908 4.908 0 01-1.153-1.772c-.252-.637-.42-1.373-.468-2.428-.04-1.013-.043-1.373-.043-3.797s.003-2.783.043-3.797c.049-1.055.216-1.79.468-2.428a4.908 4.908 0 011.153-1.772A4.908 4.908 0 015.45 2.502c.637-.252 1.373-.42 2.428-.468C8.892 2.002 9.252 2 11.685 2h.63zm-.056 2.378c-2.07 0-2.327.008-3.132.042-.803.038-1.164.166-1.405.26a2.036 2.036 0 00-.916.63A2.035 2.035 0 004.24 8.78c-.095.241-.223.6-.26 1.405-.034.805-.042 1.062-.042 3.132s.008 2.327.042 3.132c.038.803.166 1.164.26 1.405a2.036 2.036 0 00.63.916 2.035 2.035 0 00.916.63c.241.095.6.223 1.405.26.805.034 1.062.042 3.132.042s2.327-.008 3.132-.042c.803-.038 1.164-.166 1.405-.26a2.036 2.036 0 00.916-.63 2.035 2.035 0 00.63-.916c.095-.241.223-.6.26-1.405-.034-.805-.042-1.062-.042-3.132s-.008-2.327-.042-3.132c-.038-.803-.166-1.164-.26-1.405a2.036 2.036 0 00-.63-.916 2.035 2.035 0 00-.916-.63c-.241-.095-.6-.223-1.405-.26-.805-.034-1.062-.042-3.132-.042zM12 7a5 5 0 100 10 5 5 0 000-10zm0 2a3 3 0 110 6 3 3 0 010-6zm6.5-3.5a1.25 1.25 0 11-2.5 0 1.25 1.25 0 012.5 0z" clip-rule="evenodd" />
                    </svg>
                </a>
            </div>
        </div>
    </footer>

    <script>
        // Set the current year dynamically in the footer
        document.getElementById('current-year').textContent = new Date().getFullYear();

        // --- Mobile Menu Toggle Functionality ---
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const closeMobileMenuButton = document.getElementById('close-mobile-menu');
        const mobileMenu = document.getElementById('mobile-menu');

        // Event listener to open the mobile menu
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.remove('hidden'); // Show the mobile menu
        });

        // Event listener to close the mobile menu
        closeMobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.add('hidden'); // Hide the mobile menu
        });

        // --- Form Submission Handling ---
        const contactForm = document.getElementById('contact-form');
        const formMessage = document.getElementById('form-message');

        // Add event listener for form submission
        contactForm.addEventListener('submit', function(event) {
            event.preventDefault(); // Prevent the default form submission behavior (page reload)

            // Collect form data into an object
            const formData = {
                name: document.getElementById('contact-name').value,
                email: document.getElementById('contact-email').value,
                message: document.getElementById('contact-message').value
            };

            console.log('Formulir Kontak Terkirim:', formData); // Log the form data to the browser's console

            // IMPORTANT: For a real contact form, you need a backend service.
            // GitHub Pages only hosts static files and cannot run server-side code.
            // You can use services like Formspree.io, Netlify Forms, or similar.
            // Example using a hypothetical API endpoint (commented out):
            /*
            fetch('/api/submit-contact', { // Replace with your actual backend endpoint or Formspree URL
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json',
                },
                body: JSON.stringify(formData),
            })
            .then(response => response.json())
            .then(data => {
                if (data.success) {
                    formMessage.textContent = 'Pesan Anda telah terkirim! Saya akan segera membalasnya.';
                    formMessage.className = 'mt-4 p-3 rounded-md text-green-700 bg-green-100 text-center';
                    contactForm.reset();
                } else {
                    formMessage.textContent = data.message || 'Terjadi kesalahan saat mengirim pesan. Silakan coba lagi.';
                    formMessage.className = 'mt-4 p-3 rounded-md text-red-700 bg-red-100 text-center';
                }
                formMessage.classList.remove('hidden');
            })
            .catch((error) => {
                console.error('Error:', error);
                formMessage.textContent = 'Terjadi kesalahan jaringan. Silakan coba lagi nanti.';
                formMessage.className = 'mt-4 p-3 rounded-md text-red-700 bg-red-100 text-center';
                formMessage.classList.remove('hidden');
            });
            */

            // For this demonstration on GitHub Pages, we simulate a successful submission:
            formMessage.textContent = 'Pesan Anda telah terkirim! Saya akan segera membalasnya.';
            formMessage.className = 'mt-4 p-3 rounded-md text-green-700 bg-green-100 text-center';
            formMessage.classList.remove('hidden'); // Show the success message
            contactForm.reset(); // Clear the form fields

            // Automatically hide the message after 5 seconds
            setTimeout(() => {
                formMessage.classList.add('hidden');
            }, 5000);
        });

        // --- Smooth Scrolling for Navigation Links ---
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();

                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // --- Intersection Observer for Scroll-Triggered Animations ---
        // This makes elements animate when they become visible in the viewport.
        const observerOptions = {
            root: null, // Use the viewport as the root
            rootMargin: '0px',
            threshold: 0.1 // Trigger when 10% of the element is visible
        };

        const observer = new IntersectionObserver((entries, observer) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('is-visible'); // Add class to trigger animation
                    observer.unobserve(entry.target); // Stop observing once animated
                }
            });
        }, observerOptions);

        // Observe elements that should animate on scroll (e.g., section headers)
        document.querySelectorAll('.animate-on-scroll').forEach(el => {
            observer.observe(el);
        });
    </script>
</body>
</html>
