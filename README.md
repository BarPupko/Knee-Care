# KneeCare – Intelligent Knee Health Monitoring System

**KneeCare** is an innovative wearable device designed to monitor and analyze knee health in real-time. Utilizing an **ESP32 microcontroller** paired with **two gyroscopic sensors (GYROs)** mounted on a knee protector, the system captures detailed movement data during physical activities. Its portability is ensured by a battery integrated onto a breadboard adjacent to the ESP32, allowing users to move freely while wearing the device.

The collected data is transmitted to a **Firebase Realtime Database**, providing users with secure access to their personalized information through a dedicated web interface. This platform enables functionalities such as user registration, authentication, data visualization, and password management.

## Hardware Components

- **ESP32 Microcontroller**: Serves as the central processing unit, handling data acquisition and wireless communication.
- **Gyroscopic Sensors (2x GYROs)**: Attached to the knee protector to measure angular velocity and orientation.
- **Battery Module**: Mounted on a breadboard alongside the ESP32, supplying power to the entire system and facilitating mobility.
- **Knee Protector**: Acts as the structural framework, securing the electronic components comfortably around the knee.

## Software Architecture

- **Firebase Realtime Database**: Manages real-time data storage and retrieval, ensuring seamless synchronization between the device and the web interface.
- **Firebase Authentication**: Provides secure user authentication using email and password, ensuring that user data remains confidential and inaccessible to administrators.
- **Web Application**: Developed to offer users an intuitive interface for:
  - **Registration and Login**: Secure account creation and access.
  - **Unique User Identification**: Assigns a distinct ID to each user for personalized data management.
  - **Data Visualization**: Displays real-time and historical movement data.
  - **Password Recovery**: Facilitates secure password reset procedures.

## System Workflow

1. **Data Acquisition**: The ESP32 collects motion data from the gyroscopic sensors during user activity.
2. **Data Transmission**: Captured data is wirelessly transmitted to the Firebase Realtime Database.
3. **Data Access**: Users log into the web application to view and analyze their movement data, which is securely linked to their unique user ID.

## Folder Structure

The project's repository is organized as follows:
Knee-Care/ ├── Firebase-ESP/ # Firmware for ESP32 to interface with Firebase ├── JavaScript/ # JavaScript files for web application functionality ├── Working-mpu6050-to-Firebase/ # Initial attempts to connect MPU6050 sensor to Firebase ├── css/ # Stylesheets for web application ├── html/ # HTML files for web interface ├── image/ # Images used in the web application ├── website/ # Web application source code ├── README.md # Project documentation (this file) ├── package-lock.json # Dependency tree for Node.js packages └── script.js # Main JavaScript file for web application interactivity


## Security and Privacy

User data security is paramount. The system employs Firebase Authentication to ensure that all user information is protected using email and password credentials. Data stored in the Firebase Realtime Database is encrypted and remains inaccessible to administrators, safeguarding user privacy.

## Future Enhancements

Planned improvements for the KneeCare system include:

- **Integration of Machine Learning Algorithms**: To analyze movement patterns and detect potential anomalies or early signs of knee-related issues.
- **Mobile Application Development**: Offering users a more accessible platform to monitor their knee health on-the-go.
- **Extended Battery Life**: Optimizing power consumption to prolong usage between charges.
- **Additional Sensor Integration**: Incorporating other sensors to provide a more comprehensive analysis of knee health.

## Author
**Kfir Nudlman**  
Practical Software Engineer student in Kineret 

**Bar Popko**  
Automation & Validation Engineer at ACS Motion Control  
Email: [barpupco@gmail.com](mailto:barpupco@gmail.com)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

