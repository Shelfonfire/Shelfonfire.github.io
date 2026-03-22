---
layout: project
title: "London Grapple MCP"
description: "MCP server for London Grapple BJJ gym — timetables, today's classes, and instructor search across both mats."
technologies: "Python, FastMCP, BeautifulSoup, httpx"
status: live
endpoint: "https://ie34hkubddklctbkd73bfb7g2m0rmqdm.lambda-url.eu-west-2.on.aws/mcp"
github: "https://github.com/Shelfonfire/mcp"
date: 2026-03-08
---

# London Grapple MCP

## Overview

A Model Context Protocol server for the London Grapple BJJ gym timetable. Scrapes the GymDesk schedule widget and exposes class data to AI assistants.

## Tools

- **get_timetable(mat, day)** — weekly timetable, filterable by mat (1/2/all) and day
- **get_classes_today** — all classes happening today across both mats
- **search_classes(query)** — search by class name or instructor

## MCP Endpoint

`https://ie34hkubddklctbkd73bfb7g2m0rmqdm.lambda-url.eu-west-2.on.aws/mcp`
