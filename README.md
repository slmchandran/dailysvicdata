# Vetri Layer Daily

1. Create a PRIVATE GitHub repo for DATA (e.g. vetri-farm-data) with a README so `main` exists.
2. GitHub > Settings > Developer settings > Fine-grained token: only that repo, permission "Contents: Read and write".
3. Push THIS folder to a separate repo (e.g. vetri-layer-app) and import it in Netlify (no build command, publish dir `public`).
4. Netlify > Site settings > Environment variables:
   - GITHUB_TOKEN  = your token
   - GITHUB_REPO   = youruser/vetri-farm-data
   - GITHUB_BRANCH = main
   - APP_PIN       = a PIN your staff will type once per phone
5. Redeploy. Open the site on phone > Add to Home Screen.
Data lands in `data/farm.json` in the data repo; every save is a commit.