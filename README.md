<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bikewale Homepage</title>
    <style>
        body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 10O;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 30px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }

        .navbar {
            display: flex;
            justify-content: space-around;
            background-color: #f8f8f8;
            padding: 10px 0;
            border-bottom: 1px solid #ddd;
        }
        .navbar a {
            text-decoration: none;
            color: #333;
            padding: 10px 20px;
        }
        .navbar a.active {
            color: #007bff;
            border-bottom: 2px solid #007bff;
        }
        .container {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
            padding: 20px;
        }
        .item {
            text-align: center;
        }
        .item img {
            width: 50px;
            height: 50px;
        }
        .item p {
            margin-top: 10px;
            font-size: 14px;
            color: #333;
        }

    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button class="active">TRENDING</button>
            <a href="populartab.html"> <button>POPULAR</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
            <a href="upcomingtab.html"><button>UPCOMING</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="Imagepg6y-1659933227267.avif" alt="Bike Image">
                <div class="details">
                    <h3>Royal Enfield Hunter 350</h3>
                    <p class="price"><strong>₹ 1,49,900</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Ducati panigale.webp" alt="Bike Image">
                <div class="details">
                    <h3>Ducati Panigale V2</h3>
                    <p class="price"><strong>₹ 24,13,207</strong> Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="tvs-jupiter66c8598426d80.avif" alt="Bike Image">
                <div class="details">
                    <h3>TVS Jupiter</h3>
                    <p class="price"><strong>₹ 77,199</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button class="active2">COMMUTER</button>
            <a href="cruisertab.html"><button>CRUISER</button></a>
            <a href="sporttab.html"><button>SPORTS</button></a>
            <a href="touringtab.html"><button>TOURING</button></a>
            <a href="electrictabbikecat.html"><button>ELECTRIC</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="apache rtr 160.jpg" alt="Bike Image">
                <div class="details">
                    <h3>TVS Apache RTR 160</h3>
                    <p class="price"><strong>₹ 1,17,204</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="navbar">
        <a href="#">BRAND</a>
        <a href="#">BUDGET</a>
        <a href="#">DISPLACEMENT</a>
        <a href="#" class="active">BODY STYLE</a>
    </div>
    <table class="table1">
        <br>
        <tr>
            <td><a href="#"><img src="honda logo.png" alt="Honda" class="brand-logo"><br>Honda</a></td>
            <td><a href="#"><img src="royal Enfield logo2.png" alt="Royal Enfield" class="brand-logo"><br>Royal Enfield</a></td>
            <td><a href="#"><img src="Hero-Logo.png" alt="Hero" class="brand-logo"><br>Hero</a></td>
            <td><a href="#"><img src="Bajaj-logo.jpg" alt="Bajaj" class="brand-logo"><br>Bajaj</a></td>
            <td><a href="#"><img src="yamahalogo_ogp.gif" alt="Yamaha" class="brand-logo"><br>Yamaha</a></td>
        </tr>
        <tr>
            <td><a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="TVS" class="brand-logo"><br>TVS</a></td>
            <td><a href="#"><img src="kawasaki logo.webp" alt="Kawasaki" class="brand-logo"><br>Kawasaki</a></td>
            <td><a href="#"><img src="jawa logo.webp" alt="Jawa" class="brand-logo"><br>Jawa</a></td>
            <td><a href="#"><img src="bmw-logo-1997.webp" alt="BMW" class="brand-logo"><br>BMW</a></td>
            <td><a href="#"><img src="KTM-Logo.svg.png" alt="KTM" class="brand-logo"><br>KTM</a></td>
        </tr>
        <tr>
            <td colspan="5" class="view-more"><a href="#">View More Brands</a></td>
        </tr>
    </table>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    
   
    <!-- gauris code -->
    <a href="testing.html">
        <button type="button">Go to Another Page</button>
    </a>
    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>&copyHimanshutech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Budget Selection</title>
    <style>

