# typing-speed-test

This Python script allows users to test their typing speed and accuracy in a fun and interactive way.

## Features
- Provides a phrase for users to type as quickly and accurately as possible.
- Calculates typing speed in words per minute (WPM).
- Measures accuracy of the typed input compared to the provided phrase.
- Displays time taken, total words typed, typing speed, and accuracy percentage.
- Option to retry the test or exit.

## Prerequisites
- Python 3.x

## How to Use
1. Save the script as a `.py` file (e.g., `typing_test.py`).
2. Open a terminal or command prompt.
3. Run the script:
   ```bash
   python typing_test.py
   ```

### Interactive Typing Test
- The program displays a phrase for you to type.
- Type the phrase as quickly and accurately as possible.
- The results are displayed immediately after you press Enter.
- You can retry the test or exit.

## Code Overview
### Functions
#### `createbox()`
- Prints a decorative box and displays instructions for the typing test.

#### `main()`
- Handles the main logic of the test, including:
  - Displaying the phrase.
  - Measuring typing time.
  - Calculating words per minute (WPM), accuracy, and time taken.
  - Offering an option to retry the test or exit.

### Key Calculations
- **Words per minute (WPM):**
  ```python
  wordsperminute = (lengthOfInput / timeTaken) * 60
  ```
- **Accuracy:**
  ```python
  accuracy = len(set(inputText.split()) & set(string.split())) / word_count
  ```

### Key Imports
- `time` for measuring the time taken to type the phrase.
- `contextlib` for resource management.

## Notes
- This script helps users practice typing while providing feedback on speed and accuracy.
- Ensure you type the phrase exactly as shown for the most accurate results.
