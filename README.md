<!DOCTYPE html>
<html>
  <head>
    <title>YouTube Clone</title>
    <style>
      /* Add some basic styles to improve the look of the site */
      header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 10px;
        background-color: #333;
        color: #fff;
      }
      header h1 {
        margin: 0;
      }
      header nav ul {
        display: flex;
        list-style: none;
        margin: 0;
        padding: 0;
      }
      header nav a {
        display: block;
        padding: 10px;
        color: #fff;
        text-decoration: none;
      }
      header form {
        display: flex;
      }
      header input[type="text"] {
        padding: 10px;
        flex-grow: 1;
        margin-right: 10px;
      }
      main {
        padding: 10px;
      }
      main h2 {
        margin-top: 0;
      }
      footer {
        padding: 10px;
        background-color: #333;
        color: #fff;
        text-align: center;
      }
    </style>
  </head>
  <body>
    <header>
      <h1>YouTube Clone</h1>
      <nav>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Trending</a></li>
          <li><a href="#">Subscriptions</a></li>
        </ul>
      </nav>
      <form>
        <input type="text" placeholder="Search">
        <button type="submit">Go</button>
      </form>
    </header>
    <main>
      <h2>Suggested Videos</h2>
      <ul id="video-list">
        <!-- The video list will be populated with JavaScript -->
      </ul>
    </main>
    <footer>
      <p>&copy; YouTube Clone 2023</p>
    </footer>
    <script>
      // Use JavaScript to dynamically populate the video list
      const videoList = document.getElementById("video-list");
      const videos = [
        { title: "Video 1", description: "Description for Video 1