body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 10O;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 30px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }

        .budget-options {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-left: 250PX;
            margin-top: 20PX;
        }
        .budget-option {
            padding: 10px 20px;
            border: 1px solid #ccc;
            border-radius: 20px;
            cursor: pointer;
        }
        .budget-option.active {
            border: 1px solid teal;
            color: teal;
        }
        .tooltip {
            display: none;
            position: absolute;
            background-color: #fff;
            border: 1px solid #ccc;
            padding: 5px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .budget-option:hover .tooltip {
            display: block;
        }
    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button class="active">TRENDING</button>
            <a href="populartab.html"> <button>POPULAR</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
            <a href="upcomingtab.html"><button>UPCOMING</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="Imagepg6y-1659933227267.avif" alt="Bike Image">
                <div class="details">
                    <h3>Royal Enfield Hunter 350</h3>
                    <p class="price"><strong>₹ 1,49,900</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Ducati panigale.webp" alt="Bike Image">
                <div class="details">
                    <h3>Ducati Panigale V2</h3>
                    <p class="price"><strong>₹ 24,13,207</strong> Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="tvs-jupiter66c8598426d80.avif" alt="Bike Image">
                <div class="details">
                    <h3>TVS Jupiter</h3>
                    <p class="price"><strong>₹ 77,199</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button class="active2">COMMUTER</button>
            <a href="cruisertab.html"><button>CRUISER</button></a>
            <a href="sporttab.html"><button>SPORTS</button></a>
            <a href="touringtab.html"><button>TOURING</button></a>
            <a href="electrictabbikecat.html"><button>ELECTRIC</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="apache rtr 160.jpg" alt="Bike Image">
                <div class="details">
                    <h3>TVS Apache RTR 160</h3>
                    <p class="price"><strong>₹ 1,17,204</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="bike-categories">
        <button>BRAND</button>
        <button class="active2">BUDGET</button>
        
        <button>DISPLACEMNET</button>
        <button>BODY STYLE</button>
    </div>
    <div class="budget-options">
        <div class="budget-option">Under ₹50,000</div>
        <div class="budget-option">Under ₹60,000</div>
        <div class="budget-option">Under ₹70,000</div>
        <div class="budget-option">Under ₹80,000</div>
        <div class="budget-option">Under ₹1 lakh</div>
        <div class="budget-option">Under ₹1.5 lakh</div>
        <div class="budget-option active">
            Under ₹2 lakh
            <div class="tooltip">Best Bikes Under 2 lakh</div>
        </div>
        <div class="budget-option">Above ₹2 lakh</div>
    </div>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    
   
    <!-- gauris code -->
    <a href="testing.html">
        <button type="button">Go to Another Page</button>
    </a>
    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>&copyHimanshutech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CRUISER</title>
    <style>
        body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 0;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 20px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }


        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #000000;
        }
        .details .price {
            font-size: 15px;
            font-weight: bold;
        }


    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button class="active">TRENDING</button>
            <a href="populartab.html"> <button>POPULAR</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
            <a href="upcomingtab.html"><button>UPCOMING</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="Imagepg6y-1659933227267.avif" alt="Bike Image">
                <div class="details">
                    <h3>Royal Enfield Hunter 350</h3>
                    <p class="price"><strong>₹ 1,49,900</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Ducati panigale.webp" alt="Bike Image">
                <div class="details">
                    <h3>Ducati Panigale V2</h3>
                    <p class="price"><strong>₹ 24,13,207</strong> Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="tvs-jupiter66c8598426d80.avif" alt="Bike Image">
                <div class="details">
                    <h3>TVS Jupiter</h3>
                    <p class="price"><strong>₹ 77,199</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button>COMMUTER</button>
            <button class="active2">CRUISER</button>
            <a href="sporttab.html"><button>SPORTS</button></a>
            <a href="touringtab.html"><button>TOURING</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="Indian Springfield.jpg" alt="Bike Image">
                <div class="details">
                    <h3>Indian Springfield </h3>
                    <p class="price">₹ 30,60,000 Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Harley-Davidson Street Glide Special.webp" alt="Bike Image">
                <div class="details">
                    <h3>Harley-Davidson Street Glide Special</h3>
                    <p class="price">₹ 30,93,000 Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="honda-gold-wing6257b3fc639af.webp" alt="Bike Image">
                <div class="details">
                    <h3> Honda Goldwing GT 1800</h3>
                    <p class="price">₹ 28,50,000 Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="bike-categories">
        <button class="active2">BRAND</button>
        <button>BUDGET</button>
        <button>DISPLACEMNET</button>
        <button>BODY STYLE</button>
    </div>
    <table class="table1">
        <br>
        <tr>
            <td><a href="#"><img src="honda logo.png" alt="Honda" class="brand-logo"><br>Honda</a></td>
            <td><a href="#"><img src="royal Enfield logo2.png" alt="Royal Enfield" class="brand-logo"><br>Royal Enfield</a></td>
            <td><a href="#"><img src="Hero-Logo.png" alt="Hero" class="brand-logo"><br>Hero</a></td>
            <td><a href="#"><img src="Bajaj-logo.jpg" alt="Bajaj" class="brand-logo"><br>Bajaj</a></td>
            <td><a href="#"><img src="yamahalogo_ogp.gif" alt="Yamaha" class="brand-logo"><br>Yamaha</a></td>
        </tr>
        <tr>
            <td><a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="TVS" class="brand-logo"><br>TVS</a></td>
            <td><a href="#"><img src="kawasaki logo.webp" alt="Kawasaki" class="brand-logo"><br>Kawasaki</a></td>
            <td><a href="#"><img src="jawa logo.webp" alt="Jawa" class="brand-logo"><br>Jawa</a></td>
            <td><a href="#"><img src="bmw-logo-1997.webp" alt="BMW" class="brand-logo"><br>BMW</a></td>
            <td><a href="#"><img src="KTM-Logo.svg.png" alt="KTM" class="brand-logo"><br>KTM</a></td>
        </tr>
        <tr>
            <td colspan="5" class="view-more"><a href="#">View More Brands</a></td>
        </tr>
    </table>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    
   
    <!-- gauris code -->
    <a href="testing.html">
        <button type="button">Go to Another Page</button>
    </a>
    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>&copyHimanshuTech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Budget Selection</title>
    <style>

