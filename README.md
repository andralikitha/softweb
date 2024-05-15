# Ex.07 Software Product Company Website

## Date:29.04.2024

## AIM:
To develop a static company website to display the softwares and services provided by the company.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
### CSS CODE :
```css
* {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
body {
  background-color: rgb(255, 255, 255);
  color: #17421d;
}
.container {
  width: 1080px;
  margin-left: auto;
  margin-right: auto;
  border-width: 1px 1px 1px 1px;
  border-style: solid;
  box-shadow: 15px 15px 8px gray;
}

.banner {
  display: block;
  width: 100%;
  height: 180px;
  text-align: center;
  font-size: 60px;
  background-image: url("/static/img/log.png");
  background-size: 100% 100%;
  margin: 0px 0px 0px 0px;
  padding-top: 150px;
  color: #000000;
}

.menu {
  display: block;
  width: 100%;
  height: 50px;
  font-size: larger;
  background-color: #393939;
  text-align: center;
  padding-top: 15px;
  margin: 0px 0px 0px 0px;
  border-width: 1px;
}

.menuitem {
  display: inline-block;
  margin-left: 10px;
  margin-right: 10px;
}
.menuitemselected {
  display: inline-block;
  margin-left: 10px;
  margin-right: 10px;
  color: #ffffff;
}

.menuitem a {
  text-decoration: none;
  color: #9c1018;
}

.content {
  display: block;
  width: 100%;
  background-color: #fefefe;
  min-height: 500px;
  margin: 0px 0px 0px 0px;
  border-width: 1px;
  border-color: white;
  border-style: solid;
}
.homecontent {
  min-height: 500px;
  margin: 10px 10px 10px 10px;
}
.homecontent h1 {
  text-align: left;
}
.homecontent img {
  float: right;
  width: 400px;
  height: 300px;
  margin-left: 10px;
}

.contenttext {
  text-align: justify;
}

.productcontent {
  min-height: 500px;
  margin: 10px 10px 10px 10px;
}

.productcontent h1 {
  text-align: left;
}

.productitems {
  display: block;
}

.productitem {
  display: inline-block;
  width: 30%;
  height: 250px;
  text-align: center;
}

.productitem img {
  width: 100px;
  height: 100px;
  display: block;
}
.productitem .itemimage {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 100px;
  margin-bottom: 5px;
}

.productitem .itemname {
  display: block;
}
.productitem .itemprice {
  display: block;
}

.footer {
  display: block;
  width: 100%;
  height: 40px;
  background-color: #393939;
  text-align: center;
  padding-top: 10px;
  margin: 0px 0px 0px 0px;
  color: #9c1018;
}
```
### HOME PAGE HTML CODE:
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Apple Watch</title>
    <link rel="stylesheet" href="./css/layout.css" />
    <link rel="icon" href="./img/app.png" type="image/x-icon" />
  </head>

  <body>
    <div class="container">
      <div class="banner"></div>				
      <div class="menu">
        <div class="menuitemselected"><a href="/static/home.html">Home</a></div>
        <div class="menuitem"><a href="/static/products.html">Products</a></div>
        <div class="menuitem"><a href="/static/people.html">People</a></div>
        <div class="menuitem"><a href="/static/contactus.html">Contact Us</a></div>
      </div>
      <div class="content">
        <div class="homecontent">
          <h1>About Us</h1>
          <img src="./img/aw80.jpg"/>
          <div class="contenttext">
            At Tally, we believe in the power of technology to make business
            owners efficient, empowered and happier, so they can focus on what
            matters most for their business. We design our products to focus on
            just that to make our products work for you, and not the other way
            around.
            <br />
            Our new product TallyPrime takes this to a new level, making your
            start to automation, or your switch to Tally simpler than ever
            before. You can now discover the product much more easily and make
            the product do more for you, without learning anything new. There is
            greater flexibility as the product adapts to your business and your
            way of working. And the transformed look and feel will only make you
            love the product even more.
            <ul>
              <li>Simple to learn, easier to use</li>
              <li>Insightful , actionable & customizable reports</li>
              <li>Anywhere, anytime and secure access</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="footer">
        Copyright &#169; 2021 EduSoft Private Limited, Developed by Obed Otto.
      </div>
    </div>
  </body>
