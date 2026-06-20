# Psychtoolbox Visual Search Task

A MATLAB implementation of a **Visual Search Experiment** developed using **Psychtoolbox** for **NeuroLab Course – Assignment 2**.

---

## Reference

The experiment is based on the visual search paradigm described in:

> Ghazizadeh, A., Griggs, W., & Hikosaka, O. (2016). *Object-finding skill created by repeated reward experience*. *Journal of Vision*, 16(10), 17.

---

## Project Overview

This project simulates a visual search experiment in which participants search for a single **high-value (Good)** fractal among multiple **low-value (Bad)** distractors.

To mimic the original experiment:

- **Mouse position** is used to simulate eye movements.
- **Keyboard input** is used for participant responses.
  - **Space** → Accept / Select object
  - **X** → Reject trial

---

## Features

### Experimental Design

- Collects **Subject ID** and **Session Number** at the start of the experiment.
- Random display sizes:
  - 3 objects
  - 5 objects
  - 7 objects
  - 9 objects
- Random object rotation between **1° and 360°**.
- Balanced trial generation ensuring equal representation of:
  - Target Present (TP)
  - Target Absent (TA)
  - Value group
  - Perceptual group
  - Fractal appearances across all conditions

---

### State-Based Task Flow

Each trial follows the sequence:

1. Fixation
2. Stimulus presentation
3. Response collection
4. Reward delivery
5. Inter-trial interval (ITI)

---

### User Interaction

- Mouse cursor simulates eye gaze.
- Keyboard responses:
  - **Space:** Accept / Select object
  - **X:** Reject trial

---

### Visual Feedback

- 🟩 Green rectangle → Good fractal
- 🟥 Red rectangle → Bad fractal

---

### Supported Trial Outcomes

The implementation handles all experimental conditions:

- No response
- Correct rejection (TA)
- Incorrect rejection (TP)
- Correct selection
- Selection without fixating on a fractal

---

### Information Panel

During each trial, an information panel displays:

- Pressed key
- Experimental group (Value / Perceptual)
- Reward delivered

---

### Data Recording

The experiment records and saves all data into a single `.mat` file, including:

- Subject ID
- Session number
- Display size (DS)
- Trial type (TP / TA)
- Experimental group (Value / Perceptual)
- Fractal identities
- Fractal positions
- Mouse trajectory over time
- Keyboard response
- Reward amount
- Display parameters

---

## Technologies

- MATLAB
- Psychtoolbox
