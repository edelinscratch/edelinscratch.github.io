<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="widht=device-width, initial-scale=1.0">
        <title>All Products - STORE</title>
        <link rel="stylesheet" href="style.css">
        <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">"
    </head>
    <body>
        <div class="container">
            <div class="navbar">
                <div class="logo">
                    <img src="images/logo.png" width="125px">
                </div>
                <nav>
                    <ul id="MenuItems">
                        <li><a href="">Home</a></li>
                        <li><a href="">Products</a></li>
                        <li><a href="">About</a></li>
                        <li><a href="">Contact</a></li>
                        <li><a href="">Account</a></li>
                    </ul>
                </nav> 
                <img src="images/cart.png" width="30px" height="30px">
                <img src="images/menu.png" class="menu-icon"
                onclick="menutoggle()">
            </div>
        </div> 

<!-----------account-page-------------->
<div class="account-page">
    <div class="container">
        <div class="row">
            <div class="col-2">
                <img src="images/image1.png" width="100%">
            </div>
            <div class="col-2">
                <div class="form-container">
                    <div class="form-btn">
                        <span onclick="login()">Login</span>
                        <span onclick="register()">Register</span>
                        <hr id="Indicator">
                    </div>

                    <form id="LoginForm">
                        <input type="text" placeholder="Username">
                        <input type="password" placeholder="password">
                        <button type="submit" class="btn">Login</button>
                        <a href="">Forgot password</a>
                    </form>

                    <form id="RegForm">
                        <input type="text" placeholder="Username">
                        <input type="email" placeholder="Email">
                        <input type="password" placeholder="password">
                        <button type="submit" class="btn">Register</button>
                    </form>
                </div>
            </div>
        </div>
    </div>
</div>

<!----------footer--------->

<div class="footer">
    <div class="container">
        <div class="row">
            <div class="footer-col-1">
                <h3>Download Our App</h3>
                <p>Download App For Android and Ios mobile phone</p>
                <div class="app-logo">
                    <img src="images/play-store.png">
                    <img src="images/app-store.png">
                </div>
            </div>
            
            <div class="footer-col-2">
                <img src="images/logo-white.png">
                <p>Our Purpose is to sustainably make the Pleasure and Benfits of sports accesible to the Many</p> 
            </div>
            <div class="footer-col-3">
                <h3>usefull link</h3>
                <ul>
                    <li>Coupons</li>
                    <li>Blog post</li>
                    <li>Return Policy</li>
                    <li>JOin Affiliate</li>
                </ul>
            </div>
            <div class="footer-col-3">
                <h3>Follow us</h3>
                <ul>
                    <li>Facebook</li>
                    <li>Twitter</li>
                    <li>Instagram</li>
                    <li>Youtube</li>
                </ul>
            </div>
        </div>
        <hr>
        <p class="copyright">Copyright 2020 EDELIN PERIN</p>
    </div>
</div>
<!-----------js for toggle menu---------->
        <script>
            var MenuItems = document.getElementById("MenuItems");

            MenuItems.style.maxHeight = "0px";

            function menutoggle(){
                if(MenuItems.style.maxHeight == "0px")
                {
                    MenuItems.style.maxHeight = "200px";
                }
             else
                {
                    MenuItems.style.maxHeight = "0px";
                }
            }
        </script>

<!--------js for toggle Form-------->

     <script>

     var LoginForm = document.getElementById("LoginForm");
     var RegForm = document.getElementById("RegForm");
     var Indicator = document.getElementById("Indicator");

         function register(){

             RegForm.style.transform = "translateX(0px)";
             LoginForm.style.transform = "translateX(0px)";
             Indicator.style.transform = "translateX(100px)";
         }
         function login(){

             RegForm.style.transform = "translateX(300px)";
             LoginForm.style.transform = "translateX(300px)";
             Indicator.style.transform = "translateX(0px)";
         }

     </script>

 </body> 
</html>
