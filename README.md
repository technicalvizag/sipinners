# sipinners
this is a html spinner
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Spinner</title>
<style>
  .spinner {
    margin: 100px auto;
    width: 50px;
    height: 50px;
    position: relative;
    text-align: center;
    -webkit-animation: rotate 2s linear infinite;
    animation: rotate 2s linear infinite;
  }

  .spinner .dot {
    width: 10px;
    height: 10px;
    background-color: #333;
    border-radius: 50%;
    position: absolute;
    top: 0;
    bottom: 0;
    margin: auto;
  }

  .spinner .dot:nth-child(1) {
    left: 0;
    -webkit-animation: bounce 2s infinite;
    animation: bounce 2s infinite;
  }

  .spinner .dot:nth-child(2) {
    right: 0;
    -webkit-animation: bounce 2s infinite;
    animation: bounce 2s infinite;
    -webkit-animation-delay: 0.5s;
    animation-delay: 0.5s;
  }

  @-webkit-keyframes rotate {
    100% {
      -webkit-transform: rotate(360deg);
    }
  }

  @keyframes rotate {
    100% {
      transform: rotate(360deg);
    }
  }

  @-webkit-keyframes bounce {
    0%, 100% {
      -webkit-transform: translateY(0);
    }
    50% {
      -webkit-transform: translateY(-15px);
    }
  }

  @keyframes bounce {
    0%, 100% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-15px);
    }
  }
</style>
</head>
<body>
  <div class="spinner">
    <div class="dot"></div>
    <div class="dot"></div>
  </div>
</body>
</html>



