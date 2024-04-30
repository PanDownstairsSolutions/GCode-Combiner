# GCode Combiner

This program combines multiple GCode files along with an ejection GCode file into a single output file.

## Features

- Combines multiple GCode files into one.
- Supports specifying the number of copies for each GCode file.
- Inserts an ejection GCode file between each GCode file.
- Easy-to-use command-line interface.

## Usage

1. Download the executable file

2. Save your .gcode files in the same directory with the executable

3. Run the executable

4. Follow the on-screen prompts:
- Enter the total number of GCode files to combine.
- Enter the name for the combined/generated GCode file (with the .gcode extension).
- Enter the name of the ejection GCode file (with the .gcode extension).
- For each GCode file:
  - Enter the file name (with the .gcode extension).
  - Enter the number of copies.
  - The combined GCode file will be generated in current directory.

## Notes
- Ensure that all input files (GCode files and ejection GCode file) are in the same directory as the executable.
- Make sure to input valid file names and numbers.

## Disclaimer & Notes for Printing
- This app only combines GCode files. Use it wisely to prevent machine damage.
- Make sure you add a delay time or other temperature based GCode command at the very top of your ejection file, so the part has time to cool down.
- Test your ejection file before attempting to combine files, taking into account warming up the bed, position of printhead etc.

## Error Handling
- The program handles errors gracefully, such as file opening failures.
- Error messages are displayed to help diagnose and fix issues.

## Contributing
Contributions are welcome! Feel free to fork the repository, make changes, and submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
