![KneeCare Device](https://i.imgur.com/DpRrWEZ.png)
![Description of GIF](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExMTB4MzFnaDNlY2JrN2Y1YmFhMTdoenpqenU2YW96b2p0aWdzZXkydiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/PLwDML27b3sFuBYxlo/giphy.gif)
![Description of GIF](https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExcWV4YTJwam1pYjBqeGxrb3BqZHJnODVuMG5xdW11eWc0dXB2eXp2OCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/P9zKIAXygDJb7cndZM/giphy.gif)
))

https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExcWV4YTJwam1pYjBqeGxrb3BqZHJnODVuMG5xdW11eWc0dXB2eXp2OCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/P9zKIAXygDJb7cndZM/giphy.gif
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


## 📸 Example Photos

> *(Add images below once available – showing the ESP32, gyro sensors on the knee brace, breadboard setup, and screenshots of the website)*

![Knee](https://i.imgur.com/miewglJ.png)
![GYRO](https://i.imgur.com/qxzGwvp.png)


## System Workflow

1. **Data Acquisition**: The ESP32 collects motion data from the gyroscopic sensors during user activity.
2. **Data Transmission**: Captured data is wirelessly transmitted to the Firebase Realtime Database.
3. **Data Access**: Users log into the web application to view and analyze their movement data, which is securely linked to their unique user ID.

## Folder Structure Conventions
## ============================

> Folder structure options and naming conventions for software projects

### Knee-Care top-level directory layout

    .
    ├── firebase-esp/                 # ESP32 firmware interfacing with Firebase
    ├── javascript/                   # JavaScript files for web application functionality
    ├── working-mpu6050-to-firebase/  # Code for transmitting MPU6050 sensor data to Firebase
    ├── css/                          # Stylesheets for the web application
    ├── src                     # Source files (alternatively `lib` or `app`)
    ├── images/                       # Project-related images and media files
    ├── docs/                         # Documentation and design-related materials
    ├── License                       # License file for the project
    └── README.md


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

