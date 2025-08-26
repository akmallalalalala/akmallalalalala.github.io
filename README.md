<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Akmal — Portfolio</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body, html { font-family: Arial, sans-serif; height: 100%; scroll-behavior: smooth; }
    section { position: relative; min-height: 100vh; display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; padding: 2rem; }
    nav { position: fixed; top: 0; left: 0; width: 100%; background: rgba(0, 123, 255, 0.9); display: flex; justify-content: center; padding: 1rem; z-index: 1000; backdrop-filter: blur(5px); }
    nav a { color: white; text-decoration: none; margin: 0 1rem; font-size: 1rem; font-weight: bold; transition: color 0.3s ease; position: relative; }
    nav a:hover, nav a.active { color: #ffd700; }
    #about { background: url('gaming_pc1.jpg') no-repeat center center/cover; color: white; position: relative; }
    #about::after { content: ''; position: absolute; top: 0; left: 0; right: 0; bottom: 0; background: rgba(0,0,0,0.5); z-index: 1; }
    #about > * { position: relative; z-index: 2; }
    h1, h2, h3, p { margin: 1rem 0; }
    .fade { opacity: 0; transform: translateY(30px); transition: all 1s ease; }
    .fade.visible { opacity: 1; transform: translateY(0); }
    #hobbies { background: linear-gradient(to bottom, #a1c4fd, #c2e9fb); }
    #goals { background: linear-gradient(to bottom, #c2e9fb, #a1c4fd); }
    #achievements { background: linear-gradient(to bottom, #a1c4fd, #c2e9fb); }
    #projects { background: linear-gradient(to bottom, #c2e9fb, #a1c4fd); }
    #documents { background: linear-gradient(to bottom, #a1c4fd, #c2e9fb); }
    #journey { background: linear-gradient(to bottom, #c2e9fb, #fbc2eb); }
    #contact { background: linear-gradient(to bottom, #fbc2eb, #a1c4fd); }
    .gallery { display: flex; flex-wrap: wrap; gap: 1rem; justify-content: center; }
    .gallery figure { width: 300px; text-align: center; }
    .gallery img { width: 100%; height: 200px; object-fit: cover; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2); transition: transform 0.3s ease; }
    .gallery img:hover { transform: scale(1.05); }
    .btn { background: #007BFF; color: white; padding: 0.8rem 1.2rem; margin: 0.5rem; border: none; border-radius: 8px; cursor: pointer; font-size: 1rem; transition: background 0.3s ease; text-decoration: none; display: inline-flex; align-items: center; gap: 0.5rem; }
    .btn:hover { background: #0056b3; }
    .timeline { max-width: 800px; margin: auto; text-align: left; }
    .timeline div { margin: 1rem 0; }
    .skills { display: flex; justify-content: center; gap: 1.5rem; margin-top: 2rem; }
    .skill { background: white; padding: 1rem; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2); }
    .icon { width: 20px; height: 20px; display: inline-block; }
  </style>
</head>
<body>
  <nav>
    <a href="#about">About</a>
    <a href="#journey">Journey</a>
    <a href="#hobbies">Hobbies</a>
    <a href="#goals">Goals</a>
    <a href="#achievements">Achievements</a>
    <a href="#projects">Projects</a>
    <a href="#documents">Documents</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about">
    <h1 class="fade">Akmal</h1>
    <p class="fade">Future Business Leader | Former Aerospace Student | Entrepreneur</p>
    <p class="fade">I transitioned from aerospace engineering into entrepreneurship because I discovered my passion for business through hands-on ventures.</p>
  </section>

  <section id="journey">
    <h2 class="fade">My Journey</h2>
    <div class="timeline fade">
      <div><strong>2021 - 2024:</strong> Diploma in Aerospace Engineering. Started a side business that revealed my true passion for entrepreneurship.</div>
      <div><strong>2024 - 2025:</strong> Served National Service as a 3SG in SAF, developing leadership and discipline.</div>
      <div><strong>Present:</strong> Preparing to pursue a Business degree overseas, building on real-world entrepreneurial experience.</div>
    </div>
  </section>

  <section id="hobbies">
    <h2 class="fade">My Hobbies</h2>
    <p class="fade">I enjoy exploring creative outlets like fitness, photography, and traveling. These activities fuel my creativity and balance my business mindset.</p>
  </section>

  <section id="goals">
    <h2 class="fade">My Goals</h2>
    <p class="fade">To pursue a Business degree, expand entrepreneurial ventures, and inspire others to follow their passions.</p>
    <div class="skills fade">
      <div class="skill">Leadership</div>
      <div class="skill">Entrepreneurship</div>
      <div class="skill">Problem-Solving</div>
      <div class="skill">Innovation</div>
    </div>
  </section>

  <section id="achievements">
    <h2 class="fade">My Achievements</h2>
    <div class="fade">
      <h3>$40,000+</h3>
      <p>Total Sales</p>
      <h3>50+</h3>
      <p>Projects Shipped</p>
    </div>
    <p class="fade">Customer feedback: "Akmal is highly motivated and always delivers with quality and professionalism."</p>
  </section>

  <section id="projects">
    <h2 class="fade">Projects</h2>
    <div class="gallery fade">
      <figure>
        <img src="/mnt/data/rtx_3080__ryzen_9_9500x_gaming_1714333183_968d8000_progressive.jpg" alt="Gaming PC 1">
        <figcaption>Custom-built RTX 3080 & Ryzen 9 Gaming PC.</figcaption>
      </figure>
      <figure>
        <img src="/mnt/data/rtx_3080_gaming_pc_desktop_1740729790_e2325820_progressive.jpg" alt="Gaming PC 2">
        <figcaption>High-performance RGB gaming rig for esports.</figcaption>
      </figure>
      <figure>
        <img src="/mnt/data/highend_gaming_pc_desktop_rtx__1747133506_3bbbcd05_progressive.jpg" alt="Gaming PC 3">
        <figcaption>Premium gaming workstation showcasing RGB cooling.</figcaption>
      </figure>
    </div>
  </section>

  <section id="documents">
    <h2 class="fade">My Documents</h2>
    <a href="Akmal_CV.pdf" class="btn fade" download>Download CV</a>
    <a href="Motivation_Letter.pdf" class="btn fade" download>Download Motivation Letter</a>
  </section>

  <section id="contact">
    <h2 class="fade">Contact Me</h2>
    <p class="fade">Feel free to reach out to me via email or social media.</p>
    <a href="mailto:your-email@example.com" class="btn fade"><img src="email-icon.png" class="icon" alt="Email"> Email Me</a>
    <a href="https://www.linkedin.com/in/yourprofile" class="btn fade" target="_blank"><img src="linkedin-icon.png" class="icon" alt="LinkedIn"> LinkedIn</a>
    <a href="https://github.com/yourprofile" class="btn fade" target="_blank"><img src="github-icon.png" class="icon" alt="GitHub"> GitHub</a>
  </section>

  <script>
    const faders = document.querySelectorAll('.fade');
    const observer = new IntersectionObserver(entries => { entries.forEach(entry => { if (entry.isIntersecting) entry.target.classList.add('visible'); }); }, { threshold: 0.2 });
    faders.forEach(fader => observer.observe(fader));

    const sections = document.querySelectorAll('section');
    const navLinks = document.querySelectorAll('nav a');
    window.addEventListener('scroll', () => {
      let current = '';
      sections.forEach(section => {
        const sectionTop = section.offsetTop - 100;
        const sectionHeight = section.clientHeight;
        if (scrollY >= sectionTop && scrollY < sectionTop + sectionHeight) current = section.getAttribute('id');
      });
      navLinks.forEach(link => { link.classList.remove('active'); if (link.getAttribute('href') === '#' + current) link.classList.add('active'); });
    });
  </script>
</body>
</html>
