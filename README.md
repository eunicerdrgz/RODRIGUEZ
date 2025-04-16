<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Portfolio Website</title>
  <!-- Font Awesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background-color: #f4e3ff;
    }

    .nav-buttons {
      display: flex;
      justify-content: center;
      gap: 30px;
      padding: 15px 0;
      background-color: #D182B3;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 100;
    }

    .nav-button {
      background-color: #F1A7C3;
      color: white;
      border: none;
      padding: 10px 20px;
      font-size: 16px;
      border-radius: 5px;
      cursor: pointer;
      text-decoration: none;
    }

    .nav-button:hover {
      background-color: #D182B3;
    }

    .section {
      display: none;
      padding: 120px 20px 40px;
      text-align: center;
      min-height: 100vh;
    }

    .active {
      display: block;
    }

    .profile-img {
      width: 250px;
      height: 250px;
      border-radius: 50%;
      border: 5px solid white;
      margin-bottom: 20px;
    }

    .edu-photo {  
      width: 500px;
      height: auto;
      display: block;
      margin: 20px auto;
      border-radius: 10px;
    }
 

    .social-icons {
      display: flex;
      justify-content: center;
      gap: 25px;
      margin-top: 20px;
    }

    .social-icons a {
      font-size: 24px;
      color: #333;
      text-decoration: none;
      transition: color 0.3s;
    }

    .social-icons a:hover {
      color: #007bff;
    }

    .typing-text {
      display: inline-block;
      border-right: 2px solid black;
      padding-right: 5px;
      white-space: nowrap;
      overflow: hidden;
      animation: typing 2s steps(30, end), blink 0.75s step-end infinite;
    }

    @keyframes typing {
      from { width: 0; }
      to { width: 22ch; }
    }

    @keyframes blink {
      50% { border-color: transparent; }
    }

    .education-box {
      background-color: #e6d6f3;
      color: black;
      padding: 20px;
      border-radius: 10px;
      width: fit-content;
      margin: 0 auto;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    .me-img {
      width: 300px;
      height: auto;
      display: block;
      margin: 20px auto;
      border-radius: 10px;
    }   


  </style>
</head>

<body>

  <div class="nav-buttons">
    <button class="nav-button" onclick="showSection('home')">Home</button>
    <button class="nav-button" onclick="showSection('education')">Education</button>
    <button class="nav-button" onclick="showSection('about')">About Me</button>
    <button class="nav-button" onclick="showSection('contact')">Contact</button>
  </div>

  <section id="home" class="section active">
    <img src="image.jpg" alt="Personal Photo" class="profile-img" />
    <h1>Hello, it's <span>Eunice</span></h1>
    <h3 class="typing-text">Hello! Welcome to my personal website.</h3>
    <div class="social-icons">
      <a href="mailto:eunice.rodriguez0430@gmail.com"><i class="fa-solid fa-envelope"></i></a>
      <a href="https://www.facebook.com/share/1BpYRNrsa3/" target="_blank">
      <i class="#"><i class="fa-brands fa-facebook"></i>
      </a>      
      <a href=https://www.instagram.com/eunice_rdrgz/" target="_blank">
      <i class="#"><i class="fa-brands fa-instagram"></i>
      </a>

    </div>
  </section>

  <section id="education" class="section">
    <h2>Education</h2>
    <img src="education.png" alt="School Photo" class="edu-photo" />
    <div class="education-box">
    <h1>Our Lady of the Pillar Catholic School, Inc. </h1>
    <p>F. Tirona Street, Poblacion II-A, City of Imus, Cavite </p>
    <p>Nursery (2008 - 2009) <br>
       Kinder (2009 - 2010) <br>
       Preparatory (2010 - 2011) <br>
       Elementary (2011 - 2017) <br>
       Junior High School (2017 - 2021) <br>
       Senior High School (2021 - 2023) </p>
    </div>
   <img src="education 2.jpeg" alt="School Photo 2" class="edu-photo" />
    <div class="education-box">
    <h1>Imus Institute of Science and Technology, Inc. </h1> 
    <p>82 Nueno Avenue, City of Imus, Cavite  </p>
    <p>College (2023 - Present)</p>
    </div>

  </section>

  <section id="about" class="section">
    <h2>About Me</h2>
    <img src="image 2.jpeg" alt="Personal Photo 2" class="me-img" />
    <div style="width: 60%; margin: 0 auto; text-align: left;">
    <div class="education-box">
    <p>Name: Rodriguez, Eunice Valencia <br>
       Age: 20 years old <br>
       Birthday: April 30, 2004 <br>
       Gender: Female <br>
       Dream: To be a Certified Public Accountant <br>
       Favorite Color: Purple <br>
       Favorite Artist/Band: BTS <br>
       Favorite Song: Mikrokosmos and Zero O’Clock by BTS <br>
       Favorite Series: 18 Again, Still 17, and Reply 1988 <br>
       Hobbies: Listening to music, watching k-dramas, and sleeping <br>
       Favorite Bible Verse: <br>
       “For I know the plans I have for you, plans to prosper you and <br>
       not to harm you, plans to give you hope and a future.” <br>
       - Jeremiah 29:11 <br>
       Achievements:</p>
    </div>
  </section>

  <section id="contact" class="section">
    <h2>Contact</h2>
    <div style="width: 60%; margin: 0 auto; text-align: left;">
    <div class="education-box">
    <p>Email me at eunice.rodriguez0430@gmail.com</p>
    <p>Facebook: Eunice Rodriguez </p>
   </div>
  </section>

  <script>
    function showSection(sectionId) {
      const sections = document.querySelectorAll('.section');
      sections.forEach(section => {
        section.classList.remove('active');
      });
      document.getElementById(sectionId).classList.add('active');
    }
  </script>

</body>
</html>
