# BookBot
A book recommendation chatbot powered by IBM Watson Assistant
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>BookBot - Watson Assistant Chatbot</title>
  <style>
    /* Updated background and clean UI */
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #e0f7fa; /* Soft cyan background */
      color: #333;
      text-align: center;
      margin: 0;
      padding: 0;
    }

    h1 {
      background-color: #37474f; /* dark bluish-grey */
      color: white;
      padding: 20px;
      margin: 0;
    }

    p {
      font-size: 18px;
      padding: 20px;
      max-width: 600px;
      margin: auto;
    }

    .container {
      margin-top: 100px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>📚 Welcome to BookBot!</h1>
    <p>This is your personal book recommendation assistant powered by IBM Watson.</p>
  </div>

  <!-- Watson Assistant Chat Embed Script with lion icon -->
  <script>
    window.watsonAssistantChatOptions = {
      integrationID: "a0ffb805-9447-4d5d-8d84-d0914b88f168", // Replace with your integration ID
      region: "au-syd",
      serviceInstanceID: "372c0932-467c-48ca-9e2c-c9333915fbc0",
      showLauncher: true,
      launcherImage: "https://emojicdn.elk.sh/🦁", // 🦁 Lion emoji as launcher icon
      onLoad: function(instance) { instance.render(); }
    };
    setTimeout(function(){
      const t = document.createElement('script');
      t.src = "https://web-chat.global.assistant.watson.appdomain.cloud/loadWatsonAssistantChat.js";
      document.head.appendChild(t);
    });
  </script>
</body>
</html>
