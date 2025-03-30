<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Coding Skills</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js"></script>
    <style>
        /* General Styles */
        body {
            background: url("bg.jpg") no-repeat center center/cover;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            padding: 20px;
        }

        h1 {
            font-weight: bold;
            font-size: 40px;
            color: white;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.5);
            text-align: center;
            margin-bottom: 20px;
        }

        .skills-container {
            width: 100%;
            max-width: 500px;
            padding: 20px;
            background: rgba(33, 33, 33, 0.8);
            border-radius: 16px;
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(5px);
            text-align: center;
        }

        .skill {
            margin-bottom: 15px;
            text-align: left;
        }

        .skill p {
            font-weight: bold;
            margin-bottom: 5px;
            color: white;
        }

        .progress {
            height: 20px;
            background: rgba(255, 255, 255, 0.3);
            border-radius: 10px;
            overflow: hidden;
        }

        .progress-bar {
            text-align: center;
            font-weight: bold;
            line-height: 20px;
        }

        /* Responsive Design */
        @media (max-width: 600px) {
            h1 {
                font-size: 30px;
            }

            .skills-container {
                max-width: 350px;
                padding: 15px;
            }
        }
    </style>
</head>
<body>

    <h1>MY CODING SKILLS</h1>

    <div class="skills-container">
        <div class="skill">
            <p>HTML - 80%</p>
            <div class="progress">
                <div class="progress-bar bg-primary" style="width: 80%;">80%</div>
            </div>
        </div>

        <div class="skill">
            <p>CSS - 69%</p>
            <div class="progress">
                <div class="progress-bar bg-info" style="width: 69%;">69%</div>
            </div>
        </div>

        <div class="skill">
            <p>Java - 31%</p>
            <div class="progress">
                <div class="progress-bar bg-success" style="width: 31%;">31%</div>
            </div>
        </div>

        <div class="skill">
            <p>PHP - 20%</p>
            <div class="progress">
                <div class="progress-bar bg-warning text-dark" style="width: 20%;">20%</div>
            </div>
        </div>
    </div>
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            let progressBars = document.querySelectorAll(".progress-bar");
    
            progressBars.forEach(bar => {
                let width = bar.style.width;
                bar.style.width = "0%"; // Simulan sa 0%
                setTimeout(() => {
                    bar.style.transition = "width 2s ease-in-out";
                    bar.style.width = width; // Animate papunta sa target percent
                }, 500);
            });
        });
    </script>
    

</body>
</html>
