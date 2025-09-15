<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Anamnese Online | Dra. Natália Magalhães</title>

  <!-- Fontes -->
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700;800&family=Playfair+Display:wght@500;600&display=swap" rel="stylesheet">

  <style>
    :root{
      --rose-prim:#B65F56; --rose-apoio:#E6A3A3; --creme:#FCF5EB;
      --border:#e6e0d7; --txt:#2b2b2b; --muted:#7a5e59;
      --radius:18px; --shadow:0 14px 40px rgba(0,0,0,.06);
      --maxw:1000px; --gap:16px;
    }
    *{box-sizing:border-box}
    body{margin:0; color:var(--txt); font-family:Montserrat,system-ui,-apple-system,Segoe UI,Roboto,Arial; background:var(--creme)}
    img{max-width:100%; height:auto; display:block}

    header{max-width:var(--maxw);margin:28px auto 0;padding:0 16px 8px; text-align:center}
    .brand{display:flex;flex-direction:column;align-items:center;gap:12px}
    .brand img{width:clamp(160px, 28vw, 300px)}
    @media (max-width:720px){ .brand img{ width:clamp(140px, 42vw, 240px) } }
    .brand h1{
      font-family:"Playfair Display", serif; font-weight:600;
      font-size:clamp(16px, 2vw, 22px); line-height:1.15; letter-spacing:.2px; color:var(--rose-prim);
      margin:6px 0 0;
    }
    .brand p{margin-top:8px; color:var(--muted); font-size:clamp(12px, 2vw, 14px); max-width:720px}

    main{max-width:var(--maxw);margin:18px auto 50px;padding:0 16px}
    .card{background:#fff;border:1px solid var(--border);border-radius:var(--radius);box-shadow:var(--shadow);padding:clamp(16px, 2.8vw, 26px);margin-bottom:18px}
    .section-title{font-size:clamp(13px, 2.2vw, 15px);font-weight:800;letter-spacing:.3px;text-transform:uppercase;color:#5d3c38;margin:0 0 16px;border-left:6px solid var(--rose-prim);padding-left:10px}

    .row{display:grid;grid-template-columns:repeat(2,1fr);gap:var(--gap)}
    .row-3{display:grid;grid-template-columns:repeat(3,1fr);gap:var(--gap)}
    @media (max-width:1024px){ .row-3{grid-template-columns:repeat(2,1fr)} }
    @media (max-width:720px){ .row,.row-3{grid-template-columns:1fr} }

    label{font-size:clamp(12px, 2.2vw, 13.5px); color:#5d3c38; display:block; margin:0 0 8px; font-weight:600}
    input[type="text"],input[type="tel"],input[type="email"],input[type="date"],textarea,select{
      width:100%; padding:14px; min-height:44px; border:1px solid var(--border); border-radius:14px; background:#fff; outline:none; font-size:16px
    }
    textarea{min-height:120px; resize:vertical}
    .inline{display:flex;align-items:center;gap:12px;flex-wrap:wrap}
    .chip{display:inline-flex;align-items:center;gap:8px;padding:10px 14px;border:1px solid var(--border);border-radius:999px;background:#fff}
    .chip input{accent-color:var(--rose-prim)}
    .chips-wrap{display:flex;flex-wrap:wrap;gap:10px}
    .hidden{display:none}
    .required::after{content:" *";color:#b45309}
    .success{background:#ecfdf5;border:1px solid #a7f3d0;color:#065f46;padding:16px;border-radius:12px;margin-top:12px;text-align:center}
    .actions{display:flex;gap:12px;flex-wrap:wrap;justify-content:center}
    .detail.off{opacity:.6}
    .detail.off input{background:#f8f5f0}

    /* Layout: Queixa & Interesses */
    .qei-grid{display:grid;grid-template-columns: 1.05fr .95fr;gap:24px;align-items:start}
    @media (max-width:900px){ .qei-grid{ grid-template-columns:1fr } }
    .qei-box{border:1px solid var(--border);border-radius:14px;padding:16px;background:#fff}
    .qei-box .block + .block{ margin-top:16px }
    .tight{margin-bottom:8px}

    /* Acessibilidade extra */
    #feedback[role="status"]{min-height:20px}

    /* Utilitários */
    .box-muted {background:#fff7ed;border:1px solid #f2d7be;border-radius:12px;padding:12px}
    .img-preview {width:100%;max-width:260px;border:1px solid var(--border);border-radius:12px}

    /* CTA */
    .btn-cta{--h:56px;display:inline-flex;align-items:center;justify-content:center;gap:10px;min-height:var(--h);padding:0 28px;border:0;border-radius:999px;cursor:pointer;font-weight:800;font-size:17px;color:#fff;background:linear-gradient(135deg,#B65F56 0%,#E6A3A3 100%);box-shadow:0 12px 28px rgba(182,95,86,.25)}
    @media (max-width:720px){ .btn-cta{width:100%} }
    footer{ text-align:center; margin:40px 0; font-size:12px; color:#7a5e59; line-height:1.6; }
    footer .dev{background:linear-gradient(135deg,#B65F56 0%,#E6A3A3 100%);-webkit-background-clip:text;-webkit-text-fill-color:transparent;display:inline-block}
  </style>
</head>
<body>
  <header>
    <div class="brand">
      <img src="https://dranatmagalhaes.com.br/wp-content/uploads/2024/11/logo-dra-natalia.png" alt="Logo Dra. Natália Magalhães">
      <h1>Avaliação Inicial — O cuidado com você começa aqui</h1>
      <p>Esta anamnese online nos ajuda a conhecer seu histórico e objetivos para preparar um atendimento seguro e personalizado antes da consulta.</p>
    </div>
  </header>

  <main>
    <form id="form" novalidate>
      <!-- DADOS PESSOAIS -->
      <div class="card">
        <div class="section-title">Dados Pessoais</div>
        <div class="row">
          <div><label class="required" for="nome">Nome completo</label><input type="text" id="nome" name="nome" required autocomplete="name"></div>
          <div>
            <label class="required" for="nascimento">Data de nascimento</label>
            <input type="date" id="nascimento" name="nascimento" required autocomplete="bday">
          </div>
          <div><label class="required" for="telefone">Telefone (WhatsApp)</label><input type="tel" id="telefone" name="telefone" placeholder="(31) 9 0000-0000" required inputmode="tel" autocomplete="tel"></div>
          <div><label class="required" for="email">E-mail</label><input type="email" id="email" name="email" required autocomplete="email"></div>
          <div><label class="required" for="profissao">Profissão</label><input type="text" id="profissao" name="profissao" required autocomplete="organization-title"></div>
          <div><label class="required" for="cidade">Cidade/Estado</label><input type="text" id="cidade" name="cidade" placeholder="Ex.: Belo Horizonte/MG" required autocomplete="address-level2"></div>
        </div>
      </div>

      <!-- QUEIXA & INTERESSES -->
      <div class="card">
        <div class="section-title">Queixa & Interesses (Estética Regenerativa)</div>

        <div class="qei-grid">
          <!-- ESQUERDA: Opção 1 (Organizada e Direta) -->
          <div class="qei-box">
            <fieldset class="block" style="border:0;padding:0;margin:0">
              <legend class="required tight" style="font-weight:600;color:#5d3c38">Qual é seu objetivo principal com o tratamento?</legend>
              <p style="margin:0 0 10px;color:#8b6c67;font-size:12px">Marque a(s) opção(ões) que mais te representa(m)</p>
              <div class="chips-wrap" role="group" aria-label="Objetivos principais">
                <label class="chip"><input type="checkbox" name="objetivos" value="Combater a flacidez (pele mais firme)"> Combater a flacidez (pele mais firme)</label>
                <label class="chip"><input type="checkbox" name="objetivos" value="Reduzir linhas de expressão e rugas (aparência mais jovem)"> Reduzir linhas de expressão e rugas (aparência mais jovem)</label>
                <label class="chip"><input type="checkbox" name="objetivos" value="Melhorar a qualidade da pele (viço, hidratação e luminosidade)"> Melhorar a qualidade da pele (viço, hidratação e luminosidade)</label>
                <label class="chip"><input type="checkbox" name="objetivos" value="Realizar Preenchimento e/ou Rinomodelação (corrigir e harmonizar pontos específicos)"> Preenchimento e/ou Rinomodelação</label>
                <label class="chip"><input type="checkbox" name="objetivos" value="Realizar Harmonização Orofacial (melhorar proporções e contornos do rosto)"> Harmonização Orofacial</label>
                <label class="chip"><input type="checkbox" id="objetivoOutroChk" name="objetivos" value="Outro"> Outro</label>
              </div>
            </fieldset>

            <!-- Campo aberto só quando marcar "Outro" -->
            <div class="block hidden" id="wrap-objetivo-outro">
              <label for="objetivoOutro">Se quiser, descreva em poucas palavras</label>
              <textarea id="objetivoOutro" name="objetivoOutro" placeholder="Ex.: assimetria no sorriso; afinamento do queixo; marcas ao redor da boca…"></textarea>
            </div>
          </div>

          <!-- DIREITA: Interesses + Investimento -->
          <div class="qei-box">
            <fieldset class="block" style="border:0;padding:0;margin:0">
              <legend class="tight" style="font-weight:600;color:#5d3c38">Quais procedimentos te interessam?</legend>
              <div class="chips-wrap" role="group" aria-label="Procedimentos de interesse">
                <label class="chip"><input type="checkbox" name="procInteresse" value="Botox"> Botox</label>
                <label class="chip"><input type="checkbox" name="procInteresse" value="Bioreconexão"> Bioreconexão</label>
                <label class="chip"><input type="checkbox" name="procInteresse" value="Ultraformer"> Ultraformer</label>
                <label class="chip"><input type="checkbox" name="procInteresse" value="Reset"> Reset</label>
                <label class="chip"><input type="checkbox" name="procInteresse" value="Exocoll"> Exocoll</label>
                <label class="chip"><input type="checkbox" name="procInteresse" value="Protocoll"> Protocoll</label>
                <label class="chip"><input type="checkbox" name="procInteresse" value="Bioestimulador de colágeno"> Bioestimulador de colágeno</label>
                <label class="chip"><input type="checkbox" name="procInteresse" value="Preenchimento labial"> Preenchimento labial</label>
                <label class="chip"><input type="checkbox" name="procInteresse" value="Outros"> Outros…</label>
              </div>
            </fieldset>

            <fieldset class="block" style="border:0;padding:0;margin:0">
              <legend class="tight" style="font-weight:600;color:#5d3c38">Qual faixa de investimento você considera neste momento?</legend>
              <div class="chips-wrap" role="radiogroup" aria-label="Faixa de investimento">
                <label class="chip"><input type="radio" name="faixaInvest" value="Até 2.000"> Até R$ 2.000</label>
                <label class="chip"><input type="radio" name="faixaInvest" value="2.000–3.500"> R$ 2.000–3.500</label>
                <label class="chip"><input type="radio" name="faixaInvest" value="3.500–6.000"> R$ 3.500–6.000</label>
                <label class="chip"><input type="radio" name="faixaInvest" value="Acima de 6.000"> Acima de R$ 6.000</label>
                <label class="chip"><input type="radio" name="faixaInvest" value="Quero avaliar com a Dra."> Quero avaliar com a Dra.</label>
              </div>
            </fieldset>
          </div>
        </div>
      </div>

      <!-- HISTÓRICO ESTÉTICO -->
      <div class="card">
        <div class="section-title">Histórico Estético</div>
        <div class="row">
          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Já fez procedimentos estéticos?</legend>
              <div class="inline" role="radiogroup" aria-label="Já fez procedimentos estéticos?">
                <label class="chip"><input type="radio" name="jaFez" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="jaFez" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>
          <div id="wrap-quais-fez" class="hidden">
            <label for="quaisFez">Quais?</label>
            <input type="text" id="quaisFez" name="quaisFez" placeholder="Ex.: toxina, preenchedor, bioestimulador…">
          </div>

          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Você já é paciente da Dra. Natália?</legend>
              <div class="inline" role="radiogroup" aria-label="Já é paciente?">
                <label class="chip"><input type="radio" name="jaPaciente" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="jaPaciente" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>
        </div>
      </div>

      <!-- SAÚDE -->
      <div class="card">
        <div class="section-title">Saúde</div>
        <div class="row">
          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Alergia a medicamentos?</legend>
              <div class="inline" role="radiogroup">
                <label class="chip"><input type="radio" name="alergiaMedicamentos" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="alergiaMedicamentos" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>
          <div id="wrap-alergia-meds" class="detail off"><label for="quaisAlergiaMedicamentos">Quais medicamentos (alergia)?</label><input type="text" id="quaisAlergiaMedicamentos" name="quaisAlergiaMedicamentos" aria-disabled="true" disabled></div>

          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Possui outras alergias?</legend>
              <div class="inline" role="radiogroup">
                <label class="chip"><input type="radio" name="alergiasGerais" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="alergiasGerais" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>
          <div id="wrap-alergias" class="detail off"><label for="quaisAlergias">Quais alergias?</label><input type="text" id="quaisAlergias" name="quaisAlergias" aria-disabled="true" disabled></div>

          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Usa medicamentos?</legend>
              <div class="inline" role="radiogroup">
                <label class="chip"><input type="radio" name="usaMedicamentos" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="usaMedicamentos" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>
          <div id="wrap-usa-meds" class="detail off"><label for="quaisMedicamentos">Quais medicamentos?</label><input type="text" id="quaisMedicamentos" name="quaisMedicamentos" aria-disabled="true" disabled></div>

          <div>
            <label class="required">Doenças/pré-existências</label>
            <div class="inline" role="group" aria-label="Doenças e condições">
              <label class="chip"><input type="checkbox" name="doencas" value="Diabetes"> Diabetes</label>
              <label class="chip"><input type="checkbox" name="doencas" value="Hipertensão"> Hipertensão</label>
              <label class="chip"><input type="checkbox" name="doencas" value="Cardíacas"> Cardíacas</label>
              <label class="chip"><input type="checkbox" name="doencas" value="Autoimunes"> Autoimunes</label>
              <label class="chip"><input type="checkbox" name="doencas" value="Nenhuma" checked> Nenhuma</label>
            </div>
          </div>

          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Gestante ou amamentando?</legend>
              <div class="inline" role="radiogroup">
                <label class="chip"><input type="radio" name="gestante" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="gestante" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>

          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Uso de anabolizantes?</legend>
              <div class="inline" role="radiogroup">
                <label class="chip"><input type="radio" name="anabolizantes" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="anabolizantes" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>
          <div id="wrap-anabolizantes" class="detail off"><label for="quaisAnabolizantes">Quais (anabolizantes)?</label><input type="text" id="quaisAnabolizantes" name="quaisAnabolizantes" aria-disabled="true" disabled></div>

          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Cirurgias recentes (últimos 12 meses)?</legend>
              <div class="inline" role="radiogroup">
                <label class="chip"><input type="radio" name="cirurgiaRecente" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="cirurgiaRecente" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>
          <div id="wrap-cirurgias" class="detail off"><label for="quaisCirurgias">Quais cirurgias?</label><input type="text" id="quaisCirurgias" name="quaisCirurgias" aria-disabled="true" disabled></div>
        </div>

        <div class="row">
          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Tabagismo</legend>
              <div class="inline" role="radiogroup">
                <label class="chip"><input type="radio" name="tabagismo" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="tabagismo" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>
          <div id="wrap-tabagismo" class="detail off"><label for="tabagismoDetalhes">Tabagismo – detalhes</label><input type="text" id="tabagismoDetalhes" name="tabagismoDetalhes" aria-disabled="true" disabled></div>

          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Álcool</legend>
              <div class="inline" role="radiogroup">
                <label class="chip"><input type="radio" name="alcool" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="alcool" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>
          <div id="wrap-alcool" class="detail off"><label for="alcoolDetalhes">Álcool – frequência/quantidade</label><input type="text" id="alcoolDetalhes" name="alcoolDetalhes" placeholder="Ex.: 1–2x/semana; 2 doses/vez" aria-disabled="true" disabled></div>

          <div>
            <fieldset style="border:0;padding:0;margin:0">
              <legend class="required" style="font-weight:600;color:#5d3c38">Atividade física</legend>
              <div class="inline" role="radiogroup">
                <label class="chip"><input type="radio" name="atividadeFisica" value="N" checked> Não</label>
                <label class="chip"><input type="radio" name="atividadeFisica" value="S"> Sim</label>
              </div>
            </fieldset>
          </div>
          <div id="wrap-atividade" class="detail off"><label for="atividadeFisicaDetalhes">Atividade física – tipo/frequência</label><input type="text" id="atividadeFisicaDetalhes" name="atividadeFisicaDetalhes" placeholder="Ex.: musculação 3x/semana, 45min" aria-disabled="true" disabled></div>
        </div>
      </div>

      <!-- FOTOS -->
      <div class="card">
        <div class="section-title">Fotos para Avaliação</div>
        <p class="muted">Envie 3 fotos: Frente, Perfil esquerdo e Perfil direito (luz natural, fundo neutro).</p>
        <div class="row-3">
          <div><label for="selfieFront">Frente</label><input type="file" id="selfieFront" accept="image/*" capture="user"><img id="previewFront" class="hidden img-preview" alt="Prévia frente"><input type="hidden" name="selfieFrontDataURL"></div>
          <div><label for="selfieLeft">Perfil esquerdo</label><input type="file" id="selfieLeft" accept="image/*" capture="user"><img id="previewLeft" class="hidden img-preview" alt="Prévia perfil esquerdo"><input type="hidden" name="selfieLeftDataURL"></div>
          <div><label for="selfieRight">Perfil direito</label><input type="file" id="selfieRight" accept="image/*" capture="user"><img id="previewRight" class="hidden img-preview" alt="Prévia perfil direito"><input type="hidden" name="selfieRightDataURL"></div>
        </div>
      </div>

      <!-- LGPD -->
      <div class="card">
        <div class="section-title">Privacidade & LGPD</div>
        <div class="inline box-muted">
          <input type="checkbox" id="lgpd" name="lgpd" required aria-required="true" style="margin-right:8px">
          <label for="lgpd" class="required" style="margin:0">Autorizo o uso dos meus dados para fins de contato, avaliação e propostas, conforme a LGPD.</label>
        </div>
      </div>

      <div class="actions"><button type="submit" class="btn-cta">Enviar anamnese</button></div>
      <div id="feedback" class="success hidden" role="status" aria-live="polite"></div>

      <!-- UTM & tech + honeypot -->
      <input type="hidden" name="utm_source"><input type="hidden" name="utm_medium"><input type="hidden" name="utm_campaign"><input type="hidden" name="utm_content"><input type="hidden" name="utm_term"><input type="hidden" name="ua"><input type="hidden" name="ip">
      <input type="text" name="_hp" style="position:absolute;left:-9999px;opacity:0" tabindex="-1" autocomplete="off" aria-hidden="true">
    </form>
  </main>

  <footer>
    © 2025 Dra. Natália Magalhães – Todos os direitos reservados.<br>
    <span class="dev">Desenvolvido por Noelle Ventura</span>
  </footer>

  <!-- ======= SCRIPT ÚNICO ======= -->
  <script>
    // URL do Web App (Apps Script) e segredo
    const EXEC_URL = 'https://script.google.com/macros/s/AKfycbzJtn8X24JMNPgess3BhdU-8icXFc165uxt8kUOQJUfMqGF4jc3bouzIN-RGLWykk6d/exec';
    const SECRET   = 'nm_2025_24jun86_bynv';

    const $$=(s,r=document)=>Array.from(r.querySelectorAll(s));
    const getRadio=(name)=>(document.querySelector('input[name="'+name+'"]:checked')||{}).value||'';

    // Dependências (um loop controla tudo)
    const deps = [
      { gate:'jaFez', yes:true,  wrap:'#wrap-quais-fez',         input:'input[name="quaisFez"]',            hideWhenNo:true },
      { gate:'alergiaMedicamentos', yes:true, wrap:'#wrap-alergia-meds',  input:'input[name="quaisAlergiaMedicamentos"]' },
      { gate:'alergiasGerais',      yes:true, wrap:'#wrap-alergias',      input:'input[name="quaisAlergias"]' },
      { gate:'usaMedicamentos',     yes:true, wrap:'#wrap-usa-meds',      input:'input[name="quaisMedicamentos"]' },
      { gate:'anabolizantes',       yes:true, wrap:'#wrap-anabolizantes', input:'input[name="quaisAnabolizantes"]' },
      { gate:'cirurgiaRecente',     yes:true, wrap:'#wrap-cirurgias',     input:'input[name="quaisCirurgias"]' },
      { gate:'tabagismo',           yes:true, wrap:'#wrap-tabagismo',     input:'input[name="tabagismoDetalhes"]' },
      { gate:'alcool',              yes:true, wrap:'#wrap-alcool',        input:'input[name="alcoolDetalhes"]' },
      { gate:'atividadeFisica',     yes:true, wrap:'#wrap-atividade',     input:'input[name="atividadeFisicaDetalhes"]' },
    ];
    function applyDeps(){
      deps.forEach(d=>{
        const on = (document.querySelector(`input[name="${d.gate}"]:checked`)?.value||'') === (d.yes?'S':'N');
        const wrap  = document.querySelector(d.wrap);
        const input = document.querySelector(d.input);
        if (!wrap || !input) return;
        if (d.hideWhenNo) { wrap.classList.toggle('hidden', !on); } // Histórico estético
        input.disabled = !on; wrap.classList.toggle('off', !on);
        const lbl=wrap.querySelector('label'); if (lbl) lbl.classList.toggle('required', on);
        if (!on) input.value='';
      });
    }

    // “Outro” em Objetivos
    function toggleObjetivoOutro(){
      const outro = document.getElementById('objetivoOutroChk');
      const wrap  = document.getElementById('wrap-objetivo-outro');
      if (!outro || !wrap) return;
      wrap.classList.toggle('hidden', !outro.checked);
    }

    // Data de nascimento: mobile com máscara dd/mm/aaaa
    (function enableMobileDOBInput(){
      const dob = document.getElementById('nascimento');
      if (!dob) return;
      const isMobile = /Android|iPhone|iPad|iPod|Opera Mini|IEMobile/i.test(navigator.userAgent);
      if (isMobile) {
        dob.setAttribute('type','text');
        dob.setAttribute('inputmode','numeric');
        dob.setAttribute('autocomplete','bday');
        dob.setAttribute('placeholder','dd/mm/aaaa');
        dob.setAttribute('maxlength','10');
        dob.addEventListener('input',(e)=>{
          let v=e.target.value.replace(/\D/g,'').slice(0,8);
          if(v.length>=5) v=v.replace(/(\d{2})(\d{2})(\d{1,4})/,'$1/$2/$3');
          else if(v.length>=3) v=v.replace(/(\d{2})(\d{1,2})/,'$1/$2');
          e.target.value=v;
        });
        dob.addEventListener('blur',(e)=>{
          const m=/^(\d{2})\/(\d{2})\/(\d{4})$/.exec(e.target.value);
          if(!m){ e.target.setCustomValidity('Use o formato dd/mm/aaaa'); return; }
          const dd=+m[1], mm=+m[2], yyyy=+m[3];
          const ok = mm>=1 && mm<=12 && dd>=1 && dd<=31 && yyyy>=1900 && yyyy<=new Date().getFullYear();
          e.target.setCustomValidity(ok?'':'Use o formato dd/mm/aaaa');
        });
      }
    })();

    // Normaliza DOB para ISO (dd/mm/aaaa -> aaaa-mm-dd)
    function normalizeDOB(dobStr){
      if (/^\d{2}\/\d{2}\/\d{4}$/.test(dobStr)) {
        const [dd,mm,yyyy] = dobStr.split('/');
        return `${yyyy}-${mm.padStart(2,'0')}-${dd.padStart(2,'0')}`;
      }
      return dobStr;
    }

    // Imagens → DataURL leve
    function fileToDataURL(file,maxW=1200,maxH=1600,quality=0.82){
      return new Promise(res=>{
        const fr=new FileReader();
        fr.onload=()=>{ const img=new Image(); img.onload=()=>{
          const ratio = Math.min(1, maxW/img.width, maxH/img.height);
          const w = Math.round(img.width*ratio), h = Math.round(img.height*ratio);
          const c=document.createElement('canvas'); c.width=w; c.height=h;
          c.getContext('2d').drawImage(img,0,0,w,h);
          res(c.toDataURL('image/jpeg',quality));
        }; img.src=fr.result; };
        fr.readAsDataURL(file);
      });
    }
    function bindPhoto(inputId, hiddenName, previewId){
      const input=document.getElementById(inputId), prev=document.getElementById(previewId);
      if(!input || !prev) return;
      input.addEventListener('change', async (e)=>{
        const f=e.target.files && e.target.files[0]; if(!f) return;
        const d=await fileToDataURL(f);
        const hidden=document.querySelector(`input[name="${hiddenName}"]`);
        if (hidden) hidden.value=d; prev.src=d; prev.classList.remove('hidden');
      });
    }
    bindPhoto('selfieFront','selfieFrontDataURL','previewFront');
    bindPhoto('selfieLeft','selfieLeftDataURL','previewLeft');
    bindPhoto('selfieRight','selfieRightDataURL','previewRight');

    // UTM & tech
    const params=new URLSearchParams(location.search);
    ['utm_source','utm_medium','utm_campaign','utm_content','utm_term'].forEach(k=>{
      const v=params.get(k); if(v){ const el=document.querySelector(`input[name="${k}"]`); if(el) el.value=v; }
    });
    const uaEl=document.querySelector('input[name="ua"]'); if(uaEl) uaEl.value=navigator.userAgent||'';

    // Dependências em mudanças
    document.addEventListener('change', e=>{
      if (!e.target || !e.target.name) return;
      if (['jaFez','alergiaMedicamentos','alergiasGerais','usaMedicamentos','anabolizantes','cirurgiaRecente','tabagismo','alcool','atividadeFisica'].includes(e.target.name)) applyDeps();
      if (e.target.id==='objetivoOutroChk') toggleObjetivoOutro();
    });
    // Estado inicial
    applyDeps(); toggleObjetivoOutro();

    // Validação & coleta
    function validate(formEl){
      if(!document.getElementById('lgpd').checked) return false;
      if($$('input[name="objetivos"]:checked').length===0) return false;

      const req=formEl.querySelectorAll('[required]');
      for(const r of req){
        if(r.type==='checkbox' && !r.checked) return false;
        if(r.type!=='checkbox' && (r.value||'').trim()==='') return false;
      }
      if ((formEl.querySelector('input[name="_hp"]')||{}).value) return false; // honeypot
      return true;
    }
    function collect(formEl){
      const data={};
      $$('input[type="text"]:not([disabled]),input[type="email"]:not([disabled]),input[type="tel"]:not([disabled]),input[type="date"]:not([disabled]),input[type="hidden"]:not([disabled]),textarea:not([disabled]),select:not([disabled])',formEl)
        .forEach(el=>{ if(el.name) data[el.name]= (el.value||'').trim(); });

      ['jaFez','jaPaciente','usaMedicamentos','alergiaMedicamentos','alergiasGerais','gestante','anabolizantes','cirurgiaRecente','tabagismo','alcool','atividadeFisica']
        .forEach(n=> data[n]=(document.querySelector(`input[name="${n}"]:checked`)||{}).value || '' );

      data.doencas        = $$('input[name="doencas"]:checked').map(el=>el.value);
      data.procInteresse  = $$('input[name="procInteresse"]:checked').map(el=>el.value);
      data.objetivos      = $$('input[name="objetivos"]:checked').map(el=>el.value);
      data.objetivoOutro  = (document.querySelector('textarea[name="objetivoOutro"]')||{}).value||'';

      // Normaliza data
      data.nascimento = normalizeDOB(data.nascimento || '');

      // Faixa de investimento opcional -> default se vazio
      const invest=(document.querySelector('input[name="faixaInvest"]:checked')||{}).value||'';
      data.faixaInvest = invest || 'Quero avaliar com a Dra.';

      data.lgpd=document.getElementById('lgpd').checked;
      return data;
    }

    // Feedback + submit
    const form=document.getElementById('form');
    const feedback=document.getElementById('feedback');
    const submitBtn=document.querySelector('button[type="submit"]');

    function showMsg(msg){ feedback.classList.remove('hidden'); feedback.textContent=msg; feedback.scrollIntoView({behavior:'smooth'}); }
    function withTimeout(promise, ms=12000){ return Promise.race([promise, new Promise((_,rej)=>setTimeout(()=>rej(new Error('Tempo esgotado')), ms))]); }

    form.addEventListener('submit', async (e)=>{
      e.preventDefault();
      if(!validate(form)){ showMsg('Revise: dados obrigatórios, LGPD e ao menos 1 objetivo.'); return; }

      const payload=collect(form);
      const body = new URLSearchParams({ secret: SECRET, payload: JSON.stringify(payload) });

      submitBtn.disabled = true; const prevTxt = submitBtn.textContent; submitBtn.textContent='Enviando…';
      showMsg('Enviando…');

      try{
        const res = await withTimeout(fetch(EXEC_URL, { method:'POST', headers:{'Content-Type':'application/x-www-form-urlencoded'}, body }), 12000);
        const data = await res.json();
        if(data.ok && data.whatsapp){ window.location.href = data.whatsapp; }
        else { showMsg('Houve um problema ao enviar. Tente novamente.'); }
      }catch(err){
        showMsg('Erro ao enviar: ' + err.message);
      }finally{
        submitBtn.disabled=false; submitBtn.textContent=prevTxt;
      }
    });
  </script>
</body>
</html>
