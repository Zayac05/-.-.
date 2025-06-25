<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>My Portfolio</title>
  <style>
    :root {
      --main-bg: #181818;
      --accent: #e0e0e0;
      --text: #e0e0e0;
      --footer-bg: #222;
      --footer-text: #bbb;
      --header-bg: #222;
    }
    body {
      margin: 0;
      font-family: 'Segoe UI', Arial, sans-serif;
      background: var(--main-bg);
      color: var(--text);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      /* Траурный черный фон с легким паттерном */
      background-image:
        repeating-linear-gradient(
          135deg,
          rgba(255,255,255,0.03) 0px,
          rgba(255,255,255,0.03) 2px,
          transparent 2px,
          transparent 8px
        );
      background-size: 24px 24px;
    }
    header {
      background: var(--header-bg);
      padding: 2rem 1rem 1rem 1rem;
      text-align: center;
      box-shadow: 0 2px 8px rgba(0,0,0,0.13);
    }
    header h1 {
      margin: 0;
      font-size: 2.2rem;
      color: var(--accent);
      letter-spacing: 0.04em;
    }
    main {
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 2rem 1rem 2rem 1rem;
      box-sizing: border-box;
      width: 100%;
      max-width: 800px;
      margin: 0 auto;
      background: rgba(34,34,34,0.92);
      border-radius: 18px;
      box-shadow: 0 2px 16px rgba(0,0,0,0.13);
    }
    .images-section {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 1.5rem;
      flex-wrap: wrap;
      margin-bottom: 2rem;
      width: 100%;
    }
    .images-section img {
      max-width: 320px;
      width: 90vw;
      height: auto;
      border-radius: 12px;
      box-shadow: 0 2px 12px rgba(0,0,0,0.18);
      object-fit: cover;
      background: #333;
      margin-bottom: 0.5rem;
      filter: grayscale(80%);
    }
    .text-section {
      text-align: center;
      margin-bottom: 2rem;
      font-size: 1.15rem;
      line-height: 1.7;
      color: var(--text);
    }
    .audio-section {
      display: flex;
      justify-content: center;
      width: 100%;
      margin-bottom: 2rem;
    }
    audio {
      width: 100%;
      max-width: 400px;
      outline: none;
      border-radius: 6px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.18);
      background: #222;
    }
    footer {
      text-align: center;
      background: var(--footer-bg);
      color: var(--footer-text);
      padding: 1rem 0;
      font-size: 1rem;
      letter-spacing: 0.01em;
      margin-top: auto;
    }
    @media (max-width: 600px) {
      .images-section {
        flex-direction: column;
        gap: 1rem;
      }
      header h1 {
        font-size: 1.4rem;
      }
      main {
        padding: 1rem 0.5rem;
      }
      .text-section {
        font-size: 1rem;
      }
      audio {
        max-width: 100%;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Ианов Иван Иванович</h1>
  </header>
  <main>
    <section class="images-section">
      <!-- Фото пожилого человека. Можно заменить на своё, если требуется -->
      <img src="https://images.unsplash.com/photo-1464983953574-0892a716854b?auto=format&fit=facearea&w=400&h=400&facepad=2&q=80" alt="Пожилой человек" />
    </section>
    <section class="text-section">
      <p>
        Память о тебе навсегда останется в наших сердцах.<br>
        Светлая память.<br>
        Пусть земля будет пухом.<br>
        Скорбим и помним...
      </p>
    </section>
    <section class="audio-section">
      <!-- Replace 'audio.mp3' with your own audio file -->
      <audio controls>
        <source src="audio.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
      </audio>
    </section>
  </main>
  <footer>
     <!-- You can update this year --> 06.06.1945 - 06.06.2025 
  </footer>
  <!--
    To customize:
    - Replace the image link in <img src="..."> with your own photo if needed.
    - Replace 'audio.mp3' with your audio file.
    - Edit the paragraph in the text-section.
    - Edit copyright in the footer.
  -->
</body>
</html>
