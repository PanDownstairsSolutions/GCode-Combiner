# GCode Combiner

This program combines multiple GCode files along with an ejection GCode file into a single output file.

## Features

- Combines multiple GCode files into one.
- Supports specifying the number of copies for each GCode file.
- Inserts an ejection GCode file between each GCode file.
- Easy-to-use command-line interface.

## Usage

1. Compile the program using a C compiler (e.g., GCC):

   ```bash
   gcc -o gcode_combiner gcode_combiner.c

2. Run the compiled executable:
   ```bash
   ./gcode_combiner

3. Follow the on-screen prompts:
- Enter the number of GCode files to combine.
- Enter the name for the combined .gcode file.
- Enter the name of the ejection GCode file.
- For each GCode file:
  - Enter the file name.
  - Enter the number of copies.
  - The combined GCode file will be generated in current directory.

## Notes
- Ensure that all input files (GCode files and ejection GCode file) are in the same directory as the executable or provide the full file paths.
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
