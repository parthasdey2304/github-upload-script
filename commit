clear
figlet "Git!"

# Check if .git directory exists
if [ -e '.git' ]; then
    # Git directory exists
    echo -e '\e[32m[INFO] Here are all the unstaged files...\e[0m'
    git status
    echo ''
    echo ''

    # Pull any changes from the remote repository
    echo -e '\e[32m[INFO] Checking if any files need to be pulled...\e[0m'
    git pull

    # Add all files for staging
    echo -e '\e[32m[INFO] Adding all the files...\e[0m'
    git add .

    # Commit the staged files
    echo -e '\e[32m[INFO] Committing files...\e[0m'
    git commit -m "Initial commit"

    # Push the committed changes to the remote repository
    echo -e '\e[32m[INFO] Pushing files...\e[0m'
    git push --force

    # Add a 1-second delay for visual effect
    sleep 1

    # Clear the screen and display "Repo Updated" message
    clear
    figlet "Repo Updated!!"
else
    # Git directory does not exist
    echo -e '\e[31mFatal Error: Git not initialized!'
    echo -e '\e[31m.git file not found!\e[0m'
fi
