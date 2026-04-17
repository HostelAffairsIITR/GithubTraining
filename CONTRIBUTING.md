Hi! This repo has been made to help novices get comfortable with Github's workflow, especially the Fork-and-Pull model. 

Please follow these technical constraints to ensure your contribution is accepted.

## Initial Setup

1. "Fork": Click the Fork button on the top right of this page to create an online copy in your github account.
2. "Clone": Download your fork to your local machine. <br>
   ```git clone https://github.com/YOUR_USERNAME/GithubTraining.git```

3. Configure Upstream: To ensure that you can always fetch the latest copy of main repo. <br>
  ```git remote add upstream https://github.com/HostelAffairsIITR/GithubTraining.git```

## Synchronize

It is possible that since making the fork, the main branch of the official repository has been updated. It is very important to keep your current copy up-to-date.

1. Update Main: <br>
```bash
git checkout main
git pull upstream main
```

2. Branching: You **never** start editing on the main branch, always make a different branch.
```bash
git checkout -b feat/your-username
```

## Making Changes

1. Navigate to `contributors/` directory.
2. Use vim (or any other text editor) to create a new file named `your-username.md`.
3. Write your name and current date inside the file.

## Commit and Push

1. "Stage": Add only your specific file
```bash
git add contributors/your-username.md
```

2. "Commit": Be clear and concise while writing commit messages
```bash
git commit -m "feat: add [Your Name] to contributors list"
```

3. "Push": To upload your branch to github fork
```bash
git push origin feat/your-username
```

## Submitting a Pull Request

By submitting a Pull Request, you can ask the maintainer of the orignal repo to review your proposed changes. If they accept the changes, then your branch gets merged into the main branch of the repository.

1. Navigate to original repository on Github
2. A yellow banner should appear, click on 'Compare and pull request'.
3. 'Base repository' is club's repo and 'Head Repository' is your fork.
4. Submit the PR and wait for maintainer to review. 

That's it! Btw, be sure to look into the significance of the `.gitignore` file.




