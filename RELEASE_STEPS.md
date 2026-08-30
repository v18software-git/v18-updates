# Release Steps

1. Create or restore the GitHub repository:

   ```text
   V18PreniumTuition/v18-updates
   ```

2. Commit `latest-version.json` to the `main` branch.

3. Create a GitHub Release tag, for example:

   ```text
   v0.2
   ```

4. Upload these release assets:

   ```text
   V18-Windows-0.2.zip
   V18-Android-0.2.apk
   ```

5. Edit `latest-version.json`:

   - Increase `windows.version`.
   - Increase `android.version`.
   - Increase `android.versionCode`.
   - Replace both `url` values with the new release asset URLs.
   - Replace both `fileName` values with the new asset names.
   - Update `notes` and `features`.

6. Commit the updated `latest-version.json`.

The app will keep checking the same raw manifest URL. If the repo is recreated with the same owner/name and branch, the app does not need code changes.

