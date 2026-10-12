---
title: "Uge 6 - WebSockets og Webhooks"
date: 2026-10-02
---

# Uge 6 - WebSockets og Webhooks

## Fokus denne uge

Denne uge arbejder jeg med WebSockets og Webhooks. Begge teknologier handler om kommunikation mellem systemer, men på forskellige måder.

WebSockets bruges til en vedvarende, tovejs forbindelse mellem klient og server, mens Webhooks typisk bruges til at sende en HTTP-request automatisk, når en bestemt hændelse sker.

## Relevans for quiz-projektet

WebSockets er relevante, fordi quiz-systemet skal understøtte live-funktioner. Det kunne eksempelvis være flere deltagere i samme quiz, hvor spørgsmål, svar, point eller resultater skal opdateres med det samme hos alle deltagere.

Webhooks er mindre centrale for den nuværende version af projektet, men kunne blive relevante, hvis quiz-systemet senere skal sende information til andre systemer, når noget bestemt sker.

## Hvad jeg lavede

_Udfyldes senere._

## Hvad jeg lærte

_Udfyldes senere._

## Udfordringer og overvejelser

En stor overvejelse har denne uge været, hvor og hvordan jeg henter spørgsmål. Der findes et API fra OpenTDB med en stor database af spørgsmål og svar på engelsk. Det er forholdsvis enkelt at arbejde med, men det har også nogle begrænsninger. Vi kan fx ikke bruge billeder, selv styre sværhedsgrader og kategorier helt frit eller få spørgsmålene på dansk.
Derfor er den langsigtede plan at integrere et AI-API, hvor jeg selv kan definere disse parametre. Denne løsning implementeres dog først, når selve backenden fungerer stabilt. Indtil da bruger projektet OpenTDB.
For ikke at gøre resten af programmet afhængigt af én bestemt datakilde bruger jeg interfacet QuestionProvider. Tanken er, at resten af quiz-systemet blot beder en QuestionProvider om spørgsmål, uden at vide om de kommer fra OpenTDB, et AI-API eller en anden kilde. På den måde kan datakilden senere udskiftes uden større ændringer i resten af programmet.

## Refleksion

_Udfyldes senere._