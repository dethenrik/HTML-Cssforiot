/*  Complete project details: https://randomnerdtutorials.com/esp32-plot-readings-charts-multiple/  */

html {
  font-family: Arial, Helvetica, sans-serif;
  display: inline-block;
  text-align: center;
}
h1 {
  font-size: 1.8rem;
  color: white;
}
p {
  font-size: 1.4rem;
}

body {
  margin: 0;
}
.content {
  padding: 5%;
}
.card-grid {
  max-width: 1200px;
  margin: 0 auto;
  display: grid;
  grid-gap: 2rem;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
}
.card {
  background-color: white;
  box-shadow: 2px 2px 12px 1px rgba(140,140,140,.5);
}
.card-title {
  font-size: 1.2rem;
  font-weight: bold;
  color: #034078
}
.chart-container {
  padding-right: 5%;
  padding-left: 5%;
}

/*-----------------------------------*/

.topnav {
  overflow: hidden;
  background-color: #333;
  position: relative;
}

/* Hide the links inside the navigation menu (except for logo/home) */
.topnav #myLinks {
  display: none;
}

/* Style navigation menu links */
.topnav a {
  color: white;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
  display: block;
}

/* Style the hamburger menu */
.topnav a.icon {
  background: black;
  display: block;
  position: absolute;
  right: 0;
  top: 0;
}

/* Add a grey background color on mouse-over */


/* Style the active link (or home/logo) */
.active {
  background-color: #000000;
  color: white;
}












<!DOCTYPE html>
<html>
  <head>
    <title>ESP IOT DASHBOARD</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="icon" type="image/png" href="favicon.png">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <link rel="stylesheet" type="text/css" href="style.css">
    <script src="https://code.highcharts.com/highcharts.js"></script>
  </head>
  <body>
    <div class="mobile-container">

      <!-- Top Navigation Menu -->
      <div class="topnav">
        <a class="active">Esp Graf</a>
        <div id="myLinks">
          <a href="#news">News</a>
          <a href="#contact">Contact</a>
          <a href="#about">About</a>
        </div>
        <a href="javascript:void(0);" class="icon" onclick="myFunction()">
          <i class="fa fa-bars"></i>
        </a>
      </div>
      
      
      <div style="padding-left:16px">
          <div class="content">
            <div class="card-grid">
              <div class="card">
                <p class="card-title">Temperature Chart</p>
                <div id="chart-temperature" class="chart-container"></div>
              </div>
            </div>
          </div>
          <script src="script.js"></script>
      </div>
      
      <!-- End smartphone / tablet look -->
      </div>
      <script>
        function myFunction() {
          var x = document.getElementById("myLinks");
          if (x.style.display === "block") {
            x.style.display = "none";
          } else {
            x.style.display = "block";
          }
        }
        </script>
      
      </body>
      </html>
  </body>
</html>
