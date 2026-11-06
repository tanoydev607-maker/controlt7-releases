# ControlT7 public downloads repository

This starter hosts the update website. It does not build ControlT7 or enable its in-app updater by itself.

## Upload these files

1. Create a PUBLIC GitHub repository named `controlt7-releases`, with default branch `main`.
2. Extract the ZIP. Upload the CONTENTS of this folder into the repository root, including `.github/workflows/pages.yml`. Do not upload the ZIP itself or an extra enclosing folder. Using Git or GitHub Desktop preserves the hidden `.github` folder reliably.
3. Open repository Settings > Pages > Build and deployment > Source and choose GitHub Actions.
4. Open Actions > Publish update website > Run workflow, selecting main.
5. After success, open Settings > Pages to find the website address.

## Next integration step

Give your developer the public repository URL. The separate PRIVATE source repository needs a trusted Windows release workflow that builds the complete bundled app, tests it, signs the installer, and uploads release assets here. A repository-scoped publishing credential is required for that cross-repository step.

The app needs the Tauri updater integration and public signing key. After a verified release exists, publish `site/preview.json` with the actual version, release notes, Windows x64 installer HTTPS URL, and generated updater signature. Its address will be `https://OWNER.github.io/controlt7-releases/preview.json`. The workflow deploys changes to `site` automatically.

There is deliberately no placeholder preview.json: an absent feed must be shown as unavailable, not as a successful no-update check. Never publish fabricated signatures or installer URLs.

Upload installers and signatures as GitHub RELEASE assets, not as Git-tracked files. Publish required component notices/source packages with each applicable release. Keep application source, chats, credentials and private signing keys out of this public repository.

Before offering updates, test installation from one packaged version to a newer version and preservation of local user data. Existing users need one manual installation of the updater-enabled app.
