# AutoGrader using GPT-4

## Introduction

AutoGrader is an automated grading tool that leverages the power of OpenAI's GPT-4 model to grade assignments of students. It provides an efficient way to grade coding assignments by comparing student answers to a standard answer.

## Features

- Automated grading using the GPT-4 language model.
- Ability to handle multiple student submissions in zip format.
- Customizable grading rubrics and feedback.
- Error handling to ensure smooth processing.

## Prerequisites

- Python 3.x
- OpenAI API Key
- Python Libraries

## Setup

1. Clone the repository:

```
git clone <repository_link>
```


2. Install the necessary libraries:

```
pip install -r requirements.txt
```




3. Store your OpenAI API key as an environment variable:

```
export OPENAI_API_KEY=your_api_key
```


4. Update the `assignment_answers` dictionary with the standard answers for the assignments.

## Usage

1. Place all student submissions in the `./zip` directory.
2. Run the main script:

```
python autograder.py
```



3. Results will be saved in `grading_results.csv` with columns: "Student Name", "Total Score", "Feedback".

## Customization

You can customize the grading rubric by updating the `assignment_answers` dictionary and the grading logic inside the `grade_assignment_per_file` function.

## Limitations

- Ensure that student submissions are named appropriately to extract student names.
- The current version assumes Python files and certain TODO format. Adjustments might be needed based on the actual assignment format.

## Contributions

Contributions, bug reports, and improvements are welcome! Feel free to open an issue or submit a pull request.

## License

MIT License. See `LICENSE` for more information.

## Disclaimer

This tool is meant to assist in the grading process and might not be 100% accurate. Always ensure to manually verify results where necessary.
