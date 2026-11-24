# Notes app (APK) - setup

1. Create two repos on GitHub:
   - `notes-app` (Public): upload everything from this folder here.
   - `notes-data` (Private, empty): your notes will be backed up here.
2. In `notes-app`: Settings -> Pages -> Source = **GitHub Actions**.
3. In `notes-app`: Actions tab -> "Build app and website" -> Run workflow (wait ~5-10 min).
4. Open `https://YOURNAME.github.io/notes-app/` on your phone and tap Download APK.
5. GitHub -> Settings -> Developer settings -> Personal access tokens -> Fine-grained tokens -> Generate:
   Repository access = only `notes-data`; Permissions -> Contents = Read and write.
6. In the app: create your username/password, then ⋯ -> GitHub sync -> enter `YOURNAME/notes-data` + token.
7. New phone: install the APK, tap "Restore from GitHub", enter the same repo + token, then log in with your old username/password.
