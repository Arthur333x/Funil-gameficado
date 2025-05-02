# Funil-gameficado

<!DOCTYPE html><html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Funil Gamificado Ultra</title>
  <style>
    * {
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }
    body {
      margin: 0;
      background: #f9f9f9;
      color: #333;
    }
    header {
      background: linear-gradient(90deg, #ff5722, #e91e63);
      color: white;
      padding: 1rem;
      text-align: center;
    }
    .container {
      padding: 2rem;
      max-width: 600px;
      margin: auto;
    }
    .card {
      background: white;
      padding: 1.5rem;
      border-radius: 16px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.15);
      margin-bottom: 2rem;
    }
    button {
      background: #e91e63;
      color: white;
      border: none;
      padding: 1rem 2rem;
      border-radius: 8px;
      font-size: 1rem;
      cursor: pointer;
      width: 100%;
    }
    button:hover {
      background: #d81b60;
    }
    .progress-bar {
      background: #ddd;
      border-radius: 20px;
      overflow: hidden;
      height: 20px;
      margin-top: 1rem;
    }
    .progress {
      background: #e91e63;
      height: 100%;
      width: 0%;
      transition: width 0.4s;
    }
    input, select {
      width: 100%;
      padding: 0.8rem;
      margin: 0.5rem 0;
      border-radius: 8px;
      border: 1px solid #ccc;
    }
    .hidden {
      display: none;
    }
    .timer {
      font-size: 1.2rem;
      color: #ff5722;
      margin-top: 1rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>Ganhe 50% de Desconto em Minutos!</h1>
    <p>Desbloqueie agora uma oferta exclusiva com nosso funil gamificado</p>
  </header>  <div class="container">
    <div id="step1" class="card">
      <h2>Responda e desbloqueie sua oferta:</h2>
      <label>Qual é seu maior desafio com marketing digital?</label>
      <select id="quiz">
        <option value="vendas">Poucas vendas</option>
        <option value="leads">Não consigo gerar leads</option>
        <option value="escala">Não consigo escalar</option>
      </select>
      <button onclick="nextStep()">Próximo</button>
    </div><div id="step2" class="card hidden">
  <h2>Cadastre-se para liberar seu cupom exclusivo:</h2>
  <input type="text" id="nome" placeholder="Seu nome" />
  <input type="email" id="email" placeholder="Seu e-mail" />
  <input type="tel" id="whatsapp" placeholder="WhatsApp (opcional)" />
  <button onclick="submitForm()">Desbloquear Oferta</button>
</div>

<div id="step3" class="card hidden">
  <h2>Oferta Desbloqueada!</h2>
  <p>Você ganhou <strong>50% de desconto</strong> no nosso curso digital simples e direto.</p>
  <div class="progress-bar">
    <div id="progress" class="progress"></div>
  </div>
  <p class="timer" id="timer">Oferta expira em: 5:00</p>
  <button onclick="window.location.href='https://seusite.com/oferta'">Aproveitar Agora

