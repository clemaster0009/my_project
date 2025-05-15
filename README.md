mkdir my_project
cd my_project

# Initialize a new Git repository

git init
echo 'This is my project' >README.md

git add README.md

git commit -m 'Initial commit'

# Do not modify the testing mechanism
if [ -d .git ]; then echo 'Repository initialized'; else echo 'Initialization failed'; fi
if [ -f README.md ]; then echo 'File created'; else echo 'File creation failed'; fi
if git log | grep -q 'Initial commit'; then echo 'Commit successful'; else echo 'Commit failed'; fi

