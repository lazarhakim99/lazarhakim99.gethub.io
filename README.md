<!DOCTYPE html>
<html>
<head>
  <title>Wi-Fi Access</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      padding: 50px;
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <h1>Welcome!</h1>
  <p>To access our Wi-Fi, please follow our Instagram page and submit your Instagram username below:</p>
  <p><a href="https://www.instagram.com/amar.aymane" target="_blank">@yourpage</a></p>
  <form id="instagramForm" onsubmit="submitForm(event)">
    <label for="username">Instagram Username:</label><br>
    <input type="text" id="username" name="username" required><br><br>
    <input type="submit" value="Submit">
  </form>
  <div id="passwordDiv" class="hidden">
    <h2>Thank you for following us!</h2>
    <p>Here is your Wi-Fi password:</p>
    <p><strong>Password: YourPassword</strong></p>
  </div>
  <script>
    function submitForm(event) {
      event.preventDefault();
      var username = document.getElementById('username').value;
      // Here you would typically verify if the user follows the page.
      // For now, we'll just assume they did.
      document.getElementById('instagramForm').classList.add('hidden');
      document.getElementById('passwordDiv').classList.remove('hidden');
      // Optionally, send the username to your server for verification
      // and/or record keeping.
    }
  </script>
</body>
</html>
