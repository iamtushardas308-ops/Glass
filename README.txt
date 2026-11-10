Glass FLAC Player - APK project

BUILD WITHOUT ANDROID STUDIO (GitHub, free):
1. Create a new GitHub repository.
2. Upload everything from this folder, keeping the structure:
   www/index.html, package.json, capacitor.config.json, .github/workflows/build.yml
   (If the hidden .github folder won't upload: in GitHub choose Add file > Create new file,
   name it  .github/workflows/build.yml  and paste the contents of build.yml.)
3. Open the Actions tab > "Build APK" > Run workflow.
4. When it finishes (about 5 minutes), open the run and download the "Glass-APK" artifact.
5. Unzip it, copy app-debug.apk to your phone, tap it, and allow "Install unknown apps".

BUILD WITH ANDROID STUDIO:
npm install && npx cap add android && npx cap sync android && npx cap open android
