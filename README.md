# web-Kurangam
#Html file

<!DOCTYPE html> 
<html lang=”en” dir=”ltr”>
  <head>
    <meta charset=”utf-8”>
    <title>Responsive Navbar | KurangamBhowmik</title>
    <meta name=”viewport” content=”width=device-width, initial-scale=1.0”>
    <link rel=”stylesheet” href=”style.css”>
    <link rel=”stylesheet” href=https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css/>
  </head>
  <body>
    <nav>
      <input type=”checkbox” id=”check”>
      <label for=”check” class=”checkbtn”>
        <I class=”fas fa-bars”></i>
      </label>
      <label class=”logo”>DesignX</label>
      <ul>
        <li><a class=”active” href=”#”>Home</a></li>
        <li><a href=”#”>About</a></li>
        <li><a href=”#”>Services</a></li>
        <li><a href=”#”>Contact</a></li>
        <li><a href=”#”>Feedback</a></li>
      </ul>
    </nav>
    <section></section>
  </body>
</html>



#Css file

*{
  Padding: 0;
  Margin: 0;
  Text-decoration: none;
  List-style: none;
  Box-sizing: border-box;
}
Body{
  Font-family: montserrat;
}
Nav{
  Background: #0082e6;
  Height: 80px;
  Width: 100%;
}
Label.logo{
  Color: white;
  Font-size: 35px;
  Line-height: 80px;
  Padding: 0 100px;
  Font-weight: bold;
}
Nav ul{
  Float: right;
  Margin-right: 20px;
}
Nav ul li{
  Display: inline-block;
  Line-height: 80px;
  Margin: 0 5px;
}
Nav ul li a{
  Color: white;
  Font-size: 17px;
  Padding: 7px 13px;
  Border-radius: 3px;
  Text-transform: uppercase;
}
a.active,a:hover{
  background: #1b9bff;
  transition: .5s;
}
.checkbtn{
  Font-size: 30px;
  Color: white;
  Float: right;
  Line-height: 80px;
  Margin-right: 40px;
  Cursor: pointer;
  Display: none;
}
#check{
  Display: none;
}
@media (max-width: 952px){
  Label.logo{
    Font-size: 30px;
    Padding-left: 50px;
  }
  Nav ul li a{
    Font-size: 16px;
  }
}
@media (max-width: 858px){
  .checkbtn{
    Display: block;
  }
  Ul{
    Position: fixed;
    Width: 100%;
    Height: 100vh;
    Background: #2c3e50;
    Top: 80px;
    Left: -100%;
    Text-align: center;
    Transition: all .5s;
  }
  Nav ul li{
    Display: block;
    Margin: 50px 0;
    Line-height: 30px;
  }
  Nav ul li a{
    Font-size: 20px;
  }
  A:hover,a.active{
    Background: none;
    Color: #0082e6;
  }
  #check:checked ~ ul{
    Left: 0;
  }
}
Section{
  Background: url(bg1.jpg) no-repeat;
  Background-size: cover;
  Height: calc(100vh – 80px);
}

