# Old British Cars AI Video Director — Android APK Build

This is the APK-first Android project for the Old British Cars workflow.

## What is already implemented
- Simple Android UI
- Paste script
- Demo Mode with NO API spending
- Optional Gemini scene planning
- Optional ElevenLabs narration generation
- Project file saved on the phone
- Old British Cars-specific scene/B-roll instructions
- Cloud-build GitHub Actions workflow

## Important
This package is source code, not an APK binary. The included GitHub Actions workflow builds the APK in the cloud so Android Studio is not required.

## Cloud build
1. Create a GitHub repository.
2. Upload this project folder.
3. Open **Actions → Build APK → Run workflow**.
4. Download the artifact named `OldBritishCars-AI-Editor-debug`.
5. Extract it and install `app-debug.apk` on Android.

## API spending safety
The app starts with paid API calls OFF. If OFF, it uses Demo Mode and does not call Gemini or ElevenLabs. Paid calls happen only after the user enables the checkbox and supplies API keys.

## Current scope
The APK currently creates the AI director/voice/project stage. The final MP4 renderer is the next module and should run in the cloud with FFmpeg/Remotion so the phone does not need heavy rendering.