body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 10O;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 30px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }

        .budget-options {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-left: 250PX;
            margin-top: 20PX;
        }
        .budget-option {
            padding: 10px 20px;
            border: 1px solid #ccc;
            border-radius: 20px;
            cursor: pointer;
        }
        .budget-option.active {
            border: 1px solid teal;
            color: teal;
        }
        .tooltip {
            display: none;
            position: absolute;
            background-color: #fff;
            border: 1px solid #ccc;
            padding: 5px;
            border-radius: 5px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .budget-option:hover .tooltip {
            display: block;
        }
    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button class="active">TRENDING</button>
            <a href="populartab.html"> <button>POPULAR</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
            <a href="upcomingtab.html"><button>UPCOMING</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="Imagepg6y-1659933227267.avif" alt="Bike Image">
                <div class="details">
                    <h3>Royal Enfield Hunter 350</h3>
                    <p class="price"><strong>₹ 1,49,900</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Ducati panigale.webp" alt="Bike Image">
                <div class="details">
                    <h3>Ducati Panigale V2</h3>
                    <p class="price"><strong>₹ 24,13,207</strong> Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="tvs-jupiter66c8598426d80.avif" alt="Bike Image">
                <div class="details">
                    <h3>TVS Jupiter</h3>
                    <p class="price"><strong>₹ 77,199</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button class="active2">COMMUTER</button>
            <a href="cruisertab.html"><button>CRUISER</button></a>
            <a href="sporttab.html"><button>SPORTS</button></a>
            <a href="touringtab.html"><button>TOURING</button></a>
            <a href="electrictabbikecat.html"><button>ELECTRIC</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="apache rtr 160.jpg" alt="Bike Image">
                <div class="details">
                    <h3>TVS Apache RTR 160</h3>
                    <p class="price"><strong>₹ 1,17,204</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="bike-categories">
        <button>BRAND</button>
        <button>BUDGET</button>
        <button class="active2">DISPLACEMNET</button>
        <button>BODY STYLE</button>
    </div>
    <div class="budget-options">
        <div class="budget-option">Upto 100cc</div>
        <div class="budget-option">100cc-110cc</div>
        <div class="budget-option">110cc-125cc</div>
        <div class="budget-option">125cc-150cc</div>
        <div class="budget-option">150cc-200cc</div>
        <div class="budget-option">200cc-250cc</div>
        <div class="budget-option active">
            250cc-500cc
        </div>
        <div class="budget-option">Above 500cc</div>
    </div>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    
   
    <!-- gauris code -->
    <a href="testing.html">
        <button type="button">Go to Another Page</button>
    </a>
    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>&copyHimanshutech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>electrictab</title>
    <style>
        body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 0;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 20px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #000000;
        }
        .details .price {
            font-size: 15px;
            font-weight: bold;
        }


    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button>TRENDING</button>
                <a href="populartab.html"> <button>POPULAR</button></a>
                <a href="electrictab.html"><button class="active">ELECTRIC</button></a>
                <a href="upcomingtab.html"><button>UPCOMING</button></a>
            </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="tvs iqube-st66a76afa1119c.webp" alt="Bike Image">
                <div class="details">
                    <h3>TVS iQube</h3>
                    <p class="price">₹ 1,17,900 Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="ola s1x.webp" alt="Bike Image">
                <div class="details">
                    <h3>OLA S1 X</h3>
                    <p class="price">₹ 84,992 Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="bajaj chetak.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Chetak</h3>
                    <p class="price">₹ 1,10,496 Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button class="active2">COMMUTER</button>
            <a href="cruisertab.html"><button>CRUISER</button></a>
            <a href="sporttab.html"><button>SPORTS</button></a>
            <a href="touringtab.html"><button>TOURING</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="apache rtr 160.jpg" alt="Bike Image">
                <div class="details">
                    <h3>TVS Apache RTR 160</h3>
                    <p class="price"><strong>₹ 1,17,204</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="bike-categories">
        <button class="active2">BRAND</button>
        <button>BUDGET</button>
        <button>DISPLACEMNET</button>
        <button>BODY STYLE</button>
    </div>
    <table class="table1">
        <br>
        <tr>
            <td><a href="#"><img src="honda logo.png" alt="Honda" class="brand-logo"><br>Honda</a></td>
            <td><a href="#"><img src="royal Enfield logo2.png" alt="Royal Enfield" class="brand-logo"><br>Royal Enfield</a></td>
            <td><a href="#"><img src="Hero-Logo.png" alt="Hero" class="brand-logo"><br>Hero</a></td>
            <td><a href="#"><img src="Bajaj-logo.jpg" alt="Bajaj" class="brand-logo"><br>Bajaj</a></td>
            <td><a href="#"><img src="yamahalogo_ogp.gif" alt="Yamaha" class="brand-logo"><br>Yamaha</a></td>
        </tr>
        <tr>
            <td><a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="TVS" class="brand-logo"><br>TVS</a></td>
            <td><a href="#"><img src="kawasaki logo.webp" alt="Kawasaki" class="brand-logo"><br>Kawasaki</a></td>
            <td><a href="#"><img src="jawa logo.webp" alt="Jawa" class="brand-logo"><br>Jawa</a></td>
            <td><a href="#"><img src="bmw-logo-1997.webp" alt="BMW" class="brand-logo"><br>BMW</a></td>
            <td><a href="#"><img src="KTM-Logo.svg.png" alt="KTM" class="brand-logo"><br>KTM</a></td>
        </tr>
        <tr>
            <td colspan="5" class="view-more"><a href="#">View More Brands</a></td>
        </tr>
    </table>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    
   
    <!-- gauris code -->
    <a href="testing.html">
        <button type="button">Go to Another Page</button>
    </a>
    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>&copyHimanshutech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bikewale Homepage</title>
    <style>
        body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 0;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 20px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }

    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button class="active">TRENDING</button>
            <a href="populartab.html"> <button>POPULAR</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
            <a href="upcomingtab.html"><button>UPCOMING</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="Imagepg6y-1659933227267.avif" alt="Bike Image">
                <div class="details">
                    <h3>Royal Enfield Hunter 350</h3>
                    <p class="price"><strong>₹ 1,49,900</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Ducati panigale.webp" alt="Bike Image">
                <div class="details">
                    <h3>Ducati Panigale V2</h3>
                    <p class="price"><strong>₹ 24,13,207</strong> Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="tvs-jupiter66c8598426d80.avif" alt="Bike Image">
                <div class="details">
                    <h3>TVS Jupiter</h3>
                    <p class="price"><strong>₹ 77,199</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button class="active2">ELECTRIC</button>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="tvs iqube-st66a76afa1119c.webp" alt="Bike Image">
                <div class="details">
                    <h3>TVS iQube</h3>
                    <p class="price">₹ 1,17,900 Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="ola s1x.webp" alt="Bike Image">
                <div class="details">
                    <h3>OLA S1 X</h3>
                    <p class="price">₹ 84,992 Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="bajaj chetak.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Chetak</h3>
                    <p class="price">₹ 1,10,496 Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="bike-categories">
        <button class="active2">BRAND</button>
        <button>BUDGET</button>
        <button>DISPLACEMNET</button>
        <button>BODY STYLE</button>
    </div>
    <table class="table1">
        <br>
        <tr>
            <td><a href="#"><img src="honda logo.png" alt="Honda" class="brand-logo"><br>Honda</a></td>
            <td><a href="#"><img src="royal Enfield logo2.png" alt="Royal Enfield" class="brand-logo"><br>Royal Enfield</a></td>
            <td><a href="#"><img src="Hero-Logo.png" alt="Hero" class="brand-logo"><br>Hero</a></td>
            <td><a href="#"><img src="Bajaj-logo.jpg" alt="Bajaj" class="brand-logo"><br>Bajaj</a></td>
            <td><a href="#"><img src="yamahalogo_ogp.gif" alt="Yamaha" class="brand-logo"><br>Yamaha</a></td>
        </tr>
        <tr>
            <td><a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="TVS" class="brand-logo"><br>TVS</a></td>
            <td><a href="#"><img src="kawasaki logo.webp" alt="Kawasaki" class="brand-logo"><br>Kawasaki</a></td>
            <td><a href="#"><img src="jawa logo.webp" alt="Jawa" class="brand-logo"><br>Jawa</a></td>
            <td><a href="#"><img src="bmw-logo-1997.webp" alt="BMW" class="brand-logo"><br>BMW</a></td>
            <td><a href="#"><img src="KTM-Logo.svg.png" alt="KTM" class="brand-logo"><br>KTM</a></td>
        </tr>
        <tr>
            <td colspan="5" class="view-more"><a href="#">View More Brands</a></td>
        </tr>
    </table>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    
   
    
    <a href="testing.html">
        <button type="button">Go to Another Page</button>
    </a>
    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>©Himanshutech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bikewale Homepage</title>
    <style>
        body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 10O;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 30px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }

    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button class="active">TRENDING</button>
            <a href="populartab.html"> <button>POPULAR</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
            <a href="upcomingtab.html"><button>UPCOMING</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="Imagepg6y-1659933227267.avif" alt="Bike Image">
                <div class="details">
                    <h3>Royal Enfield Hunter 350</h3>
                    <p class="price"><strong>₹ 1,49,900</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Ducati panigale.webp" alt="Bike Image">
                <div class="details">
                    <h3>Ducati Panigale V2</h3>
                    <p class="price"><strong>₹ 24,13,207</strong> Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="tvs-jupiter66c8598426d80.avif" alt="Bike Image">
                <div class="details">
                    <h3>TVS Jupiter</h3>
                    <p class="price"><strong>₹ 77,199</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button class="active2">COMMUTER</button>
            <a href="cruisertab.html"><button>CRUISER</button></a>
            <a href="sporttab.html"><button>SPORTS</button></a>
            <a href="touringtab.html"><button>TOURING</button></a>
            <a href="electrictabbikecat.html"><button>ELECTRIC</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="apache rtr 160.jpg" alt="Bike Image">
                <div class="details">
                    <h3>TVS Apache RTR 160</h3>
                    <p class="price"><strong>₹ 1,17,204</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="bike-categories">
        <button class="active2">BRAND</button>
        <a href="budgettab.html"><button>BUDGET</button></a>
        <a href="displacemnettab.html"><button>DISPLACEMNET</button></a>
        <button>BODY STYLE</button>
    </div>
    <table class="table1">
        <br>
        <tr>
            <td><a href="#"><img src="honda logo.png" alt="Honda" class="brand-logo"><br>Honda</a></td>
            <td><a href="#"><img src="royal Enfield logo2.png" alt="Royal Enfield" class="brand-logo"><br>Royal Enfield</a></td>
            <td><a href="#"><img src="Hero-Logo.png" alt="Hero" class="brand-logo"><br>Hero</a></td>
            <td><a href="#"><img src="Bajaj-logo.jpg" alt="Bajaj" class="brand-logo"><br>Bajaj</a></td>
            <td><a href="#"><img src="yamahalogo_ogp.gif" alt="Yamaha" class="brand-logo"><br>Yamaha</a></td>
        </tr>
        <tr>
            <td><a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="TVS" class="brand-logo"><br>TVS</a></td>
            <td><a href="#"><img src="kawasaki logo.webp" alt="Kawasaki" class="brand-logo"><br>Kawasaki</a></td>
            <td><a href="#"><img src="jawa logo.webp" alt="Jawa" class="brand-logo"><br>Jawa</a></td>
            <td><a href="#"><img src="bmw-logo-1997.webp" alt="BMW" class="brand-logo"><br>BMW</a></td>
            <td><a href="#"><img src="KTM-Logo.svg.png" alt="KTM" class="brand-logo"><br>KTM</a></td>
        </tr>
        <tr>
            <td colspan="5" class="view-more"><a href="#">View More Brands</a></td>
        </tr>
    </table>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    
   
    <!-- gauris code -->
    <a href="testing.html">
        <button type="button">Go to Another Page</button>
    </a>
    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>&copyHimanshutech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Populartab</title>
    <style>
        body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 0;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 20px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }


        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #000000;
        }
        .details .price {
            font-size: 15px;
            
        }



    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button>TRENDING</button>
            <a href="populartab.html"> <button class="active">POPULAR</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
            <a href="upcomingtab.html"><button>UPCOMING</button></a>
        </div>
       
    <div class="bike-listings">
        <div class="bike-listing">
            <img src="hero xtreme-125r-right-front-three-quarter-2.webp" alt="Bike Image">
            <div class="details">
                <h3>Hero Xtreme 125R</h3>
                <p class="price"><strong>₹ 97,900</strong> Onwards</p>
                <p>Avg. Ex-Showroom price</p>
                <button>Check on-road price</button>
            </div>
        </div>
        <div class="bike-listing">
            <img src="ktm 200 duke.avif" alt="Bike Image">
            <div class="details">
                <h3>KTM 200 Duke</h3>
                <p class="price"><strong>₹ 1,99,207</strong> Onwards</p>
                <P>Avg. Ex-Showroom price</P>
                <button>Check on-road price</button>
            </div>
        </div>
        <div class="bike-listing">
            <img src="bmw-m-1000-r.jpg" alt="Bike Image">
            <div class="details">
                <h3>BMW M 1000 R</h3>
                <p class="price"><strong>₹ 38,00,000</strong> Onwards</p>
                <p>Avg. Ex-Showroom price</p>
                <button>Check on-road price</button>
            </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button class="active2">COMMUTER</button>
            <a href="cruisertab.html"><button>CRUISER</button></a>
            <a href="sporttab.html"><button>SPORTS</button></a>
            <a href="touringtab.html"><button>TOURING</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="apache rtr 160.jpg" alt="Bike Image">
                <div class="details">
                    <h3>TVS Apache RTR 160</h3>
                    <p class="price"><strong>₹ 1,17,204</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="bike-categories">
        <button class="active2">BRAND</button>
        <button>BUDGET</button>
        <button>DISPLACEMNET</button>
        <button>BODY STYLE</button>
    </div>
    <table class="table1">
        <br>
        <tr>
            <td><a href="#"><img src="honda logo.png" alt="Honda" class="brand-logo"><br>Honda</a></td>
            <td><a href="#"><img src="royal Enfield logo2.png" alt="Royal Enfield" class="brand-logo"><br>Royal Enfield</a></td>
            <td><a href="#"><img src="Hero-Logo.png" alt="Hero" class="brand-logo"><br>Hero</a></td>
            <td><a href="#"><img src="Bajaj-logo.jpg" alt="Bajaj" class="brand-logo"><br>Bajaj</a></td>
            <td><a href="#"><img src="yamahalogo_ogp.gif" alt="Yamaha" class="brand-logo"><br>Yamaha</a></td>
        </tr>
        <tr>
            <td><a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="TVS" class="brand-logo"><br>TVS</a></td>
            <td><a href="#"><img src="kawasaki logo.webp" alt="Kawasaki" class="brand-logo"><br>Kawasaki</a></td>
            <td><a href="#"><img src="jawa logo.webp" alt="Jawa" class="brand-logo"><br>Jawa</a></td>
            <td><a href="#"><img src="bmw-logo-1997.webp" alt="BMW" class="brand-logo"><br>BMW</a></td>
            <td><a href="#"><img src="KTM-Logo.svg.png" alt="KTM" class="brand-logo"><br>KTM</a></td>
        </tr>
        <tr>
            <td colspan="5" class="view-more"><a href="#">View More Brands</a></td>
        </tr>
    </table>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>

    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>&copyHimanshutech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>sporttab</title>
    <style>
        body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 0;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 20px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }


        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #000000;
        }
        .details .price {
            font-size: 15px;
        }


    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button class="active">TRENDING</button>
            <a href="populartab.html"> <button>POPULAR</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
            <a href="upcomingtab.html"><button>UPCOMING</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="Imagepg6y-1659933227267.avif" alt="Bike Image">
                <div class="details">
                    <h3>Royal Enfield Hunter 350</h3>
                    <p class="price"><strong>₹ 1,49,900</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Ducati panigale.webp" alt="Bike Image">
                <div class="details">
                    <h3>Ducati Panigale V2</h3>
                    <p class="price"><strong>₹ 24,13,207</strong> Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="tvs-jupiter66c8598426d80.avif" alt="Bike Image">
                <div class="details">
                    <h3>TVS Jupiter</h3>
                    <p class="price"><strong>₹ 77,199</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button class="active2">SPORTS</button>
            <a href="touringtab.html"><button>TOURING</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="Kawasaki Z650.webp" alt="Bike Image">
                <div class="details">
                    <h3>kawasaki z650</h3>
                    <p class="price"><strong>₹ 6,65,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Kawasaki Ninja ZX-4R.webp" alt="Bike Image">
                <div class="details">
                    <h3>Kawasaki Ninja ZX-4R</h3>
                    <p class="price"><strong>₹ 8,49,000</strong> Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Kawasaki Ninja 650.avif" alt="Bike Image">
                <div class="details">
                    <h3>Kawasaki Ninja 650</h3>
                    <p class="price"><strong>₹ 7,16,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="bike-categories">
        <button class="active2">BRAND</button>
        <button>BUDGET</button>
        <button>DISPLACEMNET</button>
        <button>BODY STYLE</button>
    </div>
    <table class="table1">
        <br>
        <tr>
            <td><a href="#"><img src="honda logo.png" alt="Honda" class="brand-logo"><br>Honda</a></td>
            <td><a href="#"><img src="royal Enfield logo2.png" alt="Royal Enfield" class="brand-logo"><br>Royal Enfield</a></td>
            <td><a href="#"><img src="Hero-Logo.png" alt="Hero" class="brand-logo"><br>Hero</a></td>
            <td><a href="#"><img src="Bajaj-logo.jpg" alt="Bajaj" class="brand-logo"><br>Bajaj</a></td>
            <td><a href="#"><img src="yamahalogo_ogp.gif" alt="Yamaha" class="brand-logo"><br>Yamaha</a></td>
        </tr>
        <tr>
            <td><a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="TVS" class="brand-logo"><br>TVS</a></td>
            <td><a href="#"><img src="kawasaki logo.webp" alt="Kawasaki" class="brand-logo"><br>Kawasaki</a></td>
            <td><a href="#"><img src="jawa logo.webp" alt="Jawa" class="brand-logo"><br>Jawa</a></td>
            <td><a href="#"><img src="bmw-logo-1997.webp" alt="BMW" class="brand-logo"><br>BMW</a></td>
            <td><a href="#"><img src="KTM-Logo.svg.png" alt="KTM" class="brand-logo"><br>KTM</a></td>
        </tr>
        <tr>
            <td colspan="5" class="view-more"><a href="#">View More Brands</a></td>
        </tr>
    </table>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    
   
    
    <a href="testing.html">
        <button type="button">Go to Another Page</button>
    </a>
    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>&Himanshutech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>User Reviews</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
        }
        .header {
            background: #fff;
            padding: 20px;
            border-bottom: 2px solid #0b0b0b;
        }
        .header h1 {
            margin: 1px;
        }
        .search-bar {
            margin: 20px 0;
            
        }
        .search-bar input {
            width: 40%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        .reviews {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            border-top: 20px;
        }
        .review {
            background: #fff;
            padding: 5px;
            border: 3px solid #ddd;
            border-radius: 10px;
            width: 30%;
            margin-bottom: 20px;
        }
        .review h3 {
            margin: 10px 0;
        }
        .review p {
            color: #555;
        }
        .review .stars {
            text-align: center;
            
        }
        .review .time {
            color: #999;
        }
        .review .read-more {
            color: #3498db;
            text-decoration: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>User Reviews</h1>
            <p>3000+ unbiased, verified reviews from bike owners. Know the pros and cons of 200+ bike models from real owners.</p>
            <div class="search-bar">
                <input type="text" for="search-bar" placeholder="Search bike e.g. Bajaj Dominar 400">
            </div>
        </div>
        <div class="reviews">
            <div class="review">
                <h3>Dangar Bhautik Pratapbhai</h3>
                <p>Review on <strong>Honda SP 125</strong></p>
                <p class="stars"></p>
                <p class="time">2 weeks ago</p>
                <p>"I have been driving this machine for the last 1.5 years now and giving my..."</p>
                <a href="#" class="read-more">Read Full Review</a>
            </div>
            <div class="review">
                <h3>Pranav</h3>
                <p>Review on <strong>Jawa 42 FJ</strong></p>
                <p class="stars"></p>
                <p class="time">9 hours ago</p>
                <p>"I haven't owned it yet I have driven it many times gone on many road trips..."</p>
                <a href="#" class="read-more">Read Full Review</a>
            </div>
            <div class="review">
                <h3>Harsimar</h3>
                <p>Review on <strong>Hero Xtreme 125R</strong></p>
                <p class="stars"></p>
                <p class="time">10 hours ago</p>
                <p>"I bought this bike from Flipkart for like 87k approx and it's one of the best..."</p>
                <a href="#" class="read-more">Read Full Review</a>
            </div>
        </div>
    </div>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Check On-Road Price</title>
    <style>
        body.form-container1{
            margin: 0;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }
        .form-container {
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 20px;
            color: white;
            max-width: 300px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }
    </style>
</head>
<body class="form-container1">
    <div class="form-container">
        <h2>Check On-Road Price</h2>
        <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
        <select>
            <option>Select City</option>
            <option>Mumbai</option>
            <option>Bangalor</option>
            <option>Delhi</option>
            <option>Ahmedabad</option>
            <option>Kolkata</option>
            <option>Chennai</option>
            <option>Hyderabad</option>
            <option>Pune</option>
            <option>Jaipur</option>
            <option>Surat</option>
            <option>Indore</option>
            <option>Kanpur</option>
            <option>Lucknow</option>
            <option>Bopal</option>
            <option>Gaya</option>
            <option>Kochi</option>
            <option>Nagpur</option>
            <option>Agra</option>
            <option>Navi Mumbai</option>
            <option>Patna</option>
            <option>Ludhiana</option>
            <option>Meerut</option>
            <option>Ranchi</option>
            <option>Gwalior</option>
            <option>Chandigarh</option>
            <option>Guwahati</option>
            <option>Noida</option>
            
        </select>
        <button>Check the on-road price in your city</button>
    </div>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Motorcycle Body Styles</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        .navbar {
            display: flex;
            justify-content: space-around;
            background-color: #f8f8f8;
            padding: 10px 0;
            border-bottom: 1px solid #ddd;
        }
        .navbar a {
            text-decoration: none;
            color: #333;
            padding: 10px 20px;
        }
        .navbar a.active {
            color: #007bff;
            border-bottom: 2px solid #007bff;
        }
        .container {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
            padding: 20px;
        }
        .item {
            text-align: center;
        }
        .item img {
            width: 50px;
            height: 50px;
        }
        .item p {
            margin-top: 10px;
            font-size: 14px;
            color: #333;
        }
    </style>
</head>
<body>
    <div class="navbar">
        <a href="#">BRAND</a>
        <a href="#">BUDGET</a>
        <a href="#">DISPLACEMENT</a>
        <a href="#" class="active">BODY STYLE</a>
    </div>
    <div class="container">
        <div class="item">
            <img src="sports-bike.png" alt="Sports Bike">
            <p>Sports Bike</p>
        </div>
        <div class="item">
            <img src="scooter.png" alt="Scooter">
            <p>Scooter</p>
        </div>
        <div class="item">
            <img src="cruiser.png" alt="Cruiser">
            <p>Cruiser</p>
        </div>
        <div class="item">
            <img src="commuter.png" alt="Commuter">
            <p>Commuter</p>
        </div>
        <div class="item">
            <img src="street-bike.png" alt="Street Bike">
            <p>Street Bike</p>
        </div>
        <div class="item">
            <img src="super-bike.png" alt="Super Bike">
            <p>Super Bike</p>
        </div>
        <div class="item">
            <img src="cafe-racer.png" alt="Cafe Racer">
            <p>Cafe Racer</p>
        </div>
        <div class="item">
            <img src="scrambler.png" alt="Scrambler">
            <p>Scrambler</p>
        </div>
        <div class="item">
            <img src="adventure.png" alt="Adventure">
            <p>Adventure</p>
        </div>
        <div class="item">
            <img src="moped.png" alt="Moped">
            <p>Moped</p>
        </div>
        <div class="item">
            <img src="tourer.png" alt="Tourer">
            <p>Tourer</p>
        </div>
        <div class="item">
            <img src="maxi-scooter.png" alt="Maxi Scooter">
            <p>Maxi Scooter</p>
        </div>
    </div>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>touringtab</title>
    <style>
        body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 0;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 20px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }


        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #000000;
        }
        .details .price {
            font-size: 15px;
        }


    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button class="active">TRENDING</button>
            <a href="populartab.html"> <button>POPULAR</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
            <a href="upcomingtab.html"><button>UPCOMING</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="Imagepg6y-1659933227267.avif" alt="Bike Image">
                <div class="details">
                    <h3>Royal Enfield Hunter 350</h3>
                    <p class="price"><strong>₹ 1,49,900</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Ducati panigale.webp" alt="Bike Image">
                <div class="details">
                    <h3>Ducati Panigale V2</h3>
                    <p class="price"><strong>₹ 24,13,207</strong> Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="tvs-jupiter66c8598426d80.avif" alt="Bike Image">
                <div class="details">
                    <h3>TVS Jupiter</h3>
                    <p class="price"><strong>₹ 77,199</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button class="active2">TOURING</button>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="himalayan-4506565ccada995d.webp" alt="Bike Image">
                <div class="details">
                    <h3>Royal Enfield Himalayan 450</h3>
                    <p class="price"><strong>₹ 2,98,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="KTM 390 Adventure.webp" alt="Bike Image">
                <div class="details">
                    <h3>KTM 390 Adventure</h3>
                    <p class="price"><strong>₹ 2,84,000</strong> Onwards</p>
                    <P>Avg. Ex-Showroom price</P>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="BMW-G-310-GS-bannerup.jpg.asset.1709035857090.jpg" alt="Bike Image">
                <div class="details">
                    <h3>BMW G 310 GS</h3>
                    <p class="price"><strong>₹ 3,30,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="bike-categories">
        <button class="active2">BRAND</button>
        <button>BUDGET</button>
        <button>DISPLACEMNET</button>
        <button>BODY STYLE</button>
    </div>
    <table class="table1">
        <br>
        <tr>
            <td><a href="#"><img src="honda logo.png" alt="Honda" class="brand-logo"><br>Honda</a></td>
            <td><a href="#"><img src="royal Enfield logo2.png" alt="Royal Enfield" class="brand-logo"><br>Royal Enfield</a></td>
            <td><a href="#"><img src="Hero-Logo.png" alt="Hero" class="brand-logo"><br>Hero</a></td>
            <td><a href="#"><img src="Bajaj-logo.jpg" alt="Bajaj" class="brand-logo"><br>Bajaj</a></td>
            <td><a href="#"><img src="yamahalogo_ogp.gif" alt="Yamaha" class="brand-logo"><br>Yamaha</a></td>
        </tr>
        <tr>
            <td><a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="TVS" class="brand-logo"><br>TVS</a></td>
            <td><a href="#"><img src="kawasaki logo.webp" alt="Kawasaki" class="brand-logo"><br>Kawasaki</a></td>
            <td><a href="#"><img src="jawa logo.webp" alt="Jawa" class="brand-logo"><br>Jawa</a></td>
            <td><a href="#"><img src="bmw-logo-1997.webp" alt="BMW" class="brand-logo"><br>BMW</a></td>
            <td><a href="#"><img src="KTM-Logo.svg.png" alt="KTM" class="brand-logo"><br>KTM</a></td>
        </tr>
        <tr>
            <td colspan="5" class="view-more"><a href="#">View More Brands</a></td>
        </tr>
    </table>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    
   
    <!-- gauris code -->
    <a href="testing.html">
        <button type="button">Go to Another Page</button>
    </a>
    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>&Himanshutech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Populartab</title>
    <style>
        body {
            margin: 0;
            font-family: sans-serif;
        }

        header {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #fff;
            padding: 10px;
            border-bottom: 1px solid #ccc;
        }

        header .header {
            display: flex;
            flex-direction: row;
            align-items: center;
            width: 100%;
        }

        header .logo {
            margin-right: 80px;
        }

        header .search {
            flex-grow: 1;
        }

        header .search-bar {
            display: flex;
            flex-direction: row;
            align-items: center;
            background-color: #f0f0f0;
            border-radius: 5px;
            padding: 8px 13px;
           
        }

        header .search-bar input[type="text"] {
            flex-grow: 1;
            padding: 10px;
            border: 1px solid #ccc;
        }

        header .user-actions {
            display: flex;
            flex-direction: row;
            align-items: center;
            margin-left: 20px;
        }

        header .user-actions button {
            margin-right: 3px;
            background-color: transparent;
            border: none;
            margin-left: 10px;
            cursor: pointer;
        }
        header {
            position: sticky;
            top: 0;
            z-index: 1;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: #000;
            text-decoration: none;
        }

        header .user-actions button img {
            width: 20px; 
            height: 20px;
        }


        header .search-bar button {
            background-color: transparent;
            border: none;
            cursor: pointer;
        }

        .hero {
            background-image: url('https://static.vecteezy.com/system/resources/previews/006/038/809/non_2x/motorbike-riders-motorcycle-silhouettes-in-wild-forest-mountain-nature-landscape-background-vector.jpg');
            background-size: cover;
            background-position: center;
            color: #fff;
            text-align: center;
            padding: 100px 0;
        }

        .hero h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            margin-bottom: 20px;
        }

        .hero .search-container {
            display: flex;
            justify-content: center;
            width: 100%;
            max-width: 600px;
            margin: 0 auto;
        }

        .hero input[type="text"] {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: 5px 0 0 5px;
            outline: none;
        }

        .hero button[type="submit"] {
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 12px 20px;
            border-radius: 0 5px 5px 0;
            cursor: pointer;
        }

        .featured-bikes {
            padding: 20px;
            justify-content: space-between;
        
        }

        .featured-bikes h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories {
            display: flex;
            margin-bottom: 5px;
            margin-left: 250px;
        }

        .bike-categories button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
            border-bottom: 2px solid black;
        } 

         .bike-categories button.active {
            background-color: #007bff;
            color: #fff;
        }
        .bike-categories2 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories2 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories2 button {
            background-color: transparent;
            border: none;
            padding: 8px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories2 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
        }

        .bike-categories3 {
            padding: 20px;
            justify-content: space-between;
        }

        .bike-categories3 h2 {
            font-size: 24px;
            margin-bottom: 10px;
            margin-left: 250px;
        }

        .bike-categories3 button {
            background-color: transparent;
            border: none;
            padding: 5px 15px;
            margin-right: 10px;
            border-radius: 5px;
            cursor: pointer;
        } 

         .bike-categories3 button.active2 {
            background-color: #007bff;
            color: #fff;
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #a1a1a1;
        }
        .container1 h2 {
            margin-left: 250px;
        }

        body {
            font-family: Arial, sans-serif;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .card {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .details .price {
            font-size: 15px;
            
        }

        .details .desc {
            margin-top: 10px;
        }

        .details .p {
            text-align: center;
            font-size: 14px;
            margin-bottom: 10px;
        }

        .details .h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .details .button {
            display: inline-block;
            padding: 10px 20px;
            background-color: #008CBA;
            color: white;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            border-radius: 4px;
            cursor: pointer;
        }

        .button:hover {
            background-color: #0069D9;
        }


        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: center;
        }
        th {
            background-color: #f2f2f2;
        }
        .brand-logo {
            width: 100px;
            height: auto;
        }
        .view-more {
            text-align: center;
            padding: 10px;
        }

        .table1 {
            text-align: center;
            border-radius: 20PX solid black;
            margin-left: 250px;
            margin-right: 60px;
            display: inline-block;
            
        }

        .heading {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            padding: 10px;
            text-align: center;
        }
        .footer {
            background-color: #002f5f;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .footer a {
            color: white;
            text-decoration: none;
            margin: 0 10px;
        }
        .footer .social-icons a {
            margin: 0 5px;
        }
        .footer .social-icons img {
            width: 24px;
            height: 24px;
        }
        .footer .app-links img {
            width: 120px;
            height: 120px;
            margin: 10px 5px;
        }
        .footer .brands img {
            width: 100px;
            margin: 10px 15px;
        }
        .footer .bottom-links {
            margin-top: 20px;
        }
        
        .form-container {
            margin: 0;
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/free-vector/bearded-biker-happy-girl-riding-motorbike-sunset-cartoon-vector-illustration_1284-79685.jpg?t=st=1729790655~exp=1729794255~hmac=90880e71e9e8d688ac12d5438d93b5aeb9acfdb5e0bda1191f9ed0e944d2a5d3&w=1060');
            background-size: cover;
            background-position: center;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 40px;
            border-radius: 20px;
            color: white;
            max-width: 400px;
            width: 100%;
        }
        .form-container h2 {
            margin-top: 0;
        }
        .form-container input,
        .form-container select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
        }
        .form-container input[type="text"] {
            background-color: #fff;
            color: #000;
            
        }
        .form-container select {
            background-color: #fff;
            color: #000;
        }
        .form-container button {
            width: 100%;
            padding: 10px;
            background-color: #ff6600;
            border: none;
            border-radius: 5px;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }

        .form-container{
            margin-left: 500px;

        }

        .bike-listings {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }

        .bike-listing {
            margin: 10px;
            width: calc(20.33% - 20px);
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0,0,0,0.1);
        }

        .bike-listing img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px 5px 0 0;
        }

        .bike-listing .details {
            padding: 10px;
            background-color: #fff;
            border-radius: 0 0 5px 5px;
            
        }

        .bike-listing .details h3 {
            font-size: 18px;
            margin-bottom: 5px;
        }

        .bike-listing .details p {
            font-size: 14px;
            margin-bottom: 10px;
        }
        .bike-listing .details button {
            background-color: #fff;
            border: 1px solid #218838;
            color: #218838;
            padding: 8px 16px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 4px;
        }

       .bike-listing .details button:hover {
            background-color: #000000;
        }
        .details .price {
            font-size: 15px;
          
        }


    </style>
