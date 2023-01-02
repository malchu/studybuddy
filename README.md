# studybuddy
*CMSC436 Android Final Group Project, December 2022*<br />
*Team Members: Malchu Pascual, Thomas Gacquin, Avan Balasubramaniam, Theo Rousset*
## Introduction
The goal of this app is to allow users to create flashcards that they can save and review, akin to Quizlet.
## Description
### Key Functionality
Upon booting up the app for the first time, the user should be asked to sign in using Google. After signing in, they can either make a new set of flashcards or review their previous sets (presented with two different buttons). If they choose to make a new set of flashcards, they are led to a screen where there is a button to add an empty flashcard to the set. Once they add it, there are two lines on the empty flash card: one for the term, one for the definition. Each flashcard added will also have a button on it to delete it. The user can keep adding and editing the flash cards. Once they exit the activity, their set is saved and can be reviewed by navigating to the user’s flash cards from the navigation menu. They can click on their set and can navigate through each card using arrows on the screen. Tapping on the flash card flips it to the definition.
### Architecture and Components
The app will be saving a user’s flashcards to their account in a database. As such, we will use Firebase to not only store flashcard data, but also handle log-in, registration, and authorization through Firebase’s authorization for Google sign-in. The app include 5 activities:<br />
* Sign-in page with Google authorization
* A menu to navigate to either the flashcard maker or list of the user’s flashcards
* The flashcard maker (back button included)
* List of user’s flashcards (back button included)
* Activity to review user’s flashcards (back button included)<br />
<!-- -->
Basic activities such as the sign in page, flashcard review page, and menu navigator will rely on a Constraint Layout. Activities such as the flashcard maker and list of user’s flashcards will use a RecyclerView. There will be a layout for the flashcard in the flashcard viewer and another for the flashcards in the flashcard maker. There are no plans to utilize fragments. Workload delegations are specified below.
### Screenshots
#### Flashcard Set
![Alt text](FlashcardSet.jpg?raw=true "")
#### Main Menu Set
![Alt text](MainMenuSet.jpg?raw=true "")
## Showcase
Click the YouTube link below:<br />
[[YouTube Link]](https://youtu.be/mN7u5PirROo)

