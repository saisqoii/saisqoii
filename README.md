<!DOCTYPE html>
<html lang="nl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Escape Room: Doodverklaard</title>
    <style>
        body {
            background-color: #000000;
            color: #ff0000;
            font-family: 'Creepster', sans-serif;
            text-align: center;
        }
        h1 {
            font-size: 3em;
            margin-top: 20px;
        }
        .start-screen, .end-screen, .puzzle {
            display: none;
        }
        #startScreen {
            display: block;
        }
        .btn {
            background-color: #ff0000;
            color: #000;
            padding: 10px 20px;
            font-size: 1.5em;
            border: none;
            cursor: pointer;
            margin-top: 20px;
        }
        .btn:hover {
            background-color: #b30000;
        }
        .puzzle {
            margin-top: 20px;
            font-size: 1.2em;
        }
        .puzzle input {
            padding: 10px;
            font-size: 1.2em;
            border: 1px solid #fff;
            margin-top: 10px;
        }
        .correct {
            color: #00ff00;
        }
        .incorrect {
            color: #ff3333;
        }
        .end-screen h2 {
            font-size: 2.5em;
            margin-top: 20px;
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Creepster&display=swap" rel="stylesheet">
</head>
<body>
    <div id="startScreen">
        <h1>Escape Room: Doodverklaard</h1>
        <p>Welkom bij de escape room geïnspireerd op het boek "Doodverklaard" van Inge Verbruggen. Los de raadsels op om het mysterie rondom Isa Mendock te ontrafelen!</p>
        <button class="btn" onclick="startGame()">Start de game</button>
    </div>

    <!-- Puzzle 1 -->
    <div id="puzzleScreen" class="puzzle">
        <h2>Raadsel 1</h2>
        <p>Wie is het hoofdpersonage van het boek "Doodverklaard"?</p>
        <input type="text" id="answer1" placeholder="Antwoord hier..." />
        <button class="btn" onclick="checkAnswer('answer1', 'Isa Mendock')">Check antwoord</button>
        <p id="response1"></p>
    </div>

    <!-- Puzzle 2 -->
    <div id="puzzleScreen2" class="puzzle">
        <h2>Raadsel 2</h2>
        <p>Isa Mendock wordt op een dag 'doodverklaard'. Wat betekent dit precies voor haar?</p>
        <input type="text" id="answer2" placeholder="Antwoord hier..." />
        <button class="btn" onclick="checkAnswer('answer2', 'Ze wordt officieel als dood verklaard, maar is nog in leven
