# Agentic Clinic Analyst

This is my final synthesis project for the AI Mastery Capstone. It's an agent that does
the first pass of data analysis for a clinic that doesn't have anybody on staff to do it.

You give it a CSV and one sentence about what you want to know. It reads the file to see
what columns and how many rows there are, then decides on its own which analyses are
worth running. For each one it prints what it's thinking, runs the pandas and matplotlib
code, and reads the result before deciding what to do next. When it's done it writes a
paragraph on each chart and a summary answering the original question.

Gemini does the reasoning and the writing. Pandas and matplotlib do the data work.

## What's in here

- "agentic_analyst.ipynb" - the notebook, run top to bottom
- "healthcare_dataset.csv" - the data, from Kaggle
- "charts/" - the charts from the last run, saved as PNGs
- "requirements.txt" - what you need installed
- "Reflective_Synthesis_Paper.pdf" - the writeup

## Running it

You need a Gemini API key in a ".env" file in this folder:

GEMINI_API_KEY = your_key_here


Then install the requirements and run the notebook top to bottom.

## Capstones integrated

- AI Programming Foundations - the Python implementation
- Conduct a Statistical Analysis Using Python - the cleaning, profiling and charting
- Design of Autonomous and Semi-Autonomous Agentic Workflows - the ReAct loop
- Generative AI Applications - Gemini as the reasoning and writing engine