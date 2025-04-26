# SavedInstanceStateTutorial

This project demonstrates how to save and restore activity state during configuration changes in Android. It showcases the use of **SavedInstanceState** to retain UI-related values like a counter, ensuring the state is preserved even after screen rotations or activity recreations.

## Concepts
- **SavedInstanceState**: A mechanism used in Android to save and restore activity state. It is especially useful during configuration changes like screen rotations or when an activity is destroyed and recreated.
- **onSaveInstanceState()**: This method is called to store data that should survive configuration changes. It saves data to a `Bundle`, which is passed to `onCreate()` or `onRestoreInstanceState()` during activity recreation.
- **onRestoreInstanceState()**: This method is used to retrieve data saved during configuration changes or activity recreation. It is called after `onStart()` to restore the UI to its previous state.
- **Configuration Changes**: These include screen rotations, language changes, or when the system kills and recreates an activity due to resource constraints.
- **Jetpack Compose State Management**: Jetpack Compose uses `rememberSaveable` to save UI state across configuration changes, which works under the hood with `SavedInstanceState`.

## Features
- Demonstrates saving and restoring data across configuration changes.
- Uses `onSaveInstanceState()` and `onRestoreInstanceState()` to persist and retrieve UI state.
- Works with simple UI elements (e.g., a counter) to show state preservation.

## Setup
1. Clone the repository:
    ```bash
    git clone https://github.com/tashafdev/SavedInstanceStateTutorial.git
    ```

2. Open the project in Android Studio.

3. Run the app on a physical device or emulator.

## Usage
- Interact with the UI and trigger configuration changes (like screen rotation).
- Observe how the counter value is preserved and restored during configuration changes.

## Contributing
Feel free to fork the repository and submit pull requests for enhancements or bug fixes.
