# IoT Home Automation App

## Description

This is a home automation app for controlling various devices such as cameras, lights (inside and outside), and door locks. The app allows users to register, log in, and manage different smart devices in their home. It uses SQLite for data persistence and includes functionalities like adding, deleting, and displaying devices.

## Features

- **Login/Registration**: Users can register and log in to the app to manage their devices.
- **Cameras**: Add, view, and delete camera devices.
- **Lights**: Manage inside and outside lights.
- **Lock Doors**: Control front and back doors to lock and unlock them.
- **SQLite Database**: Persist data for devices using SQLite.
- **RecyclerView**: Display devices in a list using RecyclerView.

## Installation

### Prerequisites

- Android Studio (for development)
- Android device or emulator with API level 31 or higher
- SQLite database support in Android

### Steps

1. **Clone the repository**:

   ```bash
   git clone <repository-url>
   ```

2. **Open the project in Android Studio**.

3. **Build the project** by clicking on the "Build" menu and selecting "Rebuild Project".

4. **Run the app** on an Android device or emulator.

## Application Structure

### **Main Components**

- **LoginActivity**: Handles user login.
- **Registration**: Manages user registration.
- **MainMenuActivity**: The main menu with options to navigate to cameras, lights, devices, and door locks.
- **Cameras**: Activity to manage camera devices.
- **InsideLights & OutsideLights**: Activities to manage inside and outside lights.
- **LockDoors**: Activity to control door locks.
- **Adapters**: Custom `RecyclerView` adapters (e.g., `CameraAdapter`, `DeviceAdapter`) to display devices.

### **Database Helpers**

- **CameraDBHelper**: Manages CRUD operations for cameras.
- **DeviceDBHelper**: Manages CRUD operations for devices.
- **InsideLightDBHelper**: Manages CRUD operations for inside lights.
- **OutsideLightDBHelper**: Manages CRUD operations for outside lights.

## SQLite Tables

The app uses several SQLite tables to store device data:

- **tbl_camera**: Stores camera data (ID, description, angle).
- **tbl_device**: Stores device data (ID, make/model, owner).
- **tbl_light**: Stores inside and outside lights data (ID, room, type).

## Usage

### Logging In
Users can log in using predefined credentials or after registering.

### Adding Devices
Each device type (cameras, lights, locks) has a screen for adding and removing devices. Users input details like location, type, and additional device-specific parameters.

### Managing Lights
Users can manage both inside and outside lights, including turning them on or off and viewing their status.

### Controlling Doors
Lock or unlock doors from the app interface with a simple button click.

## Screenshots

*Add screenshots here of the main functionalities like camera management, light control, etc.*

## Future Enhancements

- Add more device types (thermostats, alarms, etc.).
- Integrate with cloud-based storage for user profiles and device data.
- Add push notifications for critical actions (e.g., door unlock alerts).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to update the repository URL, screenshots, and other relevant details to match your specific project needs.
