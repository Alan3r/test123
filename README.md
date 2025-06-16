# Welcome to your Lovable project

## Project info

**URL**: https://lovable.dev/projects/fd289010-92c5-46f4-8304-ef74bc5c1ce6

## How can I edit this code?

There are several ways of editing your application.

**Use Lovable**

Simply visit the [Lovable Project](https://lovable.dev/projects/fd289010-92c5-46f4-8304-ef74bc5c1ce6) and start prompting.

Changes made via Lovable will be committed automatically to this repo.

**Use your preferred IDE**

If you want to work locally using your own IDE, you can clone this repo and push changes. Pushed changes will also be reflected in Lovable.

The only requirement is having Node.js & npm installed - [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)

Follow these steps:

```sh
# Step 1: Clone the repository using the project's Git URL.
git clone <YOUR_GIT_URL>

# Step 2: Navigate to the project directory.
cd <YOUR_PROJECT_NAME>

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Start the development server with auto-reloading and an instant preview.
npm run dev
```

**Edit a file directly in GitHub**

- Navigate to the desired file(s).
- Click the "Edit" button (pencil icon) at the top right of the file view.
- Make your changes and commit the changes.

**Use GitHub Codespaces**

- Navigate to the main page of your repository.
- Click on the "Code" button (green button) near the top right.
- Select the "Codespaces" tab.
- Click on "New codespace" to launch a new Codespace environment.
- Edit files directly within the Codespace and commit and push your changes once you're done.

## What technologies are used for this project?

This project is built with:

- Vite
- TypeScript
- React
- shadcn-ui
- Tailwind CSS

## How can I deploy this project?

Simply open [Lovable](https://lovable.dev/projects/fd289010-92c5-46f4-8304-ef74bc5c1ce6) and click on Share -> Publish.

## Can I connect a custom domain to my Lovable project?

Yes, you can!

To connect a domain, navigate to Project > Settings > Domains and click Connect Domain.

Read more here: [Setting up a custom domain](https://docs.lovable.dev/tips-tricks/custom-domain#step-by-step-guide)

## Deploying to GitHub Pages

To deploy your React (Vite) app to GitHub Pages:

1. Install the `gh-pages` package:
   ```sh
   npm install --save-dev gh-pages
   ```

2. In your `package.json`, add the following:
   - Set the `homepage` field to `"https://<your-github-username>.github.io/<your-repo-name>"`
   - Add scripts:
     ```json
     "scripts": {
       // ...existing scripts...
       "predeploy": "npm run build",
       "deploy": "gh-pages -d dist"
     }
     ```

3. Push your code to GitHub.

4. Run:
   ```sh
   npm run deploy
   ```

5. Your site will be available at `https://<your-github-username>.github.io/<your-repo-name>/`

For more details, see the [Vite deployment guide](https://vitejs.dev/guide/static-deploy.html#github-pages).

## Troubleshooting GitHub Pages Deployment

If you see this error:
```
Error: Failed to get remote.origin.url (task must either be run in a git repository with a configured origin remote or must be configured with the "repo" option)
```
Make sure you have initialized a git repository and set the remote origin:

```sh
git init
git remote add origin https://github.com/<your-github-username>/<your-repo-name>.git
```

Replace `<your-github-username>` and `<your-repo-name>` with your actual GitHub username and repository name.

## Troubleshooting Git Push Errors

If you see this error:
```
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Alan3r/test123.git'
```
This usually means you have not made any commits yet, or your branch is not named `main`. To fix:

1. Make sure you have at least one commit:
   ```sh
   git add .
   git commit -m "Initial commit"
   ```

2. If your branch is named `master` (the default for some git versions), push using:
   ```sh
   git push origin master
   ```
   Or, rename your branch to `main`:
   ```sh
   git branch -M main
   git push origin main
   ```

Check your branch name with:
```sh
git branch
```
