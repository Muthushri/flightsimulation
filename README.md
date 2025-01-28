<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mental Health Facts</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .container {
            text-align: center;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        button {
            padding: 10px 20px;
            margin-top: 20px;
            border: none;
            border-radius: 5px;
            background-color: #007BFF;
            color: white;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Mental Health Fact</h1>
        <p id="fact"></p>
        <button id="nextFact">Next Fact</button>
    </div>
    <script>
        const mentalHealthFacts = [
            "1 in 5 adults in the U.S. experience mental illness each year.",
            "Mental health disorders can affect anyone, regardless of age, gender, race, or socioeconomic status.",
            "Depression is one of the leading causes of disability worldwide.",
            "Anxiety disorders are the most common mental health disorders in the U.S.",
            "Mental health issues can lead to physical health problems, such as heart disease and diabetes.",
            "Early intervention and treatment can significantly improve outcomes for individuals with mental health disorders.",
            "Stigma surrounding mental health can prevent individuals from seeking help.",
            "Mental health is just as important as physical health.",
            "Regular physical activity can help improve mental health and reduce symptoms of anxiety and depression.",
            "Talking about mental health can help reduce stigma and encourage others to seek help."
        ];

        let currentFactIndex = 0;

        function displayFact() {
            const factElement = document.getElementById('fact');
            factElement.textContent = mentalHealthFacts[currentFactIndex];
        }

        document.getElementById('nextFact').addEventListener('click', () => {
            currentFactIndex = (currentFactIndex + 1) % mentalHealthFacts.length;
            displayFact();
        });

        // Display the first fact on page load
        displayFact();
    </script>
</body>
</html>
# flightsimulation
