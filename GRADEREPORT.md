# Grading Report

**Final Grade: 7.00/10.00**

## Rubric

| Criterion | Points |
|-----------|--------|
| `extract_data` correctly slices, title-cases names, int conversion, extracts grades, and leaves input untouched | **2.5** |
| `curve_grades` applies the curve (while loop) and caps values at 100 | **2** |
| `print_top_performers` prints only qualifying `Name: Score` lines (>= 95) | **1.5** |
| Code quality (required loop choices, clear logic) | **1** |

## General Comments

extract_data currently iterates the wrong variables and returns empty lists, implement proper parsing (split or slicing) to populate and return title-cased names and integer grades from raw_data. 

curve_grades: implemented the while loop pattern correctly. You just got confused on updating the grade for each student.

print_top_performers: implemented the for loop pattern correctly. your if logic and print are not correct.

## Functionality

- tests/test_grader.py::RosterHelperTests::test_curve_grades_values_and_clamping: Failed (0.0 points)
   Error:     TypeError: '<' not supported between instances of 'int' and 'range'

- tests/test_grader.py::RosterHelperTests::test_extract_data_parses_names_and_grades_title_case: Failed (0.0 points)
   Error:     AssertionError: Lists differ: [] != ['Ana Lopez', 'Priya Singh']

- tests/test_grader.py::RosterHelperTests::test_extract_data_returns_new_lists: Failed (0.0 points)
   Error:     AssertionError: Lists differ: [] != ['Max Jones']

- tests/test_grader.py::RosterHelperTests::test_print_top_performers_prints_name_and_score_for_ge_95: Failed (0.0 points)
   Error:     TypeError: 'list' object cannot be interpreted as an integer



