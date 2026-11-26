# ReduzirMBZenvia-TIME_MAD.U
# Reduzir arquivos

Ferramenta de uma página que reduz fotos, vídeos e áudios para caber no limite de tamanho do WhatsApp (Zenvia).
Tudo roda no navegador: os arquivos não são enviados para nenhum servidor.

## Limites
- **Zenvia / WhatsApp (padrão):** imagem 5 MB, vídeo e áudio 16 MB, documento 100 MB.
- **25 MB** ou **outro valor** para os demais casos.

## Como funciona
- **Imagens:** reencodadas em JPEG (ou PNG, se tiverem transparência), ajustando qualidade e, se preciso, o tamanho em pixels.
- **Vídeos:** convertidos para MP4 (H.264 + AAC) com taxa de bits calculada para caber no limite, usando ffmpeg.wasm (baixado na primeira vez, ~30 MB).
- **Áudios:** convertidos para M4A (AAC).
- O vídeo é processado no seu computador e pode demorar alguns minutos; mantenha a aba aberta.

## Publicar no GitHub Pages
1. Suba `index.html` e `README.md` na raiz do repositório.
2. **Settings > Pages > Deploy from a branch**, branch `main`, pasta `/ (root)`.