</head>
<body>
    <header>
        <a href="kk automotive logo.png" class="logo">Bikewale</a>
        <div class="search">
            <form class="search-bar">
                <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
                <button type="submit"><img src="icons8-search-24.png" alt="Search">
                </button>
            </form>
        </div>
        <div class="user-actions">
            <button>
                <img src="icons8-location-64.png" alt="Location">
            </button>
            <button>
                <img src="icons8-language-50.png" alt="Language">
            </button>
        </div>
    </header>
    <div class="hero">
        <h1>FIND THE RIGHT BIKE</h1>
        <p>Get Comprehensive Information on Bikes!</p>
        <div class="search-container">
            <input type="text" placeholder="Search your bike here, e.g., Royal Enfield Hunter 350">
            <button type="submit">Search</button>
        </div>
          </div>
    </div>
    <div class="featured-bikes">
        <h2>Featured Bikes</h2>
        <div class="bike-categories">
            <button>TRENDING</button>
            <a href="populartab.html"> <button>POPULAR</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
            <a href="upcomingtab.html"><button class="active">UPCOMING</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="kawasaki-klx230-s-review-first-ride.webp" alt="Bike Image">
                <div class="details">
                    <h3>Kawasaki KLX 230 S</h3>
                    <p class="price"><strong>₹ 2.00 - 2.10 Lakh </strong></p>
                    <p>Onwards Estimated Price</p>
                    <p>Oct 2024 (Tentative)Expected Launch
                    </p>
                    <button>Notify Me on Launch</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="hero xoom-160654a693db7de7.webp" alt="Bike Image">
                <div class="details">
                    <h3>Hero Xoom 160</h3>
                    <p class="price"><strong>₹ 1.10 - 1.20 Lakh </strong></p>
                    <p>Onwards Estimated Price</p>
                    <p>Oct 2024 (Tentative)Expected Launch
                    </p>
                    <button>Notify Me on Launch</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="Hero Destini 125.avif" alt="Bike Image">
                <div class="details">
                    <h3>Hero Destini 125</h3>
                    <p class="price"><strong>₹ 0.83 - 0.90 Lakh</strong> </p>
                    <p>Onwards Estimated Price</p>
                    <p>Oct 2024 (Tentative)Expected Launch
                    </p>
                    <button>Notify Me on Launch</button>
                </div>
            </div>
        </div>
    </div>
    <div class="bike-categories2">
        <h2>Bike Categories</h2>
        <div class="bike-categories">
            <button class="active2">COMMUTER</button>
            <a href="cruisertab.html"><button>CRUISER</button></a>
            <a href="sporttab.html"><button>SPORTS</button></a>
            <a href="touringtab.html"><button>TOURING</button></a>
            <a href="electrictab.html"><button>ELECTRIC</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="apache rtr 160.jpg" alt="Bike Image">
                <div class="details">
                    <h3>TVS Apache RTR 160</h3>
                    <p class="price"><strong>₹ 1,17,204</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container1">
        <h2 class="heading">Get Offers on Popular Bikes</h2>
    </div>
