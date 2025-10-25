<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>404 - Smooth Animation</title>
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body {
    background: radial-gradient(circle at center, #0a0a0a, #000);
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    color: white;
    font-family: "Poppins", sans-serif;
    overflow: hidden;
  }
  h1 {
    font-size: 15vw;
    font-weight: 700;
    letter-spacing: 10px;
    animation: float 3s ease-in-out infinite;
  }
  p {
    font-size: 1.2rem;
    opacity: 0.7;
    animation: fade 4s ease-in-out infinite alternate;
  }

  @keyframes float {
    0%, 100% {
      transform: translateY(0) scale(1);
      filter: blur(0);
    }
    50% {
      transform: translateY(-15px) scale(1.05);
      filter: blur(0.5px);
    }
  }

  @keyframes fade {
    from { opacity: 0.4; }
    to { opacity: 1; }
  }
</style>
</head>
<body>
  <h1>404</h1>
  <p>Oops... halaman tidak ditemukan</p>
</body>
</html>
