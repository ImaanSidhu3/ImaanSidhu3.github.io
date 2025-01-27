---
layout: page
title: Minesweeper AI
description: Part 2 of working up to a making a chess engine
img: assets/img/MS_start.png
importance: 2
category: Personal
---

This project is a significant step in my journey toward developing a chess AI, building on my earlier work with a Tic-Tac-Toe AI. The goal was to create an AI capable of solving Minesweeper using logical reasoning. While I incorporated some borrowed code to set up the game visuals and the Minesweeper board class in Pygame, the AI logic was entirely self-developed.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/MS_start.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image shows the start of the Minesweeper Game 
</div>

The AI uses principles of constraint satisfaction and knowledge representation. It deduces safe moves and identifies mines by analyzing neighboring cells and updating a dynamic knowledge base of logical sentences. Through iterative reasoning and inference, the AI ensures safe gameplay while minimizing risks.

<div class="row justify-content-sm-center">
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/MS_before.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col">
        {% include figure.liquid loading="eager" path="assets/img/MS_after.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
<div class="caption">
    In this example, there are no more cells adjacent to a '0' for the AI to select. Instead it must deduce a safe cell near the top by knowing that the cell diagonal to the 1 must be a mine and the cell next to that mine must be safe
</div>

This project honed my skills in Python, Pygame, and AI concepts like inference, logical reasoning, and problem-solving, serving as a stepping stone toward tackling more complex game-solving AIs like chess.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/MS_during.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Here is the terminal view during the game, showing whether the AI is able to calculate a safe move or make a random guess.
</div>

All code for this project is viewable at: [text](https://github.com/ImaanSidhu3/TicTacToe)
