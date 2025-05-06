<!DOCTYPE html>
<html>
<head>
    <title>ISTDII</title>
    <meta charset='utf-8'>
    <meta http-equiv='X-UA-Compatible' content='IE=edge'>
    <meta name='viewport' content='width=device-width, initial-scale=1'>
    <style>
        body{
            background-image: url("c:\Users\k_sam\Downloads\ISTDII OFFICIAL LOGO 2024-25.jpg");
            color: rgb(177, 240, 240);
            border-style: groove;
        }
        * {
            background-color: black;
            margin: 1;
            padding: 0;
            box-sizing: border-box;
        }

        .box {
            text-align: center;
            margin-top: 1%;
            position: relative;
        }

        .box button {
            color: rgb(0, 0, 0);
            border: 2px solid rgb(0, 195, 255);
            border-radius: 7px;
            padding: 10px 20px;
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            font-size: 14px;
            background: rgb(0, 195, 255);
            cursor: pointer;
            position: relative;
            overflow: hidden;
            transition: background 0.3s ease-in-out, color 0.3s ease-in-out, border-color 0.3s ease-in-out;
        }

        .box button:hover {
            background: transparent;
            color: white;
            border-color: white;
            box-shadow: 0 0 15px rgb(0, 194, 253);
        }

        /* Diamond Shape Stars */
        .stars {
            position: absolute;
            width: 6px;
            height: 6px;
            background-color: white;
            transform: rotate(45deg);
            box-shadow: 0 0 10px white;
            opacity: 1;
            transition: transform 0.5s ease-out, opacity 0.5s ease-in-out;
        }

        .stars.large {
            width: 10px;
            height: 10px;
        }
        h1{
            text-align: center;
        }
        h4{
            text-align: center;
                        }
                        .A1{
                            color: azure;
                            text-align: center;
                            font-size: medium;
                        }
                        .tab-container {
                            display: flex; /* Enable flex container */
                            list-style: none; /* Remove default list styling if using <ul> */
                            padding: 0;
                            margin: 0;
                        }

                        .tab-container li a { /* If using <li> elements */
                            display: block; /* Make the anchor fill the list item */
                            padding: 10px 15px;
                            text-decoration: none;
                            background-color: #f0f0f0;
                            border: 1px solid #ccc;
                            margin-right: 5px;
                        }

                        .tab-container li:last-child a {
                            margin-right: 0;
                        }

                        /* If not using <li>, target the direct children (e.g., <a>) */
                        .tab-container > a {
                            padding: 10px 15px;
                            text-decoration: none;
                            background-color: #f0f0f0;
                            border: 1px solid #ccc;
                            margin-right: 5px;
                        }

                        .tab-container > a:last-child {
                            margin-right:15%;
                        }
                        img{
                            display: block;
                            margin-left: auto;
                            margin-right: auto;
                        }
    </style>

