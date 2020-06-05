i# Popular Movies Project
![Minimum API level](https://img.shields.io/badge/API-16+-yellow)

Most of us can relate to kicking back on the couch and enjoying a movie with friends and family. In this project, you’ll build an app to allow users to discover the most popular movies playing.

You’ll build the complete functionality of this app in two stages which you will submit separately.

## Table of contents
* [General info](#general-info)
* [What I will learn](#what-i-will-learn)
* [Required Tasks](#required-tasks)
* [Stage 1: Main Discovery Screen, A Details View, and Settings](#stage-1-main-discovery-screen-a-details-view-and-settings)
    * [User Experience](#user-experience)
    * [Implementation guidance](#implementation-guidance)
    * [UX Mockups](#ux-mockups)
* [Quality guidelines](#quality-guidelines)
* [Rubric](#rubric)
* [Setup](#setup)
* [Versioning and dependencies](#versioning-and-dependencies)

## General info
This is the second project of the Udacity Android Developer Nanodegree Program.

## What I will learn
* You will fetch data from the Internet with theMovieDB API.
* You will use adapters and custom list layouts to populate list views.
* You will incorporate libraries to simplify the amount of code you need to write
* Build clean and compelling user interfaces (UIs) and optimize the experience for various mobile devices. 

## Required Tasks
* Build a UI layout for multiple Activities.
* Launch these Activities via Intent.
* Fetch data from themovieDB API

## Stage 1: Main Discovery Screen, A Details View, and Settings
### User Experience
In this stage you’ll build the core experience of your movies app.
Your app will:
* Upon launch, present the user with an grid arrangement of movie posters.
* Allow your user to change sort order via a setting:
  * The sort order can be by most popular, or by top rated
* Allow the user to tap on a movie poster and transition to a details screen with additional information such as:
  * original title
  * movie poster image thumbnail
  * A plot synopsis (called overview in the api)
  * user rating (called vote_average in the api)
  * release date
### Implementation guidance
#### Image Library - Picasso
We recommend that this project use Picasso, a powerful library that will handle image loading and caching on your behalf. If you prefer, you’re welcome to use an alternate library such as Glide.
Picasso will handle loading the images on a background thread, image decompression and caching the images.
#### themoviedb.org API
##### Stage 1 - API Hints
To fetch popular movies, you will use the API from themoviedb.org. In order to request popular movies you will want to request data from the /movie/popular and /movie/top_rated endpoints (documentation). An API Key is required.
IMPORTANT: PLEASE REMOVE YOUR API KEY WHEN SHARING CODE PUBLICALLY
### UX mockups
<img src="./docs/mockup1.png" width="80%"/> | <img src="./docs/mockup2.png" width="80%"/> |

## Quality guidelines
### Visual Design and User Interaction
#### Standard Design
- App does not redefine the expected function of a system icon (such as the Back button).
- App does not redefine or misuse Android UI patterns, such that icons or behaviors could be misleading or confusing to users.
#### Navigation
- App supports standard system Back button navigation and does not make use of any custom, on-screen "Back button" prompts.
- All dialogs are dismissible using the Back button.
- Pressing the Home button at any point navigates to the Home screen of the device.
### Functionality
#### Permissions
- App does not redefine or misuse Android UI patterns, such that icons or behaviors could be misleading or confusing to users.
- App does not request permissions to access sensitive data or services that can cost the user money, unless related to a core capability of the app.
#### User/App State
- App correctly preserves and restores user or app state, that is , student uses a bundle to save app state and restores it via onSaveInstanceState/onRestoreInstanceState. For example,
    - When a list item is selected, it remains selected on rotation.
    - When an activity is displayed, the same activity appears on rotation.
    - User text input is preserved on rotation.
    - Maintains list items positions on device rotation.
- When the app is resumed after the device wakes from sleep (locked) state, the app returns the user to the exact state in which it was last used.
- When the app is relaunched from Home or All Apps, the app restores the app state as closely as possible to the previous state.
### Performance and stability
#### Stability
- App does not crash, force close, freeze, or otherwise function abnormally on any targeted device.
- You must make sure your app does not crash when there is no network connection! 
### Google Play
#### Content policies
- All content is safe for work content.
- App adheres to the Google Play Store App policies.
- App’s code follows standard Java/Android Style Guidelines.

## Rubric

### Common Project Requirements
| MEETS SPECIFICATIONS  |
|---|
| App is written solely in the Java Programming Language |
| Movies are displayed in the main layout via a grid of their corresponding movie poster thumbnails. |
| UI contains an element (i.e a spinner or settings menu) to toggle the sort order of the movies by: most popular, highest rated. |
| UI contains a screen for displaying the details for a selected movie. |
| Movie details layout contains title, release date, movie poster, vote average, and plot synopsis. |
| App utilizes stable release versions of all libraries, Gradle, and Android Studio. |

### User Interface - Function
| MEETS SPECIFICATIONS |
|---|
| When a user changes the sort criteria (“most popular and highest rated”) the main view gets updated correctly. |
| When a movie poster thumbnail is selected, the movie details screen is launched. |

### Network API Implementation
| MEETS SPECIFICATIONS |
|---|
| In a background thread, app queries the /movie/popular or /movie/top_rated API for the sort criteria specified in the settings menu. |

### General Project Guidelines
|  MEETS SPECIFICATIONS |
|---|
| App conforms to common standards found in the [Android Nanodegree General Project Guidelines](#http://udacity.github.io/android-nanodegree-guidelines/core.html) (NOTE: For Stage 1 of the Popular Movies App, it is okay if the app does not restore the data using onSaveInstanceState/onRestoreInstanceState) |

## Setup
### themoviedb.org API key
If you don’t already have an account, you will need to create one in order to request an API Key. In your request for a key, state that your usage will be for educational/non-commercial use. You will also need to provide some personal information to complete the request. Once you submit your request, you should receive your key via email shortly after.

## Versioning and dependencies

**Target SDK Version:** 29

**Gradle Version:** 3.6.3

**Dependencies:**
- com.squareup.picasso:picasso:2.71828

**Android Studio Version:** 3.6.3 (Stable Release)

