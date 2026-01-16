
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="color-scheme" content="light only" />
  <meta name="theme-color" content="#ffffff" />

  <title>Diagnóstico Emocional de Casal | Onde estamos emocionalmente?</title>
  <meta name="description" content="Responda SIM ou NÃO e descubra onde o vínculo está desorganizado e o que precisa de cuidado agora. Envie suas respostas no WhatsApp para receber o diagnóstico." />

  <style>
    :root{
      --bg1:#f6f3ff;
      --bg2:#f7fbff;
      --card:#ffffff;
      --ink:#1f2430;
      --muted:#5b6476;
      --primary:#6c4bbf;
      --primary2:#8e6fe6;
      --accent:#2f7de1;
      --line:rgba(31,36,48,0.10);
      --shadow:0 18px 45px rgba(20, 12, 45, 0.10);
      --shadow2:0 10px 28px rgba(20, 12, 45, 0.08);
      --radius:18px;
    }

    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Arial, "Apple Color Emoji","Segoe UI Emoji";
      color:var(--ink);
      background: radial-gradient(1200px 600px at 10% 0%, var(--bg2) 0%, transparent 55%),
                  radial-gradient(900px 540px at 90% 10%, var(--bg1) 0%, transparent 55%),
                  linear-gradient(180deg, #ffffff 0%, #fbfaff 100%);
      line-height:1.55;
    }

    .wrap{
      max-width: 980px;
      margin: 0 auto;
      padding: 28px 18px 60px;
    }

    /* Top */
    .top{
      display:grid;
      grid-template-columns: 1.2fr 0.8fr;
      gap: 18px;
      align-items: stretch;
    }
    @media(max-width: 900px){
      .top{grid-template-columns: 1fr}
    }

    .hero{
      background: linear-gradient(135deg, rgba(108,75,191,0.10), rgba(47,125,225,0.10));
      border: 1px solid rgba(108,75,191,0.18);
      border-radius: var(--radius);
      padding: 28px 24px;
      box-shadow: var(--shadow);
      position:relative;
      overflow:hidden;
    }

    .badge{
      display:inline-flex;
      gap:10px;
      align-items:center;
      padding: 8px 12px;
      border-radius: 999px;
      background: rgba(108,75,191,0.12);
      border: 1px solid rgba(108,75,191,0.18);
      color: #3b2a5f;
      font-weight: 650;
      letter-spacing: .2px;
      font-size: 13px;
    }

    .title{
      margin: 14px 0 8px;
      font-size: 36px;
      line-height:1.12;
      letter-spacing:-.4px;
    }
    @media(max-width: 520px){
      .title{font-size: 30px;}
    }

    .subtitle{
      margin:0;
      color: var(--muted);
      font-size: 16.5px;
      max-width: 62ch;
    }

    .mini{
      margin-top: 18px;
      display:flex;
      flex-wrap:wrap;
      gap:10px;
    }

    .pill{
      background:#fff;
      border:1px solid var(--line);
      border-radius: 999px;
      padding: 9px 12px;
      font-size: 13.5px;
      color: #3d4658;
      box-shadow: var(--shadow2);
    }

    .side{
      background: var(--card);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      padding: 18px;
      box-shadow: var(--shadow2);
    }

    .side h3{
      margin: 0 0 10px;
      font-size: 16px;
      color: #3b2a5f;
    }
    .side p{
      margin: 0 0 10px;
      color: var(--muted);
      font-size: 14.5px;
    }

    /* ✅ Box da orientação (corrigido, sem “tarja vazia” no iPhone) */
    .rule{
      margin-top: 14px;
      padding: 14px;
      border-radius: 16px;
      background: rgba(47,125,225,0.08);
      border: 1px solid rgba(47,125,225,0.18);
      color: #244b7a;
      font-size: 14px;
    }
    .stepsRow{
      display:flex;
      flex-wrap:wrap;
      gap:10px;
      margin-top: 10px;
    }
    .stepChip{
      display:flex;
      align-items:center;
      gap:10px;
      padding: 10px 12px;
      border-radius: 14px;
      background:#fff;
      border:1px solid var(--line);
      box-shadow: 0 8px 18px rgba(20,12,45,0.06);
      color:#2a3242;
      flex: 1 1 240px;
    }
    .stepTag{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      padding: 6px 10px;
      border-radius: 999px;
      font-weight: 900;
      font-size: 12px;
      color:#2d2250;
      background: rgba(108,75,191,0.10);
      border: 1px solid rgba(108,75,191,0.18);
      white-space: nowrap;
    }
    .stepText{
      font-weight: 650;
      color:#2a3242;
      line-height: 1.25;
    }

    /* Sections */
    .section{
      margin-top: 18px;
      background: var(--card);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      padding: 22px;
      box-shadow: var(--shadow2);
    }
    .section h2{
      margin: 0 0 6px;
      font-size: 20px;
      color:#2d2250;
    }
    .section .note{
      margin: 0 0 16px;
      color: var(--muted);
      font-size: 14.5px;
    }

    /* Questions */
    .q{
      border-top: 1px solid var(--line);
      padding: 14px 0;
      display:flex;
      flex-direction: column; /* ✅ opções embaixo */
      gap: 10px;
      align-items:flex-start;
    }
    .q:first-of-type{border-top: none; padding-top: 0;}
    .q:last-of-type{padding-bottom: 0;}

    .qtext{
      width:100%;
      min-width: 0;
    }
    .qtext .n{
      display:inline-block;
      font-weight: 750;
      color: rgba(108,75,191,0.95);
      margin-right: 8px;
    }
    .qtext .t{
      font-size: 15.5px;
      color: #1f2430;
    }

    .opts{
      display:flex;
      gap:10px;
      flex-wrap: wrap;
      justify-content:flex-start; /* ✅ fica alinhado bonito no mobile */
      align-items:center;
      width:100%;
    }

    .opt{
      position:relative;
    }
    .opt input{
      position:absolute;
      opacity:0;
      pointer-events:none;
    }
    .opt label{
      display:inline-flex;
      align-items:center;
      gap: 8px;
      padding: 10px 14px;
      border-radius: 999px;
      border: 1px solid var(--line);
      background: #fff;
      color: #2b3342;
      font-size: 14px;
      font-weight: 650;
      cursor:pointer;
      user-select:none;
      transition: .18s ease;
      box-shadow: 0 6px 18px rgba(20,12,45,0.06);
      white-space:nowrap;
    }

    .opt input:checked + label{
      border-color: rgba(108,75,191,0.55);
      background: rgba(108,75,191,0.10);
      color:#2d2250;
    }

    .opt label .dot{
      width: 9px;
      height: 9px;
      border-radius: 999px;
      background: rgba(31,36,48,0.20);
    }
    .opt input:checked + label .dot{
      background: linear-gradient(135deg, var(--primary), var(--accent));
    }

    .alert{
      margin-top: 16px;
      padding: 14px 16px;
      border-radius: 14px;
      background: rgba(108,75,191,0.08);
      border: 1px solid rgba(108,75,191,0.18);
      color:#3b2a5f;
      font-size: 14px;
    }

    /* Final */
    .final{
      margin-top: 18px;
      background: linear-gradient(135deg, rgba(108,75,191,0.12), rgba(47,125,225,0.10));
      border: 1px solid rgba(108,75,191,0.18);
      border-radius: calc(var(--radius) + 4px);
      padding: 26px;
      box-shadow: var(--shadow);
    }

    .final h2{
      margin: 0 0 10px;
      font-size: 22px;
      color:#2d2250;
    }
    .final p{
      margin: 0 0 14px;
      color: var(--muted);
      font-size: 15px;
      max-width: 75ch;
    }

    .summary{
      background:#fff;
      border:1px solid var(--line);
      border-radius: 16px;
      padding: 16px;
      margin-top: 14px;
      box-shadow: var(--shadow2);
    }
    .summary .row{
      display:flex;
      gap: 12px;
      flex-wrap:wrap;
      align-items:center;
      justify-content: space-between;
      margin-top: 10px;
    }

    .count{
      display:flex;
      gap:10px;
      flex-wrap:wrap;
      align-items:center;
      color:#2d2250;
      font-weight: 700;
    }
    .chip{
      padding: 8px 12px;
      border-radius: 999px;
      border: 1px solid var(--line);
      background: rgba(47,125,225,0.06);
      color:#244b7a;
      font-size: 13.5px;
      font-weight: 700;
    }

    .btn{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      gap:10px;
      padding: 14px 18px;
      border-radius: 999px;
      text-decoration:none;
      border: none;
      cursor:pointer;
      font-weight: 800;
      font-size: 15px;
      transition: transform .12s ease, opacity .12s ease;
      user-select:none;
    }
    .btn:active{transform: scale(0.99);}
    .btn-primary{
      background: linear-gradient(135deg, var(--primary), var(--accent));
      color:#fff;
      box-shadow: 0 14px 30px rgba(108,75,191,0.22);
    }
    .btn-ghost{
      background:#fff;
      color:#2d2250;
      border:1px solid var(--line);
    }

    .small{
      margin-top: 10px;
      font-size: 12.8px;
      color: #6b7486;
    }

    .footer{
      margin-top: 30px;
      text-align:center;
      color:#7b8496;
      font-size: 13px;
    }

    .req{
      color:#a63d3d;
      font-weight: 700;
    }
  </style>
