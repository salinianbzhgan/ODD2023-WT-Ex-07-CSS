# Ex-07-CSS
name: suchitra nath dept: IT ref no: 23000325

Aim:
Using CSS media queries, Write the CSS code that implements the given requirements.

modify the webpage's color scheme, Your code should include the base styles and the appropriate media queries for small screens and dark mode preference.
How would you use a media query in CSS to apply different styles to a webpage for mobile devices (with widths less than 600px) and desktop devices (with widths greater than or equal to 600px)? Provide an example CSS snippet to demonstrate your answer.
Explain how you can use CSS media queries to apply different styles based on the orientation (landscape or portrait) of the device. Provide a CSS example where you change the background color of the body based on the orientation.
Describe how you would use media queries to adjust typography (like font size and line spacing) on a website to improve readability across different device sizes, from mobile phones to large desktop monitors. Include a CSS code snippet in your explanation.
Media queries can be used to provide print-friendly styles for web pages. How would you use a media query to change the styling of a webpage when it is printed, such as changing the background to white and hiding non-essential elements? Provide a CSS example.
With the increasing popularity of dark mode in user interfaces, explain how you would use a media query to detect if the user has set their system to prefer a dark color scheme. Provide an example of how you would change the background and text colors of a website based on this preference.
Code-1:
<html>
  <head>
    <style type="text/css">
      body{
        background-color: #f4f4f4;
        color: #333;
      }
      a{
        color: #007bff;
      }
      @media (max-width: 600px) {
        body{
          background-color: #333;
          color: #f4f4f4;
        }
        a{
          color: #28a745;
        }
      }
      @media (prefers-color-scheme: dark) {
        body{
          background-color: #000;
          color: #fff;
        }
        a{
          color: cyan;
        }
      }
    </style>
  </head>
  <body>
    <h1>web development class</h1>
  </body>
</html>
Code-2:
<!DOCTYPE html>
<html>
    <head>
        <style type="text/css">
            @media (max-width: 599px) {
                body{
                    background-color: lightgray;
                }
            }
            @media (min-width: 600px) {
                body {
                    background-color: lightblue;
                }
            }
        </style>
    </head>
    <body>
        <h1>Helloo Welcome back</h1>
    </body>
</html>
Code-3:
<!DOCTYPE html>
<html>
    <head>
        <style type="text/css">
            @media (orientation: portrait) {
                body{
                    background-color: lightpink;
                }
            }
            @media (orientation: landscape) {
                body{
                    background-color: lightblue;
                }
            }
        </style>
    </head>
    <body>
        <h1>saveetha engineering college</h1>
    </body>
</html>
Code-4:
<!DOCTYPE html>
<html>
    <head>
        <style type="text/css">
           /* Default typography styles */
           body {
            font-size: 16px;
            line-height: 1.5;
        }
        /* Media query for mobile devices */
        @media (max-width: 767px) {
            body {
                font-size: 14px;
                line-height: 1.3;
            }
        }
        /* Media query for tablets */
        @media (min-width: 768px) and (max-width: 1023px) {
            body {
                font-size: 16px;
                line-height: 1.4;
            }
        }
        /* Media query for large desktop monitors */
        @media (min-width: 1024px) {
            body {
                font-size: 18px;
                line-height: 1.6;
            }
        }
        </style>
    </head>
    <body>
        <h1>this is an example for responsive topography</h1>
        <h1>lets see how it differs from diffent devices</h1>
    </body>
</html>
Code-5:
<!DOCTYPE html>
<html>
<head>
  <title>Print Styling Example</title>
  <style>
    @media print {
      body {
        background-color: white;
      }

      .non-essential {
        display: none;
      }
    }
  </style>
</head>
<body>
  <h1>Print Styling Example</h1>
  <h1>-salini</h1>
  <p>This is some content that will be visible when the webpage is viewed in a browser, but hidden when printed.</p>
  <p class="non-essential">This is non-essential content that will be hidden when printed.</p>
</body>
</html>
Code-6:
<!DOCTYPE html>
<html>
<head>
  <title>Dark Mode Example</title>
  <style>
    body {
      background-color: white;
      color: black;
    }
    @media (prefers-color-scheme: dark) {
      body {
        background-color: black;
        color: white;
      }
    }
  </style>
</head>
<body>
  <h1>-Dark Mode Example-</h1>
  <p>salini- 23008741- saveetha engineering college</p>
</body>
</html>
