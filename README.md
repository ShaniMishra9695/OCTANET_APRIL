# Landing Page Creation Using HTML and CSS

Welcome to this guide on creating a simple landing page using HTML and CSS! In this tutorial, we'll walk you through the process of building a basic landing page layout with HTML for structure and CSS for styling.

## Prerequisites

Before we begin, make sure you have the following:

- Basic understanding of HTML and CSS
- A text editor (e.g., VSCode, Sublime Text, Atom)
- Web browser (Chrome, Firefox, Safari)

## Steps to Create Landing Page

### Step 1: Set up your project

Create a new folder for your project and inside it, create two files: `index.html` and `styles.css`.

### Step 2: HTML Structure
Open `index.html` in your text editor and set up the basic HTML structure:



<!DOCTYPE html>
<html>
    <title>Simple landing page using Html Css </title>
    <style type="text/css">
        *{padding:0; margin:0;box-sizing: border-box;}
        header{
            width: 100%;
            height: 100vh;
            background: linear-gradient(rgba(0,0,0,0.8),rgba(0,0,0,0.2)), url("npg.jpeg");
            background-size: cover;
            font-family: sans-serif;
        }
        nav{
            width: 100%;
            height: 100px;
            color: white;
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
            color: white;
            padding: 10px 20px;
            font-size: 20px;
            position: relative;

        }
        .menu a:before{
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 0%;
            height: 100%;
            border-bottom: 2px solid indianred;
            transition: 0.4s linear;
        }
        .menu a:hover:before {
            width: 90%;
        }
       .register a{
          text-decoration: none;
          color: white;
          padding: 10px 20px;
          font-size: 20px;
          background: indianred;
          border-radius: 8px;
          transition: 0.4s;
       }
       .register a:hover{
        background: transparent;
        border: 1px solid indianred;
       }
       .h-txt {
        max-width: 650px;
        position:absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
        text-align: center;
        color: white;

       }
       .h-txt span{
        letter-spacing: 5px;
       }
       .h-txt h1{
         font-size: 3.5em;

       }
       .h-txt a{
        text-decoration: none;
        background: indianred;
        color: white;
        padding: 10px 20px;
        letter-spacing: 5px;
        transition: 0.4s;
       }
       .h-txt a:hover{
        background: transparent;
        border: 1px solid indianred;
       }
    </style>
    <head>
        <body>
            <header>
                <nav>
                    <div class="logo">
                        Travel-X
                    </div>
                    <div class ="menu">
                        <a href = "#">Home</a>
                        <a href ="#">Hill Station</a>
                        <a href="#">Best Offer's</a>
                        <a href="#">Our Sites</a>
                        <a href="#">Contact</a>
                    </div>
                    <div class="register">
                        <a href="#">Register</a>
                    </div>
                </nav>
                <section class="h-txt">
                    <span>Enjoy</span>
                    <h1>International Travel Agency</h1>

                    <br>
                    <a href="#">Book Your Trip</a>
                </section>
            </header>
        </body>
    </head>
</html>
