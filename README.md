<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Front End Development with React.js</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            list-style: none;
            text-decoration: none;
            font-family: 'Roboto', sans-serif;
        }
        .home-page-content {
            text-align: center;
            padding: 200px;
            color: white;
            font-size: 30px;
        }
        body {
            background-image: url(‘https://images.app.goo.gl/GtfjnNspn1naoRQy6’); /* Replace with your image URL */
            height: 100vh;
            width: 100vw;
            position: relative;
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
        }
        nav .logo {
            color: white;
            font-size: 33px;
            font-weight: bold;
            line-height: 70px;
            padding-left: 110px;
        }
        nav {
            height: 70px;
            background: #063247;
            box-shadow: 0 3px 15px rgba(0, 0, 0, 0.4);
        }
        nav ol {
            float: right;
            margin-right: 30px;
        }
        nav ol li {
            display: inline-block;
            position: relative;
        }
        nav ol li a {
            color: white;
            display: block;
            padding: 0 15px;
            line-height: 70px;
            font-size: 20px;
            background: #063247;
            transition: 0.5s;
        }
        nav ol li a:hover,
        nav ol li a.active {
            color: #23dbdb;
        }
        nav ol ol {
            position: absolute;
            top: 70px;
            border-top: 3px solid #23dbdb;
            opacity: 0;
            visibility: hidden;
            transition: 0.3s linear;
        }
        nav ol li:hover > ol {
            opacity: 1;
            visibility: visible;
        }
        nav ol ol li {
            width: 180px;
            display: list-item;
            border: 1px solid #042331;
            border-top: none;
            background: #063247;
        }
        nav ol ol li a {
            line-height: 50px;
        }
    </style>
</head>
<body>
    <nav>
        <label class="logo">Shopping Hub</label>
        <ol>
            <li><a class="active" href="#">Home</a></li>
            <li>
                <a href="#">Categories</a>
                <ol>
                    <li><a href="#">Men</a></li>
                    <li><a href="#">Women</a></li>
                    <li><a href="#">Kids</a></li>
                </ol>
            </li>
            <li><a href="#">Customer Care</a></li>
            <li>
                <a href="#">Account</a>
                <ol>
                    <li><a href="#">Your Orders</a></li>
                    <li><a href="#">Wishlist</a></li>
                </ol>
            </li>
        </ol>
    </nav>
    <div class="overlay">
        <div class="home-page-content">
            <h1 class="text-center home-page-text h1-responsive">Welcome to Shopping Hub</h1>
            <h3 class="text-center home-supporting-text">Hurry before stock runs out!</h3>
        </div>
    </div>
</body>
</html>
