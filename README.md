# Artist Analysis with the iTunes search API

## Introduction
The goal of this coding project is to compare artists based on the number of albums they have produced and the number of large albums. To achieve this goal, we will use the iTunes search API to obtain the artist's ID and album data. We will then extract the relevant data and compare the number of albums produced by different artists.

## Data
The data used in this project is obtained using the iTunes search API. The API is queried using the requests library in Python. We obtain the artist's ID using their name and use that ID to get album data from the API. The album data obtained from the API is in the JSON format and is then parsed to extract relevant information.

## Methodology
We use two functions to obtain the required data. The first function `get_id_from_name(artist_name)` takes the name of the artist as input and returns the artist's ID. We pass the ID obtained from the first function to the second function `get_albums_from_id(id)` which returns the album data for the artist in JSON format. We then use a helper function `albumsMoreThanN(id,n)` to count the number of albums with more than n tracks. Finally, we compare the number of albums produced by two artists using the `more_productive(artist_name1, artist_name2)` function and the number of large albums produced by two artists using the `musical_generosity(artist_name1, artist_name2,n)` function.

## Results
The functions `more_productive()` and `musical_generosity()` print the results of the comparison of artists based on the number of albums and the number of large albums, respectively. The `more_productive()` function prints the total number of albums produced by each artist and the artist with more albums produced. The `musical_generosity()` function prints the total number of albums produced by each artist with more than n tracks and the artist with more albums produced.

## Conclusion
The iTunes search API provides an easy way to obtain data about artists and their albums. By using this API, we can compare artists based on the number of albums they have produced and the number of large albums. The functions developed in this project can be used to compare any two artists, making it a useful tool for music enthusiasts and researchers.

## Learnings and Skills Learned
In this project, we learned how to use the iTunes search API to obtain data about artists and their albums. We also learned how to parse JSON data in Python using the json library. The project helped us develop our skills in working with APIs, parsing JSON data, and comparing data using Python.

## Importance
The ability to compare artists based on the number of albums they have produced and the number of large albums is important for music enthusiasts and researchers. It provides a quick and easy way to compare artists and their productivity. The functions developed in this project can be used to compare any two artists, making it a valuable tool for music enthusiasts, researchers, and music industry professionals.
