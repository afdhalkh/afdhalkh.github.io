
<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        .button2 {
  display: inline-block;
  padding: 15px 25px;
  font-size: 24px;
  cursor: pointer;
  text-align: center;
  text-decoration: none;
  outline: none;
  color: #fff;
  background-color: #4CAF50;
  border: none;
  border-radius: 15px;
  box-shadow: 0 9px #999;
}    
    
        .button2:hover {background-color: #3e8e41}
        
        .button2:active {
  background-color: #3e8e41;
  box-shadow: 0 5px #666;
  transform: translateY(4px);
}
    </style>
    <link rel="shortcut icon" type="image/png" href="Favicon.png"/>
      <style>img[alt="www.000webhost.com"]{display:none;}</style>
  <base href="https://downthumbnail.000webhostapp.com/">      
  <meta charset="UTF-8">
  <meta name="description" content="This is where you download youtube Thumbnails.">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Download YouTube Video Thumbnail</title>
  <link rel="stylesheet" href="style.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"/>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body>
  <form action="/index.php" method="POST">
      
    <header>Download Thumbnail</header>
    <div class="url-input">
      <span class="title">Paste video url:</span>
      <div class="field">
        <input type="text" placeholder="https://www.youtube.com/watch?v=Tcn8vrsjpDE" required>
        <input class="hidden-input" type="hidden" name="imgurl">
        <span class="bottom-line"></span>
      </div>
    </div>
    <div class="preview-area">
      <img class="thumbnail" src="" alt="">
      <i class="icon fas fa-cloud-download-alt"></i>
      <span>Paste video url to see preview</span>
    </div>
    <button class="download-btn" type="submit" name="button">Download Thumbnail</button>
    <!-- AddToAny BEGIN -->
<a class="a2a_dd" href="https://www.addtoany.com/share">Share</a>
<script async src="https://static.addtoany.com/menu/page.js"></script>
<!-- AddToAny END -->
  </form>

  <script>
    const urlField = document.querySelector(".field input"),
    previewArea = document.querySelector(".preview-area"),
    imgTag = previewArea.querySelector(".thumbnail"),
    hiddenInput = document.querySelector(".hidden-input"),
    button = document.querySelector(".download-btn");

    urlField.onkeyup = ()=>{
      let imgUrl = urlField.value;
      previewArea.classList.add("active");
      button.style.pointerEvents = "auto";
      if(imgUrl.indexOf("https://www.youtube.com/watch?v=") != -1){
        let vidId = imgUrl.split('v=')[1].substring(0, 11);
        let ytImgUrl = `https://img.youtube.com/vi/${vidId}/maxresdefault.jpg`;
        imgTag.src = ytImgUrl;
      }else if(imgUrl.indexOf("https://youtu.be/") != -1){
        let vidId = imgUrl.split('be/')[1].substring(0, 11);
        let ytImgUrl = `https://img.youtube.com/vi/${vidId}/maxresdefault.jpg`;
        imgTag.src = ytImgUrl;
      }else if(imgUrl.match(/\.(jpe?g|png|gif|bmp|webp)$/i)){
        imgTag.src = imgUrl;
      }else{
        imgTag.src = "";
        button.style.pointerEvents = "none";
        previewArea.classList.remove("active");
      }
      hiddenInput.value = imgTag.src;
    }
  </script>
<script>
    
    // Import the functions you need from the SDKs you need
import { initializeApp } from "firebase/app";
import { getAnalytics } from "firebase/analytics";
// TODO: Add SDKs for Firebase products that you want to use
// https://firebase.google.com/docs/web/setup#available-libraries

// Your web app's Firebase configuration
// For Firebase JS SDK v7.20.0 and later, measurementId is optional
const firebaseConfig = {
  apiKey: "AIzaSyCWsr_AVHXAojve72g0HnousXdRCYw1vvI",
  authDomain: "fir-da2fe.firebaseapp.com",
  projectId: "fir-da2fe",
  storageBucket: "fir-da2fe.appspot.com",
  messagingSenderId: "51090686597",
  appId: "1:51090686597:web:eb6670c2277b3cd09e5fec",
  measurementId: "G-MS1V38KM5Y"
};

// Initialize Firebase
const app = initializeApp(firebaseConfig);
const analytics = getAnalytics(app);

</script>
<style>
    .disclaimer {
        display: none;
    }
</style>
</html>
<style>
    .a2a_dd {
        top: 16px !important;
        display: inline-block !important;
        position: relative !important;
        
        left: 166px;
    }
    
    body {
        background-color: #39afcc;
    }
</style>
<style>.footer,.generic-footer{margin-bottom:98px}@media (min-width:374px){.footer,.generic-footer{margin-bottom:78px}}@media (min-width:546px){.footer,.generic-footer{margin-bottom:56px}}@media (min-width:1055px){.footer,.generic-footer{margin-bottom:0}}.disclaimer{position:fixed;z-index:9999999;bottom:0;right:0;border-top:2px solid #ff5c62;text-align:center;font-size:14px;font-weight:400;background-color:#fff;padding:5px 10px 5px 10px}.disclaimer a:hover{text-decoration:underline}@media (min-width:1052px){.disclaimer{text-align:right;border-left:2px solid red;border-top-left-radius:10px}}@media (min-width:1920px){.disclaimer{width:60%}}</style><div class="disclaimer">We support Ukraine and condemn war. Push Russian government to act against war. Be brave, vocal and show your support to Ukraine. Follow the latest news <a title="https://www.bbc.com/news/live/world-europe-60517447" target="_blank" href="https://www.bbc.com/news/live/world-europe-60517447" style="color: black;"><b>HERE</b></a></div></body>
</html>
