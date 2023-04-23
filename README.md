# Test question randomizer and bubble sheet generator in Python


This is a small project designed to randomize the order of multiple choice questions and 
their answers using Python.

## Included files

1. [shuffle.py](\shuffle.py): A script used to take a `.txt` file with questions and answers, randomize questions and answers within  questions, and produce a `.docx` file.
2. [bubble.py](\bubble.py): A script to produce a bubble sheet with fill in spaces for each answer to each question
3. [example](\example): A folder with an example input and output exam

## How to use `shuffle.py`

1. Produce a .txt file with each question and associated answers in this format:

```{text}
Q.1. Text for question 1
a. Answer a
b. Answer b
c. Answer c
d. Answer d
e. Answer e
```

2. Edit this line in `shuffle.py`, replacing "yourfile.txt" with the name of the file from step 1:

```{python}

# Open the text file and read the lines
with open('yourfile.txt', 'r') as file:
    lines = file.readlines()

```

1. Run the `python shuffle.py` and it will produce 'shuffled_questions.docx', which can then be edited formatted as needed.

## How to use `bubble.py`

1. Edit this line to include the number of questions and the possible choices for your exam.

```{python}
# Define the number of questions and choices
num_questions = 50
choices = ['a', 'b', 'c', 'd', 'e']
```

2. Run `python bubble.py` and 'bubble_sheet.docx' will be produced.
