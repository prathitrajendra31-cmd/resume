!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Prathit Rajendra | E-Commerce & Performance Analyst</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap');

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:'Inter',sans-serif;
    background:#070707;
    color:#f5f5f5;
    line-height:1.6;
}

/* NAVBAR */

nav{
    position:fixed;
    top:0;
    width:100%;
    z-index:1000;
    padding:20px 8%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    background:rgba(7,7,7,.75);
    backdrop-filter:blur(15px);
    border-bottom:1px solid rgba(255,255,255,.08);
}

.logo{
    font-size:22px;
    font-weight:800;
    letter-spacing:2px;
}

.logo span{
    color:#9b7cff;
}

nav ul{
    display:flex;
    gap:30px;
    list-style:none;
}

nav a{
    color:#aaa;
    text-decoration:none;
    font-size:14px;
    transition:.3s;
}

nav a:hover{
    color:white;
}

/* HERO */

.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    padding:120px 8% 70px;
    position:relative;
    overflow:hidden;
}

.hero::before{
    content:"";
    position:absolute;
    width:500px;
    height:500px;
    background:#694cff;
    filter:blur(180px);
    opacity:.15;
    right:-100px;
    top:100px;
}

.hero-content{
    max-width:900px;
    position:relative;
    z-index:2;
}

.tag{
    display:inline-block;
    padding:8px 16px;
    border:1px solid #333;
    border-radius:30px;
    color:#aaa;
    font-size:13px;
    margin-bottom:25px;
}

.hero h1{
    font-size:clamp(48px,8vw,95px);
    line-height:1;
    letter-spacing:-4px;
    margin-bottom:25px;
}

