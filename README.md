<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="styles.css" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Kumbh+Sans:wght@100..900&display=swap" rel="stylesheet">
  <style>
    * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'kumbh sans', sans-serif;
}

.navbar {
    background: #131313;
    height: 80px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 1.2rem;
    position: sticky;
    top: 0;
    z-index: 999;
}

.navbar__container {
    display: flex;
    justify-content: space-between;
    height: 80px;
    z-index: 1;
    width: 100%;
    max-width: 1300px;
    margin: 0 auto;
    padding: 0 50px;
}

#navbar__logo {
    background-color: #ff8177;
    background-image: linear-gradient(to top, #ff0844 0%, #ffb199 100%);
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
    display: flex;
    align-items: center;
    cursor: pointer;
    text-decoration: none;
    font-size: 2rem;
}

.fa-gem {
    margin-right: 0.5rem;
}

.navbar__menu {
    display: flex;
    align-items: center;
    list-style: none;
    text-align: center;
}

.navbar__item {
    height: 80px;
}

.navbar__links {
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
    padding: 0 1rem;
    height: 100%;
}

.navbar__btn {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0 1rem;
    width: 100%;
}

.button {
    display: flex;
    justify-content: center;
    align-items: center;
    text-decoration: none;
    padding: 10px 20px;
    height: 100%;
    width: 100%;
    border: none;
    outline: none;
    border-radius: 4px;
    background: #f77062;
    color: #fff;
}

.button:hover {
    background: #4837ff;
    transition: all 0.3s ease;
}

.navbar__links:hover {
    color: #f77062;
    transition: all 0.3s ease;
}

@media screen and (max-width: 960px) {
    .navbar__container {
        display: flex;
        justify-content: space-between;
        height: 80px;
        z-index: 1;
        width: 100%;
        max-width: 1300px;
        padding: 0;
    }

    .navbar__menu {
        display: grid;
        grid-template-columns: auto;
        margin: 0;
        width: 100%;
        position: absolute;
        top: -1000px;
        opacity: 1; 
        transition: all 0.5s ease;
        height: 50vh;
        z-index: -1;
        background: #131313;
    }

    .navbar__menu.active {
        background: #131313;
        top: 100%;
        opacity: 1;
        transition: all 0.5s ease;
        z-index: 99;
        height: 50vh;
        font-size: 1.6rem;
    }

    #navbar__logo {
        padding-left: 25px;
    }

    .navbar__toggle .bar {
        width: 25px;
        height: 3px;
        margin: 5px auto;
        transition: all 0.3s ease-in-out;
        background: #fff;
    }

    .navbar__item {
        width: 100%;
    }

    .navbar__links {
        text-align: center;
        padding: 2rem;
        width: 100%;
        display: table;
    }

    #mobile-menu {
        position: absolute;
        top: 20%;
        right: 5%;
        transform: translate(5%, 20%);
    }

    .navbar__btn {
        padding-bottom: 2rem;
    }

    .button {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 80%;
        height: 80px;
        margin: 0;
    }

    .navbar__toggle .bar {
        display: block;
        cursor: pointer;
    }

    #mobile-menu.is-active .bar:nth-child(2) {
        opacity: 0;
    }

    #mobile-menu.is-active .bar:nth-child(1) {
        transform: translateY(8px) rotate(45deg); 
    }

    #mobile-menu.is-active .bar:nth-child(3) {
        transform: translateY(-8px) rotate(-45deg); 
    }
}

/* Hero Section CSS */
.main {
    background-color: #141414;
}

.main__container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    justify-self: center;
    margin: 0 auto;
    height: 90vh;
    background-color: #141414;
    z-index: 1;
    width: 100%;
    max-width: 1300px;
    padding: 0 50px;
}