<div class="container">
  <div class="card">
    <img src="r15-v46502c5f1a5cd8.webp" alt="R15">
    <div class="details">
    <H3>Yamaha R15M MotoGP Edition</H3>
    <p class="price"><strong>₹ 1,99,461</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src ="bmw.jpg" alt="OLA S1 Pro">
    <div class="details">
     <h3>BMW G310 RR</h3>   
    <p class="price"><strong>₹ 3,07,043</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>

  <div class="card">
    <img src="Kawasaki Ninja H2R.jpg" alt="OLA S1 Pro">
    <div class="details">
    <h3>Kawasaki Ninja H2R</h3>
    <p class="price"><strong>₹ 79,90,000</strong> Onwards</p>
    <p>Avg. Ex-Showroom price</p>
    <a href="#" class="button">Get Best Offer</a>
    </div>
  </div>
</div>
<div class="form-container">
    <h2>Check On-Road Price</h2>
    <input type="text" placeholder="Type to select bike Name eg. Royal Enfield H">
    <select>
        <option>Select City</option>
        <option>Mumbai</option>
        <option>Bangalor</option>
        <option>Delhi</option>
        <option>Ahmedabad</option>
        <option>Kolkata</option>
        <option>Chennai</option>
        <option>Hyderabad</option>
        <option>Pune</option>
        <option>Jaipur</option>
        <option>Surat</option>
        <option>Indore</option>
        <option>Kanpur</option>
        <option>Lucknow</option>
        <option>Bopal</option>
        <option>Gaya</option>
        <option>Kochi</option>
        <option>Nagpur</option>
        <option>Agra</option>
        <option>Navi Mumbai</option>
        <option>Patna</option>
        <option>Ludhiana</option>
        <option>Meerut</option>
        <option>Ranchi</option>
        <option>Gwalior</option>
        <option>Chandigarh</option>
        <option>Guwahati</option>
        <option>Noida</option>
        
    </select>
    <button>Check the on-road price in your city</button>
