# jogo
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Nevair 67: O Segredo de Vera</title>
<style>
:root {
  --bg:#090812; --panel:#171426; --purple:#a78bfa;
  --pink:#ff72b6; --blue:#67d9ff; --text:#f5efff;
  --muted:#b8aecf; --gold:#ffd36e;
}
* { box-sizing:border-box; }
body {
  margin:0; min-height:100vh; color:var(--text);
  background:
    radial-gradient(ellipse at 50% -10%,#38205d 0%,transparent 55%),
    linear-gradient(140deg,#090812,#111526 70%,#1b0b20);
  font-family:system-ui,Arial,sans-serif;
}
button { font:inherit; cursor:pointer; }
header { text-align:center; padding:26px 14px 10px; }
h1 {
  margin:0; font-size:clamp(30px,6vw,58px);
  letter-spacing:-1px; color:#fff;
  text-shadow:0 0 12px #a855f7,0 0 35px #6d28d9;
}
.subtitle { color:var(--pink); font-weight:800; letter-spacing:3px; }
main { width:min(900px,94%); margin:15px auto 35px; }
.card {
  background:linear-gradient(145deg,#19162bdc,#100e1beF);
  border:1px solid #44345f; border-radius:18px;
  padding:clamp(16px,4vw,28px);
  box-shadow:0 18px 65px #0006;
}
#hero { text-align:center; }
.hero-art {
  border-radius:14px; min-height:155px; padding:24px 8px;
  background:linear-gradient(135deg,#211738,#30132f,#111b37);
  border:1px solid #59417b; margin:18px 0;
  overflow:hidden; position:relative;
}
.giant { font-size:clamp(46px,12vw,100px); line-height:1.1; }
.hero-art .caption { color:#e6cfff; }
.intro { color:#d2c8e7; line-height:1.8; text-align:left; }
.primary,.choice,.secondary {
  width:100%; border-radius:11px; padding:14px;
  margin-top:10px; font-weight:800; transition:.15s;
}
.primary {
  background:linear-gradient(100deg,#7c3aed,#c026d3);
  border:1px solid #d8b4fe; color:white;
}
.choice {
  text-align:left; background:#211c36;
  border:1px solid #4b3c68; color:var(--text);
}
.choice:hover { background:#34254e; border-color:var(--pink); transform:translateY(-1px); }
.secondary { background:#181729; border:1px solid #51456b; color:#d6c8ef; }
.primary:hover,.secondary:hover { filter:brightness(1.2); }
.topline {
  display:flex; flex-wrap:wrap; justify-content:space-between;
  gap:8px; margin-bottom:16px;
}
.pill {
  padding:7px 11px; border-radius:30px;
  background:#29213e; border:1px solid #51406c;
  font-size:12px; color:#e4d5ff;
}
.progress {
  height:8px; border-radius:20px; background:#2c2540;
  overflow:hidden; margin:12px 0 22px;
}
#bar { height:100%; width:0; background:linear-gradient(90deg,#a855f7,#ff72b6); transition:width .3s; }
.chapter { color:var(--pink); font-size:12px; font-weight:900; letter-spacing:2px; }
#storyTitle { font-size:clamp(24px,4vw,34px); margin:7px 0 15px; }
#storyText { font-size:16px; line-height:1.9; color:#e1d9f0; white-space:pre-line; }
.dialogue {
  border-left:3px solid var(--purple); padding:12px 15px;
  margin:18px 0; background:#211a32; border-radius:0 9px 9px 0;
  color:#f1ddff; font-style:italic; line-height:1.7;
}
#choices { margin-top:22px; }
#feedback { margin-top:16px; padding:13px; border-radius:10px; background:#19182c; color:#dfd4f4; line-height:1.6; }
.hidden { display:none !important; }
.stats { display:grid; grid-template-columns:repeat(3,1fr); gap:8px; margin:14px 0; }
.stat { background:#211c36; border-radius:10px; padding:10px; text-align:center; }
.stat strong { display:block; color:var(--gold); font-size:20px; }
.stat span { color:var(--muted); font-size:11px; }
.meme {
  text-align:center; margin:18px 0 4px; color:#9b91b6;
  font-size:12px; letter-spacing:2px;
}
#ending { text-align:center; }
#endingTitle { color:var(--gold); font-size:clamp(26px,5vw,42px); }
#endingText { line-height:1.9; color:#e1d9f0; white-space:pre-line; }
.achievement { color:#ffb5df; border:1px dashed #80518c; padding:13px; border-radius:10px; margin:18px 0; }
footer { text-align:center; color:#726a8b; padding:0 12px 25px; font-size:12px; }
@media(max-width:500px) {
  .stats { grid-template-columns:1fr 1fr; }
  .stats .stat:last-child { grid-column:span 2; }
}
</style>
</head>
<body>
<header>
  <div class="subtitle">UMA INVESTIGAÇÃO ABSURDAMENTE SUSPEITA</div>
  <h1>NEVAIR 67</h1>
  <p style="color:#c7b7e8;margin-top:5px">O Segredo de Vera</p>
</header>

<main>
<section id="hero" class="card">
  <div class="hero-art">
    <div class="giant">🥛 👁️ 67</div>
    <div class="caption">UMA MENSAGEM. UMA MANSÃO. UMA MULHER COLOSSAL.</div>
  </div>
  <h2>O caso que ninguém deveria investigar.</h2>
  <p class="intro">
    03:07 da madrugada. Nevair recebe uma mensagem de um número desconhecido:
    <br><br><strong>“Eu sei o que você fez com o 67. Vera também sabe.”</strong>
    <br><br>
    Dez minutos depois, ele está diante de uma mansão que não aparece em nenhum mapa.
    Lá dentro, alguém conhece todos os seus segredos. E, aparentemente, alguém comprou
    leite suficiente para abastecer uma cidade inteira.
    <br><br>
    São <strong>40 decisões</strong>. Suas escolhas alteram as pistas, a confiança dos
    personagens e suas chances contra a chefe final. Nem toda decisão tem uma resposta óbvia.
  </p>
  <button class="primary" id="startBtn">ENTRAR NA MANSÃO →</button>
  <button class="secondary" id="continueBtn">Continuar jogo salvo</button>
  <p class="meme">NEVAIR 67 • A LORE É REAL (FONTE: CONFIA)</p>
</section>

<section id="game" class="card hidden">
  <div class="topline">
    <span class="pill" id="stepLabel">DECISÃO 1/40</span>
    <span class="pill" id="moodLabel">CLIMA: SUSPEITO</span>
  </div>
  <div class="progress"><div id="bar"></div></div>
  <div class="chapter" id="chapter"></div>
  <h2 id="storyTitle"></h2>
  <div id="storyText"></div>
  <div id="dialogue" class="dialogue"></div>
  <div class="stats">
    <div class="stat"><strong id="clueStat">0</strong><span>PISTAS</span></div>
    <div class="stat"><strong id="nerveStat">0</strong><span>CORAGEM</span></div>
    <div class="stat"><strong id="trustStat">0</strong><span>CONFIANÇA</span></div>
  </div>
  <div id="choices"></div>
  <div id="feedback" class="hidden"></div>
  <button id="nextBtn" class="primary hidden">PRÓXIMA CENA →</button>
  <button id="saveBtn" class="secondary">Salvar progresso</button>
  <button id="quitBtn" class="secondary">Voltar ao início</button>
  <div class="meme">SUSPEITO • SUSPEITÍSSIMO • NEVAIR 67</div>
</section>

<section id="ending" class="card hidden">
  <div class="giant">🏆</div>
  <h2 id="endingTitle"></h2>
  <p id="endingText"></p>
  <div class="stats">
    <div class="stat"><strong id="endClues"></strong><span>PISTAS</span></div>
    <div class="stat"><strong id="endNerve"></strong><span>CORAGEM</span></div>
    <div class="stat"><strong id="endTrust"></strong><span>CONFIANÇA</span></div>
  </div>
  <div class="achievement" id="achievement"></div>
  <button class="primary" id="restartBtn">JOGAR DE NOVO</button>
  <button class="secondary" id="menuBtn">VOLTAR AO INÍCIO</button>
</section>
</main>
<footer>NEVAIR 67: O SEGREDO DE VERA — Edição interativa 1.0</footer>

<script>
"use strict";

const $ = id => document.getElementById(id);
const SAVE_KEY = "nevair67_save_v1";

const scenes = [
{
chapter:"CAPÍTULO I — A MENSAGEM",
title:"Decisão 1 — O número desconhecido",
text:"Seu celular vibra às 03:07. Uma mensagem sem foto diz: “Venha sozinho. Traga o 67.” Você não faz ideia do que é o 67. O mais estranho: o remetente sabe seu nome completo.",
dialogue:"Nevair: “Isso é golpe, convite pra festa ou o início de um documentário criminal?”",
options:[
["Responder: “Quem é você?”", "Você recebe apenas uma localização e um emoji de vaca. Péssimo sinal.",{clue:1,trust:1}],
["Bloquear e dormir", "O celular toca mesmo bloqueado. A mensagem agora diz: “Boa tentativa.”",{nerve:1}],
["Mandar um áudio imitando um pato", "O remetente responde com outro pato. Você ganhou um inimigo ou um melhor amigo.",{trust:1}]
]},
{
chapter:"CAPÍTULO I — A MENSAGEM",title:"Decisão 2 — O pacote",
text:"Na porta da sua casa há uma caixa. Dentro: um mapa, uma chave e um bilhete escrito com caneta roxa. O bilhete tem apenas dois números: 6 e 7.",
dialogue:"Bilhete: “Não confie na pessoa que parece estar ajudando.”",
options:[
["Examinar a caixa com cuidado","Há uma marca de entrega: Mansão V. Você guarda a etiqueta.",{clue:2}],
["Levar tudo sem olhar","Você pega o pacote. Um barulho estranho vem de dentro, mas provavelmente é só a sua imaginação.",{nerve:1}],
["Deixar a caixa na calçada","Quando olha de novo, a caixa desapareceu. A chave, porém, está no seu bolso.",{trust:-1,clue:1}]
]},
{
chapter:"CAPÍTULO I — A MENSAGEM",title:"Decisão 3 — A viagem",
text:"A mansão fica no fim de uma estrada cercada por árvores. O GPS recalcula a rota sozinho e passa a mostrar: “FALTAM 67 METROS”. A placa da estrada está virada ao contrário.",
dialogue:"GPS: “Em 600 metros, vire na direção das suas decisões ruins.”",
options:[
["Seguir o GPS","Você chega à entrada principal, mas sente que alguém já esperava por você.",{clue:1}],
["Estacionar e observar","Você vê uma silhueta enorme passando atrás das cortinas.",{clue:2,nerve:1}],
["Voltar para casa","A estrada faz um círculo e devolve você ao mesmo portão. O jogo começou.",{nerve:1}]
]},
{
chapter:"CAPÍTULO I — A MENSAGEM",title:"Decisão 4 — O portão",
text:"O portão tem um teclado com quatro dígitos. Ao lado, uma placa diz: “O dobro de 33, menos um.” Há marcas de dedos no botão 6.",
dialogue:"Nevair: “Se isso for uma prova de matemática, eu quero meu dinheiro de volta.”",
options:[
["Digitar 65","O teclado apita vermelho. A placa parece ter sido alterada recentemente.",{clue:1}],
["Digitar 66","O portão abre. Um alto-falante sussurra: “Interessante...”",{clue:2,nerve:1}],
["Digitar 67","O portão abre imediatamente. Alguém colocou um adesivo “67 MOMENT” no teclado.",{clue:1,trust:1}]
]},
{
chapter:"CAPÍTULO I — A MENSAGEM",title:"Decisão 5 — A recepção",
text:"No saguão há três portas: BIBLIOTECA, COZINHA e NÃO ENTRE. Um retrato de uma mulher enorme domina a parede. Os olhos do retrato parecem acompanhar você.",
dialogue:"Voz no interfone: “A casa é sua. Por enquanto.”",
options:[
["Ir à biblioteca","Você encontra um diário com páginas arrancadas.",{clue:2}],
["Ir à cozinha","Há dezenas de caixas de leite e um bolo escrito “BEM-VINDO, NEVAIR”.",{trust:1}],
["Abrir a porta NÃO ENTRE","Do outro lado há apenas uma parede. Alguém riu pelo interfone.",{nerve:1}]
]},
{
chapter:"CAPÍTULO II — A MANSÃO",title:"Decisão 6 — O diário",
text:"O diário pertence a um antigo funcionário. Ele descreve uma festa interrompida por um apagão. Na última página legível: “Vera não quer o 67. Ela quer saber quem o escondeu.”",
dialogue:"Nevair: “O problema é que eu nem sei o que é o 67!”",
options:[
["Fotografar as páginas","A foto revela uma assinatura escondida sob a tinta.",{clue:2}],
["Arrancar a página final","O papel se desfaz e revela um símbolo de estrela.",{clue:1,nerve:1}],
["Devolver tudo exatamente como estava","Você ouve passos se afastando no andar superior.",{trust:1}]
]},
{
chapter:"CAPÍTULO II — A MANSÃO",title:"Decisão 7 — O retrato",
text:"O retrato tem uma pequena placa: VERA V. VALENÇA. A moldura está quente. No verso, alguém escreveu: “A altura dela não é o que torna Vera assustadora.”",
dialogue:"Uma risada ecoa pelo corredor. Parece vir de dentro da parede.",
options:[
["Investigar a moldura","Você encontra um compartimento com um cartão de acesso.",{clue:2}],
["Falar com o retrato","O retrato não responde. Ainda assim, você pede desculpas por interromper.",{trust:1}],
["Derrubar o retrato","Atrás dele há uma câmera. Uma luz vermelha acende.",{nerve:1,clue:1}]
]},
{
chapter:"CAPÍTULO II — A MANSÃO",title:"Decisão 8 — O funcionário",
text:"Um homem de uniforme aparece com uma bandeja vazia. Ele se apresenta como Cláudio e afirma que trabalha ali há vinte anos. Seu crachá, porém, diz “ESTAGIÁRIO — DIA 1”.",
dialogue:"Cláudio: “A empresa mudou de nome. O RH ainda não mudou de realidade.”",
options:[
["Perguntar sobre Vera","Cláudio empalidece e aponta para o elevador.",{clue:1,trust:1}],
["Perguntar pelo 67","Ele deixa cair uma pequena chave antes de fugir.",{clue:2}],
["Fingir que acredita","Cláudio sorri, aliviado por você não perguntar sobre o salário.",{trust:2}]
]},
{
chapter:"CAPÍTULO II — A MANSÃO",title:"Decisão 9 — O elevador",
text:"O elevador tem botões para os andares 1, 2, 6 e 7. Não existe andar 3, 4 ou 5. Um bilhete no painel diz: “Suba quando estiver pronto para ouvir a verdade.”",
dialogue:"Elevador: “Peso máximo: 700 kg.” A placa parece uma provocação.",
options:[
["Apertar 6 e depois 7","O elevador desce primeiro, embora você tenha pedido para subir.",{clue:1}],
["Apertar 7","As portas se fecham e uma voz pergunta: “Você trouxe o leite?”",{nerve:1}],
["Procurar uma escada","Você encontra uma escada de serviço e uma câmera quebrada.",{clue:2}]
]},
{
chapter:"CAPÍTULO II — A MANSÃO",title:"Decisão 10 — O primeiro arquivo",
text:"Uma sala de arquivos contém contratos, fotos e um envelope lacrado. Há registros de uma empresa chamada VERA 67, encerrada oficialmente há dez anos — mas com pagamentos feitos ontem.",
dialogue:"Nevair: “Empresa encerrada recebendo dinheiro? Até o contador desse lugar é suspeito.”",
options:[
["Abrir o envelope","Dentro há uma foto de Nevair entrando na mansão, tirada antes de ele chegar.",{clue:3,nerve:-1}],
["Copiar os registros","Você fotografa os pagamentos e guarda as datas.",{clue:2}],
["Fechar tudo e sair","O arquivo fecha sozinho. Um recibo cai do teto.",{trust:1}]
]},
{
chapter:"CAPÍTULO III — O SEGREDO",title:"Decisão 11 — A voz no rádio",
text:"Um rádio velho liga sozinho. Uma mulher diz: “Nevair, se você está ouvindo, não confie em Cláudio.” Em seguida, outra voz repete exatamente a mesma frase, com um segundo de atraso.",
dialogue:"Rádio: “O segredo não é quem mente. É quem precisa que você acredite.”",
options:[
["Gravar a transmissão","Você consegue salvar um trecho com um código de fundo.",{clue:2}],
["Responder ao rádio","A voz pergunta qual é o seu maior medo.",{trust:1}],
["Desligar da tomada","O rádio continua funcionando por mais três segundos.",{nerve:1}]
]},
{
chapter:"CAPÍTULO III — O SEGREDO",title:"Decisão 12 — O corredor das fotos",
text:"Há 67 fotografias de festas antigas. Em todas, Vera aparece de costas. Em uma delas, porém, o espelho mostra o rosto dela: ela está olhando diretamente para a câmera.",
dialogue:"Nevair: “Isso não é um álbum de família. É um álbum de evidências.”",
options:[
["Contar as fotos","São 67 mesmo. No verso da última, há uma data.",{clue:2}],
["Queimar o álbum","O alarme dispara. Você sente que acabou de destruir uma pista importante.",{nerve:1,clue:-1}],
["Levar uma fotografia","Você encontra uma impressão digital no canto.",{clue:1}]
]},
{
chapter:"CAPÍTULO III — O SEGREDO",title:"Decisão 13 — O celular de Cláudio",
text:"Um celular vibra embaixo de um sofá. A tela está aberta numa conversa: “Ela descobriu o arquivo. Se ele chegar à sala 67, acabou.”",
dialogue:"Última mensagem recebida: “A festa começa quando as luzes apagam.”",
options:[
["Ler a conversa inteira","Você encontra uma mensagem apagada parcialmente: “Vera não está sozinha.”",{clue:3}],
["Entregar o celular a Cláudio","Ele agradece rápido demais e sai sem olhar para trás.",{trust:2}],
["Desligar o aparelho","Uma notificação aparece: “Dispositivo rastreado.”",{nerve:1}]
]},
{
chapter:"CAPÍTULO III — O SEGREDO",title:"Decisão 14 — O mapa rasgado",
text:"Um mapa da mansão tem um pedaço faltando. A parte restante indica uma sala escondida atrás da cozinha. A marcação parece uma estrela de cinco pontas.",
dialogue:"Nevair: “Ou isso é uma passagem secreta ou alguém desenha mapas muito mal.”",
options:[
["Juntar o mapa ao símbolo do diário","Os símbolos coincidem. Você descobre a localização da passagem.",{clue:3}],
["Seguir o mapa sem conferir","Você chega a um armário cheio de vassouras.",{nerve:1}],
["Pedir ajuda pelo rádio","A voz responde com coordenadas, mas não explica como as conhece.",{trust:1,clue:1}]
]},
{
chapter:"CAPÍTULO III — O SEGREDO",title:"Decisão 15 — A sala escondida",
text:"A passagem leva a uma sala com monitores. Um deles mostra a entrada da mansão. Outro mostra o corredor em que você está. O terceiro mostra você... antes de entrar na sala.",
dialogue:"Tela: “SUJEITO IDENTIFICADO: NEVAIR. STATUS: ESPERADO.”",
options:[
["Desconectar os monitores","Você interrompe a transmissão e encontra um cartão magnético.",{clue:2,nerve:1}],
["Procurar o gravador","Um vídeo revela Vera discutindo com uma pessoa fora de quadro.",{clue:3}],
["Ficar observando","Uma câmera gira lentamente na sua direção.",{nerve:1}]
]},
{
chapter:"CAPÍTULO III — O SEGREDO",title:"Decisão 16 — O vídeo",
text:"No vídeo, Vera diz: “O 67 nunca foi um objeto. Foi um acordo.” A pessoa fora de quadro responde: “Então por que você construiu tudo isso?” O vídeo termina antes da resposta.",
dialogue:"Nevair: “Um acordo? Eu assinei alguma coisa? Eu nem leio os termos de uso!”",
options:[
["Procurar o contrato","Você acha um documento com uma assinatura muito parecida com a sua.",{clue:3}],
["Rebobinar o vídeo","No reflexo do vidro aparece Cláudio, escondido atrás de Vera.",{clue:2}],
["Apagar o vídeo","A tela apaga, mas uma impressora começa a funcionar.",{nerve:1}]
]},
{
chapter:"CAPÍTULO IV — A TRAIÇÃO",title:"Decisão 17 — O contrato",
text:"O contrato menciona um experimento social chamado PROJETO 67. O objetivo era descobrir quanto tempo uma pessoa levaria para desconfiar de todos ao seu redor. Seu nome aparece como participante.",
dialogue:"Nevair: “Eu participei de um experimento sem saber? Isso é um reality show ou um processo judicial?”",
options:[
["Guardar o contrato","Agora você tem uma prova concreta do projeto.",{clue:3}],
["Rasgar o contrato","Você perde uma evidência, mas encontra uma segunda folha escondida.",{clue:1,nerve:1}],
["Assinar a última página","A tinta muda de cor. A assinatura já estava lá antes.",{nerve:1}]
]},
{
chapter:"CAPÍTULO IV — A TRAIÇÃO",title:"Decisão 18 — A ligação",
text:"Seu telefone toca. Cláudio está do outro lado: “Eu tentei avisar. Vera não criou o projeto. Ela foi a primeira cobaia.” A ligação cai.",
dialogue:"Mensagem de voz automática: “Para ouvir novamente, pressione 67.”",
options:[
["Ligar de volta","Cláudio atende e diz para você procurar o porão.",{trust:2}],
["Verificar a origem da chamada","O número pertence à própria mansão.",{clue:2}],
["Ignorar a ligação","Você ouve três batidas na porta da sala.",{nerve:1}]
]},
{
chapter:"CAPÍTULO IV — A TRAIÇÃO",title:"Decisão 19 — O porão",
text:"O porão tem uma porta de metal e uma placa: “NÃO É UMA PRISÃO”. Do outro lado, alguém arrasta algo pesado. O som para quando você respira.",
dialogue:"Voz desconhecida: “Se você entrou, já escolheu um lado.”",
options:[
["Abrir a porta devagar","Você encontra arquivos de funcionários desaparecidos da empresa.",{clue:3,nerve:1}],
["Bater e se identificar","Uma pessoa responde: “Nevair? Finalmente.”",{trust:1}],
["Procurar outra entrada","Você descobre uma grade de ventilação e um corredor estreito.",{clue:2}]
]},
{
chapter:"CAPÍTULO IV — A TRAIÇÃO",title:"Decisão 20 — A pessoa na cela",
text:"Uma mulher de uniforme está sentada atrás de uma grade. Ela se chama Lúcia e afirma ter trabalhado no Projeto 67. Ela diz que Vera está preparando uma apresentação para esta noite.",
dialogue:"Lúcia: “Ela não quer te matar. Quer que você aceite a versão dela da história.”",
options:[
["Acreditar em Lúcia","Ela entrega um código de acesso e pede que você não conte a Cláudio.",{trust:2,clue:1}],
["Exigir provas","Ela revela uma fotografia de Vera ao lado de Cláudio, anos atrás.",{clue:3}],
["Libertá-la sem perguntas","Lúcia foge e deixa cair um crachá de segurança.",{nerve:1,trust:1}]
]},
{
chapter:"CAPÍTULO V — A VERDADE",title:"Decisão 21 — A sala 67",
text:"A porta da sala 67 tem três fechaduras: uma eletrônica, uma mecânica e uma que parece não ter chave. Você ouve música de festa lá dentro.",
dialogue:"Alguém canta baixinho: “Six... seven...” A música para quando você se aproxima.",
options:[
["Usar o cartão magnético","A primeira fechadura abre e o sistema registra sua entrada.",{clue:1}],
["Usar a chave do pacote","A segunda fechadura abre com um clique seco.",{clue:1,trust:1}],
["Examinar a fechadura estranha","Ela responde ao símbolo de estrela do mapa.",{clue:3}]
]},
{
chapter:"CAPÍTULO V — A VERDADE",title:"Decisão 22 — A festa vazia",
text:"Dentro há uma mesa posta para 67 pessoas, mas nenhuma cadeira está ocupada. No centro, uma televisão exibe uma contagem regressiva de 67 minutos.",
dialogue:"Tela: “PARTICIPANTE PRINCIPAL: NEVAIR. CONVIDADA DE HONRA: VERA.”",
options:[
["Examinar os lugares","Cada prato tem o nome de uma pessoa ligada ao projeto.",{clue:2}],
["Desligar a televisão","O cronômetro continua, agora refletido no espelho.",{nerve:1}],
["Sentar na cadeira principal","Um mecanismo liga a luz do palco. Você virou o protagonista.",{trust:1}]
]},
{
chapter:"CAPÍTULO V — A VERDADE",title:"Decisão 23 — A gravação de Vera",
text:"A televisão muda para uma gravação. Vera aparece em uma sala branca: “Eu sei que pareço o monstro dessa história. Talvez eu seja. Mas alguém precisava terminar o experimento.”",
dialogue:"Vera, na gravação: “A questão não é o que é o 67. É quem ganha quando todos acreditam nele.”",
options:[
["Ouvir até o fim","A gravação revela que o experimento foi financiado por uma empresa secreta.",{clue:3}],
["Interromper a gravação","Uma porta lateral se abre, mas você perde parte da explicação.",{nerve:1}],
["Responder à tela","O microfone está ativo. Uma voz diz: “Ela ouviu você.”",{trust:1}]
]},
{
chapter:"CAPÍTULO V — A VERDADE",title:"Decisão 24 — O arquivo financeiro",
text:"Uma gaveta contém transferências milionárias para uma organização chamada Instituto Sete. O último pagamento foi feito ontem. O destinatário: “V. Valença — manutenção do experimento”.",
dialogue:"Nevair: “Manutenção do experimento? O laboratório tem plano de assinatura?”",
options:[
["Fotografar os comprovantes","Você registra valores, datas e o nome do banco.",{clue:3}],
["Levar a pasta inteira","A pasta pesa tanto que parece conter todos os pecados fiscais do país.",{nerve:1,clue:1}],
["Procurar o responsável","Uma assinatura aparece: Cláudio.",{clue:2}]
]},
{
chapter:"CAPÍTULO V — A VERDADE",title:"Decisão 25 — A confissão de Cláudio",
text:"Cláudio surge na porta. Ele admite ter trabalhado para Vera, mas diz que mudou de lado quando percebeu que o Projeto 67 estava sendo usado para manipular pessoas de fora.",
dialogue:"Cláudio: “Eu menti sobre o crachá. Não menti sobre a empresa. Na verdade, eu menti sobre as duas coisas.”",
options:[
["Exigir a história completa","Cláudio conta que a sala final só abre com três provas.",{clue:3,trust:1}],
["Não confiar nele","Você mantém distância e anota cada contradição.",{clue:1,nerve:1}],
["Aceitar a ajuda dele","Ele entrega uma ferramenta capaz de abrir portas eletrônicas.",{trust:3}]
]},
{
chapter:"CAPÍTULO VI — SEM VOLTA",title:"Decisão 26 — O corredor vermelho",
text:"As luzes ficam vermelhas. Uma sirene anuncia: “VISITANTE NÃO AUTORIZADO NA ZONA V”. O chão começa a vibrar. No fim do corredor há uma porta enorme.",
dialogue:"Alto-falante: “A apresentação começará em breve. Por favor, mantenham a calma.”",
options:[
["Correr para a porta","Você passa antes que as travas se fechem.",{nerve:2}],
["Desligar o alarme","O silêncio volta, mas uma câmera acompanha seus passos.",{clue:2}],
["Se esconder atrás de um armário","Uma equipe passa sem notar você. Seu orgulho sofre um pouco.",{trust:1}]
]},
{
chapter:"CAPÍTULO VI — SEM VOLTA",title:"Decisão 27 — O teste de coragem",
text:"Uma sala exige que você escolha entre duas alavancas. Uma abre a passagem; a outra liga um holofote que ilumina a sala inteira. Uma inscrição diz: “A resposta está no que você já viu.”",
dialogue:"Nevair: “Eu já vi muita coisa. Inclusive o preço do leite. Nada me prepara pra isso.”",
options:[
["Acionar a alavanca marcada com estrela","O símbolo coincide com o mapa. A passagem abre.",{clue:2}],
["Acionar a alavanca sem marca","O holofote acende e revela pegadas que levam à saída.",{nerve:2}],
["Esperar e observar","Um padrão de luzes mostra a sequência correta.",{clue:3}]
]},
{
chapter:"CAPÍTULO VI — SEM VOLTA",title:"Decisão 28 — O laboratório",
text:"O laboratório está vazio, exceto por uma máquina com um visor: “67”. Há três botões — MEMÓRIA, MEDO e VERDADE. O manual foi arrancado.",
dialogue:"Uma voz digital: “Para continuar, escolha o que você está disposto a perder.”",
options:[
["Pressionar VERDADE","A máquina imprime uma foto de Vera muito mais jovem.",{clue:3}],
["Pressionar MEMÓRIA","Você recupera uma lembrança da festa que nunca recordou.",{trust:1,clue:2}],
["Pressionar MEDO","As luzes apagam. Quando voltam, a porta está aberta.",{nerve:2}]
]},
{
chapter:"CAPÍTULO VI — SEM VOLTA",title:"Decisão 29 — A lembrança",
text:"A memória mostra você numa sala de testes, assinando um formulário. Você não lembra de ter estado ali. Na gravação, alguém pergunta: “Você aceita participar?” E uma voz idêntica à sua responde: “Aceito.”",
dialogue:"Nevair: “Isso parece eu. Mas eu jamais usaria essa camisa.”",
options:[
["Aceitar que a memória é real","A imagem fica nítida. Você lembra do símbolo no formulário.",{clue:3,trust:1}],
["Considerar que pode ser falsa","Você procura cortes e falhas na gravação.",{clue:2,nerve:1}],
["Destruir o projetor","A gravação some, mas você encontra um cartão atrás do aparelho.",{nerve:2}]
]},
{
chapter:"CAPÍTULO VI — SEM VOLTA",title:"Decisão 30 — A terceira prova",
text:"A porta final exige três provas: o contrato, a gravação e o símbolo da estrela. Você confere o que reuniu. Atrás da porta, passos pesados fazem o chão tremer.",
dialogue:"Voz feminina: “Nevair. Espero que tenha trazido boas perguntas.”",
options:[
["Reunir as provas com calma","Você organiza as evidências e identifica uma contradição no contrato.",{clue:3}],
["Arrombar a porta","A porta abre, mas o alarme anuncia sua presença.",{nerve:2}],
["Tentar negociar pelo interfone","A voz responde: “Você já está negociando.”",{trust:1}]
]},
{
chapter:"CAPÍTULO VII — VERA",title:"Decisão 31 — A primeira aparição",
text:"As portas se abrem. Vera está no centro de um salão gigantesco. Ela é colossal, quase toca o lustre, e sua sombra cobre metade do chão. O salto de suas botas faz os quadros tremerem.",
dialogue:"Vera: “Finalmente, Nevair. Você demorou 67 minutos. Eu esperava mais pontualidade.”",
options:[
["Manter a postura e fazer perguntas","Você não demonstra medo. Vera parece genuinamente interessada.",{nerve:2,trust:1}],
["Recuar e observar o salão","Você identifica três painéis de controle atrás dela.",{clue:2}],
["Gritar “NEVAIR 67!” como um meme","O eco dura tanto que parece ter sido renderizado em câmera lenta.",{nerve:1,trust:-1}]
]},
{
chapter:"CAPÍTULO VII — VERA",title:"Decisão 32 — O tamanho do problema",
text:"Vera dá um passo. O lustre balança. Ela se inclina para ouvir você, e o salão inteiro escurece com a sombra dela. Um letreiro anuncia: “CHEFE FINAL — FASE 1”.",
dialogue:"Vera: “Você imaginou um monstro. Eu sou apenas a pessoa que ficou quando todos fugiram.”",
options:[
["Estudar o ritmo dos passos dela","Você percebe que ela sempre pausa após três passos.",{clue:3}],
["Tentar correr para a porta lateral","Vera bloqueia o caminho com uma mão, sem esforço.",{nerve:1}],
["Perguntar por que ela é tão gigantesca","Vera olha para o teto: “E ainda assim construíram um lustre baixo.”",{trust:1}]
]},
{
chapter:"CAPÍTULO VII — VERA",title:"Decisão 33 — A arena",
text:"O salão se transforma. Painéis sobem do chão, formando plataformas e passagens. Vera sorri. “Vamos ver se você sabe usar o que descobriu.” Você tem pouco tempo para escolher uma rota.",
dialogue:"Sistema: “FASE 1: SOBREVIVÊNCIA. FASE 2: CONSEQUÊNCIAS.”",
options:[
["Usar os painéis para se esconder","Você alcança uma plataforma com visão de todo o salão.",{clue:2,nerve:1}],
["Desafiar Vera diretamente","Ela dá uma risada tão forte que o microfone estoura.",{nerve:3}],
["Procurar os controles da arena","Você encontra um console que responde ao símbolo da estrela.",{clue:3}]
]},
{
chapter:"CAPÍTULO VII — VERA",title:"Decisão 34 — A verdade sobre o 67",
text:"No console, você descobre o arquivo original: o Projeto 67 media a capacidade de uma pessoa de distinguir confiança real de manipulação. Vera era a cobaia principal. Nevair era o participante que deveria encerrar o experimento.",
dialogue:"Vera: “Você não veio me derrotar. Veio decidir se tudo isso deve continuar.”",
options:[
["Expor os resultados publicamente","Você prepara uma cópia dos arquivos para enviar ao mundo.",{clue:3,trust:2}],
["Apagar o projeto para sempre","Você desativa parte do sistema, mas perde provas importantes.",{nerve:2,clue:-1}],
["Perguntar quem financiou tudo","Vera revela que os patrocinadores ainda estão assistindo.",{clue:3}]
]},
{
chapter:"CAPÍTULO VII — VERA",title:"Decisão 35 — A proposta",
text:"Vera oferece um acordo: você pode sair com as provas ou ficar e descobrir quem financiou o projeto. Ela afirma que só uma dessas escolhas impede que o experimento seja repetido.",
dialogue:"Vera: “Eu não preciso que você goste de mim. Preciso saber se você consegue pensar.”",
options:[
["Escolher sair com as provas","Você mantém a evidência e Vera não tenta impedir sua saída.",{trust:2,clue:1}],
["Ficar para descobrir os financiadores","Você se compromete a ir até o fim, custe o que custar.",{clue:3,nerve:1}],
["Fingir que aceita o acordo","Você ganha tempo para examinar o console.",{clue:2,nerve:2}]
]},
{
chapter:"CAPÍTULO VIII — A ÚLTIMA FASE",title:"Decisão 36 — O ataque colossal",
text:"Vera bate o pé no chão. A arena treme e uma onda de ar atravessa o salão. Você precisa escolher como evitar o próximo movimento dela.",
dialogue:"Vera: “Vamos parar de conversar?” Nevair: “Eu estava começando a gostar da conversa!”",
options:[
["Usar a rota dos painéis","Você evita o impacto e encontra uma saída para a sala de controle.",{nerve:2,clue:1}],
["Distrair Vera com uma pergunta","Ela hesita por um instante, surpresa com sua audácia.",{trust:1,nerve:1}],
["Tentar enfrentar a força dela","Você não consegue movê-la nem um centímetro. A física venceu.",{nerve:1,trust:-1}]
]},
{
chapter:"CAPÍTULO VIII — A ÚLTIMA FASE",title:"Decisão 37 — O código final",
text:"A sala de controle exige um código. As pistas apontam para o número 67, mas o sistema pede quatro dígitos. Uma anotação diz: “Não use o número. Use a razão.”",
dialogue:"Terminal: “Pense no dobro de 67 e acrescente dois.”",
options:[
["Digitar 0136","O terminal confirma. O sistema entra em modo de encerramento.",{clue:3}],
["Digitar 0067","O sistema rejeita a resposta, mas revela uma pista adicional.",{clue:1}],
["Desconectar o terminal","A máquina reinicia e exige que você resolva um enigma alternativo.",{nerve:2}]
]},
{
chapter:"CAPÍTULO VIII — A ÚLTIMA FASE",title:"Decisão 38 — O último aliado",
text:"Cláudio aparece no comunicador. “Posso abrir a porta de emergência, mas só uma vez. Se você sair agora, os arquivos continuam aqui. Se ficar, pode derrubar tudo.”",
dialogue:"Cláudio: “Eu devia ter contado a verdade antes. Talvez ainda dê para fazer uma coisa certa.”",
options:[
["Confiar em Cláudio","Ele abre a rota de emergência e mantém os arquivos seguros.",{trust:3}],
["Exigir que ele prove sua lealdade","Cláudio envia uma cópia assinada dos arquivos.",{clue:2,trust:1}],
["Desligar o comunicador","Você segue sozinho. A decisão é sua e de mais ninguém.",{nerve:2}]
]},
{
chapter:"CAPÍTULO VIII — A ÚLTIMA FASE",title:"Decisão 39 — A escolha de Vera",
text:"Vera está diante do console principal. Pela primeira vez, parece cansada. “Se você desligar o sistema, eu perco a única coisa que me restou. Se não desligar, outra pessoa será usada.”",
dialogue:"Vera: “O monstro dessa história pode ser eu. Mas quem construiu a jaula?”",
options:[
["Oferecer uma saída para Vera","Você propõe expor os financiadores e encerrar o projeto sem apagar as provas.",{trust:3,clue:1}],
["Desligar o sistema imediatamente","O painel começa a apagar os dados. Você precisa agir rápido.",{nerve:2}],
["Exigir que Vera confesse tudo","Ela olha para a câmera e começa a narrar os crimes do projeto.",{clue:3,trust:1}]
]},
{
chapter:"CAPÍTULO IX — O FIM",title:"Decisão 40 — O destino do 67",
text:"A contagem regressiva chega a 00:67 — um erro impossível, ou uma última piada de quem criou o sistema. Vera espera sua decisão. O console oferece três opções: PUBLICAR, DESTRUIR ou TRANSFERIR.",
dialogue:"Nevair: “Quarenta decisões. Uma mulher gigante. Uma conspiração. E eu ainda não sei quem pagou o leite.”",
options:[
["PUBLICAR — revelar tudo","Você envia as provas e expõe o Projeto 67. O mundo inteiro começa a fazer perguntas.",{clue:3,trust:2}, "publicar"],
["DESTRUIR — encerrar o experimento","O sistema se apaga. Você impede a repetição do teste, mas algumas respostas desaparecem.",{nerve:3}, "destruir"],
["TRANSFERIR — tomar controle do sistema","Você assume o controle do Projeto 67. A última tela pergunta: “Tem certeza de que você é diferente?”",{clue:1,nerve:2,trust:-1}, "transferir"]
]}
];

let state = null;

function newState() {
  return {
    step:0, clues:0, nerve:0, trust:0,
    history:[], selectedEnding:null
  };
}

function showScreen(id) {
  ["hero","game","ending"].forEach(name=>$(name).classList.toggle("hidden",name!==id));
}

function startNew() {
  state=newState();
  showScreen("game");
  renderScene();
  saveGame();
}

function renderScene() {
  if(!state || state.step>=scenes.length) { finishGame(); return; }
  const s=scenes[state.step];
  $("stepLabel").textContent=`DECISÃO ${state.step+1}/40`;
  $("moodLabel").textContent=
    state.nerve>=8?"CLIMA: CAOS ABSOLUTO":
    state.clues>=8?"CLIMA: INVESTIGAÇÃO":
    state.trust>=6?"CLIMA: ALIANÇAS SUSPEITAS":"CLIMA: SUSPEITO";
  $("bar").style.width=(state.step/scenes.length*100)+"%";
  $("chapter").textContent=s.chapter;
  $("storyTitle").textContent=s.title;
  $("storyText").textContent=s.text;
  $("dialogue").textContent=s.dialogue;
  $("clueStat").textContent=state.clues;
  $("nerveStat").textContent=state.nerve;
  $("trustStat").textContent=state.trust;
  $("feedback").classList.add("hidden");
  $("nextBtn").classList.add("hidden");
  const box=$("choices");
  box.innerHTML="";
  s.options.forEach((opt,index)=>{
    const b=document.createElement("button");
    b.className="choice";
    b.textContent=String.fromCharCode(65+index)+") "+opt[0];
    b.addEventListener("click",()=>choose(index));
    box.appendChild(b);
  });
  $("saveBtn").textContent="Salvar progresso";
}

function choose(index) {
  if(!state || state.step>=scenes.length) return;
  const scene=scenes[state.step];
  const opt=scene.options[index];
  if(!opt)return;
  const effect=opt[2]||{};
  state.clues=Math.max(0,state.clues+(effect.clue||0));
  state.nerve=Math.max(0,state.nerve+(effect.nerve||0));
  state.trust=Math.max(0,state.trust+(effect.trust||0));
  state.history.push({
    step:state.step,choice:index,
    label:opt[0],outcome:opt[1]
  });
  if(opt[3]) state.selectedEnding=opt[3];

  $("clueStat").textContent=state.clues;
  $("nerveStat").textContent=state.nerve;
  $("trustStat").textContent=state.trust;
  $("choices").innerHTML="";
  $("feedback").classList.remove("hidden");
  $("feedback").textContent=opt[1];
  state.step++;
  $("stepLabel").textContent=`DECISÃO ${state.step}/40`;
  $("bar").style.width=(state.step/scenes.length*100)+"%";
  $("nextBtn").classList.remove("hidden");
  $("nextBtn").textContent=state.step>=scenes.length?"VER O FINAL →":"PRÓXIMA CENA →";
  saveGame();
}

function nextScene() {
  if(!state)return;
  if(state.step>=scenes.length) {finishGame();return;}
  renderScene();
  saveGame();
  window.scrollTo({top:0,behavior:"smooth"});
}

function finishGame() {
  if(!state)return;
  showScreen("ending");
  $("bar").style.width="100%";
  let title,text,achievement;

  const ending=state.selectedEnding;
  if(ending==="transferir" && state.clues>=8) {
    title="👁️ FINAL SECRETO — O NOVO ARQUITETO";
    text="Você assume o controle do Projeto 67 e encontra a lista completa dos financiadores. Mas, ao sair, recebe uma mensagem: “Agora você entende por que Vera ficou.” Você venceu o sistema e, ao mesmo tempo, herdou sua responsabilidade. No último quadro, seu reflexo sorri antes de você.";
    achievement="CONQUISTA: O PRÓXIMO VERA? — Você encontrou a verdade e escolheu o caminho mais perigoso.";
  } else if(ending==="destruir" && state.nerve>=8) {
    title="🔥 FINAL — CINZAS DO 67";
    text="Você desliga o sistema e a mansão mergulha no silêncio. Vera observa enquanto os painéis apagam um por um. “Talvez seja melhor não saber tudo”, ela diz. Você sai com poucas respostas, mas com a certeza de que o experimento acabou. Na estrada, o rádio liga sozinho: “67... 67... 67...”";
    achievement="CONQUISTA: BOTÃO VERMELHO — Coragem suficiente para acabar com o experimento.";
  } else if(state.clues>=13 && state.trust>=6) {
    title="🏆 FINAL VERDADEIRO — O SEGREDO REVELADO";
    text="Você reúne as provas, conquista a confiança de Vera e expõe os patrocinadores. O Projeto 67 termina não com uma explosão, mas com uma coletiva de imprensa, uma investigação e um monte de advogados correndo pelos corredores. Vera depõe. Cláudio entrega os registros. Nevair finalmente descobre quem financiou tudo — e o leite era apenas uma distração ridícula para esconder a logística do projeto.";
    achievement="CONQUISTA: DETETIVE 67 — Você juntou evidências e construiu alianças sem perder a cabeça.";
  } else if(state.clues>=10) {
    title="🕵️ FINAL — A VERDADE INCOMPLETA";
    text="Você consegue expor uma parte do Projeto 67 e fugir da mansão. Vera desaparece antes de prestar depoimento. Os documentos provam que houve manipulação, mas os patrocinadores continuam anônimos. Ao amanhecer, chega uma última mensagem: “Boa investigação. Nos vemos no 68.”";
    achievement="CONQUISTA: QUASE SHERLOCK — Você descobriu muita coisa, mas a conspiração continua.";
  } else if(state.nerve>=8) {
    title="💨 FINAL — FUGA ABSURDA";
    text="Você corre, desvia dos painéis e atravessa a saída no último instante. Vera não consegue impedir sua fuga. Você sobrevive e vira uma lenda local, embora ninguém acredite na história da mulher gigantesca. O único registro é um vídeo de três segundos intitulado “nevair 67 momento”.";
    achievement="CONQUISTA: SPEEDRUN SUSPEITO — Sobreviver também é uma estratégia.";
  } else if(state.trust>=7) {
    title="🤝 FINAL — ACORDO IMPROVÁVEL";
    text="Você convence Vera e Cláudio a revelar o funcionamento do projeto. Nem todos os nomes vêm à tona, mas a mansão é fechada e os participantes recebem reparação. Vera pede desculpas por tudo. Você aceita, mas pede que ela pare de mandar mensagens às 03:07.";
    achievement="CONQUISTA: DIPLOMACIA DO LEITE — Você transformou uma batalha em uma negociação.";
  } else {
    title="🥛 FINAL — O MISTÉRIO CONTINUA";
    text="Você sai da mansão com a sensação de ter visto apenas a superfície. Vera permanece no salão, observando o sistema reiniciar. Na estrada, seu celular vibra: “Você chegou até a decisão 40. Mas será que fez as escolhas certas?” Um arquivo aparece: PROJETO_68.zip.";
    achievement="CONQUISTA: SOBREVIVENTE DO 67 — Você chegou ao fim. As respostas ainda estão por aí.";
  }

  $("endingTitle").textContent=title;
  $("endingText").textContent=text;
  $("endClues").textContent=state.clues;
  $("endNerve").textContent=state.nerve;
  $("endTrust").textContent=state.trust;
  $("achievement").textContent=achievement;
  localStorage.removeItem(SAVE_KEY);
}

function saveGame() {
  if(!state)return;
  try {
    localStorage.setItem(SAVE_KEY,JSON.stringify(state));
    if($("saveBtn")) $("saveBtn").textContent="✓ Progresso salvo";
    if($("continueBtn")) $("continueBtn").classList.remove("hidden");
  } catch(e) {
    if($("saveBtn")) $("saveBtn").textContent="Não foi possível salvar";
  }
}

function loadGame() {
  try {
    const raw=localStorage.getItem(SAVE_KEY);
    if(!raw)return false;
    const saved=JSON.parse(raw);
    if(!saved || !Number.isInteger(saved.step) ||
       saved.step<0 || saved.step>scenes.length ||
       !Array.isArray(saved.history)) return false;
    state=saved;
    showScreen("game");
    if(state.step>=scenes.length) finishGame();
    else renderScene();
    return true;
  } catch(e) {
    return false;
  }
}

function goHome() {
  showScreen("hero");
  $("continueBtn").classList.toggle("hidden",!localStorage.getItem(SAVE_KEY));
  window.scrollTo({top:0,behavior:"smooth"});
}

$("startBtn").addEventListener("click",startNew);
$("continueBtn").addEventListener("click",()=>{
  if(!loadGame()) {
    $("continueBtn").classList.add("hidden");
    alert("Nenhum jogo salvo foi encontrado. Comece uma nova investigação!");
  }
});
$("nextBtn").addEventListener("click",nextScene);
$("saveBtn").addEventListener("click",saveGame);
$("quitBtn").addEventListener("click",goHome);
$("restartBtn").addEventListener("click",startNew);
$("menuBtn").addEventListener("click",goHome);

try {
  if(localStorage.getItem(SAVE_KEY)) $("continueBtn").classList.remove("hidden");
  else $("continueBtn").classList.add("hidden");
} catch(e) {
  $("continueBtn").classList.add("hidden");
}
</script>
</body>
</html>
