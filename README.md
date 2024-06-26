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
  <p>To access our Wi-Fi, please complete the task below:</p>
  <form id="taskForm">
    <label for="task">Enter the answer to 2 + 2:</label><br>
    <input type="text" id="task" name="task"><br><br>
    <input type="button" value="Submit" onclick="checkAnswer()">
  </form>
  <div id="passwordDiv" class="hidden">
    <h2>Congratulations!</h2>
    <p>Here is your Wi-Fi password:</p>
    <p><strong>Password: YourPassword</strong></p>
  </div>
  <script>
    function checkAnswer() {
      var answer = document.getElementById('task').value;
      if (answer == '4') {
        document.getElementById('taskForm').classList.add('hidden');
        document.getElementById('passwordDiv').classList.remove('hidden');
      } else {
        alert('Incorrect answer. Please try again.');
      }
    }
  </script>
</body>
</html>
