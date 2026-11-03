# smm2-ios-build

A GitHub Actions workflow that builds [SMM2 Recomp](https://github.com/smm2recomp/smm2recomp) for iOS / iPadOS
on a macOS runner, for the repository owner's own device, from the owner's own copy of the game.

Nothing from the game is in this repository or readable from it. The input lives encrypted in a separate private
repository. The build's outputs (the IPA and the build log) are uploaded encrypted, kept for one day, and decrypted
only on the owner's machine. See `.github/workflows/ios.yml`.

Run it from the Actions tab (workflow **ios**, "Run workflow"), or with:

```sh
gh workflow run ios.yml
```
