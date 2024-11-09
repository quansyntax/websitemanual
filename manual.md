# Conference Website Manual for Future Organizers

## 1. Sign In to the GitHub Account
- **Account Name**: [Fill in your account name here]
- **Password**: [Fill in your password here]

> **Note**: Use a password manager like **Bitwarden**, **1Password**, or **LastPass** to securely store your credentials.

## 2. Create a New Repository
1. Click on the "+" icon in the upper right corner and select **"New repository"**.
2. **Name your repository**:
   - For a user or organization site, use `<yourusername>.github.io`.
   - For a project site, use any descriptive name.
3. Set the repository as **public**.
4. (Optional) Initialize the repository with a **README** file.

## 3. Clone the Repository
Clone the repository to your local machine using Git:

1. If you don't have Git installed, download it from [git-scm.com](https://git-scm.com).
2. Use the following command to clone:

    ```bash
    git clone https://github.com/yourusername/yourrepository.git
    ```

**Note**: Replace `yourusername` and `yourrepository` with your actual GitHub username and repository name.

## 4. Add Your Website Files
1. Navigate into the cloned directory:

    ```bash
    cd yourrepository
    ```

2. **Add website files**:
   - Include an `index.html` file as the entry point.
   - Add supporting files such as CSS (`style.css`), JavaScript, images, and other assets as needed.

3. **Folder Structure**:
   - Use a clear folder structure, like:
     ```
     /images
     /fonts
     /css
     /js
     index.html
     about.html
     ```

4. **Referencing Previous Sites**:
   - Check previous conference websites like **Quasy** and **Quasy2025**.
   - Include basic files like `index.html` and `style.css`.
   - Additional pages can include `call-for-paper.html`, `committee.html`, etc., as shown in **Quasy2025**.

## 5. Add Logo and Branding
1. **Logo files**:
   - The **Quasy** logo is `logo2025.png`, found in the `images` folder.
   - The SVG version is `logo2025.svg`.

2. **Modifying the logo**:
   - Edit `logo2025.svg` to replace the year `2025` with the current year.

3. **Logo Colors**:
   - Color of "Quasy": `rgb(47, 76, 92)`
   - Color for power law and syntactic trees: `rgb(7, 149, 166)`

4. **Fonts**:
   - Logo fonts are inside the `fonts` folder.

## 6. Ensure Mobile Responsiveness
Include the following code snippet in your `index.html` to make the site mobile-friendly:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

- Test the website on different devices or use browser tools to ensure the site works well on mobile screens.

## 7. Push Changes to GitHub
After adding your files, push them to GitHub:

1. **Add changes**:

    ```bash
    git add .
    ```

2. **Commit changes**:

    ```bash
    git commit -m "Initial website files"
    ```

3. **Push to GitHub**:

    ```bash
    git push -u origin main
    ```

**Tip**: Use **descriptive commit messages** to make it easier to track changes, e.g., "Add homepage content" instead of "Changes".

## 8. Enable GitHub Pages
1. **Navigate** to your GitHub repository in the browser.
2. Go to the **"Settings"** tab.
3. Click **"Pages"** in the left sidebar.
4. Under **"Source"**, select the branch to publish (usually `main`).
5. Click **"Save"**.

## 9. Access Your Website
- For **user or organization sites**, visit:

  ```
  https://<yourusername>.github.io
  ```

- For **project sites**, visit:

  ```
  https://<yourusername>.github.io/<repositoryname>/
  ```

**Note**: Replace `<yourusername>` and `<repositoryname>` with your actual GitHub username and repository name.

---

## 10. Best Practices & Additional Tips
1. **Branching**:
   - Use **feature branches** for new pages or major updates:
     ```bash
     git checkout -b feature/new-page
     ```
   - This helps keep the `main` branch stable and allows for easier collaboration.

2. **Testing Locally**:
   - Before pushing changes, use a **live server** in VS Code or similar tools to preview your website locally.
   - This helps catch issues before they go live.

3. **Deployment Checks**:
   - After enabling GitHub Pages, check if all resources (images, CSS, JavaScript) load correctly.
   - Use tools like **Google Lighthouse** for performance, accessibility, and SEO checks.

4. **Add Collaborators**:
   - If other people need to work on the site, add them as **collaborators** through repository settings.

5. **Enable Two-Factor Authentication (2FA)**:
   - Protect your GitHub account by enabling **2FA**. This adds an extra layer of security beyond just a password.

## Common Troubleshooting Tips
1. **Website Not Showing Up**: Ensure the correct branch is selected in GitHub Pages settings.
2. **Broken Links or Missing Resources**: Double-check the paths to images, CSS, and JavaScript files.

---

This Markdown document ensures compatibility with different platforms and is easy to maintain, share, and collaborate on.
