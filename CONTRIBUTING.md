
# Contributing to the Pet Adoption App - Frontend

Welcome! We are excited to have you contribute to the frontend of the Pet Adoption App. This guide will walk you through every step you need to take to get started and contribute efficiently.

## Prerequisites
- You need to have **Node.js** and **npm** installed on your machine. If you don’t have them installed, follow this guide:
  - [Install Node.js](https://nodejs.org/en/download/)
  - Node.js comes with npm, the Node package manager, which we will use to install dependencies.

- You will also need **Git** installed on your machine. If Git is not installed, follow this guide:
  - [Install Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

## Steps to Contribute

### 1. Fork the Repository

Forking the repository creates a personal copy of the repository under your GitHub account. Here's how you can do it:
- Go to the GitHub repository page for the Pet Adoption App.
- In the top-right corner, click the **Fork** button to create your own copy of the repository.

### 2. Clone the Repository to Your Local Machine

After forking, you need to **clone** the repository (download it to your local machine) so you can start working on it.

1. Go to your GitHub account and navigate to the repository you just forked.
2. Click the **Code** button and copy the URL (you can use HTTPS).
3. Open a terminal (or Git Bash) on your machine and run the following command, replacing `your-username` with your GitHub username:
   ```bash
   git clone https://github.com/your-username/pet-adoption-app.git
   ```
4. Navigate to the `frontend` directory where the frontend code is located:
   ```bash
   cd pet-adoption-app/frontend
   ```

### 3. Install the Project Dependencies

Now that you have the project files, you need to install the dependencies (external packages) that the project requires to run.

Run the following command in the `frontend` directory:
```bash
npm install
```
This will install all the necessary dependencies specified in the `package.json` file.

### 4. Create a New Branch for Your Feature or Bug Fix

**Always create a new branch** when working on a new feature or fixing a bug. This helps in keeping the codebase clean and organized.

1. Make sure you are in the `frontend` directory and your repository is up to date.
2. Run the following command to create a new branch:
   ```bash
   git checkout -b feature/my-feature
   ```
   Replace `my-feature` with a short and descriptive name for the feature or bug fix you're working on (e.g., `add-search-bar` or `fix-header`).

### 5. Make Changes to the Frontend Code

Now that you're on a new branch, you can start coding.

- Open the project in your preferred code editor (e.g., **VS Code**).
- Make sure you're following these guidelines:
  - Use **Tailwind CSS** for styling. For example:
    ```html
    <div class="bg-blue-500 text-white p-4 rounded-lg">
      This is a button!
    </div>
    ```
  - Create **reusable components** for sections like buttons, cards, or pet details that will appear multiple times.
  - Follow **React best practices** (e.g., use functional components and hooks).

### 6. Test Your Changes Locally

Once you've made changes, you can test your work by running the project locally:

1. Start the development server by running:
   ```bash
   npm run dev
   ```
2. Open your web browser and go to `http://localhost:3000` to see the app running.

Make sure everything looks good and works as expected.

### 7. Commit Your Changes

After verifying that your changes are working correctly, it's time to **commit** them to your local branch.

1. Stage all the files you changed:
   ```bash
   git add .
   ```
   This tells Git to include all modified files in your commit.

2. Commit your changes with a meaningful message. For example:
   ```bash
   git commit -m "Added a search bar to filter pets"
   ```

### 8. Push Your Changes to GitHub

After committing, you need to **push** your changes to GitHub so they can be reviewed.

Run the following command to push your branch to GitHub:
```bash
git push origin feature/my-feature
```

### 9. Create a Pull Request (PR)

Now that your changes are pushed to GitHub, it's time to create a **Pull Request** (PR) to merge your changes into the main codebase.

1. Go to the **original repository** on GitHub (not your fork).
2. You should see a message prompting you to create a pull request for the branch you just pushed.
3. Click the **Compare & Pull Request** button.
4. Write a detailed description of the changes you made and why they are needed.
5. Click **Create Pull Request**.

### 10. Review Process

Once your pull request is submitted, it will be reviewed by the team or project lead. If everything looks good, your changes will be merged into the `main` branch.

### 11. Sync Your Fork with the Main Repository

To keep your fork up to date with the latest changes in the original repository, you should regularly **sync** your fork.

1. First, add the original repository as a remote source:
   ```bash
   git remote add upstream https://github.com/original-username/pet-adoption-app.git
   ```
2. Fetch the latest changes from the original repository:
   ```bash
   git fetch upstream
   ```
3. Switch to your local `main` branch:
   ```bash
   git checkout main
   ```
4. Merge the changes from the `main` branch of the original repository:
   ```bash
   git merge upstream/main
   ```

### 12. Delete Your Feature Branch (Optional)

Once your pull request is merged, you can delete your feature branch to keep the repository clean. You can do this from GitHub, or run:
```bash
git branch -d feature/my-feature
```

## Guidelines for Frontend Developers

- **Use Tailwind CSS** for all styling. Avoid writing custom CSS unless absolutely necessary.
- **Write reusable components** for common UI elements.
- **Follow React best practices**: Use functional components, hooks, and state management properly.
- **Test your changes** thoroughly before submitting a pull request.
- **Keep your commit messages concise** but descriptive (e.g., "Added search bar functionality" or "Fixed button alignment").

## Additional Resources

- [React Documentation](https://reactjs.org/docs/getting-started.html)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)

Thank you for contributing to the Pet Adoption App! If you have any questions, feel free to reach out to the team or the project lead. Happy coding! 🎉
