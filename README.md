<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="index.css">
    <script src="https://kit.fontawesome.com/e72052e40d.js" crossorigin="anonymous"></script>
</head>
  <style>
    *{
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
    box-sizing: border-box;
}
html{
    scroll-behavior: smooth;
}
body{
    background: black;
    color: azure;
}
#header{
    width: 100%;
    height: 100vh;
}
.container{
    padding: 20px 20px;
}
nav{
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
}
.logo{
    width: 140px;
    font-size: 35px;
}
.logo span{
    font-size: 40px;
    color: #ff004f;
}
nav ul li {
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
}
nav ul li a{
    color: azure;
    text-decoration: none;
    margin: 10px;
    position: relative;
}
nav ul li a:after{
    content: '';
    width: 0;
    height: 3px;
    background: #ff004f;
    position: absolute;
    left: 0;
    bottom: -6px;
    transition: 0.5s;
}
nav ul li a:hover::after{
    width: 100%;   
}
.header-text{
    margin-top: 20%;
    font-size: 30px;
}
.header-text h1{
    margin-top: 20px;
    font-size: 60px;

}
.header-text h1 span{
    color: #ff004f;
}
/*---------------about------------------*/
#about{
    padding: 80px 0px;
    color: #ababab;
}
.row{
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}
.about-col-1{
    flex-basis: 35%;
}
.about-col-1 img{
    width: 100%;
    border-radius: 15px;
}
.about-col-2{
    flex-basis: 60%;
}
.sub-title{
    font-size: 60px;
    font-weight: 600;
    color: azure;
}
.tab-titles{
    display: flex;
    margin: 20px 0 40px;
}
.tab-links{
    margin-right: 50px;
    font-size: 18px;
    font-weight: 400;
    cursor: pointer;
    position: relative;
}
.tab-links::after{
    content: '';
    width: 0;
    height: 3px;
    background: #ff004f;
    position: absolute;
    left: 0;
    bottom: -8px;
    transition: 0.5s;
}
.tab-links.active-link::after{
    width: 50%;
}
.tab-contants ul li{
    list-style: none;
    margin: 10px 0;
}
.tab-contants ul li span{
    color: #b54768;
    font-size: 14px;
}
.tab-contants{
    display: none;
}
.tab-contants.active-tab{
    display: block;
}
/*-------------services---------------------*/
#services{
    padding: 30px 0;
}
.services-list{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
    grid-gap: 40px;
    margin-top: 50px;
}
.services-list div{
    background: #262626;
    padding: 40px;
    font-size: 13px;
    font-weight: 300;
    border-radius: 10px;
    transition: background 0.5s, tranformation 0.5s;
}
.services-list div i{
    font-size: 50px;
    margin-bottom: 30px;
}
.services-list div h2{
    font-size: 30px;
    font-weight: 500;
    margin-bottom: 13px;
}
.services-list div a{
    text-decoration: none;
    color: azure;
    font-size: 12px;
    margin-top: 20px;
    display: inline-block;
}
.services-list div:hover{
    background: #ff004f;
    transform: translateY(-10px);
}
/*---------------------portfolio-------------------*/
#portfolio{
    padding: 50px  0;
}
.work-list{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
    grid-gap: 40px;
    margin-top: 50px;
}
.work{
    border-radius: 10px;
    position: relative;
    overflow: hidden;
}
.work img{
    width: 100%;
    border-radius: 10px;
    display: block;
    transition: transform 0.5s ;
}
.layer{
    height: 0%;
    width: 100%;
    background: linear-gradient(rgba(0,0,0,0.6), #ff004f);
    border-radius: 10px;
    position: absolute;
    left: 0;
    bottom: 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 0 40px;
    text-align: center;
    font-size: 14px;
    transition: height 0.5s;
}
.layer h3{
    font-weight: 500;
    margin-bottom: 20px;
}
.layer a{
    margin-top: 20px;
    color: #ff004f;
    text-decoration: none;
    font-size: 18px;
    line-height: 60px;
    background: #fff;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    align-items: center;

}
.work:hover img{
    transform: scale(1.1);
}
.work:hover .layer{
    height: 100%;
}
.btn{
    display: block;
    margin: 50px auto;
    width: fit-content;
    border: 1px solid #ff004f;
    padding: 14px 50px;
    border-radius: 6px;
    text-decoration: none;
    color: #fff;
    transition: background 0.5s;
}
.btn:hover{
    background: #ff004f;
}

/*--------------contact-----------------*/
.contact-left{
    flex-basis: 35%;
}
.contact-right{
    flex-basis: 60%;
}
.contact-left p{
    margin-top: 30px;
}
.contact-left p i{
    color: #ff004f;
    margin-right: 15px;
    font-size: 25px;
}
.social-icons{
    margin-top: 30px;
}
.social-icons a{
    text-decoration: none;
    margin-right: 15px;
    font-size: 30px;
    display: inline-block;
    color: #fff;
    transition: transform 0.5s;
}
.social-icons a:hover{
    color: #ff004f;
    transform: translateY(-5px);
}
.btn.btn2{
    display: inline-block;
    background: #ff004f;
}
.contact-right form{
    width: 100%;;
}
form input, form textarea{
    width: 100%;
    border: 0px;
    outline: none;
    background: #262626;
    padding: 15px;
    margin: 15px 0px;
    color: #fff;
    font-size: 18px;
    border-radius: 6px;
}
form .btn2{
    padding: 14px 60px;
    font-size: 18px;
    margin-top: 20px;
    cursor: pointer;
}
.copyright{
    width: 100%;
    text-align: center;
    padding: 25px 0px;
    background: #262626;
    font-weight:300;
    margin-top: 20px;
}
.copyright i{
    color: #ff004f;
}
nav .fa-solid{
    display: none;
}
/*--------------------css for small screen---------------------*/
@media only screen and (max-width: 600px){
    nav .fa-solid{
        display: block;
        font-size: 25px;
    }
    .header-text{
        margin-top: 100%;
        font-size: 16px;
    }
    .header-text h1{
        font-size: 30px;
    }
    nav ul{
        background: #ff004f;
        position: fixed;
        top: 0px;
        right: -200px;
        width: 200px;
        height: 100vh;
        padding-top: 50px;
        z-index: 2;
        transition: right 0.5s;
    }
    nav ul li{
        display: block;
        margin: 25px;
    }
    nav ul .fa-solid{
        position: absolute;
        top: 25px;
        left: 25px;
        cursor: pointer;
    }
    .sub-title{
        font-size: 40px;
    }
    .about-col-1 ,.about-col-2{
        flex-basis: 100%;
    }
    .about-col-1{
        margin-bottom: 30px;
    }
    .about-col-2{
        font-size: 14px;
    }
    .tab-links{
        font-size: 16px;
    }
    .contact-left ,.contact-right{
        flex-basis: 100%;
    }
    .copyright{
        flex-basis: 100%;
    }
}
#msg{
    color: #61b752;
    margin-top: -40px;
    display: block;

}
  </style>
