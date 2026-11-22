# ClanArena

Game Clan and Tournament Manager. A DBMS project for Iqra University.

## What is this?

ClanArena is a database for gaming tournaments. It keeps clans, players, matches, scores, payments and prizes in one place, so nothing has to be written in chats or sheets anymore.

After every match, the clan points and the leaderboard update by themselves using triggers. There is also a chatbot, so anyone can ask "Which clan is first?" and get the answer from the database.

## Problem

Tournaments are tracked by hand in chats, so scores and payments go wrong.

## Objectives

1. Keep all clan, player, match and payment data in one safe database with proper constraints.
2. Update points, winners and the leaderboard automatically using triggers and a front end.
3. Add a chatbot that answers user questions from the database.

## Tables (9)

* Player
* Clan
* Game
* Tournament
* Registration
* Match
* Player_Score
* Payment
* Prize

There are 11 links between them. Two of them are many to many: Clan and Tournament (solved by Registration), and Player and Match (solved by Player_Score).

## ERD

[![ClanArena ERD](ClanArena_ERD.png)](https://github.com/nx7iz/ClanArena/blob/main/ClanArena.drawio.png)

You can open `ClanArena_ERD.xml` in [draw.io](https://app.diagrams.net) to see and edit the diagram.

## Planned data

About 629 entries in total: 120 players, 15 clans, 6 games, 12 tournaments, 60 registrations, 80 matches, 240 player scores, 60 payments and 36 prizes.

## Tools

* MySQL for the database
* Python (Flask or Streamlit) for the front end
* A chatbot that turns questions into queries
* draw.io for the ERD

## Files

* `README.md` is this file
* `ClanArena_ERD.png` is the ERD picture
* `ClanArena_ERD.xml` is the draw.io file

## Status

Proposal stage. The SQL files, data and front end will be added later.

## Author

Muhammad Noman

Shahzaib Sadiq
