# Achieve Pull Shark and Pair Extraordinaire Badge with Ease

This project automates the process of creating Git branches, making changes, committing them, pushing to a remote repository, creating pull requests, and merging them. It is designed to streamline repetitive tasks for developers and ensure consistency in branch naming and commit messages.

## Features

- **Automated Branch Creation**: Generates meaningful branch names using random combinations of words and numbers.
- **File Modification**: Creates or modifies a file (`text.txt`) with a small change.
- **Git Integration**: Automates adding, committing, and pushing changes to a remote repository.
- **Pull Request Management**: Creates and merges pull requests using the GitHub CLI (`gh`).
- **Customizable Execution**: Allows users to specify the number of iterations and delay between runs to avoid rate-limiting issues.

## Prerequisites

Before running this script, ensure you have the following:

1. **Python**: Installed on your system (Python 3.x recommended).
2. **Git**: Installed and configured with access to your repository.
3. **GitHub CLI (`gh`)**: Installed and authenticated with your GitHub account.
4. **Repository Setup**: The script assumes it is run in a Git repository with a `main` branch.

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/achieve-pull-shark-and-pair-extraordinaire-badge-with-ease.git
   cd achieve-pull-shark-and-pair-extraordinaire-badge-with-ease
   ```

2. Make a new repository on GitHub and clone it to your local machine.

   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

3. Copy the `main.py` script into your cloned repository.

## Usage

1. Make sure you are in the `main` branch of your repository.

   ```bash
   git checkout main
   ```

2. Run the script:

   ```bash
   python main.py
   ```

3. Follow the prompts:

   - Enter the number of iterations you want the script to run.
   - Specify the delay (in seconds) between iterations. The minimum delay is 100 seconds to avoid rate-limiting issues.

### Example

```plaintext
How many times do you want to run the script? 3
How long do you want to wait between runs? (in seconds) 120
```

The script will:

1. Generate a new branch name.
2. Create the branch.
3. Add or modify `text.txt` with a small change.
4. Commit the changes with a pre-defined message.
5. Push the branch to the remote repository.
6. Create a pull request and merge it into the `main` branch.
7. Repeat the process for the specified number of iterations.

## File Structure

- **`main.py`**: The main script that handles all automation tasks.
- **`.gitignore`**: Specifies files and directories to be ignored by Git.
- **`LICENSE`**: MIT License for the project.
- **`README.md`**: Documentation for the project.

## Key Functions in `main.py`

1. **`gen_branch_name()`**: Generates a random branch name using predefined word lists and a numeric suffix.
2. **`create_branch(branch_name)`**: Creates a new Git branch.
3. **`switch_branch(branch_name)`**: Switches to an existing branch.
4. **`run_command(command)`**: Executes shell commands and handles output/errors.
5. **`create_file(file_path)`**: Creates a file (`text.txt`) if it doesn't already exist.
6. **`add_change_to_text_file(file_path)`**: Appends a small change to `text.txt`.
7. **`main()`**: Orchestrates the entire process, including branch creation, file modification, Git operations, and pull request management.

## Configuration

- **Branch Naming**: Modify the word lists in `gen_branch_name()` to customize branch names.
- **Commit Message**: Update the `COMMIT_MESSAGE` constant to change the default commit message.
- **Co-Authors**: Update `COAUTHOR_1` and `COAUTHOR_2` constants to include different co-authors.

## Notes

- Ensure you have write access to the repository where the script is executed.
- The script uses the GitHub CLI (`gh`) for pull request creation and merging. Make sure it is installed and authenticated.

## License

This project is licensed under the [MIT License](LICENSE).

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests to improve the project.

## Disclaimer

This script is provided "as is" without warranty of any kind. Use it at your own risk.

This Script is intended for educational purposes and to help developers automate repetitive tasks. Always ensure you understand the code and its implications before running it in a production environment.

this project is made for fun and to help developers achieve the "Pull Shark" and "Pair Extraordinaire" badges on GitHub. It is not intended for malicious use or to spam repositories. Always respect the guidelines and policies of the platforms you are using. Use responsibly and ethically.

## Donate

If you find this project helpful and would like to support its development, consider buying me a coffee! Your support is greatly appreciated.

[![Buy Me a ko-fi](https://cdn.ko-fi.com/cdn/kofi3.png?v=2)](https://ko-fi.com/oceanofanythinofficial)
