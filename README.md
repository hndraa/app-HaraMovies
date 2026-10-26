# HaraMovies — Movie Discovery & Booking App

**SOFTWARE | MOBILE APPLICATION | KOTLIN · ANDROID STUDIO**

HaraMovies is an Android movie discovery and booking application developed to help users explore movies, discover upcoming releases, view movie details, save favorites, and manage selected movies through a cart. The application integrates external movie data and provides a mobile interface for browsing and managing movie selections.

## 01. Project Overview

### Description

HaraMovies is a mobile application developed as a university coursework project for the Mobile Programming course at Universitas Mataram in 2025. Built with Kotlin in Android Studio, the application provides a centralized interface for discovering movies and managing movie selections.

### Objectives

- Provide an accessible interface for exploring movies and discovering new releases.
- Help users find movies using search and genre filters.
- Present movie information, including synopsis, ratings, and cast details where available.
- Allow users to save movies to a bookmark list.
- Provide a cart interface for managing selected upcoming movies.
- Implement account-related interfaces for login, registration, and profile management.

### Problem Statement

Movie information and personal watchlists can be difficult to manage when browsing across different platforms. Users may also need convenient ways to discover movies, review their details, and organize titles they want to watch.

### Solution

HaraMovies combines movie discovery, search, genre filtering, movie details, bookmarks, a cart, and profile management in one Android application. It retrieves movie information from an external movie API and organizes the main functions into dedicated screens.

### Main Features

- **Splash Screen:** Introduction screen with a Get Started button.
- **Authentication UI:** Login, registration, and password-reset interfaces.
- **Explore Movies:** Browse top-rated, upcoming, now-playing, and recommended movies.
- **Search and Genre Filtering:** Find movies by keyword and filter by genre.
- **Movie Details:** View movie information, synopsis, cast, and available actions.
- **Bookmark:** Save movies to a personal watchlist.
- **Cart:** Manage selected upcoming movies and access the checkout interface.
- **Profile:** View and edit profile information and profile photo.

## 02. Tech Stack

| Category | Technology |
|---|---|
| Programming Language | Kotlin |
| Development Environment | Android Studio |
| Build System | Gradle |
| Movie Data API | TMDb API |
| Local Database | SQLite, through the project's `DatabaseHelper.kt` |
| UI Layout | Android XML Layouts |
| Platform | Android |

**Additional configuration:** The project includes Firebase configuration and OAuth-related settings. Firebase services and their exact usage should be verified against the implementation before being documented as active application features.

## 03. Screenshots / Results

This section documents the implemented application screens and the primary user journey.

### 3.1 Splash Screen

The initial screen introduces HaraMovies and provides a Get Started action that leads to the authentication flow.

