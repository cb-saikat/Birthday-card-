<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy Birthday Swopna!</title>
  <style>
    body, html {
      margin: 0;
      padding: 0;
      height: 100%;
      overflow: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(to top right, #ffecd2, #fcb69f);
      font-family: 'Arial', sans-serif;
    }
    .card {
      text-align: center;
      padding: 20px;
      border-radius: 20px;
      background: white;
      box-shadow: 0 4px 20px rgba(0,0,0,0.2);
      transition: all 1s ease;
    }
    .hidden-content {
      display: none;
      margin-top: 20px;
    }
    .photo {
      width: 200px;
      height: 200px;
      object-fit: cover;
      border-radius: 50%;
      margin-top: 20px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
    }
    .balloons {
      position: absolute;
      width: 100%;
      height: 100%;
      top: 0;
      left: 0;
      pointer-events: none;
      background: url('https://i.postimg.cc/TPvFtxHQ/balloons.gif') center/cover no-repeat;
      opacity: 0;
      transition: opacity 1s ease;
    }
    audio {
      display: none;
    }
  </style>
</head>
<body>

<div class="balloons" id="balloons"></div>

<div class="card" id="card" onclick="revealMessage()">
  <h1 id="main-text">Happy Birthday Swopna</h1>
  <div class="hidden-content" id="hidden-content">
    <p><b>প্রিয় স্বপ্না আপু,</b><br>Wishing you a life full of happiness, love, and endless success!<br>
    আপনি আমাদের জন্য সবসময় অনুপ্রেরণা। Keep shining!<br><b>Happy Birthday once again!</b></p>
    <img src="/mnt/data/file-JEGsKV2TD2pgV3eCxrBA2F" alt="Swopna's Photo" class="photo">
  </div>
</div>

<audio id="music" src="https://www.bensound.com/bensound-music/bensound-sunny.mp3" loop></audio>

<script>
function revealMessage() {
  document.getElementById('hidden-content').style.display = 'block';
  document.getElementById('card').style.background = '#fff0f5';
  document.getElementById('balloons').style.opacity = '0.7';
  document.getElementById('music').play();
  document.getElementById('main-text').innerText = "Lots of Love, Saikat";
  document.getElementById('card').onclick = null;
}
</script>

</body>
</html>
