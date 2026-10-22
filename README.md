# LeafSense

LeafSense is a static browser app for leaf disease scanning demos, outbreak forecasting, and multilingual field workflows. It has no build step or package dependencies.

## Run locally

On Windows, start the included server from this folder:

```powershell
powershell -ExecutionPolicy Bypass -File .\server.ps1
```

Then open http://localhost:8080. Camera access is available on localhost and secure HTTPS origins; use photo upload if camera access is unavailable.

## Deploy with GitHub Pages

The workflow in `.github/workflows/pages.yml` publishes the static project whenever a commit is pushed to `main`.

1. Push this project to a GitHub repository using the `main` branch.
2. In the repository, open **Settings > Pages** and set the build and deployment source to **GitHub Actions**.
3. Open the **Actions** tab and wait for the Pages deployment to complete. GitHub will show the published site URL in the deployment details.

The app uses relative paths for its local assets, so it works both at a repository Pages URL and at a custom domain.