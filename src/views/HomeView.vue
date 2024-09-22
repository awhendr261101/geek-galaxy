<template>
  <div class="home">
        <header>
        <div class="container">
            <h1>MovieTrailers Hub</h1>
            <nav>
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Genres</a></li>
                    <li><a href="#">Top Rated</a></li>
                    <li><a href="#">Coming Soon</a></li>
                </ul>
            </nav>
            <div class="search-bar">
                <input type="text" placeholder="Search for a movie...">
                <button>Search</button>
            </div>
        </div>
    </header>

        <section class="featured-trailer">
        <div class="container">
            <h2>Featured Trailer</h2>
            <div class="trailer-video">
                <iframe width="560" height="315" src="https://www.youtube.com/embed/sample" 
                        frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
            </div>
            <button class="watch-now">Watch Now</button>
        </div>
    </section>

    <!-- Trailer Grid Section -->
    <section class="trailer-grid">
        <div class="container">
            <h2>Popular Trailers</h2>
            <div class="grid">
                <!-- Sample Movie Item -->
                <div class="movie-item">
                    <img src="https://via.placeholder.com/200x300" alt="Movie Poster">
                    <h3>Movie Title 1</h3>
                    <button>Watch Trailer</button>
                </div>
                <div class="movie-item">
                    <img src="https://via.placeholder.com/200x300" alt="Movie Poster">
                    <h3>Movie Title 2</h3>
                    <button>Watch Trailer</button>
                </div>
                <div class="movie-item">
                    <img src="https://via.placeholder.com/200x300" alt="Movie Poster">
                    <h3>Movie Title 3</h3>
                    <button>Watch Trailer</button>
                </div>
                <!-- Add more movie items as needed -->
            </div>
        </div>
    </section>

    <!-- Footer Section -->
    <footer>
        <div class="container">
            <p>&copy; 2024 MovieTrailers Hub | All Rights Reserved</p>
        </div>
    </footer>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'HomeView',
  components: {
    
  }
}
</script>

<style>

/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

/* Container */
.container {
    width: 80%;
    margin: 0 auto;
}

/* Header */
header {
    background-color: #333;
    color: white;
    padding: 15px 0;
}

header h1 {
    display: inline-block;
    margin-left: 20px;
    font-size: 24px;
}

nav {
    display: inline-block;
    float: right;
    margin-right: 20px;
}

nav ul {
    list-style-type: none;
}

nav ul li {
    display: inline-block;
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 16px;
}

.search-bar {
    display: inline-block;
    float: right;
}

.search-bar input[type="text"] {
    padding: 5px;
    border: none;
    border-radius: 3px;
}

.search-bar button {
    padding: 5px 10px;
    background-color: #ff3333;
    color: white;
    border: none;
    border-radius: 3px;
}

/* Featured Trailer Section */
.featured-trailer {
    background-color: #222;
    color: white;
    text-align: center;
    padding: 40px 0;
}

.featured-trailer h2 {
    font-size: 28px;
    margin-bottom: 20px;
}

.trailer-video {
    margin-bottom: 20px;
}

.watch-now {
    padding: 10px 20px;
    background-color: #ff3333;
    color: white;
    border: none;
    border-radius: 5px;
    font-size: 18px;
}

.watch-now:hover {
    background-color: #ff6666;
}

/* Trailer Grid Section */
.trailer-grid {
    padding: 40px 0;
}

.trailer-grid h2 {
    text-align: center;
    font-size: 24px;
    margin-bottom: 30px;
}

.grid {
    display: flex;
    gap: 20px;
    justify-content: center;
    flex-wrap: wrap;
}

.movie-item {
    background-color: white;
    padding: 15px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    width: 200px;
    text-align: center;
}

.movie-item img {
    width: 100%;
    height: auto;
    border-radius: 5px;
}

.movie-item h3 {
    font-size: 18px;
    margin: 10px 0;
}

.movie-item button {
    padding: 8px 12px;
    background-color: #ff3333;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

.movie-item button:hover {
    background-color: #ff6666;
}

/* Footer */
footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 20px 0;
}

footer p {
    font-size: 14px;
}


</style>
