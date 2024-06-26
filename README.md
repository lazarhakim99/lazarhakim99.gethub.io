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
  </style>
  <script>
    function redirectToInstagram() {
      window.location.href = "https://www.instagram.com/yourpage";
      setTimeout(() => {
        window.location.href = "https://www.yourwebsite.com/thankyou.html"; // This is the URL of the page with the password
      }, 5000); // Adjust the delay as needed (e.g., 5000 milliseconds = 5 seconds)
    }
  </script>
</head>
<body onload="redirectToInstagram()">
  <h1>Welcome!</h1>
  <p>To access our Wi-Fi, please follow our Instagram page. You will be redirected shortly...</p>
</body>
</html>
