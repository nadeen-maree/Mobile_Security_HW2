# Project Name: Survive & Reach - Reverse Engineering

## Description

Survive & Reach is a simple game where players have to find a way to survive and reach their city. The game requires the player to enter their ID to proceed further, and then they must follow the code's instructions to navigate through the challenges.

## Table of Contents

- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [Bugs and Issues](#bugs-and-issues)
- [Contributing](#contributing)
- [License](#license)

## Installation

To get started, I followed these instructions to reverse engineer the APK file and make the application work:

1. Clone the repository to your local machine.
2. Use JADX or a similar tool to decompile the APK file. If you encounter any issues with JADX, you can try using other APK decompilation tools like JADX-GUI or apktool. (Please note that JADX was found useful in resolving the issues during the development process).
3. Create a new Android project on Android Studio.
4. Adapt the manifest file from the decompiled project and integrate it into your new project.
5. Copy the relevant files and assets from the decompiled APK into your new project.
6. Ensure the URL link format used to access game data is correct.
7. Address any bugs or errors you encounter during the process.

## Usage

1. Build and run the modified project on an Android emulator or physical device.
2. Enter your ID to proceed to the game.
3. Follow the instructions given in the game's UI to survive and reach your city.

## Bugs and Issues

During the reverse engineering process, the following bugs were encountered and fixed:

1. **APK Extraction**: Initially, the APK extraction using apktool didn't work correctly. It was resolved by using the JADX tool, which proved to be more effective for this specific project.

2. **URL Link Format**: The URL link format used to access game data was incorrect. It was corrected to ensure proper functioning of the game.

3. **Data and ID Fragmentation Bug**: An error 'java.lang.ArrayIndexOutOfBoundsException' occurred, indicating that the program was trying to access an array element that did not exist. To fix this, user input validation was implemented to check if the entered ID was at least 8 digits long. If the ID is less than 8 digits, a toast message is displayed, preventing the bug from occurring.

Please report any new bugs or issues you encounter while running the game.

## Contributing

Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License

The Survive & Reach project is licensed under the [MIT License](LICENSE).

