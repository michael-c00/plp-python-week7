# PLP Python Week 7: File Handling in Python

A hands-on project exploring safe file operations, text manipulation, CSV data parsing, and robust error handling in Python, completed as part of the [Power Learn Project](https://academy.powerlearnprojectafrica.org/dashboard) Software Engineering scholarship curriculum.

## Project Files & Structure
- `my_notes.py`: Program that creates text files, appends new content safely without overwriting previous data, reads line-by-line, and counts total lines.
- `my_notes.txt`: Generated text output file storing the saved notes.
- `hubs.csv`: Input dataset containing learner names, hub locations, and scores.
- `report_builder.py`: Data processing script that reads the CSV via `csv.DictReader`, computes pass/fail metrics and averages, handles `FileNotFoundError` gracefully, and writes a summary report.
- `report.txt`: Generated learner performance report.

## Reflection & Question 1 Answer
If the file opening mode `"a"` (append mode) were changed to `"w"` (write mode) when adding the fourth note in `my_notes.py`:
> Opening the file in `"w"` mode immediately truncates (erases) all pre-existing content in `my_notes.txt`. Consequently, the first three notes would be completely wiped out, leaving only `"I added this later"` as the sole line in the file, resulting in a total line count of `1` instead of `4`.
