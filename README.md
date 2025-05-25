<html>
<head>
  <title>Pet Shop Home</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      background-color: #ffffff;
      color: #333333;
    }
    .header-top {
      background-color: #f5f5f5;
      padding: 5px 20px;
      text-align: right;
    }
    .header-top a {
      color: #27ae60;
      margin: 0 10px;
      text-decoration: none;
    }
    .header-top a:hover {
      text-decoration: underline;
    }
    .header-main {
      background-color: #ffffff;
      padding: 10px 20px;
      box-shadow: 0 2px 5px #0000001a;
      text-align: center;
    }
    .header-main .logo {
      font-size: 1.5em;
      font-weight: bold;
      color: #27ae60;
      margin-bottom: 10px;
    }
    .header-main .nav {
      margin-bottom: 10px;
    }
    .header-main .nav a {
      color: #333333;
      margin: 0 10px;
      text-decoration: none;
      font-size: 0.9em;
    }
    .header-main .nav a:hover {
      color: #27ae60;
    }
    .header-main .search-bar {
      margin: 0 auto;
      width: 200px;
      position: relative;
    }
    .header-main .search-bar input {
      padding: 5px 10px;
      border: 1px solid #dddddd;
      border-radius: 5px;
      width: 100%;
      font-size: 0.9em;
    }
    .header-main .search-bar button {
      position: absolute;
      right: 5px;
      top: 50%;
      transform: translateY(-50%);
      background: none;
      border: none;
      cursor: pointer;
    }
    .header-main .search-bar button svg {
      width: 16px;
      height: 16px;
      stroke: #666666;
    }
    .main-content {
      position: relative;
      min-height: 500px;
      background-image: url('placeholder-top-image.jpg');
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      text-align: center;
    }
    .main-content .overlay-text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 3em;
      font-weight: bold;
      color: #ffffff;
      text-shadow: 2px 2px 4px #00000080;
      line-height: 1.2;
    }
    .main-content .overlay-text span {
      display: block;
      font-size: 0.6em;
      font-weight: normal;
    }
    .footer {
      padding: 20px;
      background-color: #f1f1f1;
      text-align: center;
      color: #666666;
    }
    .footer p {
      margin: 0;
      font-size: 0.9em;
    }
    @media (max-width: 768px) {
      .header-main .nav a {
        display: block;
        margin: 5px 0;
      }
      .header-main .search-bar {
        width: 100%;
      }
      .main-content {
        min-height: 300px;
      }
      .main-content .overlay-text {
        font-size: 2em;
      }
      .main-content .overlay-text span {
        font-size: 0.7em;
      }
    }
  </style>
</head>
<body>
  <div class="header-top">
    <a href="#">Donate</a>
  </div>

  <div class="header-main">
    <div class="logo">Pet Shop</div>
    <div class="nav">
      <a href="#">Pets & People</a>
      <a href="#">Pets for Adoption</a>
      <a href="#">Rescue Groups & Shelters</a>
      <a href="#">PetRescue Partners</a>
      <a href="#">Good Reads</a>
      <a href="#">About PetRescue</a>
    </div>
    <div class="search-bar">
      <input type="text" placeholder="Search PetRescue">
      <button>
        <svg viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/>
        </svg>
      </button>
    </div>
  </div>

  <div class="main-content">
    <div class="overlay-text">
      Create Happiness <span>Save Lives</span>
    </div>
  </div>

  <div class="footer">
    <p>© 2025 Pet Shop. All rights reserved.</p>
  </div>

  <script>
    // Search bar functionality
    var searchInput = document.querySelector('.search-bar input');
    var searchButton = document.querySelector('.search-bar button');
    searchButton.onclick = function() {
      var query = searchInput.value.trim();
      if (query) {
        alert('Searching for: ' + query);
        // Add your search logic here
      }
    };
    searchInput.onkeypress = function(e) {
      if (e.key === 'Enter') {
        var query = searchInput.value.trim();
        if (query) {
          alert('Searching for: ' + query);
          // Add your search logic here
        }
      }
    };
  </script>
</body>
</html>
