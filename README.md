# my_project
# Create a new directory and navigate into it
mkdir my_project
cd my_project

# Initialize a new Git repository
# Add your code below
git init clemaster0009/my_project
git README.md


# Do not modify the testing mechanism
if [ -d .git ]; then echo 'Repository initialized'; else echo 'Initialization failed'; fi
if [ -f README.md ]; then echo 'File created'; else echo 'File creation failed'; fi
if git log | grep -q 'Initial commit'; then echo 'Commit successful'; else echo 'Commit failed'; fi
