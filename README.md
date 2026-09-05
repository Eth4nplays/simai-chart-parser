# Simai Chart Parser
A simai chart parser that converts .simai chart data into structured CSV data.
Simai is a note syntax for simulating maimai charts.

## Installation Guide
- Clone this repo
- Make sure Python is installed

## Usage guide
- Create a new file named `chart.simai` in the same folder and paste the simai score data into it
- Run the Python program
- There will be 4 different csv printed, with 4 different structured csvs.
    - data_duration.csv (duration of how long the note appears for)
    - data_lane.csv (which lane or area does the note appear in)
    - data_time.csv (at which second of the chart will the note appear)
    - data_type.csv (what type of note does it appear as)

## Limitations
- The parse only supports these notes:
    - Tap
    - Hold
    - Touch and TouchHold
    - Breaks

    Unsupported notes:
    - Slides (only tap part)

- Simai is a complicated note syntax, the parser might have errors.

## Use cases
- This parser was used in a _Scratch_ maimai simulator. Scratch has very limited text parsing features built in, so I created this parser to simplify the simai chart data. You can view it here: https://scratch.mit.edu/projects/1270407926/