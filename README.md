# Portfolio
This is my Portfolio
<br>
Author - Umairkhan
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <link rel="stylesheet" href="style.css" />
  <title>portfolio</title>
</head>
<body>
  <header>
    <div id="hd">
      <h1 id="header">
        <span class="typewriter-text"></span><span class="typed-cursor">|</span>
      </h1>
      <div class="typing-container">
        <span id="typing-subtext"></span><span class="typed-cursor">|</span>
      </div>
      <div id="pic"></div>
    </div>
  </header>

  <main>
    <div id="ab">
      <h2>About Me</h2>
      <p id="abp">
        Name: <strong><i><u>Umair Khan</u></i></strong> <br />
        DOB: <strong>20/1/2012 </strong><br />
        Location: <strong>Karnataka/Chintamani</strong> <br />
        Profession: <strong>student/coder</strong>
      </p>
    </div>

    <div id="esc">
      <h2>Education</h2>
      <p id="escp">
        Class: <strong>8th</strong> <br />
        Syllabus: <strong>NCERT <u>(like to read CBSE)</u></strong> <br />
        School: <strong>New Kiran School</strong>
      </p>
    </div>

    <div id="slkl">
      <h2>Skills</h2>
      <div class="skill-row">
        <div id="coding"><p id="UT0">coding</p></div>
        <div id="freelancing"><p id="UT1">freelancing</p></div>
        <div id="canva"><p id="UT2">canva editing</p></div>
        <div id="Ai"><p id="UT3"> Ai prompt Expert</p></div>
      </div>
    </div>

    <div id="pro">
      <h2>projects</h2>


    </div>
     <div id="langs">
      <h2>coding langs</h2>
<div id="html"><p id="html1">HTML</p></div>
<div id="css"><p id="css2">CSS</p></div>
<div id="js"><p id="js3">JS</p></div>

    </div>
  </main>

  <footer>
    <div class="footer-container">
      <h2>Contact Me</h2>
      <p>Send me a message directly from here!</p>
      <form action="https://formsubmit.co/umairkhan786ukz786@gmail.com" method="POST" class="contact-form">
        <input type="text" name="name" placeholder="Your Name" required />
        <input type="email" name="email" placeholder="Your Email" required />
        <textarea name="message" placeholder="Your Message" rows="5" required></textarea>
        <button type="submit">📧 Send Message</button>
      </form>
      <p class="copyright">&copy; 2025 Umair Khan | All rights reserved.</p>
    </div>
  </footer>

  <script>
    // Header typewriter
    const headerSpan = document.querySelector('.typewriter-text');
    const headerText = "Hello! I'm Umair Khan, a student and a web developer";
    let i = 0;

    function typeHeader() {
      if (i < headerText.length) {
        headerSpan.textContent += headerText.charAt(i);
        i++;
        setTimeout(typeHeader, 50);
      }
    }
    typeHeader();

    // Subheading typewriter
    const subText = document.getElementById("typing-subtext");
    const roles = [
      "● Tech Solutions Expert.",
      "● Coding & Design Expert.",
      "● Technology Consultant."
    ];
    let roleIndex = 0;
    let charIndex = 0;
    let isDeleting = false;

    function typeSubtext() {
      const currentRole = roles[roleIndex];
      if (isDeleting) {
        subText.textContent = currentRole.substring(0, charIndex--);
      } else {
        subText.textContent = currentRole.substring(0, charIndex++);
      }

      if (!isDeleting && charIndex === currentRole.length) {
        isDeleting = true;
        setTimeout(typeSubtext, 1000);
      } else if (isDeleting && charIndex === 0) {
        isDeleting = false;
        roleIndex = (roleIndex + 1) % roles.length;
        setTimeout(typeSubtext, 500);
      } else {
        setTimeout(typeSubtext, isDeleting ? 50 : 100);
      }
    }

    setTimeout(typeSubtext, 3000);
  </script>
</body>
</html>
                                  
                          <!-- developed by Umair khan -->
