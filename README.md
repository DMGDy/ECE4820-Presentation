# ECE4820 Senior Design II Presentation Repo

# Claims Investigation Committee Multi-Testing Input Device

Copyright (c) 2024 Dylan Matthew-Garza
All rights reserved.

This project represents original work completed as part of Western Michigan University senior design project in collaboration with ZF Group.

While this repository is public for demonstration and educational purposes, all rights are reserved. Unauthorized copying, modification, distribution, or use for commercial purposes is strictly prohibited without explicit permission from the copyright holder.

Primary architect and implementer: Dylan Matthew-Garza

This should contain all presentations for the class
with directories named by the date to deliver the presentation.

## Marp Transpilation

```
marp <presentation>.md --html
```
When html header or syntax is embedded.


```
marp <presentation>.md --html -o <presentation>.pdf --allow-local-files
```
When html header and output is to be a .pdf format. 

## September 06 Presentation

This uses `marp` to transpile the markdown to an HTML file
that allows a browser presentation rather than a pdf.

```
marp Presentation_0906.md
```
will generate a `Presentation_0906.html` file that you can just put into your browser.


## September 13 Presentation/Progress Report #1

This presentation should contain the following

- Gantt Chart
- Budget Projection
- Progress report /# 1 (from each group member)

## September 27 Presentation/Progress Report #2 

Presentation is similar to last

- Gantt Chart (Progress Made)
- Updated Budget Projection (if any)
- Progress report updated (from each group member)

## Final Presentation
Only run when inside the `FinalPresentation-Release` directory!
```
latexmk -pdf -output-directory=build
```
