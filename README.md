<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Midnight Visitor | 8-Point Analysis</title>
    <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg: #0b0e14;
            --card: #161b22;
            --accent: #58a6ff;
            --text: #c9d1d9;
            --header: #f0f6fc;
        }

        body {
            background-color: var(--bg);
            color: var(--text);
            font-family: 'Outfit', sans-serif;
            margin: 0;
            padding: 40px 20px;
        }

        .main-title {
            text-align: center;
            font-family: 'Playfair Display', serif;
            font-size: clamp(2rem, 10vw, 4rem);
            color: var(--header);
            margin-bottom: 10px;
        }

        .subtitle {
            text-align: center;
            color: var(--accent);
            text-transform: uppercase;
            letter-spacing: 3px;
            margin-bottom: 50px;
            font-size: 0.9rem;
        }

        .grid-8 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            max-width: 1300px;
            margin: 0 auto;
        }

        .box {
            background: var(--card);
            border: 1px solid #30363d;
            border-radius: 16px;
            padding: 25px;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .box:hover {
            transform: translateY(-10px);
            border-color: var(--accent);
            box-shadow: 0 10px 30px rgba(88, 166, 255, 0.1);
        }

        .box h3 {
            color: var(--accent);
            margin-top: 0;
            font-size: 1.3rem;
            border-bottom: 1px solid #30363d;
            padding-bottom: 10px;
        }

        .box p {
