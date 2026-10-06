Setup Instructions
This document provides instructions for setting up the Noir Music project for development.
Prerequisites
- Android Studio (latest version recommended)
- Android SDK (API level as specified in build.gradle.kts)
- JDK 21
- Git
  Initial Setup
1. Clone the Repository
   git clone https://github.com/bipinsanjeeva/Noir-Music.git
   cd Noir-Music
2. Configure Local Properties
   Create a local.properties file from the template:
   cp local.properties.template local.properties
   Edit local.properties and set your Android SDK path:
   sdk.dir=/path/to/your/android/sdk
   Example paths:
- macOS: /Users/username/Library/Android/sdk
- Linux: /home/username/Android/sdk
- Windows: C:\\Users\\username\\AppData\\Local\\Android\\sdk
3. Configure Firebase (Optional)
   Firebase is used for analytics and crash reporting. If you want to use these features:
1. Create a Firebase project at Firebase Console.
2. Add an Android app to your Firebase project.
3. Download the google-services.json file.
4. Place it in the app/ directory.
   Note: If you skip Firebase setup, the app will still build and run, but analytics and crash reporting will be disabled.
4. Configure Release Signing (Optional)
   For release builds, you need to configure signing credentials. Set these as environment variables or in gradle.properties.
5. Build the Project
   Open the project in Android Studio or build from the command line.
   Noir Music has two build variants: FOSS (without Google Play Services / Cast) and GMS (with Cast support).
   Windows:
   .\gradlew.bat assembleUniversalFossDebug
   .\gradlew.bat assembleUniversalGmsDebug
   For release builds:
   .\gradlew.bat assembleUniversalFossRelease
   .\gradlew.bat assembleUniversalGmsRelease
6. Configure AI Translation (Optional)
   Noir Music supports AI-powered lyrics translation. You can configure this in Settings -> AI Settings.
   Option A: Using OpenRouter (Default)
1. Get an API Key from OpenRouter.
2. In the app, go to Settings -> AI Settings.
3. Ensure Provider is set to OpenRouter.
4. Enter your API Key.
   Option B: Using Custom Provider
   Use this for other services like OpenAI, Anthropic, or local LLMs.
1. In the app, go to Settings -> AI Settings.
2. Select your Provider.
3. If using Custom, enter your provider's Base URL.
4. Enter your API Key.
   Important Files
   Confidential Files (Never commit these)
- local.properties - Contains your local SDK path
- app/google-services.json - Contains Firebase credentials
- *.keystore - Contains signing keys for release builds
- gradle.properties - May contain signing credentials
  These files should never be committed to version control.
  Troubleshooting
  Build Fails with "SDK location not found"
  Make sure you've created local.properties with the correct SDK path.
  Gradle Sync Issues
  Try cleaning and rebuilding:
  .\gradlew.bat clean
  .\gradlew.bat build
  Contributing
  Please read CONTRIBUTING.md for details on the code of conduct and the process for submitting pull requests.
  License
  This project is licensed under the GNU General Public License v3.0 - see the LICENSE file for details.