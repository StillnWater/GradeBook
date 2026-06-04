# GradeBook

A Python-based student grade analysis tool that provides comprehensive statistical analysis and grade reporting for student marks.

## Features

- **Multiple Input Methods**: Input student grades manually or via CSV file
- **Statistical Analysis**: Calculate average, median, minimum, and maximum scores
- **Grade Assignment**: Automatically assign letter grades (A-F) based on score thresholds
- **Pass/Fail Filtering**: Identify students who passed or failed based on a 40-point threshold
- **Grade Distribution**: View the count of each letter grade
- **Detailed Results Table**: Display all students with their marks and assigned grades

## Requirements

- Python 3.x
- Standard library modules: `csv`

## Installation

1. Clone the repository:
```bash
git clone https://github.com/StillnWater/GradeBook.git
cd GradeBook
```

2. No additional dependencies required - uses only Python standard library.

## Usage

### Running the Program

```bash
python grade.py
```

### Menu Options

1. **Manual Input**: Enter student names and marks one by one
2. **CSV Input**: Load grades from a `marks.csv` file
3. **Exit Program**: Close the application

### CSV File Format

Create a `marks.csv` file with the following format:
```
StudentName1,85
StudentName2,92
StudentName3,78
```

Each row should contain: `name,marks`

## Grading Scale

| Grade | Score Range |
|-------|-------------|
| A     | 90-100      |
| B     | 80-89       |
| C     | 70-79       |
| D     | 60-69       |
| F     | Below 60    |

## Pass/Fail Criteria

- **Pass**: Score ≥ 40
- **Fail**: Score < 40

## Program Functions

- `calculate_average(marks_dict)`: Computes the mean of all marks
- `calculate_median(marks_dict)`: Computes the median of all marks
- `find_max_score(marks_dict)`: Finds the highest score
- `find_min_score(marks_dict)`: Finds the lowest score

## Output

The program displays:
1. Statistical analysis (average, median, max, min)
2. Grade distribution count for each letter grade
3. Pass/Fail summary with student names
4. Detailed results table with all students, marks, and grades

## Example

```
=== Gradebook Menu ===
1. Manual Input
2. CSV Input
3. Exit Program
Enter choice: 1
Enter the number of students: 3
Enter name for student 1: Alice
Enter marks for Alice: 95
Enter name for student 2: Bob
Enter marks for Bob: 87
Enter name for student 3: Charlie
Enter marks for Charlie: 72

--- Analysis ---
Average:    84.67
Median:     87
Max Score:  95
Min Score:  72

Grades      Total Students
A           1
B           1
C           1
D           0
F           0

Total Passed Students: 3
Names: Alice, Bob, Charlie
Total Failed Students: 0
Names: 

Name        Marks       Grade
Alice       95          A
Bob         87          B
Charlie     72          C
```

## Author

- **Name**: Manas Bhasker
- **Date**: 22/11/25

## License

This project is provided as-is for educational purposes.

## Contributing

Feel free to fork this repository and submit pull requests for any improvements!
