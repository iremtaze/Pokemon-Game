# Pokemon Game Repository

## Introduction

Welcome to the Pokemon Text-Based Game! In this adventure-filled journey, you'll embark on a quest to become the ultimate Pokemon trainer. Armed with your wit, strategy, and a trusty team of Pokemon, you'll battle fierce enemies, catch wild creatures, and strive to collect all the badges in the region. This repository contains the implementation of a simple text-based Pokemon game. The game involves battling enemies to win badges and Pokeballs or catching Pokemons using Pokeballs to expand your Pokemon collection.

## Implemented Classes

The repository includes the following four classes:

### 1. Pokemon

#### Private Attributes:
- Name
- Health Points (HP)
- Attack Value (Atk)

#### Methods:
- Constructors: 
  - Default constructor
  - Constructor with name and attack value parameters
  - Copy constructor
- Getters for all attributes

### 2. Pokedex

#### Private Attributes:
- Pokedex Array (Array that holds Pokemon objects)
- Position value

#### Methods:
- Constructor(s)
- `updatePokedex`: Method to add new Pokemons to the Pokedex array, checking for duplicates
- `printPokedex`: Method to print Pokemon names from the Pokedex array

### 3. Player

#### Private Attributes:
- Name
- Pokemon Number
- Pokeball Number
- Badge Number
- Player’s Pokemon (Object of Pokemon Class)
- Player’s Pokedex (Object with Pokedex Class)

#### Methods:
- Constructors
- `showPokemonNumber`: Method to return the number of Pokemons
- `showPokeballNumber`: Method to return the number of Pokeballs
- `showBadgeNumber`: Method to return the number of Badges
- `getPokemon`: Method to return player's Pokemon object
- `battleWon`: Method to update badge and Pokeball numbers after winning a battle
- `catchPokemon`: Method to update Pokemon and Pokeball numbers after catching a Pokemon

### 4. Enemy

#### Private Attributes:
- Name
- Enemy’s Pokemon (Object with Pokemon Class)

#### Methods:
- Constructors
- `getPokemon`: Method to return enemy's Pokemon object
- `getName`: Method to return the name of the enemy

## Necessary Methods Implemented in Main.cpp

- `readEnemyNames`: Method to read enemy names from a file
- `readPokemonNames`: Method to read Pokemon names from a file
- `characterCreate`: Method to create a character (player) with chosen name and Pokemon
- `fightEnemy`: Method for battling an enemy
- `catchPokemon`: Method for catching a Pokemon

## Gameplay

The game offers the following actions:
1. Fight for a badge
2. Catch a Pokemon
3. Display the number of Pokemons
4. Display the number of Pokeballs
5. Display the number of Badges
6. Display the Pokedex
7. Exit the game

## Are You Ready?
Prepare yourself, young trainer, for an epic adventure awaits. The world of Pokemon is vast and full of wonders, waiting for you to explore. So grab your Pokeballs, hone your skills, and embark on a journey that will test your courage, determination, and bond with your Pokemon companions. The path to greatness begins now!
## How to Compile and Your Code:

To compile and run the provided code, use the following commands: (make sure that all the files are in the same directory) 
```bash
g++ -Wall -Werror main.cpp pokemon.cpp pokemon.h -o your_file_name
./your_file_name enemyNames.txt pokemonNames.txt