.hero h1 span{
    background:linear-gradient(90deg,#fff,#9b7cff);
    -webkit-background-clip:text;
    color:transparent;
}

.hero p{
    max-width:720px;
    color:#aaa;
    font-size:18px;
    margin-bottom:35px;
}

.buttons{
    display:flex;
    gap:15px;
    flex-wrap:wrap;
}

.btn{
    padding:14px 24px;
    border-radius:8px;
    text-decoration:none;
    font-weight:600;
    transition:.3s;
}

.primary{
    background:#fff;
    color:#000;
}

.primary:hover{
    transform:translateY(-3px);
}

.secondary{
    border:1px solid #333;
    color:white;
}

.secondary:hover{
    background:#151515;
}

/* SECTIONS */

section{
    padding:110px 8%;
}

.section-title{
    font-size:42px;
    margin-bottom:15px;
    letter-spacing:-2px;
}

.section-subtitle{
    color:#888;
    margin-bottom:50px;
}

/* METRICS */

.metrics{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:20px;
}

.metric{
    padding:30px;
    background:#0e0e0e;
    border:1px solid #222;
    border-radius:15px;
    transition:.3s;
}

.metric:hover{
    transform:translateY(-6px);
    border-color:#604cff;
}

.metric h3{
    font-size:28px;
    color:#fff;
}

.metric p{
    color:#777;
    font-size:13px;
}

/* SKILLS */

.skills{
    display:flex;
    flex-wrap:wrap;
    gap:12px;
}

.skill{
    padding:12px 18px;
    border:1px solid #292929;
    background:#0e0e0e;
    border-radius:50px;
    color:#bbb;
    transition:.3s;
}

.skill:hover{
    color:#fff;
    border-color:#8b6cff;
    transform:translateY(-3px);
}

/* PROJECTS */

.projects{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:25px;
}

.project{
    padding:35px;
    background:linear-gradient(145deg,#111,#090909);
    border:1px solid #222;
    border-radius:18px;
    position:relative;
    overflow:hidden;
    transition:.4s;
}

.project:hover{
    transform:translateY(-8px);
    border-color:#604cff;
}

.project-number{
    color:#725cff;
    font-size:14px;
    font-weight:700;
}

.project h3{
    font-size:24px;
    margin:15px 0;
}

.project p{
    color:#888;
    font-size:14px;
}

/* TOOLS */

.tool-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:20px;
}

.tool{
    background:#0e0e0e;
    border:1px solid #222;
    padding:30px;
    border-radius:15px;
}

.tool h3{
    margin-bottom:8px;
}

.tool p{
    color:#777;
    font-size:14px;
}

/* EDUCATION */

.education{
    border-left:2px solid #604cff;
    padding-left:30px;
}

.education h3{
    font-size:24px;
}

.education p{
    color:#888;
}

/* CONTACT */

.contact{
    text-align:center;
    max-width:850px;
    margin:auto;
}

.contact p{
    color:#888;
    margin:20px auto 35px;
}

.contact-info{
    display:flex;
    justify-content:center;
    gap:25px;
    flex-wrap:wrap;
}

.contact-info a{
    color:#aaa;
    text-decoration:none;
    border:1px solid #292929;
    padding:12px 18px;
    border-radius:8px;
}

.contact-info a:hover{
    color:#fff;
    border-color:#725cff;
}

/* FOOTER */

footer{
    text-align:center;
    padding:30px;
    border-top:1px solid #181818;
    color:#666;
    font-size:13px;
}

/* ANIMATION */

.fade{
    opacity:0;
    transform:translateY(30px);
    transition:1s;
}

.fade.show{
    opacity:1;
    transform:translateY(0);
}

/* RESPONSIVE */

@media(max-width:900px){

    nav ul{
        display:none;
    }

    .metrics{
        grid-template-columns:repeat(2,1fr);
    }

    .projects{
        grid-template-columns:1fr;
    }

    .tool-grid{
        grid-template-columns:1fr;
    }

}

@media(max-width:600px){

    section{
        padding:80px 6%;
    }

    .hero{
        padding:120px 6% 70px;
    }

    .hero h1{
        font-size:48px;
        letter-spacing:-2px;
    }

    .hero p{
        font-size:16px;
    }

    .metrics{
        grid-template-columns:1fr;
    }

    .section-title{
        font-size:34px;
    }

}
</style>
</head>

<body>

<!-- NAVIGATION -->

<nav>

    <div class="logo">
        PRATHIT<span>.</span>
    </div>

    <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#education">Education</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>

</nav>


<!-- HERO -->

<section class="hero" id="about">

    <div class="hero-content fade">

        <div class="tag">
            E-COMMERCE • PERFORMANCE • ANALYTICS
        </div>

        <h1>
            Prathit<br>
            <span>Rajendra</span>
        </h1>

        <p>
            Data-driven Digital Business Analyst and Performance Marketing
            Analyst focused on e-commerce analytics, paid acquisition,
            conversion optimization and digital growth.
        </p>

        <div class="buttons">

            <a href="#projects" class="btn primary">
                View My Work
            </a>

            <a href="mailto:prathitrajendra31@gmail.com"
               class="btn secondary">
                Contact Me
            </a>

        </div>

    </div>

</section>


<!-- METRICS -->

<section>

    <div class="section-title fade">
        What I Work With
    </div>

    <p class="section-subtitle fade">
        Performance metrics that drive better digital decisions.
    </p>

    <div class="metrics">

        <div class="metric fade">
            <h3>CR</h3>
            <p>Conversion Rate</p>
        </div>

        <div class="metric fade">
            <h3>AOV</h3>
            <p>Average Order Value</p>
        </div>

        <div class="metric fade">
            <h3>ROAS</h3>
            <p>Return on Ad Spend</p>
        </div>

        <div class="metric fade">
            <h3>CAC</h3>
            <p>Customer Acquisition Cost</p>
        </div>

    </div>

</section>


<!-- SKILLS -->

<section id="skills">

    <h2 class="section-title fade">
        Core Competencies
    </h2>

    <p class="section-subtitle fade">
        Strategy, analytics and performance marketing capabilities.
    </p>

    <div class="skills fade">

        <div class="skill">E-Commerce Strategy</div>
        <div class="skill">Conversion Rate Optimization</div>
        <div class="skill">Funnel Analysis</div>
        <div class="skill">Customer Journey Mapping</div>
        <div class="skill">UX Optimization</div>
        <div class="skill">Landing Page Optimization</div>
        <div class="skill">GA4</div>
        <div class="skill">Web Analytics</div>
        <div class="skill">KPI Tracking</div>
        <div class="skill">Performance Dashboards</div>
        <div class="skill">Market Research</div>
        <div class="skill">Competitor Benchmarking</div>
        <div class="skill">Google Ads</div>
        <div class="skill">Meta Ads</div>
        <div class="skill">PPC</div>
        <div class="skill">SEM</div>
        <div class="skill">Audience Segmentation</div>
        <div class="skill">Retargeting</div>
        <div class="skill">A/B Testing</div>
        <div class="skill">Advanced Excel</div>

    </div>

</section>


<!-- PROJECTS -->

<section id="projects">

    <h2 class="section-title fade">
        Selected Projects
    </h2>

    <p class="section-subtitle fade">
        Practical experience and academic projects in digital business.
    </p>

    <div class="projects">

        <div class="project fade">

            <div class="project-number">
                PROJECT 01
            </div>

            <h3>
                E-Commerce Performance & Paid Media Optimization
            </h3>

            <p>
                Evaluated e-commerce storefront performance using web
                analytics methodologies, mapped multi-stage user journeys
                and identified funnel drop-off points to improve conversion.
            </p>

            <br>

            <p>
                Analyzed Google Ads and Meta Ads campaign data with focus
                on ROAS, CAC and impressions to optimize advertising
                allocation.
            </p>

        </div>


        <div class="project fade">

            <div class="project-number">
                PROJECT 02
            </div>

            <h3>
                Digital Business Strategy & Funnel Optimization
            </h3>

            <p>
                Evaluated digital-first retail business models and developed
                hypotheses for A/B testing, user journey simplification
                and checkout flow optimization.
            </p>

            <br>

            <p>
                Developed optimization strategies aimed at reducing bounce
                rates and improving Average Order Value across simulated
                e-commerce landing pages.
            </p>

        </div>


        <div class="project fade">

            <div class="project-number">
                PROJECT 03
            </div>

            <h3>
                Competitor Benchmarking
            </h3>

            <p>
                Conducted structured competitor benchmarking and market
                research to support product merchandising strategies and
                identify cross-selling opportunities.
            </p>

        </div>


        <div class="project fade">

            <div class="project-number">
                PROJECT 04
            </div>

            <h3>
                KPI & Performance Reporting
            </h3>

            <p>
                Engineered KPI tracking frameworks using Advanced Excel,
                created data visualizations and presented insights related
                to traffic acquisition and customer acquisition efficiency.
            </p>

        </div>

    </div>

</section>


<!-- TOOLS -->

<section>

    <h2 class="section-title fade">
        Analytics Stack
    </h2>

    <p class="section-subtitle fade">
        Tools used for analysis, reporting and performance optimization.
    </p>

    <div class="tool-grid">

        <div class="tool fade">
            <h3>Google Analytics 4</h3>
            <p>
                Web analytics, user journeys, funnel analysis and KPI tracking.
            </p>
        </div>

        <div class="tool fade">
            <h3>Google Ads</h3>
            <p>
                Paid acquisition, campaign analysis and performance optimization.
            </p>
        </div>

        <div class="tool fade">
            <h3>Meta Ads Manager</h3>
            <p>
                Audience analysis, paid social campaigns and retargeting.
            </p>
        </div>

        <div class="tool fade">
            <h3>Advanced Excel</h3>
            <p>
                VLOOKUP, Pivot Tables, data modeling and performance dashboards.
            </p>
        </div>

        <div class="tool fade">
            <h3>Google Ads Editor</h3>
            <p>
                Campaign management and paid media optimization.
            </p>
        </div>

        <div class="tool fade">
            <h3>Google Workspace</h3>
            <p>
                Research, reporting, collaboration and business productivity.
            </p>
        </div>

    </div>

</section>


<!-- EDUCATION -->

<section id="education">

    <h2 class="section-title fade">
        Education
    </h2>

    <p class="section-subtitle fade">
        Academic foundation in digital business.
    </p>

    <div class="education fade">

        <h3>
            Bachelor of Business Administration
        </h3>

        <p>
            Digital Business
        </p>

        <p>
            Presidency University, Bengaluru
        </p>

        <p>
            2025 — Ongoing
        </p>

    </div>

</section>


<!-- CERTIFICATIONS -->

<section>

    <h2 class="section-title fade">
        Certifications
    </h2>

    <p class="section-subtitle fade">
        Professional learning and digital analytics credentials.
    </p>

    <div class="skills fade">

        <div class="skill">
            Fundamentals of Digital Marketing — Google Certified
        </div>

        <div class="skill">
            Google Analytics 4 & Web Metrics — Google
        </div>

        <div class="skill">
            Digital Marketing & Analytics — Essential Hub
        </div>

    </div>

</section>


<!-- CONTACT -->

<section id="contact">

    <div class="contact fade">

        <h2 class="section-title">
            Let's Connect
        </h2>

        <p>
            Interested in e-commerce, performance marketing, digital
            analytics and growth strategy? Let's connect.
        </p>

        <div class="contact-info">

            <a href="mailto:prathitrajendra31@gmail.com">
                Email
            </a>

            <a href="tel:+917259809179">
                +91 7259809179
            </a>

            <a href="https://linkedin.com/in/prathit-rajendra-403046377"
               target="_blank">
                LinkedIn
            </a>

        </div>

    </div>

</section>


<!-- FOOTER -->

<footer>

    © 2026 Prathit Rajendra — E-Commerce & Performance Analyst

</footer>


<script>

/* SCROLL ANIMATION */

const elements = document.querySelectorAll('.fade');

const observer = new IntersectionObserver((entries) => {

    entries.forEach(entry => {

        if(entry.isIntersecting){
            entry.target.classList.add('show');
        }

    });

},{
    threshold:0.15
});

elements.forEach(el => observer.observe(el));

</script>

</body>
</html> 