<body>
<div id="header">
    <div class="container">
        <nav>
            <h1 class="logo"><span>S</span>ASHANK</h1>
            <ul id="sidemenu">
                <li><a href="#header">HOME</a></li>
                <li><a href="#about">ABUT US</a></li>
                <li><a href="#services">SERVICES</a></li>
                <li><a href="#portfolio">PORTFOLIO</a></li>
                <li><a href="#contact">CONTACT</a></li>
                <i class="fa-solid fa-circle-xmark" onclick="closemenu()"></i>
            </ul>
            <i class="fa-solid fa-bars" onclick="openmenu()"></i>
        </nav>
        <div class="header-text">
            <p>WEB AND APP DEVELOPER</p>
            <h1>Hi , I am <span>SASHANK</span> <br/>GARG from INDIA.</h1> 
        </div>
    </div>
</div>
<!-----------------about-------------------->
<div id="about">
    <div class="container">
        <div class="row">
            <div class="about-col-1"><img src="sodapdf-converted (2).png">
            </div>
            <div class="about-col-2">
                <h1 class="sub-title">About Me</h1>
                <p>I am learning web and app development from 1 years,
                     I master various applications, videos, photos and also app 
                     development techniques, my main task is to assess and organize various
                      apps and web for publication in the international web and app market.
                </p>
                <div class="tab-titles">
                    <p class="tab-links active-link" onclick="opentab('skills')">Skills</p>
                    <p class="tab-links" onclick="opentab('experience')">Experience</p>
                    <p class="tab-links" onclick="opentab('education')">Education</p>
                </div>
                <div class="tab-contants active-tab" id="skills">
                    <ul>
                        <li><span>Web</span><br/>Web app developer</li>
                        <li><span>UI/UX</span><br/>Designing Web AND app interface</li>
                        <li><span>App developement</span><br/>Building android/ios apps</li>
                    </ul>
                </div>
                <div class="tab-contants" id="experience">
                    <ul>
                        <li><span>2022-2023</span><br/>Web app developer at online platform</li>
                        <li><span>NO MORE EXPERIENCE</span><br/>YET</li>
                        <li><span>Dec2022</span><br/>web developement project</li>
                    </ul>
                </div>
                <div class="tab-contants" id="education">
                    <ul>
                        <li><span>2022</span><br/>Web developer course form LPU</li>
                        <li><span>2022 - 202 </span><br/> B-tech Computer science and engineering</li>
                        <li><span>2020-2022</span><br/>10th and 12th(non.medical) from KGVS</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</div>
