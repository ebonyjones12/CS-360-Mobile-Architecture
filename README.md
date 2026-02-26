# Focus - Weight Tracking App
## CS 360 Mobile Architecture & Programming

### Project Overview
Focus is an Android mobile application designed to help users track their weight over time. The app provides a simple, intuitive interface for logging daily weight entries and monitoring progress toward fitness goals.

### App Features

#### 1. User Authentication
- Secure login screen with username and password fields
- Password input is obscured for security
- New user account creation functionality
- Simple and clean user interface

#### 2. Weight Data Management
- Data Grid Display: View all weight entries in an organized table format
- Add Entries: Input date and weight measurements
- Delete Entries: Remove individual weight records with dedicated delete buttons
- Scrollable Interface: View historical data with smooth scrolling

#### 3. SMS Notifications
- Goal notification system via SMS
- Permission request handling for SMS access
- User control over notification preferences
- Notifications trigger when users reach their goal weight

### Technical Implementation

**Login Screen** (activity_login.xml)
- Username input field
- Password input field (text obscured)
- Login button
- Create Account button

**Weight Data Grid** (activity_weight_data.xml)
- Date and weight input fields
- Add button for new entries
- Data grid with headers (Date, Weight, Action)
- Delete buttons for each row
- SMS notification permission button

### Permissions & Manifest
- SMS Permission: SEND_SMS for goal notifications
- Telephony Feature: Declared in AndroidManifest.xml
- Permission handling with user consent

### Design Principles
- User-Centered Design: Clean, intuitive interface focused on ease of use
- Visual Hierarchy: Logical flow from input to data display
- Consistent Theme: Blue and white color scheme throughout
- Responsive Layout: Works across different screen sizes

### Development Environment
- IDE: Android Studio
- Language: Java
- Minimum SDK: API 24 (Android 7.0 Nougat)
- Build System: Gradle

### Author
Ebony Jones

---

## Project Reflection

**Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?**

The goal of my app was to help users track their weight and reach their fitness goals. Users needed a simple way to log their daily weight, set a goal weight, and get notified when they hit that goal. I also wanted to address the need for guidance on what to eat by adding features where users could ask the app if a meal is healthy and get portion recommendations. The app was designed to be like having a nutrition coach in your pocket.

**What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?**

The app needed a login screen for account creation and authentication, a main screen with a grid showing daily weights and dates, and the ability to add new weight entries and set a goal weight. I followed Material Design guidelines to keep the layout clean and easy to navigate. I kept users in mind by making sure the most important actions like adding weight were easy to find and only a tap or two away. The design was successful because it was simple and not cluttered with unnecessary features.

**How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?**

I took it step by step instead of trying to do everything at once. I started with the database structure and made sure I understood how the three tables (user logins, daily weights, and goal weight) would work together. Then I built out the UI screens and connected them to the database one feature at a time. I tested as I went so I could catch problems early. This approach can be applied to any future project because breaking things into smaller pieces makes the work less overwhelming.

**How did you test to ensure your code was functional? Why is this process important, and what did it reveal?**

I tested the app using the Android emulator and ran through each feature manually to make sure it worked. I would add a weight entry, check that it saved to the database, and make sure it showed up in the grid. Testing is important because it helps you find bugs before the user does. It revealed small issues like buttons not connecting to the right activity that I was able to fix before moving on.

**Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?**

One challenge was figuring out how to connect the UI to the SQLite database so that data would actually save and load correctly. I had to learn how the database helper class works and how to write queries that pull the right information. I also had to think through how to handle user permissions for SMS notifications without crashing the app if the user denied permission.

**In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?**

I was most successful with the database design and connecting it to the user interface. Setting up the three tables and making sure data flowed correctly between the screens and the database showed that I understand how the backend and frontend of an app work together. This is a skill I can use in future development projects and in my career.
