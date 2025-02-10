<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Frontend Developer Resume</title>
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    /* Background gradient */
    body {
      background: linear-gradient(to bottom right, #00b4d8, #1e3a8a);
    }
    @keyframes slideInFromBottom {
      0% {
        opacity: 0;
        transform: translateY(30px);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
      }
    }
    .fade-in {
      animation: fadeIn 1.5s ease-in-out;
    }
    @keyframes fadeIn {
      0% {
        opacity: 0;
      }
      100% {
        opacity: 1;
      }
    }
    .slide-in-bottom {
      animation: slideInFromBottom 1s ease-out forwards;
    }
    .hover\:scale-110:hover {
      transform: scale(1.1);
    }
    .skills-card:hover,
    .project-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
    }
    /* Styling for footer */
    footer {
      background: #1e3a8a;
      color: white;
    }
    footer .footer-content {
      padding: 20px;
      text-align: center;
    }
    /* Custom Navbar Styling */
    .navbar {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      z-index: 50;
      background-color: rgba(0, 0, 0, 0.7);
      padding: 8px 20px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
      transition: all 0.3s;
    }
    .navbar a {
      color: white;
      font-size: 1rem;
      margin-left: 20px;
    }
    .navbar a:hover {
      color: #00b4d8;
      text-decoration: underline;
    }
  </style>
</head>

