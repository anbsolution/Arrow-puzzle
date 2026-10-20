# Arrow Puzzle ULTRA v17 — Android APK build

This release adds configurable ULTRA PRO gameplay options: large touch controls, high contrast board, reduced motion, haptic feedback (when supported), and directional labels. Preferences are saved locally. The Capacitor wrapper and GitHub Actions workflow build a debug APK on GitHub-hosted runners; Termux does not compile the APK.

## Mobile-only steps
1. Download and extract `arrow-puzzle-ultra-v17-pwa.zip` on your phone.
2. Copy the contents of `arrow-puzzle-ultra-v17-pwa/` into your existing `Arrow-puzzle` repository folder in Termux. Keep the repository name unchanged.
3. Run `git add .`, `git commit -m "Upgrade Arrow Puzzle ULTRA v17 Pro Options"`, and `git push`.
4. On GitHub, open the repository → **Actions** → **Build Arrow Puzzle ULTRA v17 Android APK**. Wait for the workflow to finish.
5. Open the completed run → **Artifacts** → `Arrow-Puzzle-ULTRA-v17-debug-apk` → download and extract the artifact ZIP to get `app-debug.apk`.
6. Install the APK on your Android device for testing.

## Notes
- The APK is a debug build for testing, not a Play Store release.
- An APK artifact exists only after a successful GitHub Actions run.
- No Android SDK/Gradle compilation is performed in Termux.
- GitHub Pages continues to serve the root `index.html`.
