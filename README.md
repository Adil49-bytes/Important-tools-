# Important-tools-
Important tools
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AI Hub</title>

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:Arial,sans-serif;
    }

    body{
      min-height:100vh;
      display:flex;
      justify-content:center;
      align-items:center;
      background:linear-gradient(-45deg,#0f172a,#1e293b,#111827,#1d4ed8);
      background-size:400% 400%;
      animation:bgMove 12s ease infinite;
      overflow:hidden;
      color:white;
      padding:20px;
    }

    @keyframes bgMove{
      0%{background-position:0% 50%;}
      50%{background-position:100% 50%;}
      100%{background-position:0% 50%;}
    }

    .container{
      width:100%;
      max-width:1000px;
      animation:fadeIn 1.5s ease;
    }

    .title{
      text-align:center;
      margin-bottom:40px;
    }

    .title h1{
      font-size:52px;
      margin-bottom:10px;
      animation:float 3s ease-in-out infinite;
    }

    .title p{
      color:#d1d5db;
      font-size:18px;
    }

    @keyframes float{
      0%,100%{
        transform:translateY(0px);
      }
      50%{
        transform:translateY(-10px);
      }
    }

    .grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
      gap:25px;
    }

    .card{
      position:relative;
      padding:28px;
      border-radius:22px;
      background:rgba(255,255,255,0.08);
      backdrop-filter:blur(12px);
      border:1px solid rgba(255,255,255,0.1);
      overflow:hidden;
      transition:0.4s;
      animation:slideUp 1s ease;
    }

    .card::before{
      content:"";
      position:absolute;
      width:200%;
      height:200%;
      background:linear-gradient(
        45deg,
        transparent,
        rgba(255,255,255,0.15),
        transparent
      );
      top:-50%;
      left:-50%;
      transform:rotate(25deg);
      animation:shine 5s linear infinite;
    }

    @keyframes shine{
      0%{
        transform:translateX(-100%) rotate(25deg);
      }
      100%{
        transform:translateX(100%) rotate(25deg);
      }
    }

    .card:hover{
      transform:translateY(-12px) scale(1.03);
      box-shadow:0 15px 35px rgba(0,0,0,0.4);
    }

    .card h2{
      font-size:28px;
      margin-bottom:12px;
      position:relative;
      z-index:2;
    }

    .card p{
      color:#dbe4ee;
      margin-bottom:22px;
      line-height:1.5;
      position:relative;
      z-index:2;
    }

    .btn{
      display:inline-block;
      text-decoration:none;
      background:#2563eb;
      color:white;
      padding:12px 20px;
      border-radius:12px;
      font-weight:bold;
      transition:0.3s;
      position:relative;
      z-index:2;
    }

    .btn:hover{
      background:#1d4ed8;
      transform:scale(1.05);
    }

    @keyframes slideUp{
      from{
        opacity:0;
        transform:translateY(40px);
      }
      to{
        opacity:1;
        transform:translateY(0);
      }
    }

    @keyframes fadeIn{
      from{
        opacity:0;
      }
      to{
        opacity:1;
      }
    }

    .circle{
      position:absolute;
      border-radius:50%;
      background:rgba(255,255,255,0.08);
      animation:move 12s linear infinite;
    }

    .circle:nth-child(1){
      width:120px;
      height:120px;
      left:5%;
      top:10%;
    }

    .circle:nth-child(2){
      width:180px;
      height:180px;
      right:10%;
      bottom:10%;
      animation-duration:18s;
    }

    @keyframes move{
      0%{
        transform:translateY(0px) rotate(0deg);
      }
      50%{
        transform:translateY(-30px) rotate(180deg);
      }
      100%{
        transform:translateY(0px) rotate(360deg);
      }
    }

    footer{
      text-align:center;
      margin-top:35px;
      color:#cbd5e1;
    }
  </style>
</head>

<body>

  <div class="circle"></div>
  <div class="circle"></div>

  <div class="container">

    <div class="title">
      <h1>AI & Search Hub</h1>
      <p>Animated website for your favorite AI tools</p>
    </div>

    <div class="grid">

      <div class="card">
        <h2>ChatGPT</h2>
        <p>AI assistant by OpenAI for coding, chatting and learning.</p>

        <a class="btn" href="https://chat.openai.com" target="_blank">
          Open
        </a>
      </div>

      <div class="card">
        <h2>Grok</h2>
        <p>xAI chatbot with modern AI capabilities and live knowledge.</p>

        <a class="btn" href="https://grok.com" target="_blank">
          Open
        </a>
      </div>

      <div class="card">
        <h2>Gemini</h2>
        <p>Google AI assistant for research and productivity tasks.</p>

        <a class="btn" href="https://gemini.google.com" target="_blank">
          Open
        </a>
      </div>

      <div class="card">
        <h2>Nano Banana</h2>
        <p>Creative AI platform with experimental AI features.</p>

        <a class="btn" href="https://nanobanana.ai" target="_blank">
          Open
        </a>
      </div>

      <div class="card">
        <h2>Google</h2>
        <p>The world's largest and most popular search engine.</p>

        <a class="btn" href="https://google.com" target="_blank">
          Open
        </a>
      </div>

      <div class="card">
        <h2>Wikipedia</h2>
        <p>Massive free encyclopedia with knowledge on everything.</p>

        <a class="btn" href="https://wikipedia.org" target="_blank">
          Open
        </a>
      </div>

    </div>

    <footer>
      Made with HTML & CSS Animations
    </footer>

  </div>

</body>
</html>
