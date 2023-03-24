---
layout: post
title: Project "Pomodoro Tracker"
description: Notes on the Project "PomodoroTracker" - A very simplistic Pomodoro Tracker in your Z-Shell
comments: false
tags: [zsh, zshrc, applescript, status-ongoing]
---


![PomoCLI](/assets/gifs/Pomo.gif)

# General Info

I have been recently struggling with the amount of options of Pomodoro-Trackers that are out there. 
Incable of finding a simple Tracker that doesn't include any special features I have set out to build an alternative myself.

# Technical Summary

The Project essentially has two modes of operation:

- **pomoShort:** a 25(work)/5(rest) min split 
- **pomoLong:** a 50(work)/10(rest) min split

Both splits can be repeated as much as they can.

## Installation

### Zsh

This project requires the Z-Shell to work. Get more info [here](https://ohmyz.sh).

### Timer

This project requires the [timer](https://github.com/caarlos0/timer) project to work properly.

### Setup

1. Create / navigate towards your .zshrc file - ```nano ~\.zshrc```
2. Paste the script underneath your PATH variables

That's it! Now you have a quick Pomodoro-CLI for your productivity setup 

# Links and further information

* [Link to the repository](https://github.com/100xA/PomodoroTrackerCLI)

I will be updating the Project regarding my own needs while keeping it as lightweight as possible.
Thanks for reading!
