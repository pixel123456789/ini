<?php
$code = isset($_GET['code']) ? htmlspecialchars($_GET['code']) : 'No code found';
?>
<!DOCTYPE html>
<html>
<head>
    <title>OAuth Callback</title>
</head>
<body>
    <h1>Authorization Code</h1>
    <p>Please copy the following code and paste it back into the application:</p>
    <pre id="code"><?php echo $code; ?></pre>
    <button onclick="copyCode()">Copy Code</button>

    <script>
    function copyCode() {
        const codeElement = document.getElementById('code');
        const textArea = document.createElement('textarea');
        textArea.value = codeElement.textContent;
        document.body.appendChild(textArea);
        textArea.select();
        document.execCommand('copy');
        document.body.removeChild(textArea);
        alert('Code copied to clipboard!');
    }
    </script>
</body>
</html>
