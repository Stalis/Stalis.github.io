---
title: Turn-Based System Concept
description: Notes on separating a turn-based game from its interface.
date: 2021-03-03T23:04:00+03:00
tags: [pseudo-3d-js, game-development]
---

## Game responsibilities

- Store the state of game entities.
- Implement game mechanics.
- Run in turns.
- Notify external listeners about changes to the world.

## Interface responsibilities

- Render the current state of visible entities.
- Pass player actions to the game.
- React to changes in game state.

## Event model

An event includes a delay in turns only within the game server. The interface and game exchange commands and results through a shared event format.

## MVC and Event Bus

ECS acts as the model, game state as the view, and the command receiver as the controller. The client reads state, sends commands, and responds to updates. The Event Bus sends commands to the game loop and returns a result: a success flag or a description of state changes.
