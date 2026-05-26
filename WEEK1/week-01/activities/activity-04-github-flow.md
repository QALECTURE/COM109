# Activity 04: GitHub Flow

## Purpose

Introduce GitHub basics and help students understand how developers save, share and review code.

## Key Terms

| Term | Beginner-Friendly Meaning |
| --- | --- |
| Repository | A project folder tracked by Git and often stored on GitHub. |
| Commit | A saved snapshot of changes with a message explaining what changed. |
| Branch | A separate line of work, useful for trying changes without affecting the main version. |
| Push | Upload local commits to GitHub. |
| Pull Request | A request to review and merge changes into another branch. |

## Why Developers Use GitHub

Developers use GitHub to:

- Store code safely online
- Track the history of a project
- Work with other developers
- Review changes before they are accepted
- Show portfolio work to employers

## Beginner GitHub Flow Activity

## Scenario

You are working on a portfolio webpage. You want to add an About Me section and share it with your team.

## Steps

1. **Create or open a repository**  
   This is the project space for your portfolio.

2. **Make a local change**  
   Edit `index.html` and add an About Me section.

3. **Check the status**  
   Run:

   ```bash
   git status
   ```

4. **Stage the change**  
   Run:

   ```bash
   git add .
   ```

5. **Commit the change**  
   Run:

   ```bash
   git commit -m "Add about section"
   ```

6. **Push to GitHub**  
   Run:

   ```bash
   git push
   ```

7. **Review on GitHub**  
   Open the repository in GitHub and check that the commit appears.

## Pair Activity

In pairs, discuss:

- What should a good commit message say?
- Why is `Add about section` better than `stuff`?
- Why might a team use branches?
- Why might a company require pull requests?

## Lecturer Wrap-Up

GitHub is not only for storing code. It supports professional teamwork. In industry, developers often make changes locally, commit them, push them to GitHub and ask for review before the code becomes part of the main project.

