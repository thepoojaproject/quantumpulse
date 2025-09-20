<!--

  Quantum Academy - Single-file HTML template

  Replace images, text, phone/email, and any links as needed.

  - Save as index.html and host on any static host (Netlify, Vercel, GitHub Pages)

  - For backend features (payments, contact form processing, student dashboard) you'll need server code.

-->



<!doctype html>

<html lang="en">

<head>

  <meta charset="utf-8" />

  <meta name="viewport" content="width=device-width,initial-scale=1" />

  <title>Quantum Pulse Academy</title>

  <meta name="description" content="Coaching for Science & Maths | JEE & NEET | Online & Offline Classes" />

  <link rel="icon" href="data:;base64,iVBORw0KGgo=" />

  <style>

    /* Simple modern reset + utility classes */

    :root{--accent:#0b6e99;--dark:#0f1723;--muted:#64748b;--card:#ffffff}

    *{box-sizing:border-box}html,body{height:100%;margin:0;font-family:Inter,ui-sans-serif,system-ui,-apple-system,'Segoe UI',Roboto,'Helvetica Neue',Arial}

    body{background:#f6fafc;color:var(--dark);-webkit-font-smoothing:antialiased}

    .container{max-width:1100px;margin:0 auto;padding:28px}

    header{background:linear-gradient(90deg,#ffffff, #f3fbff);position:sticky;top:0;z-index:50;border-bottom:1px solid #e6eef6}

    .nav{display:flex;align-items:center;justify-content:space-between;padding:18px 0}

    .brand{display:flex;gap:12px;align-items:center}

    .logo{width:48px;height:48px;background:var(--accent);border-radius:8px;color:white;display:grid;place-items:center;font-weight:700}

    nav ul{display:flex;gap:18px;list-style:none;margin:0;padding:0}

    a{color:inherit;text-decoration:none}

    .btn{background:var(--accent);color:#fff;padding:10px 14px;border-radius:8px;border:0;cursor:pointer}

    .hero{display:grid;grid-template-columns:1fr 420px;gap:28px;align-items:center;padding:36px 0}

    .hero h1{font-size:32px;margin:0 0 12px}

    .hero p{color:var(--muted);margin:0 0 18px}

    .card{background:var(--card);border-radius:12px;padding:18px;box-shadow:0 6px 18px rgba(11,110,153,0.06)}

    .features{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:18px}

    .feature{padding:12px;border-radius:10px;border:1px solid #eef6fb}

    section{padding:44px 0}

    h2{margin:0 0 14px}

    .courses{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}

    .course{padding:16px;border-radius:12px;background:#fff;border:1px solid #eef6fb}

    .faculty-list{display:flex;gap:12px;flex-wrap:wrap}

    .teacher{width:140px;text-align:center}

    .teacher img{width:100%;height:140px;object-fit:cover;border-radius:10px}

    .testimonials{display:flex;gap:12px;overflow:hidden}

    .testimonial{min-width:280px;padding:14px;border-radius:10px;background:#fff;border:1px solid #eef6fb}

    form{display:grid;gap:10px}

    input,textarea,select{padding:10px;border-radius:8px;border:1px solid #dbe8f2}

    footer{padding:28px 0;color:var(--muted);border-top:1px solid #e6eef6}

    @media(max-width:900px){.hero{grid-template-columns:1fr;}.features{grid-template-columns:1fr 1fr}.courses{grid-template-columns:1fr 1fr}.teacher{width:120px}}

    @media(max-width:600px){.features{grid-template-columns:1fr}.courses{grid-template-columns:1fr}.nav ul{display:none}}

  </style>

</head>

<body>

  <header>

    <div class="container nav">

      <div class="brand">

        <div class="logo">QP</div>

        <div>

          <div style="font-weight:700">Quantum Pulse Academy</div>

          <div style="font-size:12px;color:var(--muted)">Science • Maths • JEE & NEET</div>

        </div>

      </div>

      <nav>

        <ul>

          <li><a href="#courses">Courses</a></li>

          <li><a href="#faculty">Faculty</a></li>

          <li><a href="#testimonials">Results</a></li>

          <li><a href="#contact">Contact</a></li>

        </ul>

      </nav>

      <div style="display:flex;gap:10px;align-items:center">

        <a class="btn" href="#enroll">Enroll</a>

      </div>

    </div>

  </header>



  <main class="container">

    <section class="hero">

      <div>

        <h1>Concept‑based learning for Class 9‑12 — JEE & NEET coaching</h1>

        <p>Live online & offline classes, weekly tests, doubt sessions and personalised mentoring to help students reach top results.</p>



        <div class="card">

          <strong>Admissions open — Limited seats</strong>

          <div class="features" style="margin-top:12px">

            <div class="feature"><strong>Live Classes</strong><div style="font-size:13px;color:var(--muted)">Interactive doubt clearing</div></div>

            <div class="feature"><strong>Mock Tests</strong><div style="font-size:13px;color:var(--muted)">Weekly & full syllabus</div></div>

            <div class="feature"><strong>One‑on‑one</strong><div style="font-size:13px;color:var(--muted)">Personal mentors</div></div>

          </div>



          <div style="display:flex;gap:12px;margin-top:14px">

            <a class="btn" href="#contact">Get Free Counselling</a>

            <a style="padding:10px 14px;border-radius:8px;border:1px solid #dbe8f2;background:transparent;text-decoration:none;display:inline-block" href="#courses">View Courses</a>

          </div>

        </div>



      </div>



      <aside>

        <div class="card">

          <h3 style="margin-top:0">Quick Enquiry</h3>

          <form id="enquiryForm">

            <input type="text" name="name" placeholder="Your name" required />

            <input type="tel" name="phone" placeholder="Phone number" required />

            <select name="classlevel">

              <option value="class9">Class 9</option>

              <option value="class10">Class 10</option>

              <option value="class11">Class 11</option>

              <option value="class12">Class 12</option>

            </select>

            <button class="btn" type="submit">Request Callback</button>

            <div id="enqMsg" style="font-size:13px;color:green;display:none;margin-top:8px">Thanks! We'll contact you soon.</div>

          </form>

        </div>



        <div style="margin-top:14px" class="card">

          <strong>Contact</strong>

          <div style="font-size:13px;color:var(--muted);margin-top:8px">386‑R, Idgah Road, Model Town, Panipat</div>

          <div style="margin-top:6px">Phone: <a href="tel:+919996671724">+91 9996671724</a></div>

          <div>Email: <a href="mailto:quantumpulseacademy@gmail.com">quantumpulseacademy@gmail.com</a></div>

        </div>

      </aside>

    </section>



    <section id="courses">

      <h2>Our Courses</h2>

      <p style="color:var(--muted);margin-top:6px">Choose classroom or online programmes — tailored batches for boards, JEE & NEET.</p>



      <div class="courses" style="margin-top:14px">

        <article class="course">

          <h3>JEE Foundation (Class 11)</h3>

          <p style="color:var(--muted);font-size:14px">Concepts + problem solving, 5 days/week, weekly tests.</p>

          <div style="margin-top:10px;font-weight:700">₹8,000 / month</div>

        </article>



        <article class="course">

          <h3>NEET Revision (Class 12)</h3>

          <p style="color:var(--muted);font-size:14px">Crash course with full syllabus mocks.</p>

          <div style="margin-top:10px;font-weight:700">₹10,000 / month</div>

        </article>



        <article class="course">

          <h3>School Board Booster</h3>

          <p style="color:var(--muted);font-size:14px">Chapter‑wise classes, NCERT focus and board practice papers.</p>

          <div style="margin-top:10px;font-weight:700">₹3,500 / month</div>

        </article>

      </div>

    </section>



    <section id="faculty">

      <h2>Faculty</h2>

      <p style="color:var(--muted);margin-top:6px">Experienced faculty with competitive exam coaching background.</p>

      <div class="faculty-list" style="margin-top:12px">

        <div class="teacher card">

          <img src="https://via.placeholder.com/280x140.png?text=Teacher+1" alt="Teacher 1" />

          <div style="font-weight:700;margin-top:8px">Mr. R. Sharma</div>

          <div style="font-size:13px;color:var(--muted)">Physics Lead</div>

        </div>

        <div class="teacher card">

          <img src="https://via.placeholder.com/280x140.png?text=Teacher+2" alt="Teacher 2" />

          <div style="font-weight:700;margin-top:8px">Ms. N. Kaur</div>

          <div style="font-size:13px;color:var(--muted)">Chemistry</div>

        </div>

        <div class="teacher card">

          <img src="https://via.placeholder.com/280x140.png?text=Teacher+3" alt="Teacher 3" />

          <div style="font-weight:700;margin-top:8px">Mr. A. Verma</div>

          <div style="font-size:13px;color:var(--muted)">Mathematics</div>

        </div>

      </div>

    </section>



    <section id="testimonials">

      <h2>Results & Testimonials</h2>

      <p style="color:var(--muted);margin-top:6px">Hear from our students — combined board toppers and successful JEE/NEET rankers.</p>



      <div class="testimonials" style="margin-top:12px" id="testiWrap">

        <div class="testimonial card">

          <strong>Student A</strong>

          <div style="font-size:13px;color:var(--muted);margin-top:6px">I improved my rank by 200 places after joining weekly mocks and doubt classes.</div>

        </div>

        <div class="testimonial card">

          <strong>Student B</strong>

          <div style="font-size:13px;color:var(--muted);margin-top:6px">Teachers explain concepts very clearly, I recommend them for board prep.</div>

        </div>

        <div class="testimonial card">

          <strong>Student C</strong>

          <div style="font-size:13px;color:var(--muted);margin-top:6px">Great mentorship and personal attention.</div>

        </div>

      </div>

    </section>



    <section id="contact">

      <h2>Contact & Visit</h2>

      <div style="display:grid;grid-template-columns:1fr 380px;gap:18px;margin-top:12px">

        <div class="card">

          <h3>Visit our centre</h3>

          <p style="color:var(--muted)">386‑R, Idgah Road, Model Town, Panipat</p>



          <h3 style="margin-top:16px">Quick Message</h3>

          <form id="contactForm">

            <input type="text" name="name" placeholder="Name" required />

            <input type="email" name="email" placeholder="Email" />

            <textarea name="message" rows="4" placeholder="How can we help?"></textarea>

            <button class="btn" type="submit">Send Message</button>

            <div id="contactMsg" style="font-size:13px;color:green;display:none;margin-top:8px">Message sent (demo only).</div>

          </form>

        </div>



        <aside class="card">

          <h3>Timing</h3>

          <div style="color:var(--muted)">Mon–Sat: 9:00 AM — 7:00 PM</div>



          <h3 style="margin-top:12px">Follow</h3>

          <div style="display:flex;gap:8px;margin-top:8px"><a href="#">Facebook</a><a href="#">Instagram</a><a href="#">YouTube</a></div>

        </aside>

      </div>

    </section>

  </main>



  <footer>

    <div class="container" style="display:flex;justify-content:space-between;align-items:center;gap:12px;flex-wrap:wrap">

      <div style="font-weight:700">Quantum Pulse Academy</div>

      <div style="color:var(--muted);font-size:13px">© <span id="yr"></span> All rights reserved</div>

    </div>

  </footer>



  <script>

    // small interactions: demo forms and testimonial slider

    document.getElementById('yr').textContent = new Date().getFullYear();



    document.getElementById('enquiryForm').addEventListener('submit',function(e){

      e.preventDefault(); document.getElementById('enqMsg').style.display='block';

      setTimeout(()=>document.getElementById('enqMsg').style.display='none',3000);

      this.reset();

    });



    document.getElementById('contactForm').addEventListener('submit',function(e){

      e.preventDefault(); document.getElementById('contactMsg').style.display='block';

      setTimeout(()=>document.getElementById('contactMsg').style.display='none',3000);

      this.reset();

    });



    // simple auto-scroll testimonials

    (function(){

      const wrap = document.getElementById('testiWrap');

      let pos = 0; setInterval(()=>{

        pos += 1; if(pos>wrap.children.length-1) pos = 0;

        wrap.style.transform = `translateX(-${pos * (wrap.children[0].offsetWidth + 12)}px)`;

      },3500);

    })();

  </script>

</body>

</html># quantumpulse
For Trail Version
