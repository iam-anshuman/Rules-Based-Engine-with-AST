# ZeoTap Assignment Rule Based Engine

This project implements a rule-based engine for evaluating complex conditions based on user-defined rules.

## Prerequisites

- Python 3.6 or higher
- SQLite3 (usually comes pre-installed with Python)

## Installation

1. Clone this repository or download the `App.py` file.
2. No additional libraries are required as the script uses only built-in Python modules.

## Usage

1. Open a terminal or command prompt.
2. Navigate to the directory containing `App.py`.
3. Run the script using Python:

   ```
   python App.py
   ```

4. The script will execute the test cases defined in the `__main__` section, demonstrating:
   - Creation of individual rules
   - Combining rules
   - Evaluating rules against sample data
   - Error handling for invalid rules
   - Rule modification

## Customizing Rules and Data

To use your own rules and data:

1. Open `App.py` in a text editor.
2. Modify the `rule1` and `rule2` strings in the `__main__` section to define your own rules.
3. Update or add more sample data dictionaries (`data1`, `data2`, etc.) to test your rules.
4. Run the script as described above to see the results.

## Understanding the Output

The script will print:
- Abstract Syntax Trees (ASTs) for individual rules
- A combined AST for multiple rules
- Evaluation results for each sample data set
- Any errors encountered during rule creation or evaluation

## Database Operations

The script includes functions for initializing a SQLite database and saving/loading rules. To use these features:

1. Call `init_db()` to create the database and table.
2. Use `save_rule(name, rule_string)` to save a rule.
3. Use `load_rule(name)` to retrieve a saved rule.

## Extending the Script

You can extend the functionality by:
- Adding more operators in the `evaluate_rule` function
- Implementing a user interface for rule input and data evaluation
- Expanding the database operations to manage multiple rule sets

## Troubleshooting

If you encounter any issues:
- Ensure you're using Python 3.6 or higher
- Check that the `App.py` file is in the correct directory
- Verify that your rule syntax matches the expected format

For any other problems, please open an issue in the project repository.

