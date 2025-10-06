<!DOCTYPE html><!DOCTYPE html>
<html lang="en" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Everland</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/feather-icons"></script>
    <script src="https://cdn.jsdelivr.net/npm/feather-icons/dist/feather.min.js"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        primary: {
                            500: '#3B82F6',
                        },
                        secondary: {
                            500: '#10B981',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .hero-bg {
            background: linear-gradient(135deg, rgba(16, 185, 129, 0.1) 0%, rgba(59, 130, 246, 0.2) 100%);
        }
        .nav-link {
            transition: all 0.3s ease;
        }
        .nav-link:hover {
            color: #3B82F6;
            transform: translateY(-2px);
        }
        .btn-primary {
            transition: all 0.3s ease;
        }
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
    </style>
</head>
<body class="bg-gray-900 text-gray-200 min-h-screen flex flex-col">
    <!-- Navigation -->
    <nav class="bg-gray-800 py-4 px-6 shadow-lg">
        <div class="container mx-auto flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <i data-feather="compass" class="text-primary-500"></i>
                <span class="text-2xl font-bold text-white">Everland</span>
            </div>
            <div class="hidden md:flex space-x-8">
                <a href="#" class="nav-link text-white font-medium hover:text-primary-500">Home</a>
                <a href="#about" class="nav-link text-gray-400 font-medium hover:text-primary-500">About</a>
                <a href="#contact" class="nav-link text-gray-400 font-medium hover:text-primary-500">Contact</a>
            </div>
            <button class="md:hidden text-gray-400">
                <i data-feather="menu"></i>
            </button>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero-bg py-20 px-6">
        <div class="container mx-auto flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-10 md:mb-0">
                <h1 class="text-4xl md:text-5xl font-bold text-white mb-6 leading-tight">Welcome to <span class="text-primary-500">Everland</span></h1>
                <p class="text-xl text-gray-300 mb-8">Your trusted partner for comprehensive solutions across multiple sectors.</p>
                <div class="flex space-x-4">
                    <a href="#about" class="btn-primary bg-primary-500 hover:bg-primary-600 text-white px-6 py-3 rounded-lg font-medium">Learn More</a>
                    <a href="#contact" class="btn-primary border border-primary-500 text-primary-500 hover:bg-primary-500 hover:text-white px-6 py-3 rounded-lg font-medium">Contact Us</a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <img src="http://static.photos/technology/640x360/1" alt="Everland Services" class="rounded-lg shadow-xl">
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 px-6 bg-gray-800">
        <div class="container mx-auto">
            <h2 class="text-3xl font-bold text-white mb-12 text-center">About <span class="text-primary-500">Everland</span></h2>
            <div class="bg-gray-700 rounded-xl p-8 shadow-lg">
                <p class="text-gray-300 mb-6 text-lg leading-relaxed">
                    Everland is a diversified company committed to delivering high-quality solutions across multiple sectors, including construction, transportation, maintenance, services, and material supply.
                </p>
                <p class="text-gray-300 mb-6 text-lg leading-relaxed">
                    With a solid foundation built on professionalism and integrity, Everland has established itself as a trusted partner for clients in both the public and private sectors.
                </p>
                <p class="text-gray-300 mb-6 text-lg leading-relaxed">
                    Our operations are guided by a strong commitment to excellence, efficiency, and reliability. We approach every project with a results-driven mindset, ensuring that we consistently meet the highest industry standards while exceeding client expectations.
                </p>
                <p class="text-gray-300 mb-6 text-lg leading-relaxed">
                    By combining expertise, innovation, and a customer-focused approach, Everland provides comprehensive solutions tailored to the specific needs of each project. Our multidisciplinary capabilities enable us to manage complex challenges while maintaining cost-effectiveness, quality, and timely delivery.
                </p>
                <p class="text-gray-300 text-lg leading-relaxed">
                    At Everland, we are not only focused on achieving business success but also on building long-term partnerships based on trust, transparency, and shared growth.
                </p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 px-6">
        <div class="container mx-auto">
            <h2 class="text-3xl font-bold text-white mb-12 text-center">Contact <span class="text-primary-500">Us</span></h2>
            <div class="max-w-3xl mx-auto bg-gray-800 rounded-xl p-8 shadow-lg">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-8">
                    <div class="flex items-start space-x-4">
                        <div class="bg-primary-500 p-3 rounded-full">
                            <i data-feather="map-pin" class="text-white"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-white mb-2">Address</h3>
                            <p class="text-gray-400">123 Business Avenue, Sulaymaniyah, Iraq</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4">
                        <div class="bg-primary-500 p-3 rounded-full">
                            <i data-feather="phone" class="text-white"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-white mb-2">Phone</h3>
                            <p class="text-gray-400">+964 770 123 4567</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4">
                        <div class="bg-primary-500 p-3 rounded-full">
                            <i data-feather="mail" class="text-white"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-white mb-2">Email</h3>
                            <p class="text-gray-400">info@everland.com</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4">
                        <div class="bg-primary-500 p-3 rounded-full">
                            <i data-feather="clock" class="text-white"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-white mb-2">Working Hours</h3>
                            <p class="text-gray-400">Sunday - Thursday: 8:00 AM - 5:00 PM</p>
                        </div>
                    </div>
                </div>
                <form class="space-y-6">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 py-8 px-6 mt-auto">
        <div class="container mx-auto">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="flex items-center space-x-2 mb-4 md:mb-0">
                    <i data-feather="compass" class="text-primary-500"></i>
                    <span class="text-xl font-bold text-white">Everland</span>
                </div>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-primary-500">
                        <i data-feather="facebook"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-primary-500">
                        <i data-feather="twitter"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-primary-500">
                        <i data-feather="linkedin"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-primary-500">
                        <i data-feather="instagram"></i>
                    </a>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 mb-4 md:mb-0">© 2023 Everland. All rights reserved.</p>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-primary-500">Privacy Policy</a>
                    <a href="#" class="text-gray-400 hover:text-primary-500">Terms of Service</a>
                    <a href="#" class="text-gray-400 hover:text-primary-500">Contact Us</a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        feather.replace();
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>

<html lang="en" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Everland</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/feather-icons"></script>
    <script src="https://cdn.jsdelivr.net/npm/feather-icons/dist/feather.min.js"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        primary: {
                            500: '#3B82F6',
                        },
                        secondary: {
                            500: '#10B981',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .hero-bg {
            background: linear-gradient(135deg, rgba(16, 185, 129, 0.1) 0%, rgba(59, 130, 246, 0.2) 100%);
        }
        .nav-link {
            transition: all 0.3s ease;
        }
        .nav-link:hover {
            color: #3B82F6;
            transform: translateY(-2px);
        }
        .btn-primary {
            transition: all 0.3s ease;
        }
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
    </style>
</head>
<body class="bg-gray-900 text-gray-200 min-h-screen flex flex-col">
    <!-- Navigation -->
    <nav class="bg-gray-800 py-4 px-6 shadow-lg">
        <div class="container mx-auto flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <i data-feather="compass" class="text-primary-500"></i>
                <span class="text-2xl font-bold text-white">Everland</span>
            </div>
            <div class="hidden md:flex space-x-8">
                <a href="#" class="nav-link text-white font-medium hover:text-primary-500">Home</a>
                <a href="#about" class="nav-link text-gray-400 font-medium hover:text-primary-500">About</a>
                <a href="#contact" class="nav-link text-gray-400 font-medium hover:text-primary-500">Contact</a>
            </div>
            <button class="md:hidden text-gray-400">
                <i data-feather="menu"></i>
            </button>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero-bg py-20 px-6">
        <div class="container mx-auto flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-10 md:mb-0">
                <h1 class="text-4xl md:text-5xl font-bold text-white mb-6 leading-tight">Welcome to <span class="text-primary-500">Everland</span></h1>
                <p class="text-xl text-gray-300 mb-8">Your trusted partner for comprehensive solutions across multiple sectors.</p>
                <div class="flex space-x-4">
                    <a href="#about" class="btn-primary bg-primary-500 hover:bg-primary-600 text-white px-6 py-3 rounded-lg font-medium">Learn More</a>
                    <a href="#contact" class="btn-primary border border-primary-500 text-primary-500 hover:bg-primary-500 hover:text-white px-6 py-3 rounded-lg font-medium">Contact Us</a>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <img src="http://static.photos/technology/640x360/1" alt="Everland Services" class="rounded-lg shadow-xl">
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 px-6 bg-gray-800">
        <div class="container mx-auto">
            <h2 class="text-3xl font-bold text-white mb-12 text-center">About <span class="text-primary-500">Everland</span></h2>
            <div class="bg-gray-700 rounded-xl p-8 shadow-lg">
                <p class="text-gray-300 mb-6 text-lg leading-relaxed">
                    Everland is a diversified company committed to delivering high-quality solutions across multiple sectors, including construction, transportation, maintenance, services, and material supply.
                </p>
                <p class="text-gray-300 mb-6 text-lg leading-relaxed">
                    With a solid foundation built on professionalism and integrity, Everland has established itself as a trusted partner for clients in both the public and private sectors.
                </p>
                <p class="text-gray-300 mb-6 text-lg leading-relaxed">
                    Our operations are guided by a strong commitment to excellence, efficiency, and reliability. We approach every project with a results-driven mindset, ensuring that we consistently meet the highest industry standards while exceeding client expectations.
                </p>
                <p class="text-gray-300 mb-6 text-lg leading-relaxed">
                    By combining expertise, innovation, and a customer-focused approach, Everland provides comprehensive solutions tailored to the specific needs of each project. Our multidisciplinary capabilities enable us to manage complex challenges while maintaining cost-effectiveness, quality, and timely delivery.
                </p>
                <p class="text-gray-300 text-lg leading-relaxed">
                    At Everland, we are not only focused on achieving business success but also on building long-term partnerships based on trust, transparency, and shared growth.
                </p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 px-6">
        <div class="container mx-auto">
            <h2 class="text-3xl font-bold text-white mb-12 text-center">Contact <span class="text-primary-500">Us</span></h2>
            <div class="max-w-3xl mx-auto bg-gray-800 rounded-xl p-8 shadow-lg">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-8">
                    <div class="flex items-start space-x-4">
                        <div class="bg-primary-500 p-3 rounded-full">
                            <i data-feather="map-pin" class="text-white"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-white mb-2">Address</h3>
                            <p class="text-gray-400">123 Business Avenue, Sulaymaniyah, Iraq</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4">
                        <div class="bg-primary-500 p-3 rounded-full">
                            <i data-feather="phone" class="text-white"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-white mb-2">Phone</h3>
                            <p class="text-gray-400">+964 770 123 4567</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4">
                        <div class="bg-primary-500 p-3 rounded-full">
                            <i data-feather="mail" class="text-white"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-white mb-2">Email</h3>
                            <p class="text-gray-400">info@everland.com</p>
                        </div>
                    </div>
                    <div class="flex items-start space-x-4">
                        <div class="bg-primary-500 p-3 rounded-full">
                            <i data-feather="clock" class="text-white"></i>
                        </div>
                        <div>
                            <h3 class="text-xl font-bold text-white mb-2">Working Hours</h3>
                            <p class="text-gray-400">Sunday - Thursday: 8:00 AM - 5:00 PM</p>
                        </div>
                    </div>
                </div>
                <form class="space-y-6">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 py-8 px-6 mt-auto">
        <div class="container mx-auto">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="flex items-center space-x-2 mb-4 md:mb-0">
                    <i data-feather="compass" class="text-primary-500"></i>
                    <span class="text-xl font-bold text-white">Everland</span>
                </div>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-primary-500">
                        <i data-feather="facebook"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-primary-500">
                        <i data-feather="twitter"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-primary-500">
                        <i data-feather="linkedin"></i>
                    </a>
                    <a href="#" class="text-gray-400 hover:text-primary-500">
                        <i data-feather="instagram"></i>
                    </a>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 mb-4 md:mb-0">© 2023 Everland. All rights reserved.</p>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-primary-500">Privacy Policy</a>
                    <a href="#" class="text-gray-400 hover:text-primary-500">Terms of Service</a>
                    <a href="#" class="text-gray-400 hover:text-primary-500">Contact Us</a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        feather.replace();
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
