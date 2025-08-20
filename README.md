# 🍵 Tea Cozy — Boutique Tea Shop Website  

A fictional **tea shop website** built with clean **HTML & CSS**.  
Designed to practice **Flexbox layouts**, responsive design, and semantic structure.  
Includes a **hero section**, a **mission statement**, a **featured teas grid**, and a **locations/contact footer**.  
Uses **Google Fonts (Playfair Display & Lato)** for an elegant retail feel, with flex properties (`display: flex`, `flex-wrap`, `justify-content`, `align-items`) for aligning product cards and sections.  

---

## 📸 Preview  
![Tea Cozy Preview](https://github.com/SunilKumarPeela/WebImages/blob/main/TeaCozy.png)  

---

## 🗂️ Project Structure  

TeaCozy/

├─ index.html

└─ style.css
---


---

## ▶️ Live Demo [![Open in CodeSandbox](https://img.shields.io/badge/Open%20in-CodeSandbox-black?style=for-the-badge&logo=codesandbox)](https://codesandbox.io/p/sandbox/github/SunilKumarPeela/TeaCozy)

---

## 🎯 Skills Practiced  
- Structuring a web page with **semantic HTML**  
- Using **Flexbox** for layouts: hero, grid, and footer  
- Applying **flex-wrap** for responsive product cards  
- Building a **sticky navigation bar**  
- Styling text with **Google Fonts**  
- Creating a **storefront look** with hero images & product showcases  

---

## 📄 index.html  

```html
<!DOCTYPE html>
<html>
<head>
  <title>The Tea Cozy</title>
  <link rel="stylesheet" href="style.css" type="text/css" />
</head>
<body>
  <header>
    <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-tea-cozy-logo.png" alt="Tea Cozy logo">
    <nav>
      <a href="#">Mission</a>
      <a href="#">Featured Tea</a>
      <a href="#">Locations</a>
     </nav> 
  </header>
  <main>
    <div class="main-text">
      <h2>Our mission</h2>
      <h4>Handpicked, Artisanally Curated, Free Range, Sustainable, Small Batch, Fair Trade, Organic Tree</h4>
    </div>
  </main>
  <section class="tea-of-the-month">
    <h2>Tea of the month</h2>
    <h4>What's Steeping at The Tea Cozy?</h4>
  
  <div class="tea-imgs">

    <div>
      <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-berryblitz.jpg" alt="Blitz Tea">
      <h4>"Fall Berry Blitz Tea" </h4>
    </div>

     <div>
      <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-spiced-rum.jpg" alt="Spiced Tea Rum">
      <h4>"Spiced Tea Rum" </h4>
    </div>

     <div>
      <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-donut.jpg" alt="Seasonal Donuts">
      <h4>"Seasonal Donuts" </h4>
    </div>

    <div>
      <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-myrtle-ave.jpg" alt="Myrtle Ave Tea">
      <h4>"Myrtle Ave Tea" </h4>
    </div>

    <div>
      <img src="https://content.codecademy.com/courses/freelance-1/unit-4/img-bedford-bizarre.jpg" alt="Bedford Bizarre Tea">
      <h4>"Bedford Bizarre Tea" </h4>
    </div>
  </div>
  </section>

  <section class="locations">
    <h2>Locations</h2>
    <div class="addresses">
      <address>
        <h4>Downtown</h4>
        <p>384 West 4th St</p>
        <p>Suite 108</p>
        <p>Portland, Maine</p>
      </address>

      <address>
        <h4>East Bayside</h4>
        <p>3433 Phiserman's Avenue</p>
        <p>(Northwest Corner)</p>
        <p>Portland, Maine</p>
      </address>

      <address>
        <h4>Oakdale</h4>
        <p>515 Crescent Avenue</p>
        <p>Second Floor</p>
        <p>Portland, Maine</p>
      </address>
    </div>
 </section>

 <footer>
  <div class="contact">
    <h2>The Tea Cozy</h2>
    <h4>contact@theteacozy.com</h4>
    <h4>917-555-8905</h4>
  </div>
  <div class="copyright">
    <h4>copyright The Tea Cozy 2025</h4>
  </div>
</footer>

</body>
</html>
```
---
##🎨 style.css
```css

*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}
body{
  font-family:Helvetica;
  font-size:22px;
  color:seashell;
  background-color:black;
  opacity:0.9;
  text-align:center;
}

header{
  height:69px;
  border-bottom: 1px solid seashell;
  display:flex;
  justify-content:space-between;
  align-items:center;
  margin:0 10px;
}

header img{
  height:50px;
  
}
nav a{
  color:inherit;
}

main{
   background-image:url("https://content.codecademy.com/courses/freelance-1/unit-4/img-mission-background.jpg");
   background-repeat:no-repeat;
   background-size:cover;
   height:700px;
   display:flex;
   align-items:Center;
}

.main-text{
  background:black;
  width:100%;
}

.main-text *{
  margin: 10px 0;
}

.tea-of-the-month{
  display:flex;
  flex-direction:column;
  align-items:center;
  padding:50px;
}
 

.tea-imgs{
  max-width:1000px;
  display:flex;
  flex-wrap:wrap;
  justify-content:center;
}

.tea-imgs img{
  width:300px;
  height:200px;
  margin:0 10px;
}  

.tea-imgs h4, .tea-of-the-month h2, .tea-of-the-month h4 {
  margin: 10px 0;
}

.locations{ 
  padding:150px 0;

  background:url("https://content.codecademy.com/courses/freelance-1/unit-4/img-locations-background.jpg");
  background-position: center;
  background-size:cover;
}

.locations h2{
  margin-bottom:20px;
}
.addresses{
  display:flex;
  justify-content:space-around;
  padding: 20px;
}

.addresses address{
  background:black;
}

address h4, address p{
  margin:15px;
}

.contact h2, .contact h4{
  margin:20px;
}

footer .copyright{
  text-align: left;
  margin-left:20px;
}
```