</head>

<body>
  <div class="wrap">

    <div class="top">
      <div class="hero">
        <div class="badge"> Diagnóstico Emocional de Casal</div>
        <h1 class="title">“Onde estamos emocionalmente como casal?”</h1>
        <p class="subtitle">
          Este diagnóstico não é para apontar culpados. É para revelar onde o vínculo está desorganizado
          e o que precisa de cuidado agora — com verdade, presença e responsabilidade.
        </p>

        <div class="mini">
          <div class="pill">✅ Respostas rápidas: SIM / NÃO</div>
          <div class="pill">🧭 Clareza sobre o vínculo</div>
          <div class="pill">🤝 Sem culpa, com cuidado</div>
        </div>
      </div>

      <div class="side">
        <h3>🧭 Orientação</h3>
        <p>
          Leia cada pergunta com calma.<br />
          Responda com honestidade — não com o que deveria ser,<br />
          mas com o que realmente é hoje.
        </p>

        <div class="rule">
          <strong>Como você recebe o diagnóstico:</strong>
          <div class="stepsRow">
            <div class="stepChip">
              <span class="stepTag">Passo 1</span>
              <span class="stepText">Responda todas as perguntas (SIM ou NÃO).</span>
            </div>
            <div class="stepChip">
              <span class="stepTag">Passo 2</span>
              <span class="stepText">No final, clique em “Enviar respostas no WhatsApp”.</span>
            </div>
            <div class="stepChip">
              <span class="stepTag">Passo 3</span>
              <span class="stepText">Eu devolvo a leitura e o ponto central do vínculo.</span>
            </div>
          </div>
        </div>

        <p class="small">
          *Se preferir, apenas uma pessoa pode responder pelo casal.
        </p>
      </div>
    </div>

    <!-- FORM -->
    <form id="quiz">

      <!-- BLOCO 1 -->
      <div class="section">
        <h2>🔍 Bloco 1 — Conexão e Presença</h2>
        <p class="note">Quando a presença diminui, o casal começa a funcionar, mas deixa de se encontrar.</p>

        <div class="q">
          <div class="qtext"><span class="n">1.</span><span class="t">Vocês se sentem emocionalmente conectados no dia a dia?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q1" id="q1s" value="SIM" required><label for="q1s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q1" id="q1n" value="NÃO"><label for="q1n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">2.</span><span class="t">As conversas entre vocês vão além da rotina e das tarefas?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q2" id="q2s" value="SIM" required><label for="q2s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q2" id="q2n" value="NÃO"><label for="q2n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">3.</span><span class="t">Vocês conseguem ficar em silêncio juntos sem sentir afastamento?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q3" id="q3s" value="SIM" required><label for="q3s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q3" id="q3n" value="NÃO"><label for="q3n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">4.</span><span class="t">Conseguem estar juntos sem distrações externas (celular, trabalho, filhos)?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q4" id="q4s" value="SIM" required><label for="q4s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q4" id="q4n" value="NÃO"><label for="q4n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">5.</span><span class="t">Existe sensação de parceria no relacionamento?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q5" id="q5s" value="SIM" required><label for="q5s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q5" id="q5n" value="NÃO"><label for="q5n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="alert">👉 Alerta: Quando a presença diminui, o casal começa a funcionar, mas deixa de se encontrar.</div>
      </div>

      <!-- BLOCO 2 -->
      <div class="section">
        <h2>🔍 Bloco 2 — Comunicação e Escuta</h2>
        <p class="note">Quando a escuta acaba, o vínculo se defende em vez de se cuidar.</p>

        <div class="q">
          <div class="qtext"><span class="n">6.</span><span class="t">Vocês se sentem ouvidos quando expressam o que sentem?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q6" id="q6s" value="SIM" required><label for="q6s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q6" id="q6n" value="NÃO"><label for="q6n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">7.</span><span class="t">As conversas costumam terminar em entendimento mútuo?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q7" id="q7s" value="SIM" required><label for="q7s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q7" id="q7n" value="NÃO"><label for="q7n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">8.</span><span class="t">Vocês conseguem falar sobre temas difíceis sem medo constante de conflito?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q8" id="q8s" value="SIM" required><label for="q8s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q8" id="q8n" value="NÃO"><label for="q8n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">9.</span><span class="t">Conseguem escutar um ao outro com presença, sem preparar defesa?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q9" id="q9s" value="SIM" required><label for="q9s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q9" id="q9n" value="NÃO"><label for="q9n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">10.</span><span class="t">Existe curiosidade para compreender o outro durante as conversas?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q10" id="q10s" value="SIM" required><label for="q10s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q10" id="q10n" value="NÃO"><label for="q10n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="alert">👉 Alerta: Quando a escuta acaba, o vínculo se defende em vez de se cuidar.</div>
      </div>

      <!-- BLOCO 3 -->
      <div class="section">
        <h2>🔍 Bloco 3 — Afeto, Intimidade e Escolha</h2>
        <p class="note">Sem afeto e admiração, o casal entra em modo de sobrevivência.</p>

        <div class="q">
          <div class="qtext"><span class="n">11.</span><span class="t">Existe demonstração espontânea de carinho entre vocês?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q11" id="q11s" value="SIM" required><label for="q11s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q11" id="q11n" value="NÃO"><label for="q11n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">12.</span><span class="t">A intimidade faz parte da relação de forma natural?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q12" id="q12s" value="SIM" required><label for="q12s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q12" id="q12n" value="NÃO"><label for="q12n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">13.</span><span class="t">Vocês ainda se sentem escolhidos um pelo outro?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q13" id="q13s" value="SIM" required><label for="q13s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q13" id="q13n" value="NÃO"><label for="q13n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">14.</span><span class="t">Há espaço para vulnerabilidade emocional no casal?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q14" id="q14s" value="SIM" required><label for="q14s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q14" id="q14n" value="NÃO"><label for="q14n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">15.</span><span class="t">Existe admiração mútua na relação?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q15" id="q15s" value="SIM" required><label for="q15s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q15" id="q15n" value="NÃO"><label for="q15n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="alert">👉 Alerta: Sem afeto e admiração, o casal entra em modo de sobrevivência.</div>
      </div>

      <!-- BLOCO 4 -->
      <div class="section">
        <h2>🔍 Bloco 4 — Conflitos e Padrões</h2>
        <p class="note">Conflitos não resolvidos se transformam em distância emocional.</p>

        <div class="q">
          <div class="qtext"><span class="n">16.</span><span class="t">Os conflitos costumam ser resolvidos sem se repetirem constantemente?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q16" id="q16s" value="SIM" required><label for="q16s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q16" id="q16n" value="NÃO"><label for="q16n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">17.</span><span class="t">Após um conflito, vocês conseguem reparar e se reaproximar?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q17" id="q17s" value="SIM" required><label for="q17s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q17" id="q17n" value="NÃO"><label for="q17n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">18.</span><span class="t">As decisões no relacionamento são tomadas de forma equilibrada?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q18" id="q18s" value="SIM" required><label for="q18s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q18" id="q18n" value="NÃO"><label for="q18n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">19.</span><span class="t">Os sentimentos difíceis são elaborados ao longo do tempo, sem acumular?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q19" id="q19s" value="SIM" required><label for="q19s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q19" id="q19n" value="NÃO"><label for="q19n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">20.</span><span class="t">Vocês conseguem construir uma história própria, sem repetir padrões familiares?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q20" id="q20s" value="SIM" required><label for="q20s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q20" id="q20n" value="NÃO"><label for="q20n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="alert">👉 Alerta: Conflitos não resolvidos se transformam em distância emocional.</div>
      </div>

      <!-- BLOCO 5 -->
      <div class="section">
        <h2>🔍 Bloco 5 — Responsabilidade e Lugar no Vínculo</h2>
        <p class="note">Quando os lugares se confundem, o amor cansa. Quando se organizam, o vínculo respira.</p>

        <div class="q">
          <div class="qtext"><span class="n">21.</span><span class="t">A responsabilidade pelo relacionamento é compartilhada entre os dois?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q21" id="q21s" value="SIM" required><label for="q21s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q21" id="q21n" value="NÃO"><label for="q21n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">22.</span><span class="t">Existe equilíbrio entre dar e receber na relação?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q22" id="q22s" value="SIM" required><label for="q22s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q22" id="q22n" value="NÃO"><label for="q22n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">23.</span><span class="t">Os papéis de cada um no casal são claros?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q23" id="q23s" value="SIM" required><label for="q23s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q23" id="q23n" value="NÃO"><label for="q23n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">24.</span><span class="t">Vocês se apoiam mutuamente nas dificuldades?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q24" id="q24s" value="SIM" required><label for="q24s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q24" id="q24n" value="NÃO"><label for="q24n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="q">
          <div class="qtext"><span class="n">25.</span><span class="t">O relacionamento é tratado como prioridade na vida de vocês?</span></div>
          <div class="opts">
            <span class="opt"><input type="radio" name="q25" id="q25s" value="SIM" required><label for="q25s"><span class="dot"></span>SIM</label></span>
            <span class="opt"><input type="radio" name="q25" id="q25n" value="NÃO"><label for="q25n"><span class="dot"></span>NÃO</label></span>
          </div>
        </div>

        <div class="alert">👉 Alerta: Quando os lugares se confundem, o amor cansa.</div>
      </div>

      <!-- FINAL -->
      <div class="final">
        <h2>✅ Finalizar e enviar para receber o diagnóstico</h2>
        <p>
          Ao clicar no botão abaixo, suas respostas serão organizadas automaticamente e enviadas no WhatsApp.
          Com base nisso, eu te devolvo a leitura do diagnóstico (vermelho / amarelo / verde) e o ponto central que aparece no vínculo.
        </p>

        <div class="summary">
          <strong>Resumo automático</strong>
          <div class="row">
            <div class="count">
              <span class="chip" id="countYes">SIM: 0</span>
              <span class="chip" id="countNo">NÃO: 0</span>
              <span class="chip" id="countMiss">Faltam: 25</span>
            </div>

            <div style="display:flex; gap:10px; flex-wrap:wrap;">
              <button type="button" class="btn btn-ghost" id="btnCopy">Copiar respostas</button>
              <a class="btn btn-primary" id="btnWhats" href="#" aria-disabled="true">Enviar respostas no WhatsApp</a>
            </div>
          </div>

          <div class="small">
            <span class="req">*</span> Para habilitar o envio, responda todas as perguntas.
          </div>
        </div>

        <div class="footer">
          © <span id="year"></span> • Diagnóstico Emocional de Casal • Desenvolvido para uma experiência simples, direta e acolhedora.
        </div>
      </div>

    </form>
  </div>

  <script>
    // CONFIG
    const WHATS_NUMBER = "5549998110445"; // Evandro - 55 + DDD + número
    const RESPONSAVEL = "Evandro Favoretto"; // aparece na mensagem

    const questions = [
      "1) Vocês se sentem emocionalmente conectados no dia a dia?",
      "2) As conversas entre vocês vão além da rotina e das tarefas?",
      "3) Vocês conseguem ficar em silêncio juntos sem sentir afastamento?",
      "4) Conseguem estar juntos sem distrações externas (celular, trabalho, filhos)?",
      "5) Existe sensação de parceria no relacionamento?",

      "6) Vocês se sentem ouvidos quando expressam o que sentem?",
      "7) As conversas costumam terminar em entendimento mútuo?",
      "8) Vocês conseguem falar sobre temas difíceis sem medo constante de conflito?",
      "9) Conseguem escutar um ao outro com presença, sem preparar defesa?",
      "10) Existe curiosidade para compreender o outro durante as conversas?",

      "11) Existe demonstração espontânea de carinho entre vocês?",
      "12) A intimidade faz parte da relação de forma natural?",
      "13) Vocês ainda se sentem escolhidos um pelo outro?",
      "14) Há espaço para vulnerabilidade emocional no casal?",
      "15) Existe admiração mútua na relação?",

      "16) Os conflitos costumam ser resolvidos sem se repetirem constantemente?",
      "17) Após um conflito, vocês conseguem reparar e se reaproximar?",
      "18) As decisões no relacionamento são tomadas de forma equilibrada?",
      "19) Os sentimentos difíceis são elaborados ao longo do tempo, sem acumular?",
      "20) Vocês conseguem construir uma história própria, sem repetir padrões familiares?",

      "21) A responsabilidade pelo relacionamento é compartilhada entre os dois?",
      "22) Existe equilíbrio entre dar e receber na relação?",
      "23) Os papéis de cada um no casal são claros?",
      "24) Vocês se apoiam mutuamente nas dificuldades?",
      "25) O relacionamento é tratado como prioridade na vida de vocês?"
    ];

    const form = document.getElementById("quiz");
    const btnWhats = document.getElementById("btnWhats");
    const btnCopy = document.getElementById("btnCopy");

    const countYes = document.getElementById("countYes");
    const countNo = document.getElementById("countNo");
    const countMiss = document.getElementById("countMiss");

    document.getElementById("year").textContent = new Date().getFullYear();

    function getAnswers(){
      const answers = [];
      let yes = 0, no = 0, miss = 0;

      for(let i=1;i<=25;i++){
        const chosen = form.querySelector(`input[name="q${i}"]:checked`);
        if(!chosen){
          answers.push({ i, q: questions[i-1], a: "—" });
          miss++;
        } else {
          const val = chosen.value;
          answers.push({ i, q: questions[i-1], a: val });
          if(val === "SIM") yes++;
          if(val === "NÃO") no++;
        }
      }
      return { answers, yes, no, miss };
    }

    function buildMessage(){
      const { answers, yes, no } = getAnswers();

      const header =
`DIAGNÓSTICO EMOCIONAL DE CASAL
(Onde estamos emocionalmente como casal?)

Responsável: ${RESPONSAVEL}

Resumo:
• SIM: ${yes}
• NÃO: ${no}

Respostas:`;

      const lines = answers.map(item => `${item.i}. ${item.a} — ${item.q}`).join("\n");

      const footer =
`\n\nPedido:
Quero receber a leitura do meu diagnóstico e o ponto central que aparece no vínculo.`;

      return { text: `${header}\n\n${lines}${footer}` };
    }

    function updateUI(){
      const { yes, no, miss } = getAnswers();

      countYes.textContent = `SIM: ${yes}`;
      countNo.textContent  = `NÃO: ${no}`;
      countMiss.textContent = `Faltam: ${miss}`;

      const allDone = miss === 0;
      btnWhats.style.opacity = allDone ? "1" : "0.55";
      btnWhats.style.pointerEvents = allDone ? "auto" : "none";
      btnWhats.setAttribute("aria-disabled", allDone ? "false" : "true");

      if(allDone){
        const { text } = buildMessage();
        btnWhats.href = `https://wa.me/${WHATS_NUMBER}?text=${encodeURIComponent(text)}`;
      } else {
        btnWhats.href = "#";
      }
    }

    form.addEventListener("change", updateUI);

    btnCopy.addEventListener("click", async () => {
      const { miss } = getAnswers();
      const { text } = buildMessage();

      if(miss !== 0){
        alert("Responda todas as perguntas para copiar o diagnóstico completo.");
        return;
      }
      try{
        await navigator.clipboard.writeText(text);
        btnCopy.textContent = "Copiado!";
        setTimeout(()=> btnCopy.textContent = "Copiar respostas", 1200);
      } catch(e){
        alert("Não consegui copiar automaticamente. Use o botão do WhatsApp para enviar.");
      }
    });

    updateUI();
  </script>
</body>
</html>
