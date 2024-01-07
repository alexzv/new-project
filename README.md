# new-project step-by-step instructions

1. Create a new "new-project" folder in your environment.

```sh
mkdir new-project
```

2. Go to the "new-project" folder.

```sh
cd new-project
```

3. Initialize the new repository in the "new-project" folder with branch "main".

```sh
git init
git branch -M main
```

3.1. Link the local repository to your GitHub public repository throw https or ssh connection.

```sh
git remote add origin https://github.com/<your_account>/new-project.git
```

or

```sh
git remote add origin ssh://git@github.com/<your_account>/new-project.git
```

4. Create a README.md file and add the first instructions to it.

```sh
touch README.md
echo "new-project step-by-step instructions" > ./README.md
```

5. Add the README.md file to repository.

```sh
git add README.md
```

6. Commit the changes with message "init".

```sh
git commit -m "init"
```

7. Create the "development" branch and switch to it.

```sh
git checkout -b development
```

8. Update the README.md file and add appropriate instructions to it. Save the changes in the README.md file to repository.

```sh
vim ./README.md
git add README.md
```

9. Commit the changes in the "development" branch with appropriate message.

```sh
git commit -m "Add step-by-step instructions to README.md"
```

10. Switch to the "main" branch and merge changes in the "development" branch with the "main" branch.

```sh
git checkout main
git merge development
```

11. Check the changes in the repository.

```sh
git status
cat ./README.md
```

12. Push the local repository to GitHub.

```sh
git push -u origin main
```

