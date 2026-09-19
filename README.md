# <!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>JARVIS AI</title>
</head>

<body>
  <h1>🤖 JARVIS AI</h1>

  <input id="message" placeholder="Ask JARVIS anything...">
  <button onclick="askJarvis()">Ask</button>

  <p id="answer">Hello! I am JARVIS.</p>

  <script>
    function askJarvis() {
      const message = document.getElementById("message").value;

      if (!message) {
        document.getElementById("answer").innerText =
          "Please type something.";
        return;
      }

      document.getElementById("answer").innerText =
        "You said: " + message;
    }
  </script>
</body>
</html>