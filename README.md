## HTML CODE HERE
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Practice folder</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="css/slicknav.min.css">
    <!--FONTAWESOME CSS LINK HERE-->
    <link rel="stylesheet" href="css/all.min.css">
    <link rel="stylesheet" href="css/fontawesome.min.css">
    <!--CSS LINK HERE-->
    <link rel="stylesheet" href="css/style.css">
    <!--RESPONSIVE LINK HERE-->
    <link rel="stylesheet" href="css/responsive.css">
</head>
<body>
  <div class="container">
    <div id="mobile-menu"></div>

    <div class="topnav" id="myTopnav">
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">News</a></li>
        <li><a href="#">Service</a>

          <ul>
            <li><a href="#">DROPDOWN MENU</a></li>
            <li><a href="#">DROPDOWN MENU</a></li>
            <li><a href="#">DROPDOWN MENU</a>

              <ul>
                <li><a href="#">DROPDOWN MENU</a></li>
                <li><a href="#">DROPDOWN MENU</a></li>
                <li><a href="#">DROPDOWN MENU</a></li>
                <li><a href="#">DROPDOWN MENU</a></li>
                <li><a href="#">DROPDOWN MENU</a></li>
              </ul>

            </li>
            <li><a href="#">DROPDOWN MENU</a></li>
            <li><a href="#">DROPDOWN MENU</a></li>
          </ul>

        </li>
        <li><a href="#">Contract</a></li>
        <li><a href="#">About</a></li>
      </ul>
    </div>

  </div>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
  <script src="js/jquery.slicknav.min.js"></script>
  <script src="js/script.js"></script>
</body>
</html>
```
## CSS CODE HERE
```css
/*=======================================================
BASIC STYLE START HERE
========================================================*/
*{
    margin:0px;
    padding:0px;
    list-style-type:none;
    font-family:"";
    font-size:16px;
    line-height:1.5rem;
    box-sizing:border-box;
    }
.container{
    width:100%;
    max-width:1280px;
    margin:0px auto;
    }
/*=======================================================
BASIC STYLE END HERE
========================================================*/
.topnav{
    width:100%;
    /* overflow:hidden; */
    background-color:rgb(49, 48, 48);
    }
.topnav ul{
    margin:0px;
    padding:0px;
    text-align:center;
    }
.topnav ul li{
    display:inline-block;
    position:relative;
    }
.topnav ul li a{
    display:block;
    font-family:"";
    font-size:18px;
    color:white;
    text-decoration:none;
    padding:12px 18px;
    font-style:normal;
    font-weight:normal;
    transition:0.5s ease;
    }
.topnav ul li ul li{
    display:block;
    }
.topnav ul li:hover a{
    color:rgb(165, 22, 22);
    }
.topnav ul li:hover ul li a{
    color:white;
    }
.topnav ul li ul li:hover a{
    color:rgb(165, 22, 22);
    }
.topnav ul li ul li:hover ul li a{
    color:white;
    }
.topnav ul li ul li ul li:hover a{
    color:rgb(165, 22, 22);
    }
.topnav ul ul{
    width:200px;
    position:absolute;
    background-color:rgb(209, 206, 206);
    display:none;
    }
.topnav ul ul ul{
    left:200px;
    top:0px;
    }
.topnav ul li:hover ul{
    display:block;
    }
.topnav ul li:hover ul ul{
    display:none;
    }
.topnav ul ul li:hover ul{
    display:block;
    }



.slicknav_menu{
    display:none;
    }
```
## JAVASCRIPT CODE HERE
```javascript
$(function(){
    $('#myTopnav').slicknav({
        'label' :'',
        'prependTo':'#mobile-menu'
    });
});
```
