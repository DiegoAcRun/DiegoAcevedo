# Portfolio Website Management Plan

## Step 1: Set Up Your GitHub Repository
1. **Create a GitHub Repository**:
   - Go to [GitHub](https://github.com) and create a new repository.
   - Name it something like `portfolio-website`.
   - Initialize the repository with a README file.

2. **Clone the Repository Locally**:
   - Open VS Code and use the terminal to clone your repository:
     ```bash
     git clone https://github.com/your-username/portfolio-website.git
     ```
   - Navigate to the cloned folder:
     ```bash
     cd portfolio-website
     ```

---

## Step 2: Start Building Your Website
1. **Create the Initial Files**:
   - Add your HTML, CSS, and JavaScript files (e.g., `index.html`, `style.css`, `script.js`) to the repository folder.

2. **Stage and Commit Your Changes**:
   - Stage the files:
     ```bash
     git add .
     ```
   - Commit the changes:
     ```bash
     git commit -m "Initial commit: Added portfolio website files"
     ```

3. **Push to GitHub**:
   - Push the changes to your repository:
     ```bash
     git push origin main
     ```

---

## Step 3: Deploy Your Website
1. **Use GitHub Pages for Deployment**:
   - Go to your repository on GitHub.
   - Navigate to **Settings > Pages**.
   - Under "Source," select the branch (e.g., `main`) and folder (e.g., `/root`).
   - GitHub Pages will generate a URL for your website (e.g., `https://your-username.github.io/portfolio-website`).

2. **Preview Your Website**:
   - Open the URL provided by GitHub Pages in your browser to see your deployed website.

---

## Step 4: Modify and Test Changes
1. **Make Changes Locally**:
   - Edit your files in VS Code (e.g., update `index.html` or `style.css`).

2. **Preview Locally**:
   - Use the Live Server extension in VS Code:
     - Install the extension from the marketplace.
     - Right-click your `index.html` file and select **Open with Live Server**.
   - This will open a local preview in your browser.

3. **Stage, Commit, and Push Changes**:
   - After testing locally, stage and commit your changes:
     ```bash
     git add .
     git commit -m "Updated portfolio design"
     git push origin main
     ```
   - GitHub Pages will automatically update your website.

---

## Step 5: Roll Back Changes
1. **View Commit History**:
   - Use the following command to see all previous commits:
     ```bash
     git log
     ```

2. **Roll Back to a Previous Commit**:
   - If you want to undo changes and go back to a specific commit:
     ```bash
     git checkout <commit-hash>
     ```
   - To reset the repository to a previous state:
     ```bash
     git reset --hard <commit-hash>
     ```

3. **Create a New Branch for Testing** (Optional):
   - To test changes without affecting the main branch:
     ```bash
     git checkout -b test-branch
     ```
   - Make changes, test, and merge back to the main branch when satisfied:
     ```bash
     git checkout main
     git merge test-branch
     ```

---

## Step 6: Continuous Deployment
1. **Automate Deployment**:
   - Use GitHub Actions to automate deployment whenever you push changes to the repository.
   - Add a workflow file (`.github/workflows/deploy.yml`) to configure this.

---

## Step 7: Share and Collaborate
1. **Share Your Website**:
   - Share the GitHub Pages URL with others for feedback.

2. **Collaborate**:
   - If you want others to contribute, invite collaborators to your repository.