.main__content h1 {
    font-size: 4rem;
    background-color: #ff8177;
    background-image: linear-gradient(to top, #ff0844 0%, #ffb199 100%);
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
}

.main__content h2 {
    font-size: 4rem;
    background-color: #ff8177;
    background-image: linear-gradient(to top, #b721ff 0%, #21d4fd 100%);
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparen
}

.main__content p {
    margin-top: 1rem;
    font-size: 2rem;
    font-weight: 700;
    color: #fff;
}

.main__btn {
    font-size: 1rem;
    background-image: linear-gradient(to top, #f77062 0%, #fe5196 100%);
    padding: 14px 32px;
    border: none;
    border-radius: 4px;
    color: #fff;
    margin-top: 2rem;
    cursor: pointer;
    position: relative;
    transition: all 0.35s;
    outline: none;
}

.main__btn a {
    position: relative;
    z-index: 2;
    color: #fff;
    text-decoration: none;
}

.main__btn:after {
    position: absolute;
    content: '';
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background: #4837ff;
    transition: all 0.35s;
    border-radius: 4px;
}

.main__btn:hover {
    color: #fff;
}

.main__btn:hover:after {
    width: 100%;
}

.main__img--container {
    text-align: center;
}

#main__img {
    height: 80%;
    width: 80%;
}

/* Mobile Responsive */
@media screen and (max-width: 768px) {
    .main__container {
        display: grid;
        grid-template-columns: auto;
        align-items: center;
        justify-self: center;
        width: 100%;
        margin: 0 auto;
        height: 90vh;
    }

    .main__content {
        text-align: center;
        margin-bottom: 4rem;
   }

   .main__content h1 {
        font-size: 2.5rem;
        margin-top: 2rem;
   }

   .main__content h2 {
        font-size: 3rem;
   }

   .main__content p {
        margin-top: 1rem;
        font-size: 1.5rem;
   }
}

@media screen and (max-width: 480px) {
    .main__content h1 {
        font-size: 2rem;
        margin-top: 3rem;
   }

   .main__content h2 {
        font-size: 2rem;
   }

   .main__content p {
        margin-top: 2rem;
        font-size: 1.5rem;
   }

   .main__btn {
        padding: 12px 36px;
        margin: 2.5rem 0;

   }
}

/* Services Section CSS*/
.services {
    background: #141414;
    display:flex;
    flex-direction: column;
    align-items: center;
    height: 100vh;
}

.services h1 {
    background-color: #ff8177;
    background-image: linear-gradient(to right, #ff8177 0%, #ff867a 0%, #ff8c7f 21%, #f99185 52%, #cf556c 78%, #b12a5b 100%);
    background-size: 100%;
    margin-bottom: 5rem;
    font-size: 2.5rem;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
}

.services__container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.services__card {
    margin: 1rem;
    height: 525px;
    width: 400px;
    border-radius: 4px;
    background-image: linear-gradient(to bottom, rgba(0,0,0,0) 0%, rgba(17, 17, 17, 0.6) 100%), url('/com/HI/hey.jpg');
    background-size: cover;
    position: relative;
    color: #fff;
}

.services__card:nth-child(2) {
    background-image: linear-gradient(to bottom, rgba(0,0,0,0) 0%, rgba(17, 17, 17, 0.6) 100%), url('/com/HI/hm.jpg');
}

.services h2 {
    position: absolute;
    top: 350px;
    left: 30px;
}

.services__card p {
    position: absolute;
    top: 400px;
    left: 30px;
}

.services__card button {
    color: #fff;
    padding: 10px 20px;
    border: none;
    outline:none;
    border-radius: 4px;
    background: #f77062;
    position: absolute;
    top: 440px;
    left: 30px;
    font-size: 1rem;
    cursor: pointer;
}

.services__card:hover {
    transform: scale(1.075);
    transition: 0.2s ease-in;
    cursor: pointer;
}

@media screen and (max-width: 960px) {
    .services {
        height: 1600px;
    }

    .services h1 {
        font-size: 2rem;
        margin-top: 12rem;
    }
}

@media screen and (max-width: 480px) {
    .services {
        height: 1400px;
    }

    .services h1 {
        font-size: 1.2rem;
    }

    .services__card {
        width: 300px;
    }
}

/* Footer CSS */
.footer__container {
    background-color: #141414;
    padding: 5rem 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

#footer__logo {
    color: #fff;
    display: flex;
    align-items: center;
    cursor: pointer;
    text-decoration: none;
    font-size: 2rem;
}

.footer__links {
    width: 100%;
    max-width: 1000px;
    display: flex;
    justify-content: center;
}

.footer__links--wrapper {
    display: flex;
}

.footer__links--items {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    margin: 16px;
    text-align: left;
    width: 160px;
    box-sizing: border-box;
}

.footer__links--items h2 {
    margin-bottom: 16px;
}

.footer__links--items > h2 {
    color: #fff;
    text-decoration: none;
    margin-bottom: 0.5rem;

}

  </style>
</head>
<body>
    <!-- Navbar Section -->
    <nav class="navbar">
        <div class="navbar__container">
            <a href="/" id="navbar__logo"><i class="fas fa-gem"></i> NEXT
            </a>
            <div class="navbar__toggle" id="mobile-menu">
                <span class="bar"></span>
                <span class="bar"></span>
                <span class="bar"></span>
            </div>
            <ul class="navbar__menu">
                <li class="navbar__item">
                    <a href="/" class="navbar__links">Home</a>
                </li>
                <li class="navbar__item">
                    <a href="/tech.html" class="navbar__links">Tech</a>
                </li>
                <li class="navbar__item">
                    <a href="/" class="navbar__links">Products</a>
                </li>   
                <li class="navbar__btn">
                    <a href="/" class="button">Sign Up</a>
                </li>         
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <div class="main">
        <div class="main__container">
            <div class="main__content">
                <h1>NEXT GENERATION</h1>
                <H2>TECHNOLOGY</H2>
                <P>See what make us different.</P>
                <button class="main__btn"><a href="/">Get Started</a></button>
            </div>
            <div class="main__img--container">
                <img src="huy.svg" alt="pic" id="main__img">
            </div>
        </div>
    </div>

    <!-- Services Section -->
    <div class="services">
        <h1>See what the hype is about</h1>
        <div class="services__container">
            <div class="services__card">
                <h2>Experience Bliss</h2>
                <p>AI powered technology</p>
                <button>Get Started</button>
                <img src="hey.jpg" alt="pic" id="main__img">
            </div>
            <div class="services__card">
                <h2>Are you ready?</h2>
                <p>Take the leap</p>
                <button>Get Started</button>
                <img src="hm.jpg" alt="pic" id="main__img">
            </div>
        </div>
    </div>

    <!-- Footer Section -->
    <div class="footer__container">
        <div class="footer__links">
            <div class="footer__link--wrapper">
                <div class="footer__link--items">
                    <h2>About Us</h2>
                    <a href="/sign up" class="">How it works</a>
                    <a href="/" class="">Testimonals</a>
                    <a href="/" class="">Careers</a>
                    <a href="/" class="">Investments</a>
                    <a href="/" class="">Terms of Service</a>
                </div>
                <div class="footer__link--items">
                    <h2>Contact Us</h2>
                    <a href="/" class="">Contact</a>
                    <a href="/" class="">Support</a>
                    <a href="/" class="">Destinations</a>
                    <a href="/" class="">Sponsorships</a>
                </div>
            </div>
            <div class="footer__link--wrapper">
                <div class="footer__link--items">
                    <h2>Videos</h2>
                    <a href="/" class="">Submit Video</a>
                    <a href="/" class="">Ambassadors</a>
                    <a href="/" class="">Agency</a>
                    <a href="/" class="">Influencer</a>
                </div>
                <div class="footer__link--items">
                    <h2>Social Media</h2>
                    <a href="/" class="">Instagram</a>
                    <a href="/" class="">Facebook</a>
                    <a href="/" class="">youtube</a>
                    <a href="/" class="">Twitter</a>
                </div>
            </div>
        </div>
        <div class="social__media">
            <div class="social__media--wrap">
                <div class="footer__logo">
                   <a href="/" id="footer__logo"><i class="fas faa-gem"></i>NEXT</a> 
                </div>
                <p class="website__right">NEXT 2020. All rights reserved</p>
                <div class="social__icons">
                    <a href="/" class="social__icons--link" target="-blank">
                        <i class="fab fa-facebook"></i>
                    </a>
                    <a href="/" class="social__icons--link" target="-blank">
                        <i class="fab fa-instagram"></i>
                    </a>
                    <a href="/" class="social__icons--link" target="-blank">
                        <i class="fab fa-twitter"></i>
                    </a>
                    <a href="/" class="social__icons--link" target="-blank">
                        <i class="fab fa-linkedin"></i>
                    </a>
                    <a href="/" class="social__icons--link" target="-blank">
                        <i class="fab fa-youtube"></i>
                    </a>
                </div>
            </div>
        </div>
    </div>

    <script src="app.js"></script>
</body>
</html>
