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
            padding: 20px;
            color: white;
            font-size: 20px;
        }
        body {
            background-image: url('https://example.com/shopping-background.jpg'); /* Replace with your image URL */
            background-color: #f8f9fa; /* Fallback color */
            background-size: cover;
            background-position: center;
            height: 100%;
            margin: 0;
            padding: 0;
        }
        nav .logo {
            color: white;
            font-size: 24px;
            font-weight: bold;
            line-height: 70px;
            padding-left: 20px;
        }
        nav {
            background: #063247;
            box-shadow: 0 3px 15px rgba(0, 0, 0, 0.4);
            overflow: hidden;
        }
        nav ol {
            float: right;
            margin-right: 20px;
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
            font-size: 16px;
            transition: 0.5s;
        }
        nav ol li a:hover,
        nav ol li a.active {
            color: #23dbdb;
        }
        nav ol ol {
            position: absolute;
            top: 100%;
            left: 0;
            background: #063247;
            width: 100%;
            display: none;
        }
        nav ol li:hover > ol {
            display: block;
        }
        nav ol ol li {
            width: 100%;
            display: block;
            border-top: 1px solid #042331;
        }
        nav ol ol li a {
            line-height: 50px;
            padding-left: 30px;
        }
        @media screen and (max-width: 768px) {
            nav {
                height: auto;
            }
            nav ol {
                float: none;
                text-align: center;
                margin: 0;
                padding: 10px 0;
            }
            nav ol li {
                display: block;
            }
            nav ol ol {
                position: static;
                display: block;
                background: none;
            }
            nav ol ol li {
                display: block;
                border: none;
            }
            .home-page-content {
                padding: 20px;
                font-size: 18px;
            }
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
    <div class="home-page-content">
        <h1>Welcome to Shopping Hub</h1>
        <p>Hurry before stock runs out!</p>
    </div>
</body>
</html>
