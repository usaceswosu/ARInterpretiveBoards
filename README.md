<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home Page</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: grey;
            border: 3px solid black;
        }
        header {
            display: flex;
            align-items: center;
            background-color: darkred;
            border: 3px solid black
            padding: 20px;
        }
        header img {
            width: 150px;
            height: auto;
        }
        .container {
            display: flex;
        }
        .sidebar {
            width: 250px;
            background-color: goldenrod;
            padding: 20px;
            height: 100vh;
        }
        .sidebar h2 {
            font-size: 45px;
            margin-bottom: 20px;
            border: black;
            color: white
        }
        .sidebar ul {
            list-style-type: none;
            padding: 0;
        }
        .sidebar ul li {
            margin-bottom: 10px;
        }
        .sidebar ul li a {
            text-decoration: none;
            color: black;
            word-spacing: 0px;
            font-size: 35px;
        }
        .content {
            flex-grow: 1;
            padding: 20px;
            color: white;
        }
        .video-container {
            text-align: center;
        }
        .video {
            border: 5px solid black;
            width: 100%;
            max-width: 1000px;
            margin: 0 auto 20px auto;
            height: 562.5px;
        }
        .video-tabs {
            display: flex;
            justify-content: center;
            margin-top: 10px;
        }
        .video-tabs button {
            background-color: darkred;
            color: white;
            border: none;
            padding: 10px 20px;
            margin: 25px;
            cursor: pointer;
            font-size: 34px;
        }
        .video-tabs button:hover {
            background-color: ;
        }
    </style>
</head>
<body>

    <header>
        <img src="https://i.imgur.com/oHMjfNz.png" alt="Website Logo">
    </header>

    <div class="container">
        <div class="sidebar">
            <ul>
                <li><a href="Homepage.html">Home</a></li>
                <li><a href="Northwest.html">Northwest</a></li>
                <li><a href="Southpacific.html">South Pacific</a></li>
                <li><a href="Southwest.html">Southwest</a></li>
                <li><a href="mississippiValley.html">Mississippi Valley</a></li>
                <li><a href="Southeast.html">Southeast</a></li>
                <li><a href="GreatLakesAndOhioRiver.html">Great Lakes</a></li>
                <li><a href="NorthAtlantic.html">North Atlantic</a></li>
                <li><a href="PacificOcean.html">Pacific Ocean</a></li>

            </ul>
        </div>

        <div class="content">
            <div class="video-container">
                <iframe class="video" id="mainVideo" src="https://www.youtube.com/embed/dQw4w9WgXcQ" 
                        frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                        allowfullscreen></iframe>

                <div class="video-tabs">
                    <button onclick="changeVideo('https://www.youtube.com/embed/e5UOtzRybzU')">Lake</button>
                    <button onclick="changeVideo('https://www.youtube.com/embed/4NnM9Bu-BU0')">Boat</button>
                    <button onclick="changeVideo('https://www.youtube.com/embed/Gt97WoWfzmo')">Forest</button>
                </div>
            </div>
        </div>
    </div>

    <script>
        function changeVideo(videoUrl) {
            document.getElementById('mainVideo').src = videoUrl;
        }
    </script>

</body>
</html>