</html>
```
### PRODUCTS PAGE HTML CODE:
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>APPLE Private Limited</title>
    <link rel="stylesheet" href="./css/layout.css" />
    <link rel="icon" href="./img/app.png" type="image/x-icon" />
  </head>

  <body>
    <div class="container">
      <div class="banner"></div>
      <div class="menu">
        <div class="menuitem"><a href="/static/home.html">Home</a></div>
        <div class="menuitemselected"><a href="/static/products.html">Products</a></div>
        <div class="menuitem"><a href="/static/people.html">People</a></div>
        <div class="menuitem"><a href="/static/contactus.html">Contact Us</a></div>
      </div>
      <div class="content">
        <div class="productcontent">    
          <h1>Our Premium Products</h1>
          <div class="productitems">
              <div class="productitem"> 
                  <div class="itemimage">
                  <img src="/static/img/awse.jpg" alt="product image">
                  </div>
                  <div class="itemname">Apple Watch SE</div>
                  <div class="itemprice">Price: Rs.25,000.00 </div>
                  <a href="payform.html" target="_blank" ><button>Buy now</button></a>
              </div>
              <div class="productitem"> 
                  <div class="itemimage">
                  <img src="/static/img/aw8.jpg"  alt="product image">
                  </div>
                  <div class="itemname">Apple Watch 8</div>
                  <div class="itemprice">Price: Rs.40,000.00 </div>
                  <a href="payform.html" target="_blank" ><button>Buy now</button></a>
              </div>
              <div class="productitem"> 
                  <div class="itemimage">
                  <img src="/static/img/aw7.jpg"  alt="product image">
                  </div>
                  <div class="itemname">Apple Watch 7</div>
                  <div class="itemprice">Price: Rs.35,000.00 </div>
                  <a href="payform.html" target="_blank" ><button>Buy now</button></a>
              </div>
              <div class="productitem"> 
                  <div class="itemimage">
                  <img src="/static/img/aw5.jpg"  alt="product image">
                  </div>
                  <div class="itemname">Apple Watch 5</div>
                  <div class="itemprice">Price: Rs.20,000.00 </div>
                  <a href="payform.html" target="_blank" ><button>Buy now</button></a>
              </div>
              <div class="productitem"> 
                  <div class="itemimage">
                  <img src="/static/img/aw4.jpg"  alt="product image">
                  </div>
                  <div class="itemname">Apple Watch 4</div>
                  <div class="itemprice">Price: Rs.17,000.00 </div>
                  <a href="payform.html" target="_blank" ><button>Buy now</button></a>
              </div>
              <div class="productitem"> 
                  <div class="itemimage">
                  <img src="/static/img/aw3.jpg"  alt="product image">
                  </div>
                  <div class="itemname">Apple Watch 3</div>
                  <div class="itemprice">Price: Rs.15,000.00 </div>
                  <a href="payform.html" target="_blank" ><button>Buy now</button></a>
              </div>
          </div>
          </div>        
      </div>
      <div class="footer">
        Copyright &#169; 2021 EduSoft Private Limited, Developed by Obed Otto.
      </div>
    </div>
  </body>
</html>
```
### PEOPLE PAGE HTML CODE:
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Apple Watch</title>
    <link rel="stylesheet" href="./css/layout.css" />
    <link rel="icon" href="./img/app.png" type="image/x-icon" />
  </head>

  <body>
    <div class="container">
      <div class="banner"></div>					
      <div class="menu">
        <div class="menuitemselected"><a href="/static/home.html">Home</a></div>
        <div class="menuitem"><a href="/static/products.html">Products</a></div>
        <div class="menuitem"><a href="/static/people.html">People</a></div>
        <div class="menuitem"><a href="/static/contactus.html">Contact Us</a></div>
      </div>
      <div class="content">
        <div class="homecontent">
          <h1>About Our CEO</h1>
          <img src="./img/ceo.jpg"/>
          <div class="contenttext">
            <h2>Steve Jobs</h2>
            Steve Jobs was a charismatic pioneer of the personal computer era. With Steve Wozniak, Jobs founded Apple Inc. in 1976 and transformed the company into a world leader in telecommunications. Widely considered a visionary and a genius, he oversaw the launch of such revolutionary products as the iPod and the iPhone.
            <br />
            <h2>Tim Cook</h2>
            Timothy Donald Cook (born November 1, 1960) is an American business executive who has been the chief executive officer of Apple Inc. since 2011. Cook previously served as the company's chief operating officer under its co-founder Steve Jobs. 
            <h2>Similarities Between Steve Jobs and Tim Cook </h2>
            <ul>
              <li><h4>Creating Buildup: </h4>Before revealing the new products, both Steve and Tim ensure that they remind people how great Apple products are, especially the iPhone. They walk the audience through a quick history of the iPhone and talk about the values of Apple.</li>
              <li><h4>Superlative Words: </h4>When Steve Jobs described Apple products, it seemed as if it is the best product available in the world and no Company can even match them. While launching iPhone 6, Tim Cook used a similar approach to tell the public just how 'WOW' the Smartphone is and that it beats any other Smartphone out there. Below is a comparison of the words that were used by Steve Jobs and Tim Cook during the launch of iPhone 4 and iPhone 6 respectively.</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="footer">
        Copyright &#169; 2021 EduSoft Private Limited, Developed by Obed Otto.
      </div>
    </div>
  </body>
