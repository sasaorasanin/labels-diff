# Language Labels Comparison Tool

A simple web-based tool to compare language labels and identify differences between two sets of key-value pairs. Built with HTML, JavaScript, and Tailwind CSS, this tool is useful for developers working on localization to find missing translations between two languages.

## Features
- Compare two sets of language labels in `key=value` format.
- Displays labels present in one language but missing in the other.
- Responsive design with a modern UI using Tailwind CSS.
- Smooth scrolling to results for better user experience.
- Lightweight and dependency-free (uses Tailwind CSS via CDN).

## Demo
Try the tool by opening `index.html` in a browser. Enter labels in the format `key=value` (one per line) in the two input textareas, then click "Find Difference" to see the results.

**Example Input**:
- **First Language**:
  ```
  home=Home
  settings=Settings
  profile=Profile
  ```
- **Second Language**:
  ```
  home=Početna
  profile=Profil
  ```

**Output**:
- **First Language Missing in Second**: `settings=Settings`
- **Second Language Missing in First**: (empty)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/language-labels-comparison.git
   ```
2. Navigate to the project folder:
   ```bash
   cd language-labels-comparison
   ```
3. Open `index.html` in a web browser, or serve it using a local server:
   ```bash
   python -m http.server 8000
   ```
   Then visit `http://localhost:8000` in your browser.

## Usage
1. Open `index.html` in a web browser.
2. In the "First Language Labels" textarea, enter labels for the first language (e.g., `key=value`, one per line).
3. In the "Second Language Labels" textarea, enter labels for the second language.
4. Click the **Find Difference** button.
5. View the results in the two output textareas:
   - Labels present in the first language but missing in the second.
   - Labels present in the second language but missing in the first.
6. The page will automatically scroll to the results.

## Project Structure
- `index.html`: The main file containing the HTML, JavaScript, and Tailwind CSS (via CDN) for the comparison tool.
- `README.md`: This file, providing documentation for the project.

## Dependencies
- [Tailwind CSS](https://tailwindcss.com/) (loaded via CDN, no local installation required).

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit (`git commit -m "Add feature"`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## Future Improvements
- Add support for importing/exporting `.json` or `.php` language files (e.g., Laravel localization files).
- Integrate with translation APIs for automatic translation suggestions.
- Enhance the UI with a table-based comparison view.
- Add file upload functionality to load language files directly.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For questions or suggestions, feel free to open an issue or contact the maintainer at [your-email@example.com].
