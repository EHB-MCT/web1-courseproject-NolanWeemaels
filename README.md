# Readme

This Readme provides all the sources used to create this website.

## Sources + code


## Instagram: 
### Source:
    Softwarechemist. (2024, augustus). Trick and Treat Toggle Switch animation| Using HTML and CSS. Geraadpleegd op 19 november 2024, van https://www.instagram.com/p/C_HwXxcy7A1/
     
### Code:

    .container2 {
        display: flex;
        flex-wrap: wrap;
        margin: 0px 0 0 0px;
        width: 80%;
        height: 450px;
        display: flex;
        justify-content: center;
        gap: 10px;
        background-color: white;
        padding-top: 10px;
        padding-left: 10%;
    }

    .container2 img {
        width: 12.5%;
        height: 100%;
        object-fit: cover;
        border-radius: 16px;
        border: 2px solid beige;
        transition: all ease-in-out 0.5s;
        justify-content: start;
    }
    .container2Mobile{
        display: flex;
        justify-content: center;
        align-items: center;
        display: none;
    }

## Instagram
### Source:
    uvais.codes. (2024, oktober). Infinite Scrolling Marquee. Instagram. Geraadpleegd op 22 november 2024, van https://www.instagram.com/p/DCjU4NTzr4t/

### Code:

    .scroll {
        position: relative;
        display: flex;
        width: 85%;
        overflow: hidden;
        padding-top: 100px;
        margin: auto;
        padding: 10px;

    -webkit-mask-image: linear-gradient(
        90deg,
        transparent,
        #fff 30%,
        #fff 70%,
        transparent
    );
    }

    .scroll div {
        white-space: nowrap;
        animation: animate var(--t) linear infinite;
    }

    .scroll div:nth-child(2) {
        animation: animate2 var(--t) linear infinite;
    }

    @keyframes animate {
        0% {
            transform: translateX(100%);
        }
        100% {
        transform: translateX(-100%);
        }
    }

    @keyframes animate2 {
        0% {
            transform: translateX(0);
        }
        100% {
            transform: translateX(-200%);
        }
    }

    .scroll div span {
        display: inline-flex;
        margin: 10px;
        padding: 5px 10px;
        border-radius: 5px;
        background: #333;
        color: #fff;
        transition: 0.5s;
    }

    .scroll div span:hover {
        background: blue;
        cursor: pointer;
    }

## W3Schools

### Source:
    W3Schools.com. (z.d.). Geraadpleegd op 21 december 2024, van https://www.w3schools.com/howto/howto_js_mobile_navbar.asp

### Code:
#### HTML:
     <nav class="navbar">
      <div class="jobs-logo">
        <a href="index.html"><img src="images/appleLogoSteveJobsWhite.png"></a>
        
      </div>
      <div class="menu-toggle" id="menu-toggle">
          <div class="bar"></div>
          <div class="bar"></div>
          <div class="bar"></div>
      </div>
      <ul class="nav-links">
          <li><a href="HomeFR.html">Accueil</a></li>
          <li><a href="iLifeFR.html">iVie</a></li>
          <li><a href="ProductsFR.html">Produits</a></li>
          
      </ul>
     </nav>

#### CSS:
    .navbar {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding-top: 10px;
        padding-bottom: 10px;
        opacity: 85%;
        background: transparent;
        background-color: #333;
        color: white;
        align-items: center;
        position: fixed;
        width: 100vw;
        border-bottom: gray;
        z-index: 99999999;
    }



    .nav-links {
        display: flex;
        list-style: none;
        padding: 0;
        margin: 0;
        padding-left: 40%;
        padding: 10px;
        position: fixed;
        padding-right: 100px;
        align-items: end;
    }

  
    .nav-links li {
        margin: 0 10px;
    }

    .nav-links a {
        color: white;
        text-decoration: none;
        padding: 5px 10px;
        transition: background 0.3s;
        font-size: 20px;
        text-align: center;
        margin-right: 60px;
        margin-left: 60px;
        font-size: 18px;
    }

    .nav-links a:hover {
         background: #555;
        border-radius: 5px;
        text-decoration: none;
    }

    .menu-toggle {
        display: none;
        flex-direction: column;
        cursor: pointer;
        align-items: end;
        padding-right: 50px;
    }

    .menu-toggle .bar {
        width: 25px;
        height: 3px;
        background-color: white;
        margin: 3px 0;
    }

    @media (max-width: 768px) {
    .nav-links {
        display: none;
        flex-direction: column;
        background-color: #333;
        position: absolute;
        top: 60px;
        right: 20px;
        width: 200px;
        border-radius: 5px;
    }

    .nav-links.active {
        display: flex;
    }

    .menu-toggle {
        display: flex;
    }
    }
