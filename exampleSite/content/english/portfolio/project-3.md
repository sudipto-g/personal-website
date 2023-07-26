---
title: "Snake++"
date: 2019-05-12T12:14:34+06:00
image: "images/portfolio/item-2.png"
project_url : "https://github.com/sudipto-g/SnakeGame"
categories: ["development"]
description: "An attempt to build a game that was ubiquitious when Nokia cells were around"
draft: false
---

#### Project Requirements

This project was inspired by [this StackExchange post](https://codereview.stackexchange.com/questions/212296/snake-game-in-c-with-sdl) and set of responses.  
Much as the GIF suggests, this project was an attempt to revive the Game I grew up playing frequently on Nokia phones.  
In extension, an option has been set for an AI to play the game.  
(Caveat: the AI is not fool-proof and in a future extension, I wish to handle the corner case wherein the game ends since the AI fails to see the situation where the snake's head hits its tail, owing to its body length being too long).  



#### Project Details

The Standard Controller(), Play(), Render() moves were used to develop this Game Loop, much like all other games.
[![The Game Loop](https://github.com/sudipto-g/SnakeGame/blob/master/code_structure.png)
