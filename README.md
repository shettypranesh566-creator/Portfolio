<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        .project-card {
            transition: transform 0.3s ease-in-out;
        }
        .project-card:hover {
            transform: scale(1.05);
        }
        .smooth-scroll {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-gray-100 font-sans text-gray-800 smooth-scroll">
    <!-- Navigation -->
    <nav class="bg-white shadow-md fixed w-full top-0 z-10">
        <div class="max-w-6xl mx-auto px-4 py-4 flex justify-between items-center">
            <h1 class="text-2xl font-bold text-blue-600">My Portfolio</h1>
            <div class="space-x-4">
                <a href="#home" class="text-gray-600 hover:text-blue-600">Home</a>
                <a href="#projects" class="text-gray-600 hover:text-blue-600">Projects</a>
                <a href="#skills" class="text-gray-600 hover:text-blue-600">Skills</a>
                <a href="#contact" class="text-gray-600 hover:text-blue-600">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen flex items-center justify-center bg-gradient-to-r from-blue-500 to-purple-600 text-white">
        <div class="text-center">
            <h2 class="text-5xl font-bold mb-4">Hi, I'm [Your Name]</h2>
            <p class="text-xl mb-6">A passionate [Your Profession, e.g., Web Developer] creating innovative solutions</p>
            <a href="#contact" class="bg-white text-blue-600 px-6 py-3 rounded-full font-semibold hover:bg-blue-100">Get in Touch</a>
        </div>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="py-16 bg-white">
        <div class="max-w-6xl mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-8">My Projects</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project 1 -->
                <div class="project-card bg-gray-100 rounded-lg shadow-md overflow-hidden">
                    <img src="https://via.placeholder.com/400x200" alt="Project 1" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Project One</h3>
                        <p class="text-gray-600 mb-4">A brief description of your first project. Highlight key features and technologies used.</p>
                        <a href="#" class="text-blue-600 hover:underline">View Project</a>
                    </div>
                </div>
                <!-- Project 2 -->
                <div class="project-card bg-gray-100 rounded-lg shadow-md overflow-hidden">
                    <img src="https://via.placeholder.com/400x200" alt="Project 2" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Project Two</h3>
                        <p class="text-gray-600 mb-4">A brief description of your second project. Mention what makes it unique.</p>
                        <a href="#" class="text-blue-600 hover:underline">View Project</a>
                    </div>
                </div>
                <!-- Project 3 -->
                <div class="project-card bg-gray-100 rounded-lg shadow-md overflow-hidden">
                    <img src="https://via.placeholder.com/400x200" alt="Project 3" class="w-full h-48 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-semibold mb-2">Project Three</h3>
                        <p class="text-gray-600 mb-4">A brief description of your third project. Showcase your skills and impact.</p>
                        <a href="#" class="text-blue-600 hover:underline">View Project</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-16 bg-gray-100">
        <div class="max-w-6xl mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-8">My Skills</h2>
            <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
                <div class="bg-white p-4 rounded-lg shadow-md text-center">HTML</div>
                <div class="bg-white p-4 rounded-lg shadow-md text-center">CSS</div>
                <div class="bg-white p-4 rounded-lg shadow-md text-center">JavaScript</div>
                <div class="bg-white p-4 rounded-lg shadow-md text-center">React</div>
                <div class="bg-white p-4 rounded-lg shadow-md text-center">Python</div>
                <div class="bg-white p-4 rounded-lg shadow-md text-center">Node.js</div>
                <div class="bg-white p-4 rounded-lg shadow-md text-center">Git</div>
                <div class="bg-white p-4 rounded-lg shadow-md text-center">SQL</div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 bg-white">
        <div class="max-w-6xl mx-auto px-4">
            <h2 class="text-3xl font-bold text-center mb-8">Get in Touch</h2>
            <div class="max-w-lg mx-auto">
                <p class="text-gray-600 mb-4 text-center">Feel free to reach out for collaborations or just a friendly chat!</p>
                <div class="space-y-4">
                    <p class="text-center"><strong>Email:</strong> <a href="mailto:your.email@example.com" class="text-blue-600 hover:underline">your.email@example.com</a></p>
                    <p class="text-center"><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/yourprofile" class="text-blue-600 hover:underline">linkedin.com/in/yourprofile</a></p>
                    <p class="text-center"><strong>GitHub:</strong> <a href="https://github.com/yourusername" class="text-blue-600 hover:underline">github.com/yourusername</a></p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-4">
        <div class="max-w-6xl mx-auto px-4 text-center">
            <p>&copy; 2025 [Your Name]. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Smooth scroll for navigation links
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
