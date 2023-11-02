 <!DOCTYPE html>
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>
        /* Common styles for all views */
        body {
            font-family: Arial, sans-serif;
        }
        h1 {
            text-align: center;
            margin: 20px 0;
        }
        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
        }
        .section {
            background-color: #F0F0F0;
            border: 1px solid #000;
            margin: 10px;
            padding: 20px;
            flex: 1;
            box-sizing: border-box;
            position: relative;
        }
        .section-title {
            position: absolute;
            top: 0;
            right: 0;
            background-color: #333;
            color: #FFF;
            padding: 5px 10px;
            font-size: 25px;
        }

        /* Styles for desktop view (992px and above) */
        @media screen and (min-width: 992px) {
            .section {
                width: 33.33%; /* Equal width for all sections */
            }
        }

        /* Styles for tablet view (768px to 991px) */
        @media screen and (min-width: 768px) and (max-width: 991px) {
            .section {
                width: 50%; /* First 2 sections share the row */
            }
        }

        /* Styles for mobile view (767px and below) */
        @media screen and (max-width: 767px) {
            .section {
                width: 100%; /* Each section in a new row */
            }
        }
    </style>
</head>
<body>
    <h1>Responsive Layout Example</h1>
    <div class="container">
        <div class="section">
            <div class="section-title">Chicken</div>
            <h2>Section 1</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
        <div class="section">
            <div class="section-title">Beef</div>
            <h2>Section 2</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
        <div class="section">
            <div class="section-title">Sushi</div>
            <h2>Section 3</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
    </div>
</body>
</html>

