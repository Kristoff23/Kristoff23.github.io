<!DOCTYPE html>
<html>
<head>
    <style>
        .container {
            display: flex;
            flex-direction: column; /* Stack paintings vertically */
            align-items: flex-start; /* Align paintings to the left */
            padding: 20px;
        }

        .painting-container {
            position: relative; /* Required for absolute positioning of painting info */
            margin-bottom: 20px; /* Added margin for vertical spacing */
        }

        .painting-frame {
            cursor: pointer;
            width: 300px;
            height: 400px;
            position: relative; /* Required for absolute positioning of painting info */
        }

        .painting-info {
            position: absolute; /* Position painting info relative to painting frame */
            top: 0;
            left: 100%; /* Position painting info to the right of painting frame */
            margin-left: 20px;
            width: 300px;
            height: 400px;
            background-color: #f0f0f0;
            display: none;
            padding: 20px;
        }

        .painting-container:hover .painting-info,
        .painting-frame.clicked + .painting-info {
            display: block;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="painting-container">
            <img class="painting-frame" src="Jose Rizal.jpg" alt="Jose Rizal">
            <div class="painting-info">
                <h2>Title of Painting</h2>
                <p>Description of the painting goes here.</p>
                <p>Artist: Leonardo da Vinci</p>
                <p>Year: 1503–1506</p>
            </div>
        </div>
        <!-- Add more paintings below -->
        <div class="painting-container">
            <img class="painting-frame" src="pacquiao.jpg" alt="pacquiao">
            <div class="painting-info">
                <h2>Title of Another Painting</h2>
                <p>Description of another painting goes here.</p>
                <p>Artist: [Artist Name]</p>
                <p>Year: [Year]</p>
            </div>
        </div>
        <!-- Add more paintings as needed -->
    </div>

    <!-- Add more paintings as needed -->
</body>
</html>
