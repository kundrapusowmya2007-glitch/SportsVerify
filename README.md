# SportsVerify
AI-Powered Sports
<!DOCTYPE html>
<html>
<head>
  <title>AI Sports Content Protection</title>
</head>
<body style="text-align:center; font-family:Arial; margin-top:50px;">

  <h1>AI Sports Content Protection</h1>
  <p>Upload an image to check for copyright violation</p>

  <input type="file">
  <br><br>
  <button onclick="check()">Analyze</button>

  <h3 id="result"></h3>

  <script>
    function check() {
      document.getElementById("result").innerText = "Analyzing...";

      setTimeout(() => {
        let r = Math.random();
        if (r > 0.5) {
          document.getElementById("result").innerText =
            "⚠️ Copyright Violation Detected";
        } else {
          document.getElementById("result").innerText =
            "✅ Content is Original";
        }
      }, 1500);
    }
  </script>

</body>
</html>