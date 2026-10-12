---
title: "Uge 5 - REST Assured og tests"
date: 2026-10-01
---

# Uge 5 - REST Assured og tests

## Fokus denne uge

Denne uge arbejdede jeg med test af REST API'et ved hjælp af REST Assured. Formålet var at kontrollere, at endpoints returnerer de forventede data og statuskoder.

## Hvad jeg lavede

Jeg skrev integrationstests til API'et og testede blandt andet `GET`, `POST`, `PUT` og `DELETE`. Testene blev kørt mod en rigtig testdatabase, så både API-laget og databaseadgangen blev testet samlet, uden at den rigtige database blev påvirket.

## Hvad jeg lærte

Jeg fik en bedre forståelse for forskellen mellem at teste enkelte metoder og at teste hele flowet gennem API'et. REST Assured gjorde det muligt at sende requests og kontrollere både response body og HTTP-statuskoder.

## Udfordringer og refleksion

En af udfordringerne var, at små forskelle i eksempelvis forventede statuskoder kunne få en test til at fejle. Det gjorde det tydeligt, hvor vigtigt det er, at API'et har en konsekvent og veldefineret opførsel.