![HaraMovies Splash Screen](https://github.com/user-attachments/assets/61f55c41-b3c1-4c0b-a5c9-6d7b9fe3db7e)

### 3.2 Login

The login screen provides the interface for existing users to access the application.

![HaraMovies Login](https://github.com/user-attachments/assets/aa6847d2-e4d5-44d9-bd77-08a7d216a3b4)

### 3.3 Sign Up

The registration screen provides the interface for new users to create an account.

![HaraMovies Sign Up](https://github.com/user-attachments/assets/f9c1bde8-7998-4f48-9950-09d4bb02dd83)

### 3.4 Explore Movies

The Explore screen displays movie collections, including top movies, upcoming releases, now-playing titles, and recommendations.

![HaraMovies Explore](https://github.com/user-attachments/assets/620e8f24-2f22-4933-8c86-b49854b96de1)

![HaraMovies Movie Collections](https://github.com/user-attachments/assets/2a4b4a5a-c272-4dd2-9a15-a837212fd4f7)

### 3.5 Search and Genre Filtering

Users can search for movies and filter the displayed titles by genre.

![HaraMovies Search](https://github.com/user-attachments/assets/2fc680bb-e7ce-460e-9066-f706a9b8b736)

![HaraMovies Genre Filter](https://github.com/user-attachments/assets/20ac8c5f-0793-4dba-bec7-2ebb2bf6399b)

### 3.6 See All Movies

The See All screens allow users to browse a more complete list of movies within a selected collection.

![HaraMovies See All 1](https://github.com/user-attachments/assets/793b24d3-16fa-499f-925a-d8fd1e149658)

![HaraMovies See All 2](https://github.com/user-attachments/assets/9b3974c0-5b02-44fd-beb3-ba5c7e4e6ac1)

![HaraMovies See All 3](https://github.com/user-attachments/assets/7e32206d-36f7-41d0-8331-c48efd35ce3e)

### 3.7 Movie Details

The movie detail screen presents information about a selected movie, including its synopsis and cast, along with actions such as saving the movie.

![HaraMovies Movie Details](https://github.com/user-attachments/assets/0938a280-bf2f-488c-8249-d01ba3f53ee1)

### 3.8 Bookmark

The Bookmark screen displays movies saved by the user for future viewing.

![HaraMovies Bookmark](https://github.com/user-attachments/assets/1e3b7ba1-48d8-4687-a747-9d0f5e3d390f)

### 3.9 Cart

The Cart screen displays selected upcoming movies and provides access to the checkout interface.

![HaraMovies Cart](https://github.com/user-attachments/assets/d97999f7-e267-43a6-92b3-62a21c4d316d)

### 3.10 Profile

The Profile screen displays user information and provides profile editing options.

![HaraMovies Profile](https://github.com/user-attachments/assets/5085effc-bb92-4a38-8f84-3bdc5a3a715a)

### Results

The project demonstrates the implementation of an Android application with multiple screens, movie API integration, search and filtering interfaces, local data handling, and account-related UI.

The screenshots document the implemented user interface. They do not independently verify the security, production readiness, or end-to-end functionality of every external service.

## 04. Installation & Usage

### Prerequisites

- Android Studio compatible with the project's Gradle and Android Gradle Plugin versions.
- A compatible Java Development Kit (JDK), as required by the project.
- Android SDK and an Android emulator or physical Android device.
- Internet connection for retrieving movie data.
- Required service configuration, such as Firebase configuration, if needed by the implementation.

### Project Structure

```text
app-HaraMovies/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/
│   │       │   └── com/example/projectmobiles/
│   │       │       ├── data/
│   │       │       ├── domain/
│   │       │       └── presentation/
│   │       ├── res/
│   │       │   ├── drawable/
│   │       │   ├── layout/
│   │       │   ├── menu/
│   │       │   ├── navigation/
│   │       │   └── values/
│   │       └── AndroidManifest.xml
│   └── build.gradle.kts
├── gradle/
│   └── wrapper/
├── .gitignore
├── build.gradle.kts
├── gradle.properties
├── settings.gradle.kts
├── gradlew
└── gradlew.bat
```

*Note: This is a simplified overview. The actual repository may contain additional files and directories.*

### Installation Steps

**1. Clone the repository**

```bash
git clone https://github.com/hndraa/app-HaraMovies.git
cd app-HaraMovies
```

**2. Open the project**

Open Android Studio, select **Open**, and choose the cloned project directory containing `settings.gradle.kts`.

**3. Sync Gradle**

Allow Android Studio to synchronize the Gradle project and download the required dependencies.

**4. Configure external services**

Provide your own valid configuration for services required by the application. Do not commit private credentials, service-account keys, or secrets to the repository.

If Firebase is required, obtain an appropriate `google-services.json` for an authorized Firebase project and the application's configured package name. The original project configuration is not included in this repository.

**5. Run the application**

- Start an Android emulator or connect a compatible device.
- Select the application run configuration in Android Studio.
- Click **Run** to build and launch HaraMovies.

### Usage Flow

1. Launch HaraMovies and open the authentication interface.
2. Access the Explore screen.
3. Browse movie collections or search by title.
4. Filter movies by genre.
5. Open a movie to view its details.
6. Save a movie to Bookmark or add an eligible movie to Cart.
7. Open the Profile screen to view or edit profile information.

### Configuration Notes

- Movie data availability depends on the external API and network connection.
- Authentication and profile features may require the original backend or Firebase configuration, depending on their implementation.
- Cart and checkout interfaces should not be assumed to represent a production-ready payment flow without verification.
- Never include a Midtrans **Server Key**, private credentials, or other server-side secrets in Android source code or a public repository.

---