<body class="font-sans text-white">

  <!-- Navbar -->
  <nav class="navbar">
    <div class="container mx-auto flex items-center justify-between">
      <a href="#hero" class="font-bold text-xl">top</a>
      <div>
        <a href="#summary" class="px-4 py-2">Summary</a>
        <a href="#skills" class="px-4 py-2">Skills</a>
        <a href="#experience" class="px-4 py-2">Experience</a>
        <a href="#projects" class="px-4 py-2">Projects</a>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <header id="hero" class="flex flex-col items-center justify-center min-h-screen text-center text-white py-10 px-6">
    <div class="relative mb-4">
      <!-- Profile Image -->
      <img src="Mgk5QW5i.jpg" alt="John Doe" class="w-36 h-36 rounded-full object-cover border-4 border-blue-500 shadow-lg hover:scale-110 transition-transform duration-300">
    </div>
    <h1 class="text-4xl sm:text-5xl font-bold mb-4 animate__fadeIn">
      Hello, I'm <span class="text-blue-200">sugam pathak</span>
    </h1>
    <p class="text-xl sm:text-2xl mb-6 opacity-90">Frontend Developer | Passionate about web design and user experience</p>
    <div class="flex space-x-6 mb-4">
      <a href="mailto:johndoe@example.com" class="text-blue-700 hover:text-blue-100 transition-colors duration-300">Email</a>
      <a href="https://www.linkedin.com/in/johndoe" target="_blank" class="text-blue-700 hover:text-blue-100 transition-colors duration-300">LinkedIn</a>
      <a href="https://github.com/johndoe" target="_blank" class="text-blue-700 hover:text-blue-100 transition-colors duration-300">GitHub</a>
    </div>
    <a href="#summary" class="bg-blue-500 px-6 py-3 rounded-full text-lg font-medium hover:bg-blue-600 transition-colors duration-300">Explore My Work</a>
  </header>

  <!-- Summary Section -->
  <section id="summary" class="container mx-auto py-12 text-center fade-in">
    <h2 class="text-3xl font-semibold text-gray-900 mb-6">Summary</h2>
    <p class="text-lg sm:text-xl text-gray-800 leading-relaxed">
      I’m a Frontend Developer with over 2 years of experience creating engaging, interactive, and user-friendly web applications. 
      I am passionate about bringing ideas to life with modern technologies such as React, HTML5, CSS3, and JavaScript. 
      My focus is on building performant, accessible, and scalable websites with a great user experience.
    </p>
  </section>

  <!-- Skills Section -->
  <section id="skills" class="bg-gray-50 py-12 fade-in">
    <div class="container mx-auto text-center">
      <h2 class="text-3xl font-semibold text-gray-900 mb-8">Skills</h2>
      <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-4 gap-8">
        <div class="skills-card p-6 bg-white rounded-lg shadow-lg hover:scale-110 transition-all duration-300">
          <h3 class="text-2xl font-semibold text-blue-600">HTML5</h3>
          <p class="mt-2 text-gray-700">Building the structure and foundation of web pages.</p>
        </div>
        <div class="skills-card p-6 bg-white rounded-lg shadow-lg hover:scale-110 transition-all duration-300">
          <h3 class="text-2xl font-semibold text-blue-600">CSS3</h3>
          <p class="mt-2 text-gray-700">Stylizing websites to look beautiful and responsive.</p>
        </div>
        <div class="skills-card p-6 bg-white rounded-lg shadow-lg hover:scale-110 transition-all duration-300">
          <h3 class="text-2xl font-semibold text-blue-600">JavaScript</h3>
          <p class="mt-2 text-gray-700">Making websites interactive and functional.</p>
        </div>
        <div class="skills-card p-6 bg-white rounded-lg shadow-lg hover:scale-110 transition-all duration-300">
          <h3 class="text-2xl font-semibold text-blue-600">React</h3>
          <p class="mt-2 text-gray-700">Building modern, efficient, and scalable web apps.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Experience Section -->
  <section id="experience" class="container mx-auto py-12 text-center fade-in">
    <h2 class="text-3xl font-semibold text-gray-900 mb-8">Experience</h2>
    <div class="space-y-6">
      <div class="bg-white p-6 rounded-lg shadow-lg">
        <h3 class="text-2xl font-semibold text-gray-800">Frontend Developer - ABC Web Solutions</h3>
        <p class="text-gray-600 italic">June 2024 - Present</p>
        <ul class="list-disc pl-6 mt-4 text-gray-700">
          <li>Developed responsive and dynamic web applications using React and Redux.</li>
          <li>Optimized performance to ensure faster load times and smooth transitions.</li>
          <li>Collaborated with backend teams to integrate APIs seamlessly into the frontend.</li>
        </ul>
      </div>
      <div class="bg-white p-6 rounded-lg shadow-lg">
        <h3 class="text-2xl font-semibold text-gray-800">Junior Frontend Developer - XYZ Digital Studio</h3>
        <p class="text-gray-600 italic">Jan 2023 - May 2024</p>
        <ul class="list-disc pl-6 mt-4 text-gray-700">
          <li>Designed and developed websites with a mobile-first approach.</li>
          <li>Worked with modern tools like Sass and Webpack to optimize the workflow.</li>
          <li>Collaborated with the UI/UX team to bring designs to life with pixel-perfect accuracy.</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects" class="container mx-auto py-12 text-center fade-in">
    <h2 class="text-3xl font-semibold text-gray-900 mb-8">Projects</h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
      <div class="project-card bg-white p-6 rounded-lg shadow-lg hover:scale-110 transition-all duration-300">
        <h3 class="text-2xl font-semibold text-blue-600">Personal Portfolio</h3>
        <p class="mt-2 text-gray-700">A website to showcase my skills and projects. Built with React and Tailwind CSS.</p>
      </div>
      <div class="project-card bg-white p-6 rounded-lg shadow-lg hover:scale-110 transition-all duration-300">
        <h3 class="text-2xl font-semibold text-blue-600">Weather App</h3>
        <p class="mt-2 text-gray-700">Weather forecasting app using the OpenWeather API. Built with React and styled-components.</p>
      </div>
      <div class="project-card bg-white p-6 rounded-lg shadow-lg hover:scale-110 transition-all duration-300">
        <h3 class="text-2xl font-semibold text-blue-600">E-commerce Store</h3>
        <p class="mt-2 text-gray-700">A mock e-commerce site built with React, Redux, and Stripe for payments.</p>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="text-white">
    <div class="footer-content">
      <p>&copy; 2025 sugam. All rights reserved.</p>
      <p class="text-gray-400 text-sm">Made with 💙 using Tailwind CSS</p>
    </div>
  </footer>

</body>

</html>
