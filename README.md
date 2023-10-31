<!DOCTYPE html>
<html>
    <head>
        <title> Landing Page</title>
        <link href="task1.css" rel="stylesheet">
    </head>
    <body>
        <header>
           <nav>
            <div class="logo">
                Indiana
            </div>
            <div class="menu">
                <a href="#">Home</a>
                <a href="#">Gallery</a>
                <a href="#">About</a>
                <a href="#">Our sites</a>
                <a href="#">Contact</a>
            </div>
            <div class="register">
                <a href="#">Sign Up</a>
            </div>
           </nav>
           <section class="h-txt">
            <span>Enjoy</span><br>
            <h1>India</h1>
            <h2> The Land of diversity and rich history</h2> <br>
            <a href="#">Explore</a>
           </section>
        </header>
    </body>
</html>
css- code:
*{
    padding:0;
    margin:0;
    box-sizing: border-box;
}
header{
    width:100%;
    height:100vh;
    background:linear-gradient(rgba(0,0,0,0.8),rgba(0,0,0,0.2)),url('landing background.jpg');
    background-size: cover;
    font-family: sans-serif;
}
nav{
    width:100%;
    height:100px;
    color:white;
    display:flex;
    justify-content: space-around;
    align-items: center;
}
.logo{
    font-size: 2em;
    letter-spacing: 2px;
}

.menu a{
    text-decoration: none;
    color:white;
    padding: 10px 20px;
    font-size: 20px;
    position: relative;
}
.menu a:before{
    content: '';
    position: absolute;
    top:0;
    left: 0;
    width:0%;
    height: 100%;
    border-bottom: 2px solid indianred;
    transition:0.4 linear;
}
.menu a:hover::before{
      width:99%;
}
.register a{
    text-decoration: none;
    color:white;
    padding: 10px 20px;
    font-size: 20px;
    background: indianred;
    border-radius: 8px;
    transition: .4s;
}
.register a:hover{
    background: transparent;
    border: 1px solid indianred;
}
.h-txt {
    max-width: 100%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform:translate(-50%,-50%);
    text-align: center;
    color: white;
    font-display: inherit;
}
.h-txt span{
    letter-spacing: 5px;
}
.h-txt h1{
    font-size: 3.5em;
    
}

.h-txt a{
    text-decoration: none;
    background-color: indianred;
    color:white;
    padding:1px 20px;
    letter-spacing: 5px;
    border-radius: 8px;
    transition:0.4s;
}
.h-txt a:hover{
    background: transparent;
    border: 1px solid indianred;
}
