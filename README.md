<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Midnight Visitor | Mindmap</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #1a1c2c;
            --accent: #ff4757;
            --text-dark: #2f3542;
            --bg-gradient: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }

        /* Fade In Animation */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: var(--bg-gradient);
            background-attachment: fixed;
            color: var(--text-dark);
            margin: 0;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            overflow-x: hidden;
        }

        header {
            text-align: center;
            padding: 50px 20px;
            background: var(--primary);
            color: white;
            border-radius: 20px;
            width: 100%;
            max-width: 900px;
            margin-bottom: 40px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            animation: fadeInUp 0.8s ease-out forwards;
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3rem;
            margin: 0;
            letter-spacing: 2px;
        }

        .container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            width: 100%;
            max-width: 1100px;
        }

        .card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.05);
            border-top: 6px solid var(--accent);
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            opacity: 0; /* Hidden initially for animation */
            animation: fadeInUp 0.8s ease-out forwards;
        }

        /* Staggered Animation Delays */
        .card:nth-child(1) { animation-delay: 0.2s; }
        .card:nth-child(2) { animation-delay: 0.4s; }
        .card:nth-child(3) { animation-delay: 0.6s; }
        .card:nth-child(4) { animation-delay: 0.8s; }

        .card:hover {
            transform: scale(1.05);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        h2 {
            font-family: 'Playfair Display', serif;
            color: var(--primary);
            border-bottom: 2px solid #f1f2f6;
            padding-bottom: 10px;
        }

        li {
            margin-bottom: 15px;
            line-height: 1.6;
            list-style: none;
            padding-left: 20px;
            position: relative;
        }

        li::before {
            content: "✦";
            position: absolute;
            left: 0;
            color: var(--accent);
        }

        .footer {
            margin: 50px 0;
            font-size: 0.8rem;
            color: #777;
            animation: fadeInUp 1s ease-out 1.2s forwards;
            opacity: 0;
        }
    </style>
</head>
<body>

    <header>
        <h1>THE MIDNIGHT VISITOR</h1>
        <p>A Professional Literary Mindmap</p>
    </header>

    <div class="container">
        <div class="card">
            <h2>👥 Characters</h2>
            <ul>
                <li><b>Ausable:</b> The mastermind who relies on 100% wit.</li>
                <li><b>Max:</b> The intruder who fell for the perfect bluff.</li>
                <li><b>Fowler:</b> The writer who learned that appearances deceive.</li>
            </ul>
        </div>

        <div class="card" style="border-top-color: #2ed573;">
            <h2>🏨 Setting</h2>
            <ul>
                <li><b>French Hotel:</b> A top-floor room (6th floor).</li>
                <li><b>The Window:</b> The focal point of the deadly deception.</li>
            </ul>
        </div>

        <div class="card" style="border-top-color: #1e90ff;">
            <h2>🎭 Plot Twist</h2>
            <ul>
                <li><b>The Balcony:</b> A purely imaginary escape route.</li>
                <li><b>The Knock:</b> Just the waiter with a bottle of wine.</li>
            </ul>
        </div>

        <div class="card" style="border-top-color: #ffa502;">
            <h2>💡 Themes</h2>
            <ul>
                <li><b>Perception:</b> Reality vs. Expectation.</li>
                <li><b>Wisdom:</b> Presence of mind beats a pistol.</li>
            </ul>
        </div>
    </div>

    <div class="footer">
        Design by vairalingam7 &bull; GitHub Pages
    </div>

</body>
</html>
