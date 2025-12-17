# Final-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Passion: Artificial Intelligence</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="header">
        <h1>My Passion: Artificial Intelligence and Creativity</h1>
        <nav>
            <a href="index.html">Back to Professional Home</a> | 
            <a href="resume.html">Résumé</a> |
            <a href="#tableau">Jump to Tableau Viz</a> |
            <a href="joke-app.html">Try My AI-Assisted Joke Generator App</a>
        </nav>
    </div>

    <div class="content">
        <h2>About My Fascination with AI</h2>
        <p>AI is transforming creativity — from generating art to helping code amazing things.</p>

        <img src="https://www.cgspectrum.com/hs-fs/hubfs/what-is-ai-art-impact-on-artists-header-1.webp" alt="AI-generated art illustration" width="600">

        <img src="https://thumbs.dreamstime.com/b/robots-programming-coding-hobby-kid-vector-apps-logic-creativity-skills-projects-challenges-character-people-flat-cartoon-393132308.jpg" alt="Programming as a hobby illustration" width="600">

        <h2>Why I Love Coding and AI</h2>
        <ol>
            <li>It's creative</li>
            <li>Reasons:
                <ul>
                    <li>Solving puzzles</li>
                    <li>Building tools</li>
                    <li>Exploring new ideas</li>
                </ul>
            </li>
            <li>Endless learning</li>
        </ol>

        <h2>An Inspiring Video on AI</h2>
        <iframe width="560" height="315" src="https://www.youtube.com/embed/dk5890BA1dU" title="How AI Could Empower Any Business" allowfullscreen></iframe>

        <h2 id="tableau">Interactive Tableau Visualization</h2>
        <p>Here's a cool interactive dashboard on global renewable energy (explore filters and hover!):</p>
        <script type="module" src="https://public.tableau.com/javascripts/api/tableau.embedding.3.latest.min.js"></script>
        <tableau-viz id="tableauViz" src="https://public.tableau.com/views/WorldEnergyConsumptionDashboard/EnergyDashboard" width="100%" height="800px" toolbar="bottom"></tableau-viz>
    </div>
body {
    background-image: url('https://depositphotos-blog.s3.eu-west-1.amazonaws.com/uploads/2017/07/Soothing-nature-backgrounds-2.jpg');
    background-size: cover;
    background-attachment: fixed;
    font-family: 'Arial', sans-serif;
    color: #333;
    margin: 0;
    padding: 20px;
}

.header {
    background-color: rgba(255, 255, 255, 0.8);
    padding: 20px;
    text-align: center;
    border-radius: 10px;
}

.content {
    background-color: rgba(255, 255, 255, 0.9);
    padding: 30px;
    margin: 20px auto;
    max-width: 900px;
    border-radius: 10px;
}

.footer {
    background-color: rgba(0, 0, 0, 0.7);
    color: white;
    text-align: center;
    padding: 10px;
    border-radius: 10px;
}

h1, h2 {
    font-family: 'Georgia', serif;
    color: #006400;
}

a {
    color: #00008b;
}<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dad Joke Generator (AI-Assisted App)</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(to bottom, #skyblue, #white);
            text-align: center;
            padding: 50px;
            margin: 0;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            background: white;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }
        h1 {
            color: #333;
        }
        #joke {
            font-size: 24px;
            margin: 30px;
            min-height: 100px;
            color: #444;
        }
        button {
            padding: 15px 30px;
            font-size: 18px;
            background: #ff6b6b;
            color: white;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: 0.3s;
        }
        button:hover {
            background: #ff4757;
            transform: scale(1.05);
        }
        a {
            display: block;
            margin-top: 40px;
            color: #0066cc;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Dad Joke Generator</h1>
        <p>Click for a groan-worthy dad joke! (Built with AI collaboration)</p>
        <div id="joke">Click the button to get started!</div>
        <button id="newJoke">New Joke 😂</button>
        <a href="scratch.html">Back to Scratch Page</a>
    </div>

    <script>
        const jokeElement = document.getElementById('joke');
        const button = document.getElementById('newJoke');

        async function fetchJoke() {
            jokeElement.textContent = 'Loading...';
            try {
                const response = await fetch('https://icanhazdadjoke.com/', {
                    headers: { 'Accept': 'application/json' }
                });
                const data = await response.json();
                jokeElement.textContent = data.joke;
            } catch (error) {
                jokeElement.textContent = 'Oops! No joke right now. Try again!';
            }
        }

        button.addEventListener('click', fetchJoke);
        // Load one on start
        fetchJoke();
    </script>
</body>
</html>
    <div class="footer">
        <p>Scratch page created from blank HTML. Professional pages are separate.</p>
    </div>
</body>
</html>
