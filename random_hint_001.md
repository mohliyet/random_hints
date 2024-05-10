# Pushing a Local Repository to GitHub

Follow these steps to push a local repository to GitHub:

1. **Initialize a local Git repository**: Navigate to the project directory in the terminal and run the following command:

    ```bash
    cd your_project_directory
    git init
    ```

2. **Add files to the repository**: Add all the files in the directory to the staging area of Git with the following command:

    ```bash
    git add .
    ```

3. **Commit the files**: Save the changes in the staging area to the local repository with the following command:

    ```bash
    git commit -m "First commit"
    ```

4. **Create a new repository on GitHub**: Go to GitHub, click on the '+' button on the top right corner, and select 'New repository'. Fill in the repository name and description, and click 'Create repository'.

5. **Link the local repository to the GitHub repository**: Copy the URL of the GitHub repository and add it as the 'origin' in the local repository with the following command. If you're using HTTPS and have two-factor authentication enabled, replace `your_PAT` with your personal access token:

    ```bash
    git remote add origin https://your_PAT@github.com/username/repo.git
    ```

6. **Push the local repository to GitHub**: Push the commits in the local repository to the GitHub repository with the following command:

    ```bash
    git push -u origin master
    ```