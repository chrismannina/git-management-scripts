# Git Management Scripts

This repository contains a collection of bash scripts designed to help manage multiple Git repositories. These scripts are useful for developers with numerous projects, enabling them to quickly check the status of all repositories or update them with ease.

## Scripts

- **check_git_status.sh**: Iterates through directories and checks the Git status of each repository, including the current branch and whether there are uncommitted changes.
- **update_git_repos.sh**: Goes through each Git repository in a specified directory and updates it by pulling the latest changes from the main branch.

## Getting Started

### Prerequisites

- Git installed on your machine.
- Bash shell.

### Installation

1. Clone this repository to your local machine:

```bash
git clone https://github.com/chrismannina/git-management-scripts.git
```

2. Navigate to the cloned directory:

```bash
cd git-management-scripts
```

3. Make the scripts executable:

```bash
chmod +x check_git_status.sh update_git_repos.sh
```

### Usage

1. **Checking the status of all repositories:**

```bash
./check_git_status.sh
```

- Make sure to update the `PROJECTS_DIR` variable inside `check_git_status.sh` to point to your projects directory.

2. **Updating all repositories:**

```bash
./update_git_repos.sh
```

- Update the `PROJECTS_DIR` variable inside `update_git_repos.sh` to your projects directory.
- Ensure the branch you wish to pull from is correctly set in the script. By default, it's set to `main`.

## Customizing

- You can modify the `PROJECTS_DIR` variable in each script to point to your specific projects directory.
- If your default branch is different from `main`, update the `git pull` command in `update_git_repos.sh` accordingly.

## Contributing

Contributions are welcome! Feel free to fork the repository and submit pull requests.

## License

This project is open source and available under the [MIT License](LICENSE).
