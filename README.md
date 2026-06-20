# Psychtoolbox-VisualSearch
Visual Search Task (Psychtoolbox - MATLAB)

This repository contains my implementation of a Visual Search Experiment developed in MATLAB using Psychtoolbox as part of the NeuroLab Course Assignment 2.

> The experiment is based on the visual search paradigm described in:
> 
> 
> 
> Ghazizadeh, A., Griggs, W., & Hikosaka, O. (2016). Object-finding skill created by repeated reward experience. Journal of Vision, 16(10), 17.

**Project Overview**
The task simulates a visual search experiment in which participants search for a high-value (Good) fractal among multiple low-value (Bad) distractors. Mouse position is used to simulate eye movements, while keyboard responses simulate object selection and rejection decisions.

**Features Implemented**

Subject ID and session number collection at the beginning of the experiment.

Four display sizes (3, 5, 7, and 9 objects) assigned randomly.

Random object rotation (1–360°).

Balanced generation of:

Target Present (TP) and Target Absent (TA) trials.

Value and Perceptual object groups.

Equal fractal appearance across all experimental conditions.

State-based experiment flow including:

Fixation period

Stimulus presentation

Response collection

Reward delivery

Inter-trial interval (ITI)

Mouse cursor used as simulated eye gaze.

Keyboard controls:

Space: Accept / Select object

X: Reject trial

Visual feedback using colored rectangles:

Green for Good fractals

Red for Bad fractals

Handling of all experimental outcomes:

No response

Correct rejection

Incorrect rejection

Correct selection

Selection without choosing a fractal

Trial information panel displaying:

Pressed key

Value/Perceptual group

Reward amount

Complete trial logging into a single .mat file.

