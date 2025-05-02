
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Praveen Shukla - Portfolio</title>
    <!-- AOS CSS -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.css" rel="stylesheet">
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <!-- Custom CSS -->
    <link rel="stylesheet" href="{{ url_for('static', filename='css/main.css') }}">
</head>

<script>
    document.addEventListener('keydown', function(event) {
        if (event.key === 'F12' || (event.ctrlKey && event.shiftKey && event.key === 'I')) {
            alert('DevTools is disabled!');
            event.preventDefault();
        }
    });

    // Disable right-click
    document.addEventListener('contextmenu', function(event) {
        event.preventDefault();
        alert("Right-click is disabled!");
    });

    // Disable Ctrl+U and F12 (DevTools)
    document.addEventListener('keydown', function(event) {
        if (event.ctrlKey && (event.key === 'u' || event.key === 'U')) {
            event.preventDefault();
            alert("Viewing source is disabled!");
        }
        if (event.key === 'F12') {
            event.preventDefault();
            alert("DevTools are disabled!");
        }
    });
</script>

<script src="https://cdnjs.cloudflare.com/ajax/libs/aos/2.3.4/aos.js"></script>

<script>
    document.addEventListener('DOMContentLoaded', function () {
        AOS.init();
    });
</script>

<body>
    <header class="fixed-header">
        <div class="container">
            <nav class="navbar navbar-expand-lg navbar-light">
                <div class="container-fluid px-0">
                    <!-- Updated AI/DS themed logo -->
                    <a class="navbar-brand logo-container" href="#">
                        <div class="logo-icon">
                            <i class="fas fa-robot"></i>
                            <i class="fas fa-chart-line"></i>
                        </div>
                        <div class="logo-text">
                            <span class="name">Praveen Shukla</span>
                        </div>
                    </a>

                    <button class="navbar-toggler collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                        <span class="navbar-toggler-icon"></span>
                    </button>
                    
                    <div class="collapse navbar-collapse" id="navbarNav">
                        <ul class="navbar-nav ms-auto">
                            <li class="nav-item">
                                <a class="nav-link" href="#about">About Me</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#education">Education</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#publications">Publications</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#experience">Experience</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#projects">Projects</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="#contact">Contact</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </nav>
        </div>
    </header>

    <div class="container main-container">
        <main>
            <!-- About Me Section -->
            <section id="about" class="section">
                <div class="row g-4">
                    <div class="col-lg-3 col-md-4">
                        <div class="profile-header">
                            <div class="profile-img-container">
                                <img src="{{ url_for('static', filename='img/profile.jpg') }}" alt="Praveen Shukla" class="profile-img">
                            </div>
                            <div class="profile-info">
                                <h2 class="name">Praveen Shukla</h2>
                                <div class="specialties">
                                    <p>Graph Deep Learning</p>
                                    <p>Data Distillation</p>
                                    <p>AI in Healthcare</p>
                                    <p>Spatial databases</p>
                                </div>
                                <div class="contact-info" style="margin-top: 10px;">
                                    <p>prashuiit@gmail.com</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-lg-9 col-md-8">
                        <h2 class="section-title">About me</h2>
                        <div class="section-content">
                            <p>I'm an undergraduate student in Data Science & Artificial Intelligence at IIT Madras with a strong passion for building intelligent systems that solve real-world problems. My current work lies at the intersection of graph deep learning, spatio-temporal analytics, data distillation, and efficient information retrieval. I'm also diving into the world of LLMs, prompt engineering, and agentic frameworks to explore the future of human-AI collaboration.</p>
                            <p>Outside of research, I enjoy decoding ancient science, listening to instrumental music, and working on hands-on tech projects—from AI-powered bots to intelligent web apps. Right now, I'm balancing my academic life with a bit of curiosity, caffeine, and code. :3</p>
                        </div>

                        <h2 class="section-title">Affiliations</h2>
                        <div class="section-content">
                            <div class="affiliation">
                                <h3>Indian Institute of Technology Madras</h3>
                                <p class="timeframe">Incoming May 2024 - Present | Chennai, TN, India</p>
                                <p class="position">Research Intern (under Dr. <a href="https://rbcdsai.iitm.ac.in/people/krishnan-balasubramanian/" class="researcher-link">Krishnan Balasubramanian</a>)- Center for Non Destructive Evaluation Lab (<a href="https://www.cnde.in/" class="researcher-link">CNDE Lab</a>)</p>
                            </div>
                            <div class="affiliation">
                                <h3>Indian Institute of Information Technology, Design and Manufacturing, Kancheepuram</h3>
                                <p class="timeframe">January 2025 - March 2025 | Kancheepuram, TN, INdia</p>
                                <p class="position">Research Intern (under Dr. <a href="https://www.leaplab-iiitdm.co.in/team" class="researcher-link">Uttam Mrinal Pal</a>)- Light Engineering and Applied Photonics Lab (LEAP Lab)</p>
                            </div>

                            <div class="affiliation">
                                <h3>Indian Institute of Remote Sensing - ISRO</h3>
                                <p class="timeframe">August 2021 - Present | Mumbai, MH, India</p>
                                <p class="position">Outreach Coordinator (under Zonal Org <a href="#" class="researcher-link">GLOBAL SCIENCE</a>) - Zonal Organization and External Engagements</p>
                            </div>

                            <div class="affiliation">
                                <h3>VIGYAN PRASAR, DST, Govt. of India</h3>
                                <p class="timeframe">February 2020 - November 2023 | Mumbai, MH, India</p>
                                <p class="position">Science Club Cooridnator (under <a href="https://www.indiascienceandtechnology.gov.in/listingpage/vigyan-prasar-completes-33-glorious-years-science-communication-popularisation-extension" class="researcher-link">VIPNET</a>)-  VIgyan Prasar NETwork (VIPNET) of Science Clubs in multiple science club.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Education Section -->
            <section id="education" class="section" data-aos="fade-up" data-aos-delay="100">
                <div class="row">
                    <div class="col-12">
                        <h2 class="section-title">Education</h2>
                        <div class="section-content">
                            <div class="row flex-column gap-4">
                                <div class="education" data-aos="fade-up" data-aos-delay="50">
                                    <h3>Indian Institute of Technology Madras</h3>
                                    <p class="timeframe">2024 - 2028 | Chennai, TN India</p>
                                    <p class="degree">Bachelors in Artificial Intelligence & Data Science</p>
                                </div>

                                <div class="education" data-aos="fade-up" data-aos-delay="100">
                                    <h3>M H High School & Jr College</h3>
                                    <p class="timeframe">2021 - 2023 | Mumbai, MH India</p>
                                    <p class="degree">Higher Secondary Education (MH State Board) | GPA: 8/10</p>
                                </div>

                                <div class="education" data-aos="fade-up" data-aos-delay="150">
                                    <h3>SMT. Shushiladevi Deshmukh Vidyalaya & Jr College</h3>
                                    <p class="timeframe">2014 - 2021 | Mumbai, MH India</p>
                                    <p class="degree">Secondary Education (MH State Board) | GPA: 9.1/10</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Publications Section -->
            <section id="publications" class="section">
                <div class="row">
                    <div class="col-12">
                        <h2 class="section-title">Publications</h2>
                        <div class="section-content">
                            <div class="row g-4">
                                <div class="publication">
                                    <h3><a href="#" class="publication-link">Bonsai: Gradient-free Graph Distillation for Node Classification</a></h3>
                                    <p class="authors">Mritul Gupta, Samyak Jain, Praveen Shukla , Hariprasad Kodamana and Sayan Ranu</p>
                                    <p class="venue">The Thirteenth International Conference on Learning Representations, 2025</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            <!-- Scholastic Achievements Section -->
            <section id="achievements" class="section" data-aos="fade-up" data-aos-delay="100">
                <div class="row">
                    <div class="col-12">
                        <h2 class="section-title">Scholastic Achievements</h2>
                        <div class="section-content">
                            <ul class="achievement-list">
                                <li>
                                    Pulse @ Techfest - IIT Bombay: Finalist in GenAI Buildathon
                                    <span class="timeframe"> - 2024</span>
                                </li>
                                <li>Co-discoverer of the Main Belt Asteroid 2020UJ37, named by the IAU's Minor Planet Center <span class="timeframe">- 2020</span>          </li>
                                <li>Among the top 20 in the AI Quiz on National Science Day (NSD-2022), conducted by Bhabha Atomic Research Center (BARC), Mumbai <span class="timeframe">- 2022</span></li>
                                <li>State topper in Mathematics in the Matriculation examination conducted by MSBSHSE, Pune. <span class="timeframe">- 2021</span> </li>
                                <li>Top performer in Weekly Quiz 2018–19 by MyGov, MeitY, Govt. of India <span class="timeframe">– 2018</span> </li>
                                <li>Awarded 1<sup>st</sup> Position in Youth Invention with a cash prize of ₹5,000, a certificate, and a medal <span class="timeframe">– 2020</span></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </section>


            <!-- Experience Section -->
            <section id="experience" class="section" data-aos="fade-up" data-aos-delay="100">
                <div class="row">
                    <div class="col-12">
                        <h2 class="section-title">Experience</h2>
                        <div class="section-content">
                            <div class="row row-cols-1 row-cols-md-2 g-4">
                                <div class="experience">
                                    <!-- Content will be based on the screenshots or additional information provided -->
                                    <div class="experience" data-aos="fade-up" data-aos-delay="150">
                                        <h3>Indian Institute of Information Technology, Design and Manufacturing, Kancheepuram</h3>
                                        <p class="timeframe">Jan 2025 - Mar 2025 | Kancheepuram, TN India</p>
                                        <p class="role"><strong>Research Intern</strong></p>
                                        <p class="details">Developed deep learning models for early detection and classification of Oral Potentially Malignant Disorders (OPMDs) using clinical image data. Conducted literature review, dataset preparation, and domain-specific annotation of lesions. Implemented YOLO-based object detection and CNN classifiers in PyTorch to identify high-risk conditions like leukoplakia, erythroplakia, OLP, OSF, and PVL. Enhanced model performance through targeted augmentation and lesion-specific feature engineering. Collaborated with clinical researchers to ensure diagnostic accuracy and translational impact in oral cancer screening.</p>
                                    </div>
                                    <div class="experience" data-aos="fade-up" data-aos-delay="200">
                                        <h3>Lumio AI</h3>
                                        <p class="timeframe">Oct 2024 - Nov 2024 | Mumbai, MH India</p>
                                        <p class="role"><strong>AI Engineer Intern</strong></p>
                                        <p class="details">Developed and optimized end-to-end AI solutions for real-time client projects, applying advanced deep learning techniques and algorithm fine-tuning. Integrated Retrieval-Augmented Generation (RAG) with large language models (LLMs) to elevate context-aware responses in AI systems. Led model experimentation, feature engineering, and evaluation, ensuring high performance and reliability. Collaborated across engineering and product teams to deliver AI-driven features aligned with business goals. Demonstrated expertise in artificial intelligence, strategic communication, and problem-solving in fast-paced, innovation-driven environments.</p>
                                    </div>
                                    <div class="experience" data-aos="fade-up" data-aos-delay="250">
                                        <h3>GLOBAL SCIENCE</h3>
                                        <p class="timeframe">Feb 2020 - Present | Mumbai, MH India</p>
                                        <p class="role"><strong>Founder & Director</strong></p>
                                        <p class="details">
                                            Started GLOBAL SCIENCE at the <span class="semi-bold">age of 12</span>, which later became affiliated with 
                                            <span class="semi-bold">Vigyan Prasar (DST, GoI)</span> as a nationally recognized science communication initiative. 
                                            Led NASA-funded asteroid discovery campaigns (19 finds), and organized India Techno Fest featuring experts from ISRO, IIT, and Meta. 
                                            Initiated impactful programs such as <em>Inspiring Young</em> and <em>Science at Home</em> (including virtual CERN tours), reaching over 50,000 students across India.<br><br>
                                            Built a network of 150+ district coordinators and 10 mentors from leading institutions. Spearheaded national science fairs, historical science series, and pandemic-era STEM outreach efforts to promote hands-on learning. 
                                            Recognized with the <span class="semi-bold">Award of Excellence</span> by Vigyan Prasar for two consecutive years (2020–21 and 2021–22) for contributions to science communication.
                                        </p>
                                    </div>
                                    <div class="experience" data-aos="fade-up" data-aos-delay="250">
                                        <h3>International Astronomical Search Collaboration (IASC)</h3>
                                        <p class="timeframe">October 2020 - November 2021 | Mumbai, MH India</p>
                                        <p class="role"><strong>Citizen Scientist</strong></p>
                                        <p class="details">Spearheaded the Saptarishi VIPNET 03 campaign as Team Leader, mentoring government school teachers across three Indian states in the discovery of 10 preliminary Main Belt asteroids. Elevated to National Mentor, where I successfully led and trained multiple teams of students and educators, achieving 19 preliminary asteroid discoveries under my guidance. Played a pivotal role in capacity-building through technical training on Astrometrica and MPC reporting, empowering grassroots citizen scientists to contribute to global astronomical research.</p>
                                    </div>        
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Projects Section -->
            <section id="projects" class="section">
                <div class="row">
                    <div class="col-12">
                        <h2 class="section-title">Projects</h2>
                        <div class="section-content">
                            <div class="row row-cols-1 row-cols-lg-2 g-4">
                                <div class="col">
                                    <div class="project">
                                        <h3>MolMerger: Molecular Solubility Prediction</h3>
                                        <p>Molecule approach. Implemented attention mechanisms with GNNs on graphs, achieving an R² score of 0.94 for aqueous solubility prediction. Designed MolMerger to represent solute-solvent pairs with virtual bonds, modeling molecular interactions. Achieved an R² of 0.787 and MAE of 0.78 on the test set, with an average MAE of 0.79 across 65 solvents. Performed SHAP analysis for explainability, identifying atom type, formal charge, and aromatic rings as key factors.</p>
                                        <p><a href="https://github.com/VanshRamani/MolMerger-Solubility-Prediction" class="project-link">https://github.com/VanshRamani/MolMerger-Solubility-Prediction</a></p>
                                    </div>
                                </div>
                                <div class="col">
                                    <div class="project">
                                        <h3>Comprehensive Deepfake Detection System</h3>
                                        <p>Developed a robust Deepfake detection model by optimizing two key components: an MTCNN-based frame-by-frame classifier with EfficientNet and a fact-checking approach that matches audio to visual features. Designed a streamlined pipeline combining both components using a weighted mean, achieving an award-winning 93% accuracy in Deepfake detection.</p>
                                        <p><a href="https://github.com/jdhruv1503/deepfake-detection" class="project-link">https://github.com/jdhruv1503/deepfake-detection</a></p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Contact Section -->
            <section id="contact" class="section">
                <div class="row">
                    <div class="col-12">
                        <h2 class="section-title">Contact</h2>
                        <div class="section-content">
                            <div class="d-flex gap-3">
                                <p><a href="https://www.linkedin.com/in/praveen-ashukla/" class="contact-link">LinkedIn</a></p>
                                <p><a href="mailto:prashuiit@gmail.com" class="contact-link">Email</a></p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </main>
    </div>

    <!-- Wave Divider -->
    <div style="height: 30px; overflow: hidden;">
        <svg viewBox="0 0 500 150" preserveAspectRatio="none" style="height: 100%; width: 100%;">
            <path d="M0.00,49.98 C150.00,150.00 349.00,-49.98 500.00,49.98 L500.00,150.00 L0.00,150.00 Z"
                style="stroke: none; fill: #1f2e3c;"></path>
        </svg>
    </div>

    <!-- Footer Section -->
    <footer style="background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);" class="text-white pt-4 pb-3">
        <div class="container text-center text-md-start">
            <div class="row">
                <!-- Left Section -->
                <div class="col-md-6 mb-3 mb-md-0">
                    <h5 class="fw-bold">Praveen Shukla</h5>
                    <p class="text-white-50 small">AI & Data Science Enthusiast | Portfolio 2025</p>
                    <div class="mt-3 d-flex flex-wrap justify-content-center justify-content-md-start gap-3">
                        <i class="fab fa-python fa-lg text-white-50"></i>
                        <i class="fas fa-brain fa-lg text-white-50"></i>
                        <i class="fas fa-chart-line fa-lg text-white-50"></i>
                        <i class="fab fa-github fa-lg text-white-50"></i>
                    </div>
                </div>

                <!-- Right Section -->
                <div class="col-md-6 d-flex justify-content-center justify-content-md-end align-items-center gap-3">
                    <a href="mailto:prashuiit@gmail.com" class="text-white text-decoration-none footer-link">
                        <i class="fas fa-envelope me-1"></i> Email
                    </a>
                    <a href="http://github.com/PraveenAShukla/" class="text-white footer-link" target="_blank">
                        <i class="fab fa-github"></i>
                    </a>
                    <a href="https://www.linkedin.com/in/praveen-ashukla/" class="text-white footer-link" target="_blank">
                        <i class="fab fa-linkedin"></i>
                    </a>
                </div>
            </div>

            <hr class="border-light my-3">

            <div class="text-center small text-white-50">
                © 2025 Praveen Shukla. All Rights Reserved.
            </div>
        </div>
    </footer>

    <!-- Back to Top Button -->
    <a href="#about" class="btn btn-outline-info btn-sm rounded-circle position-fixed bottom-0 end-0 m-3" title="Back to Top">
        <i class="fas fa-arrow-up"></i>
    </a>

    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
    <!-- Custom JS -->
    <script src="{{ url_for('static', filename='js/main.js') }}"></script>

    <script>
        // Smooth scroll and close menu on click (for mobile)
        document.querySelectorAll('a.nav-link').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                document.querySelector(targetId).scrollIntoView({
                    behavior: 'smooth'
                });

                // Collapse the navbar if it's open (on mobile)
                const navbarToggler = document.querySelector('.navbar-toggler');
                const navbarCollapse = document.querySelector('.navbar-collapse');
                if (navbarToggler && navbarCollapse.classList.contains('show')) {
                    navbarToggler.click(); // this simulates a click to close it
                }
            });
        });
    </script>
    <script>
        const btn = document.querySelector('.btn.btn-outline-info');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 300) {
                btn.style.display = 'block';
            } else {
                btn.style.display = 'none';
            }
        });
    </script>
</body>
</html>
