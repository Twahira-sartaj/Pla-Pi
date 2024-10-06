<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exoplanet Quiz</title>
    <style>
        body { 
            font-family: Arial, sans-serif; 
            background-color: #0c0049; 
            color: white; 
            margin: 0; 
            padding: 20px; 
            display: flex; 
            flex-direction: column; 
            align-items: center; 
        }
        h1 { 
            margin-bottom: 20px; 
        }
        form { 
            background: rgba(255, 255, 255, 0.1); 
            padding: 20px; 
            border-radius: 8px; 
            width: 100%; 
            max-width: 600px; 
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
        }
        ol { 
            padding-left: 20px; 
        }
        li { 
            margin: 15px 0; 
        }
        label { 
            cursor: pointer; 
        }
        button { 
            background-color: #1a1a1a; 
            color: #fff; 
            border: none; 
            padding: 10px 20px; 
            border-radius: 5px; 
            cursor: pointer; 
            transition: background-color 0.3s; 
        }
        button:hover { 
            background-color: #444; 
        }
        .hidden { 
            display: none; 
        }
        .results { 
            margin-top: 20px; 
            background: rgba(255, 255, 255, 0.1); 
            padding: 20px; 
            border-radius: 8px; 
            width: 100%; 
            max-width: 600px; 
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
        }
        .question { 
            font-weight: bold; 
            color: #FFD700; 
        }
    </style>
</head>
<body>
    <h1>Exoplanet Quiz</h1>
    <form id="quizForm">
        <ol>
            <li>
                <p class="question">What is the name of the first exoplanet discovered?</p>
                <label><input type="radio" name="q1" value="A"> Proxima b</label><br>
                <label><input type="radio" name="q1" value="B"> 51 Pegasi b</label><br>
                <label><input type="radio" name="q1" value="C"> Kepler-22b</label><br>
                <label><input type="radio" name="q1" value="D"> GJ 1214 b</label><br>
            </li>
            <li>
                <p class="question">Which star system has the most exoplanets?</p>
                <label><input type="radio" name="q2" value="A"> TRAPPIST-1</label><br>
                <label><input type="radio" name="q2" value="B"> Proxima Centauri</label><br>
                <label><input type="radio" name="q2" value="C"> Kepler-90</label><br>
                <label><input type="radio" name="q2" value="D"> HD 10180</label><br>
            </li>
            <li>
                <p class="question">Which exoplanet is known as the "water world"?</p>
                <label><input type="radio" name="q3" value="A"> GJ 1214 b</label><br>
                <label><input type="radio" name="q3" value="B"> Kepler-452 b</label><br>
                <label><input type="radio" name="q3" value="C"> Kepler-22b</label><br>
                <label><input type="radio" name="q3" value="D"> HD 40307 g</label><br>
            </li>
            <li>
                <p class="question">Which method is commonly used to discover exoplanets?</p>
                <label><input type="radio" name="q4" value="A"> Transit Method</label><br>
                <label><input type="radio" name="q4" value="B"> Radial Velocity Method</label><br>
                <label><input type="radio" name="q4" value="C"> Direct Imaging</label><br>
                <label><input type="radio" name="q4" value="D"> All of the above</label><br>
            </li>
            <li>
                <p class="question">Which exoplanet is closest to Earth?</p>
                <label><input type="radio" name="q5" value="A"> Proxima Centauri b</label><br>
                <label><input type="radio" name="q5" value="B"> Kepler-186 f</label><br>
                <label><input type="radio" name="q5" value="C"> TRAPPIST-1 e</label><br>
                <label><input type="radio" name="q5" value="D"> GJ 667 Cc</label><br>
            </li>
            <li>
                <p class="question">What is the name of the exoplanet that orbits two stars?</p>
                <label><input type="radio" name="q6" value="A"> Kepler-16b</label><br>
                <label><input type="radio" name="q6" value="B"> Kepler-20e</label><br>
                <label><input type="radio" name="q6" value="C"> Kepler-69c</label><br>
                <label><input type="radio" name="q6" value="D"> Kepler-62f</label><br>
            </li>
            <li>
                <p class="question">Which exoplanet is in the habitable zone of its star?</p>
                <label><input type="radio" name="q7" value="A"> Proxima Centauri b</label><br>
                <label><input type="radio" name="q7" value="B"> Kepler-22b</label><br>
                <label><input type="radio" name="q7" value="C"> TRAPPIST-1e</label><br>
                <label><input type="radio" name="q7" value="D"> All of the above</label><br>
            </li>
            <li>
                <p class="question">What is the primary component of an exoplanet's atmosphere?</p>
                <label><input type="radio" name="q8" value="A"> Hydrogen</label><br>
                <label><input type="radio" name="q8" value="B"> Helium</label><br>
                <label><input type="radio" name="q8" value="C"> Methane</label><br>
                <label><input type="radio" name="q8" value="D"> Varies per exoplanet</label><br>
            </li>
            <li>
                <p class="question">What is the name of the first potentially habitable exoplanet discovered?</p>
                <label><input type="radio" name="q9" value="A"> Kepler-186f</label><br>
                <label><input type="radio" name="q9" value="B"> Kepler-22b</label><br>
                <label><input type="radio" name="q9" value="C"> Proxima Centauri b</label><br>
                <label><input type="radio" name="q9" value="D"> GJ 667 Cc</label><br>
            </li>
            <li>
                <p class="question">Which exoplanet is known for its extremely short orbital period?</p>
                <label><input type="radio" name="q10" value="A"> HD 209458 b</label><br>
                <label><input type="radio" name="q10" value="B"> Kepler-78b</label><br>
                <label><input type="radio" name="q10" value="C"> TRAPPIST-1d</label><br>
                <label><input type="radio" name="q10" value="D"> 51 Pegasi b</label><br>
            </li>
        </ol>
        <button type="button" onclick="submitQuiz()">Submit</button>
    </form>

    <div class="results hidden" id="results">
    <h1>Exoplanet Quiz Results</h1>
    <h2>Your Score: <span id="score"></span> out of 10</h2>
    <ul>
        <li>Q1: 51 Pegasi b</li>
        <li>Q2: Kepler-90</li>
        <li>Q3: GJ 1214 b</li>
        <li>Q4: All of the above</li>
        <li>Q5: Proxima Centauri b</li>
        <li>Q6: Kepler-16b</li>
        <li>Q7: All of the above</li>
        <li>Q8: Varies per exoplanet</li>
        <li>Q9: Kepler-22b</li>
        <li>Q10: Kepler-78b</li>
    </ul>
</div>

    <script>
        const correctAnswers = {
            q1: "B",
            q2: "C",
            q3: "A",
            q4: "D",
            q5: "A",
            q6: "A",
            q7: "D",
            q8: "D",
            q9: "B",
            q10: "B"
        };

        function submitQuiz() {
            const form = document.getElementById('quizForm');
            const results = document.getElementById('results');
            let score = 0;

            for (let q in correctAnswers) {
                const userAnswer = form[q].value;
                if (userAnswer === correctAnswers[q]) {
                    score++;
                }
            }

            form.classList.add('hidden');
            results.classList.remove('hidden');
            document.getElementById('score').textContent = score;
        }
    </script>
</body>
</html>
