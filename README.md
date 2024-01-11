# Movie-recommendation-system
<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
  </a>

  <h3 align="center">MOVIE RECOMMENDATION SYSTEM</h3>

  <p align="center">
    An awesome UI software which can recommend you movies,webshows!! 
    <br />
    <a href="https://github.com/SRM-3rd-Year-Project/Movie-recommendation-system-/blob/main/PPT/Mini%20Project%20Review.pdf"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://www.youtube.com/watch?v=k5e0udGD1OM&ab_channel=NisargDoshi">View Demo</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li>Built Using</li>
      </ul>
    </li>
    <li>
      <a href="#website-Preview">Website Preview</a>
      <ul>
        <li>User Access Page</li>
        <li>Home Page</li>
        <li>Watchlist Section</li>
        <li>Tracker Section</li>
        <li>Recommendation Section</li>
        <li>Explore Section</li>
        <li>Support Section</li>
      </ul>
    </li>
    <li><a href="#block-Diagram">Block Diagram</a></li>
    <li><a href="#user-Based-Collaborative-Filtering">User-Based Collaborative Filtering</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
    <li><a href="#contributing">Contributing</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<p align="left">
A recommendation system is a type of information filtering system which attempts to predict the 
preferences of a user, and make suggests based on these preferences. There are a wide variety of 
applications for recommendation systems. These have become increasingly popular over the last few 
years and are now utilized in most online platforms that we use. The content of such platforms varies 
from movies, music, books and videos, to friends and stories on social media platforms, to products on 
e-commerce websites, to people on professional and dating websites, to search results returned on 
Google. Often, these systems are able to collect information about a users choices, and can use this 
information to improve their suggestions in the future. In the browser, if we search movie name it will 
give similar movies related to that input movie. This is done by three recommendation engine such as 
popular based recommendation engine, content-based recommendation engine, collaborative filtering based recommendation engine.</p>
<p align="left">
The popular based recommendation engine is nothing but trending list on YouTube, Netflix, etc. They 
will keep on tracking the video views and update the on-trending list. The content-based 
recommendation engine is taking the input from the user and give a similar rank list based on the 
content related to the input movie. In this project, the content-based recommendation engine is used. 
The collaborative filtering-based recommendation engine is first search the similar user based on their 
activity and behavior and if the first user and second user have seen the same movie and if the first 
user has seen the new movie but if the second user not. It recommends new movies to a second user and 
vice-versa</p>

### Built Using

This section consist of list of major frameworks that were used in our project. Additionally add-ons/plugins are mentioned in the  acknowledgements section. Here are a few examples.
* [Javascript](https://www.javascript.com/)
* [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
* [MySql](https://www.mysql.com/)
* [Python](https://www.python.org/)
* [NodeJs](https://nodejs.org/en/)


<!-- Preview -->
## Website Preview

1. User Access Page
![Sign - up](https://user-images.githubusercontent.com/70905787/207915340-ced2aea5-007f-4f50-bffc-161591d164f5.jpg)

2. Home Page
![Home page](https://user-images.githubusercontent.com/70905787/207915396-1f4c583c-4c97-44ea-a9eb-335220b1275b.jpg)

3. Watchlist Section
![watchlist](https://user-images.githubusercontent.com/70905787/207915452-e3590d9a-685e-496d-ba5a-2bbea628fadb.jpg)

4. Tracker Section
![tracker](https://user-images.githubusercontent.com/70905787/207915517-e24e1c8a-7332-4035-819c-6d9ae01349bb.jpg)

5. Recommendation Section
![recommendations](https://user-images.githubusercontent.com/70905787/207915566-9b1940b4-c3dd-4a4e-b716-d376db74b3ab.jpg)

6. Explore Section
![explore](https://user-images.githubusercontent.com/70905787/207915613-8cc9dfa7-1245-4f15-99cd-7475f7716f0b.jpg)

7. Support Section
![support](https://user-images.githubusercontent.com/70905787/207915681-88efd676-076a-4009-85c4-2ccc4cf29b5c.jpg)

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/your_username_/Project-Name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```JS
   const API_KEY = 'ENTER YOUR API';
   ```



<!-- BLOCK DIAGRAM -->
## Block Diagram

![image](https://user-images.githubusercontent.com/70905787/207917110-0083d65c-b579-472f-a6f9-05d8365a6e14.png)



<!-- Algo -->
## User-Based Collaborative Filtering

Imagine that we want to recommend a movie to our friend Stanley. We could assume that similar people will have similar taste. Suppose that me and Stanley have seen the same movies, and we rated them all almost identically. But Stanley hasn’t seen ‘The Godfather: Part II’ and I did. If I love that movie, it sounds logical to think that he will too. With that, we have created an artificial rating based on our similarity.

Well, UB-CF uses that logic and recommends items by finding similar users to the active user (to whom we are trying to recommend a movie). A specific application of this is the user-based Nearest Neighbor algorithm. This algorithm needs two tasks:

1.Find the K-nearest neighbors (KNN) to the user a, using a similarity function w to measure the distance between each pair of users:

<img width="1005" alt="image" src="https://user-images.githubusercontent.com/70905787/207918176-e5a50f35-3a65-40d6-b732-130cc923a772.png">

2.Predict the rating that user a will give to all items the k neighbors have consumed but a has not. We Look for the item j with the best predicted rating.

In other words, we are creating a User-Item Matrix, predicting the ratings on items the active user has not see, based on the other similar users. This technique is memory-based.

![image](https://user-images.githubusercontent.com/70905787/207918226-179e0262-bd2d-4722-9cba-5b64c45827bb.png)


<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [User-Based Collaborative Filtering](https://medium.com/@cfpinela/recommender-systems-user-based-and-item-based-collaborative-filtering-5d5f375a127f)
* [IMDB API](https://imdb-api.com/)


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Team Members 🤝

- **[Nisarg Doshi](https://github.com/Nisarg20)**: Developer 1
- **[Suraj Mishra](https://github.com/sm5689)**: Developer 2

- Both of us have played a pivotal role in shaping the backend architecture and integrating machine learning models and we specializes in data analysis and algorithm optimization, ensuring top-notch recommendations.


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
