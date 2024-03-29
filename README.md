# Guardians' Playlist Generator
This repository contains my JavaScript solution for generating personalized playlists for the Guardians based on their preferred music genres.

## Overview
The program utilizes a set of predefined songs and each Guardian's preferred genre to create custom playlists. It selects songs from the available pool based on the genre preference of each Guardian and generates a playlist containing three randomly chosen songs for each Guardian.

### Implementation
***The solution consists of the following components:***
1. ***Songs Database:*** An array of song objects containing information about the title, artist, and genre of each song.
2. ***Guardians' Preferences:*** An object mapping each Guardian to their preferred music genre.
3. ***Playlist Generation Function:*** A function (generatePlaylist) that takes in the Guardians' preferences and the songs database to generate personalized playlists.
4. ***Playlist Display Function:*** A helper function (displayPlaylists) to visually represent the generated playlists on an HTML page.

### How It Works
1. The generatePlaylist function iterates through each Guardian's preference.
2. For each Guardian, it filters the songs database to retrieve songs matching the Guardian's preferred genre.
3. From the filtered list, it selects three random songs to include in the playlist.
4. The Guardian's name is added as the title of the playlist.
5. Finally, the playlists are displayed on the HTML page using the displayPlaylists function.

### Challenges Faced
1. ***Data Filtering:*** One challenge was filtering the songs based on each Guardian's preferred genre.
   While the logic to filter songs based on a single genre is straightforward, handling multiple Guardians with different preferences required careful handling of data structures and iteration.
2. ***Random Selection:*** Another challenge was selecting random songs for each playlist.
   While JavaScript provides methods for randomizing arrays, ensuring that each playlist contains a unique selection of songs without duplicates required additional logic to handle.
3. ***HTML Rendering:*** Displaying the playlists on an HTML page posed a challenge, especially when dynamically generating HTML elements to represent the playlists and songs.
   Ensuring proper structure and styling while dynamically adding elements to the DOM required attention to detail.
4. ***Testing:*** Testing the solution thoroughly to ensure that it correctly generated playlists for each Guardian's preferred genre was essential.
   This involved running the code multiple times with different configurations of songs and Guardian preferences to verify its correctness.

### Lessons Learned
1. ***Data Manipulation:*** I learned various techniques for manipulating arrays and objects in JavaScript, such as filtering, mapping, and sorting.
   These skills are crucial for working with complex data structures and implementing algorithms efficiently.
2. ***Randomization:*** Understanding how to randomize elements in an array while ensuring uniqueness was an important lesson.
   I gained insights into using JavaScript's built-in functions for random number generation and array manipulation to achieve this.
3. ***DOM Manipulation:*** Working with the Document Object Model (DOM) to dynamically generate and modify HTML elements improved my understanding of web development fundamentals.
   I learned how to create and append elements, set attributes, and structure HTML content programmatically.
4. ***Problem-Solving:*** This project honed my problem-solving skills, especially in breaking down complex problems into smaller, manageable tasks and finding efficient solutions.
   It taught me the importance of clear logic, careful planning, and iterative development in tackling coding challenges.
5. ***Collaboration:*** While this project was completed individually, reflecting on potential collaboration scenarios helped me appreciate the importance of communication and teamwork in software development.
   Discussing ideas, sharing insights, and receiving feedback can lead to better outcomes and foster a collaborative spirit.

Overall, coding the solution to create playlists for the Guardians provided valuable learning experiences and reinforced essential programming concepts and skills.
