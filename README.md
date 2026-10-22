# LeafSense

LeafSense is a static browser app for leaf disease scanning demos, outbreak forecasting, and multilingual field workflows. It has no build step or package dependencies.

## Run locally

On Windows, start the included server from this folder:

```powershell
powershell -ExecutionPolicy Bypass -File .\server.ps1
```

Then open http://localhost:8080. Camera access is available on localhost and secure HTTPS origins; use photo upload if camera access is unavailable.

## Deploy with Vercel

Import `kadiyaharsh19-commits/LeafSense` into Vercel and keep the project root at `./`. This is a static HTML app with no build command or dependencies; Vercel can deploy it directly. Connect the project to the `main` branch to deploy each GitHub push automatically.

The app uses relative paths for its local assets and works from the project root on Vercel.