---
title: "Uge 4 - REST API"
date: 2026-09-25
---

# Uge 4 - REST API

## Fokus denne uge

Denne uge var fokus på REST API og på at gøre quiz-systemets funktionalitet tilgængelig gennem HTTP-endpoints. Det var et vigtigt skridt, fordi backend nu ikke kun består af Java-klasser og databaseadgang, men kan kommunikere med en klient gennem et API.

## Hvad jeg lavede

Jeg arbejdede med Javalin og oprettede routes og endpoints til quiz-systemet. Controller-laget blev brugt til at modtage HTTP-requests og sende responses tilbage, mens DAO-laget fortsat stod for kommunikationen med databasen.

Jeg arbejdede blandt andet med de almindelige HTTP-metoder som `GET`, `POST`, `PUT` og `DELETE` og med at sende data som JSON.

## Hvad jeg lærte

Jeg fik en bedre forståelse for, hvordan et REST API opdeles i forskellige lag. Routes bestemmer, hvilke URL'er der findes, controlleren håndterer request og response, og DAO-laget arbejder med databasen.

Jeg lærte også mere om HTTP-statuskoder og om, hvorfor det er vigtigt at returnere den rigtige statuskode afhængigt af resultatet af en request.

## Udfordringer og overvejelser

En af udfordringerne var at holde ansvarsområderne adskilt. Det ville være nemt at placere meget logik direkte i endpoints, men det gør koden sværere at vedligeholde. Derfor forsøgte jeg at holde routing, controller-logik og databaseadgang adskilt.

Jeg skulle også tænke over, hvordan entities skulle sendes gennem API'et. Her blev DTO'er relevante, fordi API'ets dataformat ikke nødvendigvis bør være identisk med database-modellen.

## Refleksion

REST API-delen gjorde projektets arkitektur langt tydeligere for mig. De tidligere dele med JPA og databaseadgang blev nu koblet sammen med et interface, som en frontend senere kan kommunikere med.

Det var også her, quiz-projektet begyndte at ligne en rigtig backend-applikation frem for blot et Java-program med en database.