<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Inter Space Technology Developing Institute of India</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet" />
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    .tab-navigation {
      display: flex;
      border-bottom: 1px solid rgba(255, 255, 255, 0.1);
      margin-bottom: 2rem;
    }
    .tab-link {
      padding: 0.75rem 1.5rem;
      cursor: pointer;
      transition: color 0.3s ease;
    }
    .tab-link.active {
      color: #63b3ed;
      border-bottom: 2px solid #63b3ed;
    }
    .tab-content {
      display: none;
      animation: fade-in 0.5s ease-in-out;
    }
    .tab-content.active {
      display: block;
    }
    @keyframes fade-in {
      from { opacity: 0; transform: translateY(-10px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body class="bg-black text-white font-inter">
  <header class="bg-gray-900 bg-opacity-90 sticky top-0 z-10 shadow-md">
    <div class="container mx-auto px-4 py-3 flex justify-between items-center">
      <a href="#" class="flex items-center text-xl font-semibold text-blue-400 hover:text-blue-300 transition duration-300">
        <span class="mr-2">ISTDII</span>
      </a>
    </div>
  </header>

  <main class="container mx-auto px-4 py-8">
    <nav class="tab-navigation">
      <a href="#" data-tab="home-page" class="tab-link active">Home</a>
      <a href="#" data-tab="about-astronomy-page" class="tab-link">About Astronomy</a>
      <a href="#" data-tab="about-us-page" class="tab-link">About Us</a>
    </nav>

    <div id="home-page" class="tab-content active mb-16">
      <h2 class="text-3xl font-semibold text-blue-400 mb-6 text-center animate-fade-in">Home Page</h2>
      <div class="text-center">
        <h1 class="text-4xl font-bold text-blue-400 mb-4 animate-pulse">INTER SPACE TECHNOLOGY DEVELOPING INSTITUTE OF INDIA</h1>
        <h4 class="text-lg text-gray-300 mb-6 animate-fade-in-down">The Secret of Success</h4>
        <p class="text-md text-gray-200 mb-8 animate-slide-in-left">ASTRONOMY IS NOT A WAY TO GET MONEY. IT IS AN AMBITION AND FUTURE OF MANY PEOPLE. IT IS NOT A STUDY, IT IS THE STUDY.</p>
      </div>
    </div>

    <div id="about-astronomy-page" class="tab-content mb-16">
      <h2 class="text-3xl font-semibold text-blue-400 mb-6 text-center animate-fade-in">About Astronomy Page</h2>
      <div class="text-gray-300 space-y-6 text-justify">
        <p><strong>Astronomy</strong> is the scientific study of celestial objects, space, and the universe as a whole. It seeks to understand phenomena beyond Earth's atmosphere, including stars, planets, comets, galaxies, and the cosmos.</p>
        <p>Astronomy dates back thousands of years. Ancient civilizations like the Babylonians, Greeks, Chinese, and Mayans studied the night sky, developed calendars, and made predictions based on celestial cycles.</p>
        <p><strong>Key Areas in Astronomy:</strong>
          <ul class="list-disc list-inside ml-4">
            <li><strong>Astrophysics</strong>: Physics of celestial bodies.</li>
            <li><strong>Cosmology</strong>: Study of the universe’s origin, evolution, and fate.</li>
            <li><strong>Planetary Science</strong>: Study of planets and their systems.</li>
            <li><strong>Stellar Astronomy</strong>: Understanding stars and their life cycles.</li>
            <li><strong>Exoplanet Research</strong>: Discovery of planets outside our solar system.</li>
          </ul>
        </p>
        <p><strong>Facts about Astronomy:</strong>
          <ul class="list-disc list-inside ml-4">
            <li>The light from the Sun takes about 8 minutes and 20 seconds to reach Earth.</li>
            <li>One day on Venus is longer than its year.</li>
            <li>Neutron stars are so dense that a teaspoon of their matter weighs around 6 billion tons.</li>
            <li>The observable universe is estimated to be about 93 billion light-years in diameter.</li>
            <li>There are more stars in the universe than grains of sand on all the beaches of Earth.</li>
            <li>Black holes warp space and time and nothing, not even light, can escape their gravitational pull.</li>
            <li>The Milky Way and Andromeda galaxies are on a collision course and will merge in about 4.5 billion years.</li>
            <li>The Hubble Space Telescope has helped identify over a million new galaxies.</li>
            <li>Jupiter’s moon Europa may harbor a subsurface ocean that could support life.</li>
          </ul>
        </p>
        <p><strong>Modern Astronomy</strong> uses tools like space telescopes, radio observatories, and deep-space probes to uncover the secrets of the cosmos. New frontiers include gravitational wave detection, quantum cosmology, and AI-driven simulations of cosmic evolution.</p>
        <p>Through constant exploration, astronomy helps us grasp our place in the universe, driving innovation and inspiring humanity to look beyond our planetary boundaries.</p>
      </div>
    </div>

    <div id="about-us-page" class="tab-content mb-16">
      <h2 class="text-3xl font-semibold text-blue-400 mb-6 text-center animate-fade-in">About Us Page</h2>
      <div class="text-gray-200 text-justify">
        <p><strong>ISTDII</strong> (<strong>Inter Space Technology Developing Institute of India</strong>) emerged on <strong>Teacher's Day in 2023</strong>, a testament to the dedication and collaborative spirit of its six founding members: <strong>A. Samantaray</strong>, <strong>A. Kamila</strong>, <strong>Adyasha.P. Paikeray</strong>, <strong>Ritesh.K. Jena</strong>, <strong>Sampad.S. Nayak</strong>, and <strong>Sai Krishna</strong>.</p>
        <p>Born from shared aspirations in the realm of space technology, the institute has navigated numerous challenges with resilience and determination.</p>
        <p>This close-knit group has forged a strong foundation, learning valuable lessons through their collective struggles. Their journey reflects a commitment to innovation and a persistent drive to push the boundaries of space technology development within India.</p>
        <p><strong>ISTDII's ethos</strong> is one of unwavering perseverance, with a vision that extends far into the future. Their initial hardships have only strengthened their resolve, solidifying their commitment to continuous growth and enduring impact in the field.</p>
        <p>The institute stands as a <strong>symbol of collaborative ambition</strong> and the <strong>power of facing adversity head-on</strong>, poised to contribute meaningfully to India's space endeavors for years to come.</p>
      </div>
    </div>
  </main>

  <script>
    document.querySelectorAll('.tab-link').forEach(link => {
      link.addEventListener('click', function (e) {
        e.preventDefault();

        document.querySelectorAll('.tab-link').forEach(tab => tab.classList.remove('active'));
        document.querySelectorAll('.tab-content').forEach(content => content.classList.remove('active'));

        this.classList.add('active');
        const target = this.getAttribute('data-tab');
        document.getElementById(target).classList.add('active');
      });
    });
  </script>
</body>
</html>
