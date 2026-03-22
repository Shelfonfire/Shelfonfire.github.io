---
layout: project
title: "Peckhamplex Cinema MCP"
description: "MCP server for Peckhamplex cinema showtimes — films, screenings by date, and accessibility info via the Veezi API."
technologies: "Python, FastMCP, httpx, AWS Lambda"
status: live
endpoint: "https://tovxj6sddrwssxhbk4eepq5fpe0kzfqs.lambda-url.eu-west-2.on.aws/mcp"
github: "https://github.com/Shelfonfire/mcp"
date: 2026-03-10
---

# Peckhamplex Cinema MCP

## Overview

A Model Context Protocol server that exposes Peckhamplex cinema data to AI assistants. Pulls real-time film listings and showtimes from the Peckhamplex API.

## Tools

- **get_all_films** — list all films currently showing or coming soon
- **get_screenings_by_film(title)** — search screenings by film name (fuzzy match)
- **get_screenings_by_date(date)** — all screenings on a given date

## Data

Includes accessibility flags: autism-friendly, hard-of-hearing, and watch-with-baby screenings. Booking URLs returned for each showtime.

## MCP Endpoint

`https://tovxj6sddrwssxhbk4eepq5fpe0kzfqs.lambda-url.eu-west-2.on.aws/mcp`
