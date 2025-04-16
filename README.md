<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="description" content="AI & Content Tools and Website & Performance Tools and SEO & Digital Marketing Tools helps you analyze and generate optimized titles, thumbnails, descriptions, and tags for your videos using data from platforms like Google, YouTube, Facebook, Instagram, Deep Seek, and ChatGPT." />
  <title>AI & Content Tools</title>
  <style>
    body {
      background-color: #0d1117;
      color: #e6edf3;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
    }
    header, footer {
      text-align: center;
      padding: 20px;
      background-color: #161b22;
    }
    h1 {
      color: #ff4c4c;
    }
    .container {
      padding: 30px;
      max-width: 800px;
      margin: auto;
    }
    .form-section {
      background-color: #21262d;
      padding: 20px;
      border-radius: 10px;
    }
    input[type="file"], select, button {
      display: block;
      margin: 15px 0;
      padding: 10px;
      width: 100%;
      border: none;
      border-radius: 5px;
      background-color: #30363d;
      color: #e6edf3;
    }
    button {
      background-color: #ff4c4c;
      cursor: pointer;
    }
    .result {
      margin-top: 20px;
      background-color: #1c1f26;
      padding: 20px;
      border-radius: 10px;
    }
    .copy-btn {
      margin-top: 10px;
      background-color: #238636;
    }
    .footer-links a {
      color: #58a6ff;
      margin: 0 10px;
      text-decoration: none;
    }
  </style>
</head>
<body>
  <header>
    <h1>AI & Content Tools and Digital Marketing Suite</h1>
  </header>
  <div class="container">
    <div class="form-section">
      <label for="videoUpload">Upload Your Video:</label>
      <input type="file" id="videoUpload" accept="video/*" /><label for="categorySelect">Select Category:</label>
  <select id="categorySelect">
    <option value="education">Education</option>
    <option value="entertainment">Entertainment</option>
    <option value="technology">Technology</option>
    <option value="health">Health</option>
    <option value="lifestyle">Lifestyle</option>
  </select>

  <button onclick="generateContent()">Get AI-Powered Insights</button>

  <div id="result" class="result" style="display: none;">
    <h3>Generated Data:</h3>
    <p><strong>Title:</strong> <span id="title"></span></p>
    <p><strong>Thumbnail:</strong> <span id="thumbnail"></span></p>
    <p><strong>Description:</strong> <span id="description"></span></p>
    <p><strong>Tags:</strong> <span id="tags"></span></p>
    <button class="copy-btn" onclick="copyResults()">Copy All</button>
  </div>
</div>

  </div>  <footer>
    <div class="footer-links">
      <a href="#">Privacy Policy</a>
      <a href="#">Contact Us</a>
    </div>
    <p>&copy; 2025 AI & Content Tools</p>
  </footer>  <script>
    function generateContent() {
      const category = document.getElementById("categorySelect").value;

      // Simulate content generation
      document.getElementById("title").textContent = `Amazing ${category} Video You Can't Miss!`;
      document.getElementById("thumbnail").textContent = `Generated thumbnail for ${category}`;
      document.getElementById("description").textContent = `This ${category} video is optimized with AI insights from Google, YouTube, Facebook, Instagram, Deep Seek, and ChatGPT.`;
      document.getElementById("tags").textContent = `#${category} #AItools #ContentCreation #Marketing`;

      document.getElementById("result").style.display = "block";
    }

    function copyResults() {
      const title = document.getElementById("title").textContent;
      const thumbnail = document.getElementById("thumbnail").textContent;
      const description = document.getElementById("description").textContent;
      const tags = document.getElementById("tags").textContent;
      const textToCopy = `Title: ${title}\nThumbnail: ${thumbnail}\nDescription: ${description}\nTags: ${tags}`;
      navigator.clipboard.writeText(textToCopy).then(() => alert("Copied to clipboard!"));
    }
  </script></body>
</html>
Title: Amazing education Video You Can't Miss!
Thumbnail: Generated thumbnail for education
Description: This education video is optimized with AI insights from Google, YouTube, Facebook, Instagram, Deep Seek, and ChatGPT.
Tags: #education #AItools #ContentCreation #Marketing
