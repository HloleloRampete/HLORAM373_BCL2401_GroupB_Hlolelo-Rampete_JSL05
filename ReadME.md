# Guardians' Playlist Generator
## Manipulating Arrays data structres 

### Solutions 

``` function generatePlaylist(guardians, songs) {
    // Initialize an empty object to store playlists for each Guardian
    const playlists = {};

    // Iterate over each Guardian in the guardians array
    guardians.forEach(guardian => {
        // Generate a playlist for the current Guardian using the map() function
        // Map each song genre to a randomly selected song from that genre
        const playlist = songs.map(genre => {
            // Select a random song index for the current genre
            const randomIndex = Math.floor(Math.random() * genre.songs.length);
            // Return the randomly selected song for the current genre
            return genre.songs[randomIndex];
        });

        // Store the generated playlist for the current Guardian in the playlists object
        playlists[guardian] = playlist;
    });
 
    // Return the playlists object containing playlists for each Guardian
    return playlists;
}```



***Extra Notes:*** 
1. The function generatePlaylist() takes two parameters: guardians (an array containing the names of the Guardians) and songs (an array of objects, where each object represents a song genre along with an array of songs belonging to that genre).
2. Inside the function, an empty object playlists is initialized to store playlists for each Guardian.
3. The forEach() method is used to iterate over each Guardian in the guardians array.
4. Inside the loop, the map() function is used to generate a playlist for each Guardian. For each genre, a random song from the corresponding array of songs is selected.
5. The generated playlist for each Guardian is stored in the playlists object with the Guardian's name as the key.
6. Finally, the playlists object containing playlists for each Guardian is returned.
