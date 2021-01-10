<html>
<title> Fabbrica </title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">

<style>
body, html {
  height: 100%;
  font-family: "Calibri", sans-serif;
}

.bgimg {
  background-position: center;
  background-size: cover;
  min-height: 75%;
}

.menu {
  display: none;
}
</style>
<body>

<!-- Links (sit on top) -->
<div class="w3-top">
  <div class="w3-row w3-padding w3-black">
    <div class="w3-col s3">
      <a href="#" class="w3-button w3-block w3-grey">HOME</a>
    </div>
    <div class="w3-col s3">
      <a href="#about" class="w3-button w3-block w3-black">ABOUT</a>
    </div>
    <div class="w3-col s3">
      <a href="#menu" class="w3-button w3-block w3-grey">MENU</a>
    </div>
    <div class="w3-col s3">
      <a href="#where" class="w3-button w3-block w3-black">WHERE</a>
    </div>
  </div>
</div>

<!-- Header with image -->
<header class="bgimg w3-display-container w3-grayscale-min" id="home">
  <div class="w3-display-bottomleft w3-center w3-padding-large w3-hide-small">
    <span class="w3-tag">Open from 10am to 10 pm</span>
  </div>
  <div class="w3-display-middle w3-center">
    <span class="w3-text-white" style="font-size:90px">Fabbrica </span>
  </div>
  <div class="w3-display-bottomright w3-center w3-padding-large">
    <span class="w3-text-white"> Ground, 8A, Allenby Rd, Sreepally, Elgin, Kolkata, West Bengal 700020 </span>
  </div>
</header>

<!-- Add a background color and large text to the whole page -->
<div class="w3-sand w3-grayscale w3-large">

<!-- About Container -->
<div class="w3-container" id="about">
  <div class="w3-content" style="max-width:700px">
    <h5 class="w3-center w3-padding-64"><span class="w3-tag w3-wide">About Fabbrica </span></h5>
    <p> This is a restraunt which offers various pizzas and other italian food items . It was founded by Giovanni Agnelli .</p>
    
    <div class="w3-panel w3-leftbar w3-light-grey">
    
      <p>Chef, Founder :Giovanni Angelli </p>
    </div>
   
    <p><strong>Opening hours:</strong> 10 am to 10 pm.</p>
    <p><strong>Address:</strong> 144 A, Ground, 8A, Allenby Rd, Sreepally, Elgin, Kolkata, West Bengal 700020  </p>
  </div>
</div>

Some of the items in the menu are listed below :

<!-- Menu Container -->
<div class="w3-container" id="menu">
  <div class="w3-content" style="max-width:700px">
 
    <h5 class="w3-center w3-padding-48"><span class="w3-tag w3-wide">THE MENU</span></h5>
  
    <div class="w3-row w3-center w3-card w3-padding">
      <a href="javascript:void(0)" onclick="openMenu(event, 'Sides');" id="myLink">
        <div class="w3-col s6 tablink">Sides</div>
      </a>
      <a href="javascript:void(0)" onclick="openMenu(event, 'Pizza');">
        <div class="w3-col s6 tablink">Pizza</div>
      </a>
    </div>

    <div id="Sides" class="w3-container menu w3-padding-48 w3-card">
      <h5> Olives </h5>
      Nocellara , Queen Green & Moroccan Black
    
      <h5>Green Salad</h5>
  Mixed leaves, olive oil, balsamic and parmesian .
      <h5>Burratina </h5>
    Mozzarella stuffed with cream, drizzled wrt olive oil and served with sour cream. 
      <h5>Meat PLate </h5>
      A selection of charcuterie from local cureres . 
   
      
    </div>

    <div id="Pizza" class="w3-container menu w3-padding-48 w3-card">
      <h5>Daily Special </h5>
    
    
      <h5> Lorena </h5>
   
      <h5>Margherita </h5>
     
      <h5>Jon Bon Chovy </h5>
      
      <h5>Wonton Soup </h5>
    
    </div>  
   
  </div>
</div>

<!-- Contact/Area Container -->
<div class="w3-container" id="where" style="padding-bottom:32px;">
  <div class="w3-content" style="max-width:700px">
    <h5 class="w3-center w3-padding-48"><span class="w3-tag w3-wide">WHERE TO FIND US</span></h5>
    <p>Find us at the address mentioned above</p>
 
    
    <p><strong>Reserve</strong> a table, ask for today's special or just send us a message:</p>
    Send your responses <a href="https://forms.gle/1kMhg7TFfXXP7ret8">here!</a>
  </div>
</div>

<!-- End page content -->
</div>

<script>
// Tabbed Menu
function openMenu(evt, menuName) {
  var i, x, tablinks;
  x = document.getElementsByClassName("menu");
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < x.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" w3-dark-grey", "");
  }
  document.getElementById(menuName).style.display = "block";
  evt.currentTarget.firstElementChild.className += " w3-dark-grey";
}
document.getElementById("myLink").click();
</script>

</body>
</html>