</head>
<body>

    <h2>Content from MAIN PAGE</h2>
    <div class="box""tab-container">
        <button id="glowButton"><a href="ISTDII.html">HOME</a></button>
        <button id="glowButton"><a href="KNOW ABOUT ASTRONOMY.html">ABOUT ASTRONOMY</a></button>
        <button id="glowButton"><a href="ABOUT us.html">ABOUT US</a></button>
    </div>
    <h1>INTER SPACE TECHNOLOGY DEVELOPING INSTITUTE OF INDIA</h1>
    <h4>The Secret of sucess</h4>
    <p class="A1">ASTRONOMY IS NOT A WAY TO GET MONEY.  IT IS A Ambition AND FITURE OF MANY PEOPLE. IT IS NOT A STUDY IT IS THE STUDY.</p>
    <img src="c:\Users\k_sam\Downloads\ISTDII.html\Screenshot 2025-04-26 214055.png"
    class="ISTDIILOGO" width="350px" height="300px">
    <script>
        const button = document.getElementById("glowButton");
        let stars = [];

        button.addEventListener("mouseover", () => {
            removeStars();
            for (let i = 0; i < 5; i++) {
                let star = document.createElement("div");
                star.classList.add("stars");
                if (Math.random() > 0.5) star.classList.add("large");
                document.body.appendChild(star);

                let buttonRect = button.getBoundingClientRect();
                let startX = Math.random() * buttonRect.width + buttonRect.left;
                let startY = Math.random() * buttonRect.height + buttonRect.top;

                star.style.left = `${startX}px`;
                star.style.top = `${startY}px`;

                setTimeout(() => {
                    let angle = Math.random() * 2 * Math.PI;
                    let distance = Math.random() * 50 + 20;
                    let moveX = Math.cos(angle) * distance;
                    let moveY = Math.sin(angle) * distance;
                    star.style.transform = `rotate(45deg) translate(${moveX}px, ${moveY}px)`;
                    star.style.opacity = "1";
                }, 50);

                stars.push(star);
            }
        });

        button.addEventListener("mouseleave", () => {
            removeStars();
        });

        function removeStars() {
            stars.forEach(star => {
                star.style.opacity = "0";
                setTimeout(() => star.remove(), 500);
            });
            stars = [];
        }
    </script>

    <hr>
    <h2>Content from 2nd page</h2>
    <div class="box">
        <ul class="tab-container">
            <li><button id="glowButton"><a href="ISTDII.html">HOME</a></button></li>
            <li><button id="glowButton"><a href="KNOW ABOUT ASTRONOMY.html">ABOUT ASTRONOMY</a></button></li>
            <li><button id="glowButton"><a href="ABOUT us.html">ABOUT US</a></button></li>
        </ul>
    </div>
    <h1>KNOW ABOUT ASTRONOMY</h1>
    <h1>Current Affairs in Astronomy - April 26, 2025</h1>
    <p>The field of astronomy is dynamic, with new discoveries, ongoing missions, and celestial events constantly unfolding. As of April 26, 2025, several noteworthy developments and observations are capturing the attention of astronomers and space enthusiasts alike.</p>

    <h2>Missions and Spacecraft Activities</h2>
    <p>Several space missions are actively contributing to our understanding of the cosmos:</p>
    <ul>
        <li><b>Lucy Mission's Asteroid Encounter</b>: NASA's Lucy spacecraft, en route to study the Jupiter Trojan asteroids, recently made a close-up observation of a peculiar asteroid named Donaldjohanson. This asteroid, previously thought to be a contact binary (two asteroids touching each other) due to its variable brightness, was surprisingly found to have a connecting bridge between its two components. This flyby provided valuable images and data, showcasing the spacecraft's capabilities and offering insights into the formation of objects in the early solar system. The Lucy mission is expected to reach its primary target, the Trojan asteroid Eurybates, in August 2027.</li>
        <li><b>Hubble Space Telescope's </b>Anniversary: The iconic Hubble Space Telescope (HST) celebrated its 35th year since its launch. Despite initial challenges with its optics, which were famously corrected in a daring space mission, Hubble has revolutionized our understanding of the universe. It has delivered breathtaking images and crucial scientific data across various astronomical fields, from the solar system to the most distant galaxies. NASA has released online galleries and videos highlighting Hubble's significant contributions over the past three and a half decades.</li>
        <li><b>TRACERS Mission Launch</b>: Earlier in April, a SpaceX Falcon 9 rocket launched NASA's TRACERS (Tandem Reconnection and Cusp Electrodynamics Reconnaissance Satellites) mission. This mission involves two twin satellites orbiting Earth to study magnetic reconnection, a process where magnetic fields from the Sun interact with Earth's magnetic field, causing space weather phenomena. The data gathered by TRACERS will help scientists better understand and prepare for the impacts of solar activity on Earth.</li>
        <li><b>Lucy's Flyby of Donaldjohanson</b>: On April 20, 2025, NASA’s Lucy spacecraft executed a flyby of the main belt asteroid 52246 Donaldjohanson. This flyby served as a crucial test for the spacecraft’s systems and provided the second close-up view of an asteroid during its 12-year journey to the Jupiter Trojan asteroids. The data collected will help refine our understanding of these early solar system remnants.</li>
        <li><b>Soyuz MS-26 Crew Return</b>: On April 19, 2025, the Soyuz MS-26 spacecraft carrying NASA astronaut Don Petitt and Roscosmos cosmonauts Aleksey Ovchinin and Ivan Vagner returned to Earth, landing safely in Kazakhstan. This marked the end of their Expedition 72 mission on the International Space Station (ISS).</li>
        <li><b>SpaceX Fram2 Mission</b>: At the beginning of April, SpaceX launched its Fram2 mission, a four-person crewed flight aboard a Crew Dragon capsule. This mission focused on observing Earth's polar regions, studying the impact of spaceflight on the human body, and capturing the first human X-ray images in space.</li>
        <li><b>Soyuz Mission to ISS</b>: On April 8, 2025, a Russian Soyuz rocket launched NASA astronaut Jonathan Kim alongside Russian cosmonauts Sergey Ryzhikov and Aleksey Zubritsky to the ISS for an extended eight-month stay. They will be conducting scientific research and maintaining the orbiting laboratory.</li>
        <li><b>ULA's Vulcan Centaur Launch</b>: United Launch Alliance (ULA) is expected to launch its new Vulcan Centaur rocket for the first time in April 2025. This launch will carry the first batch of Project Kuiper megaconstellation internet satellites for the U.S. Space Force. The Vulcan Centaur is the successor to ULA's Atlas V rocket.</li>
    </ul>

    <h2>Astronomical Discoveries and Research</h2>
    <p>Recent research and observations have yielded interesting findings:</p>
    <ul>
        <li><b>Super-Earth Exoplanet Prevalence</b>: Astronomers have discovered evidence suggesting that super-Earth exoplanets, which are more massive than Earth but smaller than Neptune, might be more common across the universe than previously estimated. While planets orbiting close to their stars are easier to detect, new methods are helping to identify those with wider orbits, indicating a potentially vast population of these worlds.</li>
        <li><b>James Webb Space Telescope's Solar System Origins Research</b>: The James Webb Space Telescope (JWST) has been used to analyze Trans-Neptunian Objects (TNOs), icy bodies beyond Neptune, revealing varying traces of methanol. These findings are contributing to a better understanding of the origins and evolution of our solar system.</li>
        <li><b>Disintegrating Exoplanet with Comet-like Tail</b>: Astronomers have observed a planet approximately 140 light-years away that is rapidly disintegrating due to its close proximity to its host star. This process is creating a comet-like tail of debris as the planet evaporates under the intense stellar radiation.</li>
        <li><b>Insights into Stellar-Mass Black Hole Plasma Jets</b>: Scientists have made progress in understanding the conditions necessary for stellar-mass black holes to emit powerful plasma jets. Their research indicates that rapid shrinkage of superheated gas material towards the black hole is a key factor in the generation of these energetic outflows.</li>
        <li><b>Curiosity Rover's Carbon Deposits on Mars</b>: NASA's Curiosity rover has found evidence of significant carbon deposits on ancient Mars, suggesting the presence of a carbon cycle in the planet's past. This discovery has implications for the potential for past life on Mars.</li>
        <li><b>Visible Tunable Filtergraph (VTF) on the Inouye Solar Telescope</b>: The Daniel K. Inouye Solar Telescope in Hawaii has received a major upgrade with the installation of the Visible Tunable Filtergraph (VTF). After 15 years of development, this new instrument is now producing unprecedentedly detailed images of the Sun. The first images reveal features with a resolution of about 10 kilometers per pixel, offering a new window into solar activity.</li>
    </ul>

    <h2>Celestial Events</h2>
    <p>April 2025 has also featured several notable celestial events:</p>
    <ul>
        <li><b>Lyrid Meteor Shower Peak</b>: The Lyrid meteor shower, one of the oldest recorded meteor showers, reached its peak around April 22-23. Under favorable dark sky conditions, observers could spot around 15-20 meteors per hour. This year, a waxing crescent moon set early, providing good viewing conditions.</li>
        <li><b>Venus at its Brightest</b>: Venus reached its maximum brightness in the early morning sky around April 24. As the closest planet to Earth, and covered in highly reflective clouds, Venus appears as the brightest object in the sky after the Sun and the Moon.</li>
        <li><b>Pink Moon</b>: The full moon in April, known as the Pink Moon, occurred on April 12. Despite its name, the moon does not appear pink; the name originates from pink wildflowers that bloom in early spring. This Pink Moon also coincided with Easter and was a micromoon, appearing slightly smaller and less bright than an average full moon.</li>
        <li><b>Lunar Occultation of the Pleiades</b>: On April 1st, the Moon passed in front of the Pleiades star cluster, an event known as a lunar occultation. While the Moon and the star cluster appear close in the sky, they are vastly different in distance.</li>
        <li><b>Planetary Alignments and Conjunctions</b>: Throughout April, there have been several close approaches and alignments of planets, including Mercury, Venus, Saturn, and Mars, offering interesting viewing opportunities for astronomers and skywatchers. For instance, a southern planetary alignment involving Venus, Saturn, Mercury, and Neptune occurred around April 17.</li>
    </ul>

    <h2>New Telescopes and Technology</h2>
    <p>Advancements in telescope technology continue to push the boundaries of astronomical observation:</p>
    <ul>
        <li><b>Visible Tunable Filtergraph (VTF) for the Inouye Solar Telescope</b>: As mentioned earlier, the installation of the VTF represents a significant technological leap in solar observation, allowing for the capture of extremely detailed images of the Sun's surface and atmosphere.</li>
        <li><b>SPHEREx Mission</b>: NASA's Spectro-Photometer for the History of the Universe, Epoch of Reionization and Ices Explorer (SPHEREx) mission, launched in March, has begun its work. This space telescope will conduct the first all-sky spectroscopic survey in the near-infrared, gathering data on hundreds of millions of galaxies to study the origins of the universe, galaxy formation, and the ingredients for life. The SPHEREx team was recently recognized at the New York Stock Exchange, highlighting the mission's significance.</li>
    </ul>

    <h2>Dr. K. Kasturirangan's Passing</h2>
    <p>The Indian space community mourned the loss of <b>Dr. K. Kasturirangan</b>, a distinguished astrophysicist and former Chairman of the Indian Space Research Organisation (ISRO), who passed away on April 25, 2025, at the age of 84. He played a pivotal role in the success of India's early space missions, including Chandrayaan-1, India's first lunar mission. His contributions extended beyond space science to national education policy.</p>

    <p>In summary, <i>April 2025</i> has been an active month in astronomy, marked by significant spacecraft encounters, intriguing research findings, captivating celestial events, and advancements in observational technology. These developments continue to deepen our understanding of the universe and our place within it.</p>

    <h1>Space Policy and International Collaboration</h1>
    <p>The landscape of space exploration and research is increasingly shaped by policy decisions and international partnerships:</p>
    <ul>
        <li><b>Artemis Program Updates</b>: NASA's Artemis program, aiming to return humans to the Moon, continues to make progress. Recent discussions have focused on the development of sustainable lunar infrastructure and the involvement of international partners, including the <i>European Space Agency (ESA)</i> and the Canadian Space Agency <i>(CSA)</i>, in future missions. The timeline for the crewed <i>Artemis III mission,</i> targeting a lunar south pole landing, remains a key point of discussion.</li>
        <li><b>International Space Station <i>(ISS)</i> Extension</b>
