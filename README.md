Project Description: FaceTagger

Project Overview: FaceTagger is an Android app designed to scan a user's photo gallery, detect human faces in camera-captured images, and provide a seamless way to tag each detected face. The app leverages modern Android development practices using Jetpack Compose for a fluid and dynamic user interface, MediaPipe for efficient face detection, and Kotlin Flows for handling asynchronous data processing. It also includes a detailed view where users can see bounding boxes around detected faces.

Key Features:

Camera-Only Image Selection:
FaceTagger scans the user's photo gallery and loads only those images that were captured using the camera. This ensures a focused set of images for processing, filtering out screenshots, downloaded images, or other media files.

Face Detection with MediaPipe:
The app uses Google's MediaPipe framework for detecting human faces in each selected image. It identifies faces, marks their positions, and draws bounding boxes around them to visualize the detection.

Grid Display of Photos:
Images containing faces are displayed in a grid view using Jetpack Compose's LazyVerticalGrid. This allows users to easily browse through all the photos where faces have been detected.

Real-Time Progress Indicator:
FaceTagger shows the progress of face detection with a counter that updates in real time. This indicates how many images have been processed and how many contain detected faces, providing users with a clear view of the app’s activity.

Interactive Image Detail View:
When a user selects an image from the grid, the app navigates to a detailed view where the selected image is displayed with bounding boxes drawn around each detected face. Users can easily view the exact location of detected faces.

Tagging Faces:
Users can tap on detected faces in the detailed view to add tags or names, helping them organize and remember faces in their photos. This feature adds a personal touch, making it easier to identify people in the images.

Modern Architecture & Best Practices:

Jetpack Compose: Ensures a responsive and modern UI.
Kotlin Flows: Used for managing asynchronous data streams, such as loading images and detecting faces.
MVVM Architecture: For a clean separation of concerns, with ViewModel handling business logic and UI-related data.
Accompanist Permissions: Manages runtime permissions for gallery access.
Room Database: Stores tagged face data locally for easy retrieval.
Technical Stack:

Programming Language: Kotlin
UI Framework: Jetpack Compose
Image Loading: Coil (for displaying images)
Face Detection: MediaPipe
Asynchronous Handling: Kotlin Flows & Coroutines
State Management: ViewModel and StateFlow
Permissions: Accompanist for handling runtime permissions
Local Storage: Room for storing user-defined tags
User Flow:

Gallery Permission:
Upon launching the app, the user is prompted to grant permission to access their photo gallery.

Image Loading:
FaceTagger scans the gallery and loads only camera-captured images. A loading indicator shows the progress as images are analyzed for faces.

Face Detection:
The app filters out images without faces and displays those with detected faces in a scrollable grid.

Viewing and Tagging Faces:
Users can tap any image in the grid to open a detailed view, where bounding boxes highlight detected faces. Users can then tap on faces to add tags or names.

Summary of Detected Faces:
The app provides a summary of how many images were processed and how many contained faces, giving users insight into the face detection results.

Use Cases:

Personal Photo Management: Easily organize and tag photos of friends and family.
Event Organization: Tag people in photos from events like weddings, parties, or gatherings.
Security and Monitoring: Useful for quickly scanning through camera images to identify human presence.
Evaluation Criteria:

Completeness: Ensuring all requirements are met, including proper image filtering, face detection, and tagging.
Code Organization: Follows a clean and modular structure, adhering to MVVM design principles and Compose best practices.
Performance: Efficient image loading and face detection using background threads and Kotlin Coroutines.
UI/UX Design: A user-friendly interface that aligns with Material Design guidelines and provides a smooth experience.
Submission:
The completed app will be submitted as a GitHub repository, with a README providing an overview of the solution, setup instructions, and architecture details. A screen recording demonstrating the app's functionality will be included to showcase the user experience.

