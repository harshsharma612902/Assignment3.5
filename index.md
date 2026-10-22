<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alex Rivera | Portfolio & Blog</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#f0f9ff',
                            100: '#e0f2fe',
                            500: '#0284c7',
                            600: '#0284c7',
                            700: '#0369a1',
                        }
                    }
                }
            }
        }
    </script>
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .glassmorphism {
            background: rgba(255, 255, 255, 0.7);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
        }
        .dark .glassmorphism {
            background: rgba(15, 23, 42, 0.75);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 dark:bg-slate-900 dark:text-slate-100 transition-colors duration-300 min-h-screen flex flex-col justify-between">

    <!-- Header & Navigation Bar -->
    <header class="sticky top-0 z-50 glassmorphism border-b border-slate-200 dark:border-slate-800 transition-colors duration-300">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
            <!-- Name / Logo -->
            <a href="#hero" class="flex items-center space-x-3 group">
                <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-sky-500 to-indigo-600 flex items-center justify-center text-white font-bold text-xl shadow-md group-hover:scale-105 transition-transform">
                    AR
                </div>
                <span class="font-bold text-xl tracking-tight text-slate-900 dark:text-white">Alex Rivera</span>
            </a>

            <!-- Desktop Navigation -->
            <nav class="hidden md:flex items-center space-x-8 font-medium text-sm">
                <a href="#about" class="hover:text-sky-500 dark:hover:text-sky-400 transition-colors">About Me</a>
                <a href="#skills" class="hover:text-sky-500 dark:hover:text-sky-400 transition-colors">Skills</a>
                <a href="#projects" class="hover:text-sky-500 dark:hover:text-sky-400 transition-colors">Projects</a>
                <a href="#blog" class="hover:text-sky-500 dark:hover:text-sky-400 transition-colors">Blog</a>
                <a href="#links" class="hover:text-sky-500 dark:hover:text-sky-400 transition-colors">Links</a>
                <a href="#contact" class="hover:text-sky-500 dark:hover:text-sky-400 transition-colors">Contact</a>
            </nav>

            <!-- Theme Toggle & Mobile Menu Button -->
            <div class="flex items-center space-x-4">
                <button id="theme-toggle" aria-label="Toggle Theme" class="p-2 rounded-lg bg-slate-200 dark:bg-slate-800 text-slate-700 dark:text-slate-300 hover:ring-2 hover:ring-sky-500 transition-all">
                    <i id="theme-toggle-dark-icon" class="fas font-solid fa-moon hidden"></i>
                    <i id="theme-toggle-light-icon" class="fas font-solid fa-sun hidden"></i>
                </button>
                
                <button id="mobile-menu-btn" aria-label="Open Menu" class="md:hidden p-2 rounded-lg text-slate-600 dark:text-slate-300 hover:bg-slate-200 dark:hover:bg-slate-800">
                    <i class="fas fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Navigation Menu -->
        <div id="mobile-menu" class="hidden md:hidden border-b border-slate-200 dark:border-slate-800 bg-white dark:bg-slate-900 px-4 pt-2 pb-4 space-y-3 font-medium">
            <a href="#about" class="block py-2 hover:text-sky-500 transition-colors mobile-link">About Me</a>
            <a href="#skills" class="block py-2 hover:text-sky-500 transition-colors mobile-link">Skills</a>
            <a href="#projects" class="block py-2 hover:text-sky-500 transition-colors mobile-link">Projects</a>
            <a href="#blog" class="block py-2 hover:text-sky-500 transition-colors mobile-link">Blog</a>
            <a href="#links" class="block py-2 hover:text-sky-500 transition-colors mobile-link">Links</a>
            <a href="#contact" class="block py-2 hover:text-sky-500 transition-colors mobile-link">Contact</a>
        </div>
    </header>

    <main class="flex-grow">
        <!-- Hero Section -->
        <section id="hero" class="py-20 md:py-28 px-4 max-w-6xl mx-auto">
            <div class="flex flex-col-reverse md:flex-row items-center justify-between gap-12">
                <div class="flex-1 text-center md:text-left">
                    <span class="inline-block px-3 py-1 text-xs font-semibold uppercase tracking-wider text-sky-600 dark:text-sky-400 bg-sky-100 dark:bg-sky-900/40 rounded-full mb-4">Welcome to my space</span>
                    <h1 class="text-4xl md:text-6xl font-extrabold tracking-tight mb-6">
                        Crafting Digital <span class="text-transparent bg-clip-text bg-gradient-to-r from-sky-500 to-indigo-600">Experiences</span> & Code.
                    </h1>
                    <p class="text-lg text-slate-600 dark:text-slate-300 mb-8 max-w-2xl leading-relaxed">
                        Full-Stack Developer, Creative Designer, and Tech Writer passionate about building intuitive web applications and writing insightful articles.
                    </p>
                    <div class="flex flex-wrap items-center justify-center md:justify-start gap-4">
                        <a href="#projects" class="px-6 py-3 bg-sky-600 hover:bg-sky-700 text-white font-medium rounded-xl shadow-lg shadow-sky-500/25 transition-all transform hover:-translate-y-0.5">
                            View My Work
                        </a>
                        <a href="#contact" class="px-6 py-3 bg-slate-200 dark:bg-slate-800 hover:bg-slate-300 dark:hover:bg-slate-700 font-medium rounded-xl transition-all">
                            Get In Touch
                        </a>
                    </div>
                </div>
                <div class="flex-1 flex justify-center">
                    <figure class="relative">
                        <div class="absolute -inset-1 bg-gradient-to-r from-sky-500 to-indigo-600 rounded-full blur opacity-50 group-hover:opacity-100 transition duration-1000"></div>
                        <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&q=80&w=500" 
                             alt="Profile photo of Alex Rivera" 
                             class="relative w-64 h-64 md:w-80 md:h-80 rounded-full object-cover border-4 border-white dark:border-slate-800 shadow-2xl"
                             onerror="this.src='https://placehold.co/400x400/0284c7/ffffff?text=Alex+Rivera'">
                    </figure>
                </div>
            </div>
        </section>

        <!-- About Me Section -->
        <section id="about" class="py-16 bg-slate-100/50 dark:bg-slate-800/30 border-y border-slate-200 dark:border-slate-800">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-12">
                    <h2 class="text-3xl font-bold tracking-tight mb-2">About Me</h2>
                    <div class="w-16 h-1 bg-sky-500 mx-auto rounded-full"></div>
                </div>
                <div class="grid md:grid-cols-2 gap-12 items-center">
                    <div>
                        <h3 class="text-2xl font-semibold mb-4">Passionate Software Engineer & Content Creator</h3>
                        <p class="text-slate-600 dark:text-slate-300 mb-4 leading-relaxed">
                            Hello! I'm Alex Rivera, a Computer Science student with over 3 years of hands-on experience building modern, accessible, and user-centric web applications.
                        </p>
                        <p class="text-slate-600 dark:text-slate-300 mb-6 leading-relaxed">
                            My journey began with plain HTML and CSS back in high school, and it has evolved into mastering modern JavaScript frameworks, backend development, and cloud platform integrations.
                        </p>
                        <div class="grid grid-cols-2 gap-4">
                            <div class="p-4 rounded-xl bg-white dark:bg-slate-800 shadow-sm border border-slate-100 dark:border-slate-700">
                                <span class="text-2xl font-bold text-sky-500">15+</span>
                                <p class="text-sm text-slate-500 dark:text-slate-400">Projects Completed</p>
                            </div>
                            <div class="p-4 rounded-xl bg-white dark:bg-slate-800 shadow-sm border border-slate-100 dark:border-slate-700">
                                <span class="text-2xl font-bold text-sky-500">10+</span>
                                <p class="text-sm text-slate-500 dark:text-slate-400">Blog Articles</p>
                            </div>
                        </div>
                    </div>
                    <div class="space-y-4">
                        <div class="p-6 rounded-2xl bg-white dark:bg-slate-800 shadow-sm border border-slate-100 dark:border-slate-700">
                            <h4 class="font-bold text-lg mb-2 flex items-center">
                                <i class="fas fa-graduation-cap text-sky-500 mr-3"></i> Education
                            </h4>
                            <p class="text-sm font-semibold">B.S. in Computer Science</p>
                            <p class="text-xs text-slate-500 dark:text-slate-400">State University • 2022 - Present</p>
                        </div>
                        <div class="p-6 rounded-2xl bg-white dark:bg-slate-800 shadow-sm border border-slate-100 dark:border-slate-700">
                            <h4 class="font-bold text-lg mb-2 flex items-center">
                                <i class="fas fa-briefcase text-sky-500 mr-3"></i> Experience
                            </h4>
                            <p class="text-sm font-semibold">Frontend Developer Intern</p>
                            <p class="text-xs text-slate-500 dark:text-slate-400">TechCorp Solutions • Summer 2024</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Skills & Interests Section -->
        <section id="skills" class="py-16">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-12">
                    <h2 class="text-3xl font-bold tracking-tight mb-2">Skills & Interests</h2>
                    <p class="text-slate-500 dark:text-slate-400">Tools, technologies, and activities I am passionate about</p>
                    <div class="w-16 h-1 bg-sky-500 mx-auto rounded-full mt-2"></div>
                </div>

                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Technical Skills List -->
                    <div class="p-6 rounded-2xl bg-white dark:bg-slate-800 shadow-md border border-slate-100 dark:border-slate-700">
                        <div class="w-12 h-12 rounded-xl bg-sky-100 dark:bg-sky-900/50 text-sky-600 dark:text-sky-400 flex items-center justify-center text-xl mb-4">
                            <i class="fas fa-code"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-4">Frontend Development</h3>
                        <ul class="space-y-2 text-slate-600 dark:text-slate-300">
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> HTML5 & Semantic Web</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> CSS3 & Tailwind CSS</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> JavaScript (ES6+)</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> React & Next.js</li>
                        </ul>
                    </div>

                    <!-- Tools & Frameworks -->
                    <div class="p-6 rounded-2xl bg-white dark:bg-slate-800 shadow-md border border-slate-100 dark:border-slate-700">
                        <div class="w-12 h-12 rounded-xl bg-indigo-100 dark:bg-indigo-900/50 text-indigo-600 dark:text-indigo-400 flex items-center justify-center text-xl mb-4">
                            <i class="fas fa-layer-group"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-4">Tools & Backend</h3>
                        <ul class="space-y-2 text-slate-600 dark:text-slate-300">
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Node.js & Express</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> Git & GitHub Version Control</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> RESTful APIs & GraphQL</li>
                            <li class="flex items-center"><i class="fas fa-check text-green-500 mr-2"></i> MongoDB & PostgreSQL</li>
                        </ul>
                    </div>

                    <!-- Personal Interests -->
                    <div class="p-6 rounded-2xl bg-white dark:bg-slate-800 shadow-md border border-slate-100 dark:border-slate-700">
                        <div class="w-12 h-12 rounded-xl bg-purple-100 dark:bg-purple-900/50 text-purple-600 dark:text-purple-400 flex items-center justify-center text-xl mb-4">
                            <i class="fas fa-heart"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-4">Personal Interests</h3>
                        <ol class="list-decimal list-inside space-y-2 text-slate-600 dark:text-slate-300">
                            <li class="inline-block w-full"><span class="font-medium">Technical Writing:</span> Tech trends & tutorials</li>
                            <li class="inline-block w-full"><span class="font-medium">UI/UX Design:</span> Wireframing & prototyping</li>
                            <li class="inline-block w-full"><span class="font-medium">Open Source:</span> Community contributions</li>
                            <li class="inline-block w-full"><span class="font-medium">Photography:</span> Urban and nature shots</li>
                        </ol>
                    </div>
                </div>
            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects" class="py-16 bg-slate-100/50 dark:bg-slate-800/30 border-t border-slate-200 dark:border-slate-800">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-8">
                    <h2 class="text-3xl font-bold tracking-tight mb-2">Featured Projects</h2>
                    <p class="text-slate-500 dark:text-slate-400">Explore some of my recent work</p>
                    <div class="w-16 h-1 bg-sky-500 mx-auto rounded-full mt-2"></div>
                </div>

                <!-- Project Category Filters -->
                <div class="flex justify-center gap-2 mb-10">
                    <button class="filter-btn active px-4 py-2 text-sm rounded-xl font-medium bg-sky-600 text-white transition-all" data-filter="all">All</button>
                    <button class="filter-btn px-4 py-2 text-sm rounded-xl font-medium bg-slate-200 dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-300 transition-all" data-filter="web">Web Apps</button>
                    <button class="filter-btn px-4 py-2 text-sm rounded-xl font-medium bg-slate-200 dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-300 transition-all" data-filter="design">UI/UX</button>
                </div>

                <!-- Projects Grid -->
                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8" id="projects-container">
                    <!-- Project Card 1 -->
                    <article class="project-card group bg-white dark:bg-slate-800 rounded-2xl overflow-hidden shadow-md border border-slate-100 dark:border-slate-700 flex flex-col" data-category="web">
                        <figure class="relative overflow-hidden h-48">
                            <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?auto=format&fit=crop&q=80&w=600" 
                                 alt="Task Management Dashboard" 
                                 class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-300"
                                 onerror="this.src='https://placehold.co/600x400/0284c7/ffffff?text=Task+Manager'">
                            <div class="absolute inset-0 bg-slate-900/40 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center gap-3">
                                <a href="https://github.com" target="_blank" rel="noopener noreferrer" aria-label="GitHub Repository" class="p-2 bg-white rounded-full text-slate-900 hover:scale-110 transition-transform"><i class="fab fa-github text-lg"></i></a>
                                <a href="https://example.com" target="_blank" rel="noopener noreferrer" aria-label="Live Demo" class="p-2 bg-sky-600 rounded-full text-white hover:scale-110 transition-transform"><i class="fas fa-external-link-alt text-lg"></i></a>
                            </div>
                        </figure>
                        <div class="p-6 flex-grow flex flex-col justify-between">
                            <div>
                                <span class="text-xs font-semibold text-sky-500 uppercase tracking-wider">Web Application</span>
                                <h3 class="text-xl font-bold mt-1 mb-2">DevFlow Task Manager</h3>
                                <p class="text-sm text-slate-600 dark:text-slate-300 mb-4">A real-time collaborative task board designed for developer teams with status tracking and analytics.</p>
                            </div>
                            <div class="flex flex-wrap gap-2">
                                <span class="px-2 py-1 text-xs bg-slate-100 dark:bg-slate-700 rounded-md">React</span>
                                <span class="px-2 py-1 text-xs bg-slate-100 dark:bg-slate-700 rounded-md">Tailwind</span>
                                <span class="px-2 py-1 text-xs bg-slate-100 dark:bg-slate-700 rounded-md">Firebase</span>
                            </div>
                        </div>
                    </article>

                    <!-- Project Card 2 -->
                    <article class="project-card group bg-white dark:bg-slate-800 rounded-2xl overflow-hidden shadow-md border border-slate-100 dark:border-slate-700 flex flex-col" data-category="design">
                        <figure class="relative overflow-hidden h-48">
                            <img src="https://images.unsplash.com/photo-1507238691740-187a5b1d37b8?auto=format&fit=crop&q=80&w=600" 
                                 alt="E-Commerce Redesign" 
                                 class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-300"
                                 onerror="this.src='https://placehold.co/600x400/0284c7/ffffff?text=E-Commerce+App'">
                            <div class="absolute inset-0 bg-slate-900/40 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center gap-3">
                                <a href="https://github.com" target="_blank" rel="noopener noreferrer" aria-label="GitHub Repository" class="p-2 bg-white rounded-full text-slate-900 hover:scale-110 transition-transform"><i class="fab fa-github text-lg"></i></a>
                                <a href="https://example.com" target="_blank" rel="noopener noreferrer" aria-label="Live Demo" class="p-2 bg-sky-600 rounded-full text-white hover:scale-110 transition-transform"><i class="fas fa-external-link-alt text-lg"></i></a>
                            </div>
                        </figure>
                        <div class="p-6 flex-grow flex flex-col justify-between">
                            <div>
                                <span class="text-xs font-semibold text-purple-500 uppercase tracking-wider">UI/UX Design</span>
                                <h3 class="text-xl font-bold mt-1 mb-2">Minimalist E-Commerce</h3>
                                <p class="text-sm text-slate-600 dark:text-slate-300 mb-4">Complete redesign of a modern fashion store focusing on seamless checkout flow and mobile accessibility.</p>
                            </div>
                            <div class="flex flex-wrap gap-2">
                                <span class="px-2 py-1 text-xs bg-slate-100 dark:bg-slate-700 rounded-md">Figma</span>
                                <span class="px-2 py-1 text-xs bg-slate-100 dark:bg-slate-700 rounded-md">UX Research</span>
                                <span class="px-2 py-1 text-xs bg-slate-100 dark:bg-slate-700 rounded-md">HTML/CSS</span>
                            </div>
                        </div>
                    </article>

                    <!-- Project Card 3 -->
                    <article class="project-card group bg-white dark:bg-slate-800 rounded-2xl overflow-hidden shadow-md border border-slate-100 dark:border-slate-700 flex flex-col" data-category="web">
                        <figure class="relative overflow-hidden h-48">
                            <img src="https://images.unsplash.com/photo-1526374965328-7f61d4dc18c5?auto=format&fit=crop&q=80&w=600" 
                                 alt="AI Weather App" 
                                 class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-300"
                                 onerror="this.src='https://placehold.co/600x400/0284c7/ffffff?text=Weather+App'">
                            <div class="absolute inset-0 bg-slate-900/40 opacity-0 group-hover:opacity-100 transition-opacity flex items-center justify-center gap-3">
                                <a href="https://github.com" target="_blank" rel="noopener noreferrer" aria-label="GitHub Repository" class="p-2 bg-white rounded-full text-slate-900 hover:scale-110 transition-transform"><i class="fab fa-github text-lg"></i></a>
                                <a href="https://example.com" target="_blank" rel="noopener noreferrer" aria-label="Live Demo" class="p-2 bg-sky-600 rounded-full text-white hover:scale-110 transition-transform"><i class="fas fa-external-link-alt text-lg"></i></a>
                            </div>
                        </figure>
                        <div class="p-6 flex-grow flex flex-col justify-between">
                            <div>
                                <span class="text-xs font-semibold text-sky-500 uppercase tracking-wider">Web Application</span>
                                <h3 class="text-xl font-bold mt-1 mb-2">Weather AI Forecast</h3>
                                <p class="text-sm text-slate-600 dark:text-slate-300 mb-4">Intelligent weather forecast app providing AI-driven clothing and activity recommendations.</p>
                            </div>
                            <div class="flex flex-wrap gap-2">
                                <span class="px-2 py-1 text-xs bg-slate-100 dark:bg-slate-700 rounded-md">JavaScript</span>
                                <span class="px-2 py-1 text-xs bg-slate-100 dark:bg-slate-700 rounded-md">OpenWeather API</span>
                            </div>
                        </div>
                    </article>
                </div>
            </div>
        </section>

        <!-- Blog Posts Section -->
        <section id="blog" class="py-16">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-12">
                    <h2 class="text-3xl font-bold tracking-tight mb-2">Latest Blog Posts</h2>
                    <p class="text-slate-500 dark:text-slate-400">Thoughts, tutorials, and insights on modern web development</p>
                    <div class="w-16 h-1 bg-sky-500 mx-auto rounded-full mt-2"></div>
                </div>

                <div class="grid md:grid-cols-2 gap-8">
                    <!-- Blog Article 1 -->
                    <article class="p-6 bg-white dark:bg-slate-800 rounded-2xl shadow-sm border border-slate-100 dark:border-slate-700 flex flex-col justify-between">
                        <div>
                            <div class="flex items-center space-x-2 text-xs text-slate-400 mb-3">
                                <span><i class="far fa-calendar mr-1"></i> Oct 15, 2026</span>
                                <span>•</span>
                                <span><i class="far fa-clock mr-1"></i> 5 min read</span>
                            </div>
                            <h3 class="text-xl font-bold mb-3 hover:text-sky-500 transition-colors">
                                <a href="#blog" class="blog-read-btn" data-title="Mastering Semantic HTML5" data-content="Semantic HTML is the backbone of web accessibility and SEO. By using structural elements like header, main, section, article, and footer correctly, you allow search engines and assistive technologies to better understand your web content structure. It makes maintenance easier and improves performance.">Mastering Semantic HTML5 for Better SEO & Accessibility</a>
                            </h3>
                            <p class="text-slate-600 dark:text-slate-300 text-sm mb-4 leading-relaxed">
                                Understanding why structured tags like &lt;header&gt;, &lt;article&gt;, and &lt;section&gt; matter more than ever in modern web development...
                            </p>
                        </div>
                        <button class="blog-read-btn inline-flex items-center text-sm font-semibold text-sky-600 dark:text-sky-400 hover:underline" data-title="Mastering Semantic HTML5" data-content="Semantic HTML is the backbone of web accessibility and SEO. By using structural elements like header, main, section, article, and footer correctly, you allow search engines and assistive technologies to better understand your web content structure. It makes maintenance easier and improves performance.">
                            Read Full Article <i class="fas fa-arrow-right ml-2 text-xs"></i>
                        </button>
                    </article>

                    <!-- Blog Article 2 -->
                    <article class="p-6 bg-white dark:bg-slate-800 rounded-2xl shadow-sm border border-slate-100 dark:border-slate-700 flex flex-col justify-between">
                        <div>
                            <div class="flex items-center space-x-2 text-xs text-slate-400 mb-3">
                                <span><i class="far fa-calendar mr-1"></i> Sep 28, 2026</span>
                                <span>•</span>
                                <span><i class="far fa-clock mr-1"></i> 8 min read</span>
                            </div>
                            <h3 class="text-xl font-bold mb-3 hover:text-sky-500 transition-colors">
                                <a href="#blog" class="blog-read-btn" data-title="Why Tailwind CSS accelerates workflow" data-content="Tailwind CSS provides utility-first classes that speed up design iterations without leaving your HTML files. Through design tokens, responsiveness, and dark mode configuration directly in your markup, utility frameworks empower developers to build custom user interfaces efficiently.">Why Utility-First CSS Accelerates Frontend Workflows</a>
                            </h3>
                            <p class="text-slate-600 dark:text-slate-300 text-sm mb-4 leading-relaxed">
                                Exploring how utility-first frameworks help developers rapidly build responsive designs without writing custom CSS files...
                            </p>
                        </div>
                        <button class="blog-read-btn inline-flex items-center text-sm font-semibold text-sky-600 dark:text-sky-400 hover:underline" data-title="Why Utility-First CSS Accelerates Frontend Workflows" data-content="Tailwind CSS provides utility-first classes that speed up design iterations without leaving your HTML files. Through design tokens, responsiveness, and dark mode configuration directly in your markup, utility frameworks empower developers to build custom user interfaces efficiently.">
                            Read Full Article <i class="fas fa-arrow-right ml-2 text-xs"></i>
                        </button>
                    </article>
                </div>
            </div>
        </section>

        <!-- Useful Links Section -->
        <section id="links" class="py-16 bg-slate-100/50 dark:bg-slate-800/30 border-y border-slate-200 dark:border-slate-800">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-12">
                    <h2 class="text-3xl font-bold tracking-tight mb-2">Useful Links & Resources</h2>
                    <p class="text-slate-500 dark:text-slate-400">External resources and platforms I frequently use</p>
                    <div class="w-16 h-1 bg-sky-500 mx-auto rounded-full mt-2"></div>
                </div>

                <div class="grid sm:grid-cols-2 md:grid-cols-4 gap-6">
                    <a href="https://github.com" target="_blank" rel="noopener noreferrer" class="p-5 bg-white dark:bg-slate-800 rounded-2xl shadow-sm hover:shadow-md border border-slate-100 dark:border-slate-700 flex items-center space-x-4 transition-all group">
                        <div class="w-10 h-10 rounded-xl bg-slate-100 dark:bg-slate-700 flex items-center justify-center text-slate-800 dark:text-white group-hover:scale-110 transition-transform">
                            <i class="fab fa-github text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-sm">GitHub</h4>
                            <span class="text-xs text-slate-400">Code repositories</span>
                        </div>
                    </a>

                    <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer" class="p-5 bg-white dark:bg-slate-800 rounded-2xl shadow-sm hover:shadow-md border border-slate-100 dark:border-slate-700 flex items-center space-x-4 transition-all group">
                        <div class="w-10 h-10 rounded-xl bg-blue-100 dark:bg-blue-900/40 flex items-center justify-center text-blue-600 dark:text-blue-400 group-hover:scale-110 transition-transform">
                            <i class="fab fa-linkedin-in text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-sm">LinkedIn</h4>
                            <span class="text-xs text-slate-400">Professional network</span>
                        </div>
                    </a>

                    <a href="https://developer.mozilla.org" target="_blank" rel="noopener noreferrer" class="p-5 bg-white dark:bg-slate-800 rounded-2xl shadow-sm hover:shadow-md border border-slate-100 dark:border-slate-700 flex items-center space-x-4 transition-all group">
                        <div class="w-10 h-10 rounded-xl bg-slate-100 dark:bg-slate-700 flex items-center justify-center text-slate-800 dark:text-white group-hover:scale-110 transition-transform">
                            <i class="fas fa-book text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-sm">MDN Web Docs</h4>
                            <span class="text-xs text-slate-400">Web documentation</span>
                        </div>
                    </a>

                    <a href="https://dev.to" target="_blank" rel="noopener noreferrer" class="p-5 bg-white dark:bg-slate-800 rounded-2xl shadow-sm hover:shadow-md border border-slate-100 dark:border-slate-700 flex items-center space-x-4 transition-all group">
                        <div class="w-10 h-10 rounded-xl bg-green-100 dark:bg-green-900/40 flex items-center justify-center text-green-600 dark:text-green-400 group-hover:scale-110 transition-transform">
                            <i class="fab fa-dev text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-sm">DEV Community</h4>
                            <span class="text-xs text-slate-400">Developer articles</span>
                        </div>
                    </a>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="py-16">
            <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-12">
                    <h2 class="text-3xl font-bold tracking-tight mb-2">Get In Touch</h2>
                    <p class="text-slate-500 dark:text-slate-400">Have a question or want to work together?</p>
                    <div class="w-16 h-1 bg-sky-500 mx-auto rounded-full mt-2"></div>
                </div>

                <div class="bg-white dark:bg-slate-800 rounded-2xl shadow-xl p-8 border border-slate-100 dark:border-slate-700">
                    <form id="contact-form" class="space-y-6">
                        <div class="grid md:grid-cols-2 gap-6">
                            <div>
                                <label for="name" class="block text-sm font-medium mb-2">Your Name</label>
                                <input type="text" id="name" required placeholder="John Doe" class="w-full px-4 py-3 rounded-xl border border-slate-200 dark:border-slate-700 bg-slate-50 dark:bg-slate-900 focus:ring-2 focus:ring-sky-500 outline-none transition-all">
                            </div>
                            <div>
                                <label for="email" class="block text-sm font-medium mb-2">Your Email</label>
                                <input type="email" id="email" required placeholder="john@example.com" class="w-full px-4 py-3 rounded-xl border border-slate-200 dark:border-slate-700 bg-slate-50 dark:bg-slate-900 focus:ring-2 focus:ring-sky-500 outline-none transition-all">
                            </div>
                        </div>
                        <div>
                            <label for="subject" class="block text-sm font-medium mb-2">Subject</label>
                            <input type="text" id="subject" required placeholder="Project Inquiry" class="w-full px-4 py-3 rounded-xl border border-slate-200 dark:border-slate-700 bg-slate-50 dark:bg-slate-900 focus:ring-2 focus:ring-sky-500 outline-none transition-all">
                        </div>
                        <div>
                            <label for="message" class="block text-sm font-medium mb-2">Message</label>
                            <textarea id="message" rows="4" required placeholder="Hello Alex, I'd like to discuss..." class="w-full px-4 py-3 rounded-xl border border-slate-200 dark:border-slate-700 bg-slate-50 dark:bg-slate-900 focus:ring-2 focus:ring-sky-500 outline-none transition-all"></textarea>
                        </div>
                        <button type="submit" class="w-full py-4 bg-sky-600 hover:bg-sky-700 text-white font-medium rounded-xl shadow-lg shadow-sky-500/25 transition-all">
                            Send Message
                        </button>
                    </form>
                    <div id="form-status" class="mt-4 text-center hidden text-sm font-medium p-3 rounded-xl"></div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-slate-900 text-slate-400 py-12 border-t border-slate-800">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row justify-between items-center gap-6">
                <div class="text-center md:text-left">
                    <span class="text-xl font-bold text-white tracking-tight">Alex Rivera</span>
                    <p class="text-sm text-slate-500 mt-1">Assignment 3.5 — Personal Blog & Portfolio Website</p>
                </div>

                <!-- Social Links -->
                <div class="flex items-center space-x-6">
                    <a href="https://github.com" target="_blank" rel="noopener noreferrer" aria-label="GitHub" class="hover:text-white transition-colors text-xl">
                        <i class="fab fa-github"></i>
                    </a>
                    <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn" class="hover:text-white transition-colors text-xl">
                        <i class="fab fa-linkedin"></i>
                    </a>
                    <a href="https://twitter.com" target="_blank" rel="noopener noreferrer" aria-label="Twitter" class="hover:text-white transition-colors text-xl">
                        <i class="fab fa-twitter"></i>
                    </a>
                    <a href="mailto:alex.rivera@example.com" aria-label="Email" class="hover:text-white transition-colors text-xl">
                        <i class="fas fa-envelope"></i>
                    </a>
                </div>
            </div>

            <div class="mt-8 pt-8 border-t border-slate-800 text-xs text-center text-slate-500">
                <p>&copy; 2026 Alex Rivera. All rights reserved. Created for Assignment 3.5.</p>
            </div>
        </div>
    </footer>

    <!-- Article Modal -->
    <div id="article-modal" class="fixed inset-0 z-50 bg-slate-900/60 backdrop-blur-sm flex items-center justify-center p-4 hidden">
        <div class="bg-white dark:bg-slate-800 rounded-2xl max-w-xl w-full p-6 shadow-2xl border border-slate-100 dark:border-slate-700 relative">
            <button id="close-modal" aria-label="Close Modal" class="absolute top-4 right-4 text-slate-400 hover:text-slate-600 dark:hover:text-white text-lg">
                <i class="fas fa-times"></i>
            </button>
            <h3 id="modal-title" class="text-2xl font-bold mb-4"></h3>
            <p id="modal-content" class="text-slate-600 dark:text-slate-300 leading-relaxed mb-6"></p>
            <button id="modal-ok-btn" class="px-5 py-2 bg-sky-600 text-white rounded-xl text-sm font-medium">Close</button>
        </div>
    </div>

    <!-- JavaScript Interactions -->
    <script>
        // Dark Theme Logic
        const themeToggleBtn = document.getElementById('theme-toggle');
        const darkIcon = document.getElementById('theme-toggle-dark-icon');
        const lightIcon = document.getElementById('theme-toggle-light-icon');

        if (localStorage.getItem('color-theme') === 'dark' || (!('color-theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
            document.documentElement.classList.add('dark');
            lightIcon.classList.remove('hidden');
        } else {
            document.documentElement.classList.remove('dark');
            darkIcon.classList.remove('hidden');
        }

        themeToggleBtn.addEventListener('click', () => {
            darkIcon.classList.toggle('hidden');
            lightIcon.classList.toggle('hidden');

            if (document.documentElement.classList.contains('dark')) {
                document.documentElement.classList.remove('dark');
                localStorage.setItem('color-theme', 'light');
            } else {
                document.documentElement.classList.add('dark');
                localStorage.setItem('color-theme', 'dark');
            }
        });

        // Mobile Navigation Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const mobileLinks = document.querySelectorAll('.mobile-link');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        mobileLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // Project Filter Functionality
        const filterBtns = document.querySelectorAll('.filter-btn');
        const projectCards = document.querySelectorAll('.project-card');

        filterBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                filterBtns.forEach(b => {
                    b.classList.remove('active', 'bg-sky-600', 'text-white');
                    b.classList.add('bg-slate-200', 'dark:bg-slate-800', 'text-slate-600', 'dark:text-slate-300');
                });
                btn.classList.add('active', 'bg-sky-600', 'text-white');
                btn.classList.remove('bg-slate-200', 'dark:bg-slate-800', 'text-slate-600', 'dark:text-slate-300');

                const filter = btn.getAttribute('data-filter');
                projectCards.forEach(card => {
                    if (filter === 'all' || card.getAttribute('data-category') === filter) {
                        card.style.display = 'flex';
                    } else {
                        card.style.display = 'none';
                    }
                });
            });
        });

        // Blog Article Modal Logic
        const modal = document.getElementById('article-modal');
        const modalTitle = document.getElementById('modal-title');
        const modalContent = document.getElementById('modal-content');
        const closeModal = document.getElementById('close-modal');
        const modalOkBtn = document.getElementById('modal-ok-btn');
        const readBtns = document.querySelectorAll('.blog-read-btn');

        readBtns.forEach(btn => {
            btn.addEventListener('click', (e) => {
                e.preventDefault();
                modalTitle.textContent = btn.getAttribute('data-title');
                modalContent.textContent = btn.getAttribute('data-content');
                modal.classList.remove('hidden');
            });
        });

        const hideModal = () => modal.classList.add('hidden');
        closeModal.addEventListener('click', hideModal);
        modalOkBtn.addEventListener('click', hideModal);

        // Contact Form Handler
        const contactForm = document.getElementById('contact-form');
        const formStatus = document.getElementById('form-status');

        contactForm.addEventListener('submit', (e) => {
            e.preventDefault();
            formStatus.textContent = "Thank you! Your message has been sent successfully.";
            formStatus.className = "mt-4 text-center text-sm font-medium p-3 rounded-xl bg-green-100 text-green-700 dark:bg-green-900/40 dark:text-green-300";
            contactForm.reset();
            setTimeout(() => {
                formStatus.classList.add('hidden');
            }, 5000);
        });
    </script>
</body>
</html>