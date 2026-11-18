# Flamingos · blocking 3D (playblast)

Blocking 3D estilo playblast para guiar IA de vídeo: 30 s a 24 qps (720 quadros), câmera em roll 180°
vendo o reflexo na água, pouso dos flamingos e giro de 180° que revela o mundo real.

Tudo roda no navegador, num arquivo só (`index.html`): Three.js r170 e mp4-muxer vêm do jsDelivr, não
precisa instalar nada.

## Abrir

- **Online:** ative o GitHub Pages neste repositório (Settings → Pages → branch `main`, pasta `/root`).
  O app fica em `https://<seu-usuario>.github.io/<nome-do-repo>/`.
- **No computador:** abra o `index.html` por um servidor local (os módulos não carregam via `file://`):
  `python3 -m http.server` na pasta e acesse `http://localhost:8000`.

## Usar

- **Linha do tempo:** play, quadro a quadro (◀ ▶ ou setas), marcadores de beat clicáveis.
- **Botão HUD** (ou tecla **H**): liga/desliga todos os textos na tela e no vídeo.
- **Câmera do filme / Vista de trabalho:** a vista de trabalho mostra a cena de fora (arraste para girar).
- **Painéis:** tempo dos beats, flamingos (bloco do corpo com largura/altura/comprimento), câmera,
  água (intensidade e formato da distorção), cenário, estética (cinza ou cores), visualização.
  Duplo clique num slider volta ao padrão.
- **Render final na sua GPU:** escolha a versão (blocos rosa, blocos cinza, ou sem blocos/só a água),
  a resolução (720p, 1080p, 4K) e clique em *Renderizar MP4*. Precisa de Chrome ou Edge atualizados
  (WebCodecs). Mantenha a aba visível durante o render.
- **Ajustes:** copiar/colar todos os sliders em JSON; os ajustes também ficam salvos no navegador.