</html>
```
### CONTACT PAGE HTML CODE:
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Apple Watch</title>
    <link rel="stylesheet" href="./css/layout.css" />
    <link rel="icon" href="./img/app.png" type="image/x-icon" />
  </head>

  <body>
    <div class="container">
      <div class="banner"></div>					
      <div class="menu">
        <div class="menuitemselected"><a href="/static/home.html">Home</a></div>
        <div class="menuitem"><a href="/static/products.html">Products</a></div>
        <div class="menuitem"><a href="/static/people.html">People</a></div>
        <div class="menuitem"><a href="/static/contactus.html">Contact Us</a></div>
      </div>
      <div class="content">
        <div class="homecontent">
          <h1>Contacting Apple</h1>
          <img src="./img/as.jpg"/>
          <div class="contenttext">
            
<h2>Apple Online Service</h2>

Apple.com is a convenient place to purchase Apple products and accessories from Apple. You can buy online or call 000800 040 1966.

You can get information about an order you placed on the Apple Online Store through the Order Status page. If you prefer, you can also get order status or make changes by phone at 000800 040 1966.

            <br />
           
<h2>Registered Office</h2>

<p>19th Floor, Concorde Tower C,</p>
<p>UB City, No.24, Vittal Mallya Road,</p>
<p></p>Bangalore 560001, India.</p>

<p>CIN: U30007KA1996PTC019630</p>

<p>91 80 4045 5150</p> 
<p>Fax: 91 80 4045 5197</p>

<p>bangalore</p>
<p>admin@apple.com</p>

          </div>
        </div>
      </div>
      <div class="footer">
        Copyright &#169; 2021 EduSoft Private Limited, Developed by Obed Otto.
      </div>
    </div>
  </body>
</html>
```

## OUTPUT:

### HOME PAGE OUTPUT:

![image](https://github.com/Yugendaran/softweb/assets/128135616/10c65de1-baf7-483c-8c84-35065ba1067a)


### PRODUCT PAGE OUTPUT:

![image](https://github.com/Yugendaran/softweb/assets/128135616/53d92215-b001-47af-a0f3-33b536046b38)


### PEOPLE PAGE OUTPUT:

![image](https://github.com/Yugendaran/softweb/assets/128135616/c4c1534b-244e-4d16-a79a-c0a1ca812377)


### CONTACT PAGE OUTPUT:
![image](https://github.com/Yugendaran/softweb/assets/128135616/43c388b1-28c0-481a-b65b-db5ca71f0999)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
