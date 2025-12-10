# parallel-text-processing-handler
A text processing system for rule-based analysis of the 'I Have a Dream' speech.
✨ Parallel Text Processing Handler – Speech Analysis Project
By Hepshibha Majji


📌 1. Project Overview

This project is a Parallel Text Processing System built to analyze the speech “I Have a Dream” by Martin Luther King Jr.
The goal is to demonstrate how large text can be processed efficiently using:

Regex-based rule detection

Parallel Processing (multiprocessing)

Automated sentence scoring

Database storage (SQLite)

Visualisation using charts

This pipeline represents a complete text analytics engine, built step-by-step across milestones.

📂 2. Project Structure

<img width="500" height="500" alt="Image Dec 4, 2025, 09_30_33 PM" src="https://github.com/user-attachments/assets/528143e5-d178-453f-a80b-a50f6b5fdae8" />



🧠 3. Problem Statement

To design a Parallel Text Processing Handler capable of:

Reading and splitting large text efficiently

Detecting meaningful patterns using Regex rules

Processing text using parallel multiprocessing

Storing results in CSV + SQLite database

Visualizing insights from the processed text

🎯 4. Why This Data?

Even though the dataset is a speech, it is rich in:

Repeated thematic words (freedom, justice, dream)

Emotion-heavy sentences

Locations, metaphors, and political references

Clear structure useful for rule-based analysis

This makes it ideal for pattern detection, parallel processing, and building a text analytics pipeline.

⚙️ 5. Technologies Used

<img width="500" height="500" alt="Image Dec 4, 2025, 09_38_47 PM" src="https://github.com/user-attachments/assets/5db990b7-0d17-4762-97c7-ff8d1ec81ed4" />



🧩 6. System Architecture

<img width="500" height="500" alt="Image_q5o5anq5o5anq5o5" src="https://github.com/user-attachments/assets/bfb46dae-c742-4e63-a01b-d69faef1f44e" />



🔍 7. Rule Categories Used

A total of 10 rule patterns were created:

Freedom rule

Dream rule

Justice rule

Hope rule

Metaphor rule

Location rule

Positive emotion rule

Negative emotion rule

Repetition rule

People reference rule

Each rule uses regex to detect specific themes or sentence patterns.

🚀 8. How the Pipeline Works


✔ Step 1 – Data Reading

Loads the speech text from the input folder.

✔ Step 2 – Chunk Splitting

Text is divided into paragraphs or grouped lines.

✔ Step 3 – Rule Detection

Each chunk is scanned using regex patterns.

✔ Step 4 – Parallel Processing

Word frequency counting is done using multiprocessing.

✔ Step 5 – Scoring

Chunks are scored based on how many rules they match.

✔ Step 6 – Storage

Output is saved as:

results_dream.csv

matches_all_chunks.csv

chunk_scores.csv

results_dream.db (SQLite DB)

✔ Step 7 – Visualisation

Pie chart → Rule distribution
Bar chart → Word frequency
Histogram → Chunk score distribution

📊 9. Output Files

Your output folder will contain:

CSV files

results_dream.csv- This file contains word frequency counts from the entire speech.

matches_all_chunks.csv-stores every single sentence that matched a rule, along with its chunk number and rule name

chunk_scores.csv- shows how many rules each chunk matched- a "complexity score."

Database

results_dream.db-  A structured database version of your output.

Charts

rule_distribution_pie.png-  shows which rules matched the most sentences.

word_frequency_bar.png- Top 15 meaningful words

chunk_score_histogram.png- shows how many chunks matched 0,1,1,3+ rules.

🧪 10. Sample Results


✔ Rule Matches

Shows which sentences triggered which rule.

✔ Word Frequencies

Identifies top meaningful words in the speech.

✔ Chunk Scores

Shows how many rules each chunk satisfies.

⚠️ 11. Challenges Faced

Identifying the right regex patterns for meaningful detection

Splitting text cleanly into sentences and chunks

Handling inconsistent formatting inside the dataset

Combining multiple rule outputs into a clean structured system

Managing multiple output formats (CSV + DB + charts)

🎓 12. Key Learnings

Working with large text using automation

Designing custom rules using regex

Implementing multiprocessing for faster workflows

Structuring data for real-world analysis

Creating a complete processing pipeline end-to-end

📈 13. Future Scope

Add machine learning models for text classification

Add sentiment analysis and entity extraction

Build a web dashboard for visualising results

Support multiple datasets beyond speeches

✔️ 14. How to Run This Project


Step 1: Clone Repository
git clone https://github.com/Hepshibha-787/parallel-text-processing-handler

Step 2: Open the Notebook
code/final_notebook.ipynb

Step 3: Install Requirements (if any)
pip install matplotlib

Step 4: Run All Cells

The notebook automatically:

Reads input

Runs rules

Creates outputs

Saves results

Generates visualisation

🏁 15. Conclusion

This project demonstrates an end-to-end parallel text processing system that converts raw text into structured insights using rules, scoring, storage, and visualization. It provides a strong foundation for more advanced NLP and automation systems.