</div>
<div class="bike-categories3">
    <h2>Browse Bikes By</h2>
    <div class="bike-categories">
        <button class="active2">BRAND</button>
        <button>BUDGET</button>
        <button>DISPLACEMNET</button>
        <button>BODY STYLE</button>
    </div>
    <table class="table1">
        <br>
        <tr>
            <td><a href="#"><img src="honda logo.png" alt="Honda" class="brand-logo"><br>Honda</a></td>
            <td><a href="#"><img src="royal Enfield logo2.png" alt="Royal Enfield" class="brand-logo"><br>Royal Enfield</a></td>
            <td><a href="#"><img src="Hero-Logo.png" alt="Hero" class="brand-logo"><br>Hero</a></td>
            <td><a href="#"><img src="Bajaj-logo.jpg" alt="Bajaj" class="brand-logo"><br>Bajaj</a></td>
            <td><a href="#"><img src="yamahalogo_ogp.gif" alt="Yamaha" class="brand-logo"><br>Yamaha</a></td>
        </tr>
        <tr>
            <td><a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="TVS" class="brand-logo"><br>TVS</a></td>
            <td><a href="#"><img src="kawasaki logo.webp" alt="Kawasaki" class="brand-logo"><br>Kawasaki</a></td>
            <td><a href="#"><img src="jawa logo.webp" alt="Jawa" class="brand-logo"><br>Jawa</a></td>
            <td><a href="#"><img src="bmw-logo-1997.webp" alt="BMW" class="brand-logo"><br>BMW</a></td>
            <td><a href="#"><img src="KTM-Logo.svg.png" alt="KTM" class="brand-logo"><br>KTM</a></td>
        </tr>
        <tr>
            <td colspan="5" class="view-more"><a href="#">View More Brands</a></td>
        </tr>
    </table>
    <div class="bike-categories2">
        <h2>Latest Updates</h2>
        <div class="bike-categories">
            <button class="active2">NEWS</button>
            <a href="cruisertab.html"><button>EXPERT REVIEWS</button></a>
            <a href="sporttab.html"><button>VIDEOS</button></a>
        </div>
        <div class="bike-listings">
            <div class="bike-listing">
                <img src="HONDA_CB1000R_20221222_01_editedB.jpg" alt="Bike Image">
                <div class="details">
                    <h3>2025 Honda CB1000 Hornet launched in the UK</h3>
                    <p>By Rishabh Bhaskar 9 hours ago</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="mt-15-2-06613f88e55a43.webp" alt="Bike Image">
                <div class="details">
                    <h3>Yamaha MT 15 V2</h3>
                    <p class="price"><strong>₹ 1,69,207</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
            <div class="bike-listing">
                <img src="pulsar-150-ns65e02a081ccf1.avif" alt="Bike Image">
                <div class="details">
                    <h3>Bajaj Pulsar NS160</h3>
                    <p class="price"><strong>₹ 1,50,000</strong> Onwards</p>
                    <p>Avg. Ex-Showroom price</p>
                    <button>Check on-road price</button>
                </div>
            </div>
        </div>
    
   
   
        
    <a href="testing.html">
        <button type="button">Go to Another Page</button>
    </a>
    <footer>
        <div class="footer">
            <div class="language">
                <a href="#">Language: English</a> | <a href="#">हिंदी</a>
            </div>
            <br>
            <div class="links">
                <a href="#">About Us</a> | <a href="#">Advertise</a>
            </div>
            <br>
            <div class="social-icons">
                <a href="#"><img src="facebook png.png" alt="Facebook"></a>
                <a href="#"><img src="tweeter png.png" alt="Twitter"></a>
                <a href="#"><img src="youtube png.png" alt="YouTube"></a>
                <a href="#"><img src="linkedin png.png" alt="LinkedIn"></a>
                <a href="#"><img src="instagram png.png" alt="Instagram"></a>
            </div>
            <div class="app-links">
                <a href="#"><img src="appstore png.png" alt="App Store"></a>
                <a href="#"><img src="googlestore png.png" alt="Google Play"></a>
            </div>
            <div class="brands">
                <a href="#"><img src="tvs-logo-tvs-icon-transparent-free-png.webp" alt="tvslogo"></a>
                <a href="#"><img src="bmwlogo png.png" alt="BMW"></a>
                <a href="#"><img src="kawasakilogo png.png" alt="kawasaki"></a>
                <a href="#"><img src="ducati logo png.png" alt="ducati"></a>
                <a href="#"><img src="yamahalogo2 png.png" alt="Yamaha"></a>
                <a href="#"><img src="herologo png.png" alt="hero"></a>
                <a href="#"><img src="bajajlogo png.png" alt="Bajaj"></a>
            </div>
            <div class="bottom-links">
                <p>&copyHimanshutech.</p>
                <a href="#">Visitor Agreement & Privacy Policy</a>
            </div>
        </div>
      
    </footer>
</body>
</html>
