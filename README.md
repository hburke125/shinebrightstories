# shinebrightstories
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Shine Bright Stories | Diversity & Inclusion for Little Ones</title>
    
    <!-- Google Fonts: Quicksand for a friendly, rounded look suitable for children's brands -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@300;400;600;700&display=swap" rel="stylesheet">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>

    <!-- Tailwind Configuration for Custom Colors -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            pink: '#FF8F8F',
                            cream: '#FFF1CB',
                            blue: '#C2E2FA',
                            purple: '#B7A3E3',
                            dark: '#4A4A4A', // Soft dark gray for text instead of harsh black
                        }
                    },
                    fontFamily: {
                        sans: ['Quicksand', 'sans-serif'],
                    }
                }
            }
        }
    </script>

    <style>
        /* Custom Styles for smooth scrolling and animations */
        html {
            scroll-behavior: smooth;
        }
        
        .blob-shape {
            border-radius: 60% 40% 30% 70% / 60% 30% 70% 40%;
        }

        .wave-separator {
            width: 100%;
            height: auto;
            display: block;
        }

        /* Floating animation for hero image */
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }
        .float-anim {
            animation: float 4s ease-in-out infinite;
        }
    </style>
</head>
<body class="font-sans text-brand-dark bg-white">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 bg-white/90 backdrop-blur-sm shadow-sm transition-all duration-300">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Logo -->
                <div class="flex-shrink-0 flex items-center gap-2 cursor-pointer" onclick="window.scrollTo(0,0)">
                    <div class="w-10 h-10 bg-brand-pink rounded-full flex items-center justify-center text-white">
                        <i data-lucide="sparkles" class="w-6 h-6"></i>
                    </div>
                    <span class="font-bold text-xl tracking-tight text-brand-purple">Shine Bright <span class="text-brand-pink">Stories</span></span>
                </div>

                <!-- Desktop Menu -->
                <div class="hidden md:flex space-x-8">
                    <a href="#mission" class="text-gray-600 hover:text-brand-pink font-semibold transition">Our Mission</a>
                    <a href="#books" class="text-gray-600 hover:text-brand-pink font-semibold transition">Books</a>
                    <a href="#about" class="text-gray-600 hover:text-brand-pink font-semibold transition">About Hannah</a>
                    <a href="#contact" class="px-4 py-2 bg-brand-blue text-brand-dark font-bold rounded-full hover:bg-brand-purple hover:text-white transition shadow-sm">Get in Touch</a>
                </div>

                <!-- Mobile Menu Button -->
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-btn" class="text-gray-600 hover:text-brand-pink focus:outline-none">
                        <i data-lucide="menu" class="w-8 h-8"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu Panel -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-brand-cream">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3 text-center">
                <a href="#mission" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-brand-pink hover:bg-brand-cream">Our Mission</a>
                <a href="#books" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-brand-pink hover:bg-brand-cream">Books</a>
                <a href="#about" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-brand-pink hover:bg-brand-cream">About Hannah</a>
                <a href="#contact" class="block px-3 py-2 mt-4 rounded-md text-base font-bold bg-brand-blue text-brand-dark">Get in Touch</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="pt-32 pb-20 bg-brand-cream relative overflow-hidden">
        <!-- Decorative blobs -->
        <div class="absolute top-20 left-0 w-64 h-64 bg-brand-pink opacity-20 blob-shape blur-2xl -translate-x-1/2"></div>
        <div class="absolute bottom-0 right-0 w-80 h-80 bg-brand-blue opacity-30 blob-shape blur-2xl translate-x-1/3"></div>

        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="flex flex-col md:flex-row items-center justify-between">
                <div class="md:w-1/2 mb-10 md:mb-0 text-center md:text-left">
                    <div class="inline-block px-4 py-1 mb-4 bg-white rounded-full border border-brand-purple text-brand-purple text-sm font-bold uppercase tracking-wide">
                        For Ages 0-3
                    </div>
                    <h1 class="text-4xl md:text-6xl font-bold leading-tight mb-6 text-brand-dark">
                        Big concepts for <br>
                        <span class="text-brand-pink relative inline-block">
                            little minds.
                            <svg class="absolute w-full h-3 -bottom-1 left-0 text-brand-blue opacity-60" viewBox="0 0 200 9" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M2.00025 6.99997C2.00025 6.99997 45.4268 9.20002 96.9326 2.50002C148.438 -4.19998 200.001 5.99997 200.001 5.99997" stroke="currentColor" stroke-width="3" stroke-linecap="round"/></svg>
                        </span>
                    </h1>
                    <p class="text-xl text-gray-600 mb-8 leading-relaxed">
                        We create stories that foster diversity, inclusion, and kindness. Helping you raise a generation that shines bright.
                    </p>
                    <div class="flex flex-col sm:flex-row gap-4 justify-center md:justify-start">
                        <a href="#books" class="px-8 py-4 bg-brand-pink text-white font-bold rounded-full shadow-lg hover:bg-red-400 hover:-translate-y-1 transition transform flex items-center justify-center gap-2">
                            <i data-lucide="book-open" class="w-5 h-5"></i> Shop Books
                        </a>
                        <a href="#mission" class="px-8 py-4 bg-white text-brand-purple border-2 border-brand-purple font-bold rounded-full hover:bg-brand-purple hover:text-white transition transform flex items-center justify-center">
                            Learn More
                        </a>
                    </div>
                </div>
                
                <!-- Hero Image / Illustration Placeholder -->
                <div class="md:w-5/12 relative float-anim">
                    <div class="relative w-full aspect-square bg-white rounded-full p-8 border-4 border-dashed border-brand-blue shadow-xl flex items-center justify-center overflow-hidden">
                        <!-- Placeholder Concept Art -->
                        <div class="text-center">
                            <div class="flex justify-center mb-4">
                                <div class="flex -space-x-4">
                                    <div class="w-16 h-16 rounded-full bg-brand-pink border-2 border-white flex items-center justify-center text-white"><i data-lucide="smile" class="w-10 h-10"></i></div>
                                    <div class="w-16 h-16 rounded-full bg-brand-blue border-2 border-white flex items-center justify-center text-white"><i data-lucide="smile" class="w-10 h-10"></i></div>
                                    <div class="w-16 h-16 rounded-full bg-brand-purple border-2 border-white flex items-center justify-center text-white"><i data-lucide="smile" class="w-10 h-10"></i></div>
                                </div>
                            </div>
                            <h3 class="text-2xl font-bold text-gray-400">Illustration Here</h3>
                            <p class="text-sm text-gray-400 mt-2">Diversity & Joy</p>
                        </div>
                    </div>
                    <!-- Decorative Elements -->
                    <i data-lucide="star" class="absolute -top-4 -right-4 text-brand-purple w-12 h-12 fill-current animate-pulse"></i>
                    <i data-lucide="heart" class="absolute bottom-10 -left-6 text-brand-pink w-10 h-10 fill-current"></i>
                </div>
            </div>
        </div>
        
        <!-- Wave Divider -->
        <div class="absolute bottom-0 w-full leading-none text-white">
            <svg class="w-full h-12 md:h-24" viewBox="0 0 1440 320" xmlns="http://www.w3.org/2000/svg">
                <path fill="#ffffff" fill-opacity="1" d="M0,224L48,213.3C96,203,192,181,288,181.3C384,181,480,203,576,224C672,245,768,267,864,250.7C960,235,1056,181,1152,165.3C1248,149,1344,171,1392,181.3L1440,192L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
            </svg>
        </div>
    </section>

    <!-- Mission Section -->
    <section id="mission" class="py-20 bg-white">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-brand-dark mb-4">Why We Shine</h2>
                <p class="text-lg text-gray-600">
                    Representation matters, even for the tiniest readers. Our board books are designed to introduce the beauty of our world's diversity.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
                <!-- Feature 1 -->
                <div class="p-8 rounded-3xl bg-brand-cream/30 border border-brand-cream hover:shadow-lg transition">
                    <div class="w-16 h-16 mx-auto bg-brand-cream rounded-full flex items-center justify-center text-yellow-600 mb-6">
                        <i data-lucide="baby" class="w-8 h-8"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Designed for 0-3</h3>
                    <p class="text-gray-600">Sturdy pages, high contrast visuals, and simple language perfect for developing brains.</p>
                </div>

                <!-- Feature 2 -->
                <div class="p-8 rounded-3xl bg-brand-pink/10 border border-brand-pink/30 hover:shadow-lg transition">
                    <div class="w-16 h-16 mx-auto bg-brand-pink rounded-full flex items-center justify-center text-white mb-6">
                        <i data-lucide="globe-2" class="w-8 h-8"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">True Diversity</h3>
                    <p class="text-gray-600">Celebrating different abilities, skin tones, family structures, and cultures.</p>
                </div>

                <!-- Feature 3 -->
                <div class="p-8 rounded-3xl bg-brand-blue/30 border border-brand-blue hover:shadow-lg transition">
                    <div class="w-16 h-16 mx-auto bg-brand-blue rounded-full flex items-center justify-center text-blue-600 mb-6">
                        <i data-lucide="heart-handshake" class="w-8 h-8"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Inclusive Values</h3>
                    <p class="text-gray-600">Teaching kindness, empathy, and acceptance from the very first story time.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Products Section -->
    <section id="books" class="py-20 bg-brand-blue/20 relative">
         <!-- Wave Divider Top -->
         <div class="absolute top-0 w-full leading-none text-white transform rotate-180">
            <svg class="w-full h-12" viewBox="0 0 1440 120" xmlns="http://www.w3.org/2000/svg">
                <path fill="#ffffff" fill-opacity="1" d="M0,64L48,58.7C96,53,192,43,288,48C384,53,480,75,576,80C672,85,768,75,864,64C960,53,1056,43,1152,42.7C1248,43,1344,53,1392,58.7L1440,64L1440,120L1392,120C1344,120,1248,120,1152,120C1056,120,960,120,864,120C768,120,672,120,576,120C480,120,384,120,288,120C192,120,96,120,48,120L0,120Z"></path>
            </svg>
        </div>

        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 pt-10">
            <div class="flex items-end justify-between mb-12">
                <div>
                    <h2 class="text-3xl md:text-4xl font-bold text-brand-dark">Our Collection</h2>
                    <p class="text-brand-purple font-semibold mt-2">Bright stories for bright futures.</p>
                </div>
                <a href="#" class="hidden md:flex items-center text-brand-pink font-bold hover:text-brand-purple transition">
                    View all books <i data-lucide="arrow-right" class="w-5 h-5 ml-2"></i>
                </a>
            </div>

            <!-- Product Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <!-- Product 1 -->
                <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:-translate-y-2 transition duration-300">
                    <div class="bg-brand-cream h-64 flex items-center justify-center relative p-6">
                        <!-- Book Cover Placeholder -->
                        <div class="w-3/4 h-full bg-red-400 rounded-r-md rounded-l-sm shadow-xl flex flex-col items-center justify-center text-center p-4 border-l-4 border-red-600">
                            <span class="text-white font-bold text-lg leading-tight">Different is Dazzling</span>
                            <i data-lucide="sun" class="text-white w-8 h-8 mt-2 opacity-80"></i>
                        </div>
                        <div class="absolute top-4 right-4 bg-white px-3 py-1 rounded-full text-xs font-bold text-brand-dark shadow-sm">New!</div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-brand-dark mb-1">Different is Dazzling</h3>
                        <p class="text-sm text-gray-500 mb-4">Board Book • Ages 0-3</p>
                        <p class="text-gray-600 text-sm mb-6 line-clamp-2">A colorful journey celebrating what makes every child unique and wonderful.</p>
                        <div class="flex items-center justify-between">
                            <span class="text-2xl font-bold text-brand-pink">$12.99</span>
                            <button class="bg-brand-purple text-white p-2 rounded-full hover:bg-brand-dark transition">
                                <i data-lucide="shopping-bag" class="w-5 h-5"></i>
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Product 2 -->
                <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:-translate-y-2 transition duration-300">
                    <div class="bg-brand-pink/20 h-64 flex items-center justify-center relative p-6">
                        <!-- Book Cover Placeholder -->
                        <div class="w-3/4 h-full bg-blue-400 rounded-r-md rounded-l-sm shadow-xl flex flex-col items-center justify-center text-center p-4 border-l-4 border-blue-600">
                            <span class="text-white font-bold text-lg leading-tight">The Colors of Us</span>
                            <i data-lucide="palette" class="text-white w-8 h-8 mt-2 opacity-80"></i>
                        </div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-brand-dark mb-1">The Colors of Us</h3>
                        <p class="text-sm text-gray-500 mb-4">Board Book • Ages 0-3</p>
                        <p class="text-gray-600 text-sm mb-6 line-clamp-2">Exploring skin tones and cultures through the eyes of art and love.</p>
                        <div class="flex items-center justify-between">
                            <span class="text-2xl font-bold text-brand-pink">$12.99</span>
                            <button class="bg-brand-purple text-white p-2 rounded-full hover:bg-brand-dark transition">
                                <i data-lucide="shopping-bag" class="w-5 h-5"></i>
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Product 3 -->
                <div class="bg-white rounded-2xl overflow-hidden shadow-lg hover:-translate-y-2 transition duration-300">
                    <div class="bg-brand-purple/20 h-64 flex items-center justify-center relative p-6">
                        <!-- Book Cover Placeholder -->
                        <div class="w-3/4 h-full bg-yellow-400 rounded-r-md rounded-l-sm shadow-xl flex flex-col items-center justify-center text-center p-4 border-l-4 border-yellow-600">
                            <span class="text-white font-bold text-lg leading-tight">Love Makes a Family</span>
                            <i data-lucide="users" class="text-white w-8 h-8 mt-2 opacity-80"></i>
                        </div>
                        <div class="absolute top-4 right-4 bg-brand-pink text-white px-3 py-1 rounded-full text-xs font-bold shadow-sm">Best Seller</div>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-brand-dark mb-1">Love Makes a Family</h3>
                        <p class="text-sm text-gray-500 mb-4">Board Book • Ages 0-3</p>
                        <p class="text-gray-600 text-sm mb-6 line-clamp-2">Showing all different types of families, united by the most important thing: love.</p>
                        <div class="flex items-center justify-between">
                            <span class="text-2xl font-bold text-brand-pink">$14.99</span>
                            <button class="bg-brand-purple text-white p-2 rounded-full hover:bg-brand-dark transition">
                                <i data-lucide="shopping-bag" class="w-5 h-5"></i>
                            </button>
                        </div>
                    </div>
                </div>

            </div>
            
            <div class="mt-8 text-center md:hidden">
                <a href="#" class="inline-flex items-center text-brand-pink font-bold hover:text-brand-purple transition">
                    View all books <i data-lucide="arrow-right" class="w-5 h-5 ml-2"></i>
                </a>
            </div>
        </div>
    </section>

    <!-- About Hannah Section -->
    <section id="about" class="py-20 relative overflow-hidden">
        <div class="absolute right-0 top-0 w-1/3 h-full bg-brand-cream/40 rounded-l-full hidden lg:block"></div>
        
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="flex flex-col lg:flex-row items-center gap-12">
                <!-- Image -->
                <div class="lg:w-1/2">
                    <div class="relative">
                        <div class="absolute inset-0 bg-brand-purple rounded-full rotate-6 transform translate-x-2 translate-y-2"></div>
                        <div class="relative w-80 h-80 sm:w-96 sm:h-96 mx-auto bg-gray-200 rounded-full border-8 border-white shadow-xl overflow-hidden flex items-center justify-center">
                            <!-- Placeholder for Hannah's Photo -->
                            <div class="text-center text-gray-400">
                                <i data-lucide="camera" class="w-16 h-16 mx-auto mb-2"></i>
                                <span class="block font-bold">Hannah Burke</span>
                                <span class="text-sm">Founder Photo</span>
                            </div>
                            <!-- If you have a real image, use: <img src="path/to/hannah.jpg" class="w-full h-full object-cover"> -->
                        </div>
                        
                        <!-- Floating badge -->
                        <div class="absolute bottom-4 right-10 md:right-20 bg-white p-4 rounded-xl shadow-lg border border-brand-pink/20">
                            <div class="flex items-center gap-2">
                                <i data-lucide="heart" class="text-brand-pink w-6 h-6 fill-current"></i>
                                <div>
                                    <p class="text-xs text-gray-500 font-bold uppercase">Founder</p>
                                    <p class="font-bold text-brand-dark">Shine Bright</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <!-- Content -->
                <div class="lg:w-1/2 text-center lg:text-left">
                    <h2 class="text-sm font-bold tracking-widest text-brand-pink uppercase mb-2">Meet the Founder</h2>
                    <h3 class="text-4xl font-bold text-brand-dark mb-6">Hi, I'm Hannah Burke.</h3>
                    
                    <div class="space-y-6 text-lg text-gray-600 leading-relaxed">
                        <p>
                            I started <span class="font-bold text-brand-purple">Shine Bright Stories</span> with a simple but powerful belief: it is never too early to teach children about the beautiful diversity of our world.
                        </p>
                        <p>
                            As an educator and a storyteller, I noticed a gap in the bookshelf for the 0-3 age group. I wanted to create board books that weren't just durable, but meaningful—books that plant seeds of inclusion, kindness, and self-love.
                        </p>
                        <p>
                            Every story we create is a labor of love, designed to help you start important conversations with your little ones, one page at a time.
                        </p>
                    </div>

                    <div class="mt-8 pt-8 border-t border-gray-100 flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-6">
                        <img src="https://upload.wikimedia.org/wikipedia/commons/c/ca/1x1.png" alt="Signature" class="h-12 opacity-50 bg-gray-200 w-32 rounded"> 
                        <!-- Replace above img with signature image if available -->
                        <div class="flex gap-4">
                            <a href="#" class="w-10 h-10 rounded-full bg-brand-blue flex items-center justify-center text-white hover:bg-blue-400 transition"><i data-lucide="instagram" class="w-5 h-5"></i></a>
                            <a href="#" class="w-10 h-10 rounded-full bg-brand-pink flex items-center justify-center text-white hover:bg-pink-400 transition"><i data-lucide="twitter" class="w-5 h-5"></i></a>
                            <a href="#" class="w-10 h-10 rounded-full bg-brand-purple flex items-center justify-center text-white hover:bg-purple-400 transition"><i data-lucide="linkedin" class="w-5 h-5"></i></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact / Newsletter -->
    <section id="contact" class="py-20 bg-brand-purple relative">
         <!-- Wave Divider Top -->
         <div class="absolute top-0 w-full leading-none text-white transform rotate-180">
            <svg class="w-full h-12 md:h-24" viewBox="0 0 1440 320" xmlns="http://www.w3.org/2000/svg">
                <path fill="#ffffff" fill-opacity="1" d="M0,96L48,112C96,128,192,160,288,160C384,160,480,128,576,112C672,96,768,96,864,112C960,128,1056,160,1152,165.3C1248,171,1344,149,1392,138.7L1440,128L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
            </svg>
        </div>

        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center relative z-10 pt-16">
            <div class="bg-white rounded-3xl p-10 shadow-2xl">
                <div class="w-16 h-16 bg-brand-cream rounded-full flex items-center justify-center mx-auto mb-6 text-brand-dark">
                    <i data-lucide="mail" class="w-8 h-8"></i>
                </div>
                <h2 class="text-3xl font-bold text-brand-dark mb-4">Let's Stay Connected</h2>
                <p class="text-gray-600 mb-8 max-w-lg mx-auto">
                    Join our mailing list for diversity tips, new book announcements, and free printable activities for your little ones.
                </p>
                
                <form class="flex flex-col sm:flex-row gap-4 max-w-lg mx-auto" onsubmit="event.preventDefault(); alert('Thanks for subscribing! (This is a demo)');">
                    <input type="email" placeholder="Your email address" class="flex-1 px-6 py-4 rounded-full border-2 border-brand-cream focus:border-brand-pink focus:outline-none bg-gray-50 text-brand-dark" required>
                    <button type="submit" class="px-8 py-4 bg-brand-pink text-white font-bold rounded-full hover:bg-brand-dark transition shadow-md">
                        Subscribe
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-brand-purple text-white pt-16 pb-8">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-12">
                <div class="col-span-1 md:col-span-1">
                    <div class="flex items-center gap-2 mb-4 font-bold text-xl">
                        <i data-lucide="sparkles" class="w-6 h-6 text-brand-cream"></i>
                        <span>Shine Bright</span>
                    </div>
                    <p class="text-white/80 text-sm">
                        Creating a more inclusive world, one board book at a time.
                    </p>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4 text-brand-cream">Shop</h4>
                    <ul class="space-y-2 text-sm text-white/80">
                        <li><a href="#" class="hover:text-white">All Books</a></li>
                        <li><a href="#" class="hover:text-white">New Arrivals</a></li>
                        <li><a href="#" class="hover:text-white">Bundles</a></li>
                        <li><a href="#" class="hover:text-white">Gift Cards</a></li>
                    </ul>
                </div>

                <div>
                    <h4 class="font-bold mb-4 text-brand-cream">Company</h4>
                    <ul class="space-y-2 text-sm text-white/80">
                        <li><a href="#about" class="hover:text-white">About Hannah</a></li>
                        <li><a href="#mission" class="hover:text-white">Our Mission</a></li>
                        <li><a href="#" class="hover:text-white">Wholesale</a></li>
                        <li><a href="#" class="hover:text-white">Contact Us</a></li>
                    </ul>
                </div>

                <div>
                    <h4 class="font-bold mb-4 text-brand-cream">Follow Us</h4>
                    <div class="flex gap-4">
                        <a href="#" class="hover:text-brand-cream transition"><i data-lucide="instagram" class="w-5 h-5"></i></a>
                        <a href="#" class="hover:text-brand-cream transition"><i data-lucide="facebook" class="w-5 h-5"></i></a>
                        <a href="#" class="hover:text-brand-cream transition"><i data-lucide="twitter" class="w-5 h-5"></i></a>
                    </div>
                </div>
            </div>
            
            <div class="border-t border-white/20 pt-8 text-center text-sm text-white/60">
                <p>&copy; 2023 Shine Bright Stories. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Script to Initialize Icons and Mobile Menu -->
    <script>
        // Initialize Lucide Icons
        lucide.createIcons();

        // Mobile Menu Toggle
        const btn = document.getElementById('mobile-menu-btn');
        const menu = document.getElementById('mobile-menu');

        btn.addEventListener('click', () => {
            menu.classList.toggle('hidden');
        });

        // Close mobile menu when a link is clicked
        const links = menu.querySelectorAll('a');
        links.forEach(link => {
            link.addEventListener('click', () => {
                menu.classList.add('hidden');
            });
        });
    </script>
</body>
</html>