<!-----------------sevices-------------------->
<div id="services">
    <div class="container">
        <h1 class="sub-title">My Services</h1>
        <div class="services-list">
            <div>
                <i class="fa-solid fa-code"></i>
                <h2>Web Design</h2>
                <p> is the creation of websites and pages to reflect a company's brand
                    and information and ensure a user-friendly experience. Appearance and design
                    are incorporated as vital elements whether you're designing a website, 
                    mobile app or maintaining content on a web page
                </p>
                <a href="#">Learn more</a>
            </div>
            <div>
                <i class="fa-solid fa-crop"></i>
                <h2>UI/UX</h2>
                <p> UI refers to the screens, buttons, toggles, icons, and other visual elements that you interact
                    with when using a website, app, or other electronic device. UX refers to the entire interaction 
                    you have with a product, including how you feel about the interaction
                </p>
                <a href="#">Learn more</a>
            </div>
            <div>
                <i class="fa-brands fa-app-store"></i>
                <h2>App developement</h2>
                <p> is the set of processes and procedures involved in writing software for small,
                    wireless computing devices, such as smartphones and other hand-held devices.
                </p>
                <a href="#">Learn more</a>
            </div>
        </div>
    </div>
</div>
<!---------------------PORTFOLIO----------------->
<div id="portfolio">
    <div class="container">
        <h1 class="sub-title">My Work</h1>
        <div class="work-list">
            <div class="work">
                <img src="sara-kurfess-6lcT2kRPvnI-unsplash.jpg">
                <div class="layer">
                    <h3>Mobile App</h3>
                    <p>the app connacts you yu the talented people around the world.
                        Download it form play store.</p>
                        <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                </div>
            </div>
            <div class="work">
                <img src="christian-lue-ExYywhe26vE-unsplash.jpg">
                <div class="layer">
                    <h3>Music App</h3>
                    <p>the app connacts you yu the talented people around the world.
                        Download it form play store.</p>
                        <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                </div>
            </div>
            <div class="work">
                <img src="cardmapr-nl-hTUZW7E7krg-unsplash.jpg">
                <div class="layer">
                    <h3>Online Shopping App</h3>
                    <p>the app connacts you yu the talented people around the world.
                        Download it form play store.</p>
                        <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                </div>
            </div>
        </div>
        <a href="#" class="btn">See More</a>
    </div>
</div>
<!----------contact--------------------->
<div id="contact">
    <div class="container">
        <div class="row">
            <div class="contact-left">
                <h1 class="sub-title">Contact Me</h1>
                <p><i class="fa-solid fa-paper-plane"></i>sashankgarg23@gmail.com</p>
                <p><i class="fa-solid fa-phone"></i>+91-9871510464</p>
                <div class="social-icons">
                <a href="https://www.facebook.com/profile.php?id=100027698713354"><i class="fa-brands fa-facebook"></i></a>
                <a href="https://www.quora.com/profile/Sashank-Garg-1"><i class="fa-brands fa-quora"></i></a>
                <a href="https://www.hackerrank.com/sashankgarg23"><i class="fa-brands fa-hackerrank"></i></a>
                <a href="https://github.com/sashank23"><i class="fa-brands fa-github"></i></a>
                </div>
                <a href="cvvvvvvv.png" download class="btn btn2">Download CV</a>
            </div>
            <div class="contact-right">
                <form name="submit-to-google-sheet">
                    <input type="text" name="Name" placeholder="Your Name" required>
                    <input type="email" name="Email" placeholder="Your Email" required>
                    <textarea name="Message" rows="6" placeholder="Your Message"></textarea>
                    <button type="submit" class="btn btn2">Submit</button>
                </form>
                <span id="msg"></span>
            </div>
        </div>
    </div>
    <div class="copyright">Copyright @ Sashank. Made with <i class="fa-solid fa-music"></i> Music</div>
</div>
<script>
    var tablinks = document.getElementsByClassName("tab-links");
    var tabcontants = document.getElementsByClassName("tab-contants");

    function opentab(tabname){
        for (tablink of tablinks){
            tablink.classList.remove("active-link");
        }
        for (tabcontant of tabcontants){
            tabcontant.classList.remove("active-tab");
        }
        event.currentTarget.classList.add("active-link");
        document.getElementById(tabname).classList.add("active-tab");
    }
</script>
<script>

    var sidemnu = document.getElementById("sidemenu");

    function openmenu(){
        sidemnu.style.right = "0"
    }
    function closemenu(){
        sidemnu.style.right = "-200px"
    }
</script>
<script>
    const scriptURL = 'https://script.google.com/macros/s/AKfycbzvdGtLJws5ZcX0zac88Q9ku2qKlBIA2jb6wC6guRoYviwIVC1DeXr5PQYt0_snFvyl/exec'
    const form = document.forms['submit-to-google-sheet']
    const msg = document.getElementById("msg")
  
    form.addEventListener('submit', e => {
      e.preventDefault()
      fetch(scriptURL, { method: 'POST', body: new FormData(form)})
        .then(response => {
            msg.innerHTML = "Message sent successfully"
            setTimeout(function(){
                msg.innerHTML = ""
            },5000)
            form.reset()
        })
        .catch(error => console.error('Error!', error.message))
    })
  </script>
</body>
</html>
