# Profilaxia Antirrábica — São Luís/MA

Aplicativo web aberto para apoio à orientação sobre profilaxia antirrábica humana em São Luís/MA.

## O que o app faz

- Orienta a conduta inicial com base nas respostas informadas pelo usuário.
- Informa esquemas de vacinação, reexposição, soroterapia e pontos de atendimento.
- Gera comprovante de orientação para impressão ou salvamento como PDF pelo navegador.
- Pode ser instalado na tela inicial do celular ou na área de trabalho como PWA.
- Possui funcionamento offline após o primeiro acesso, desde que o navegador permita o cache do app.

## Importante sobre o PDF

O botão **Gerar comprovante PDF** abre a janela de impressão do navegador. Para salvar como PDF, selecione **Salvar como PDF** no destino da impressão.

O app não envia, armazena nem coleta os dados digitados no comprovante. Os dados são usados apenas localmente no navegador para compor a impressão.

## Publicação no GitHub Pages

1. Envie todos os arquivos deste pacote para um repositório no GitHub.
2. Acesse **Settings > Pages**.
3. Em **Build and deployment**, selecione a branch `main` e a pasta `/root`.
4. Salve e aguarde a publicação.

## Instalação no celular

No Android/Chrome: abra o link publicado, toque no menu do navegador e selecione **Adicionar à tela inicial** ou **Instalar app**.

No iPhone/Safari: abra o link, toque em **Compartilhar** e selecione **Adicionar à Tela de Início**.

## Elaboração técnica

Giuliane Ferreira Lopes dos Santos  
Coordenadora de Vigilância Epidemiológica – COVEP/SVES/SEMUS  
Matrícula SEMUS: 25.613

## Base técnica utilizada

- Nota Técnica nº 35/2026 – Ministério da Saúde.
- Nota Técnica nº 134/2022 – Ministério da Saúde.
- Nota Técnica nº 8/2022 – Ministério da Saúde.
- Nota Técnica nº 160/2024 – Ministério da Saúde.
- Nota Técnica nº 007/2024/SVES/SEMUS – São Luís/MA.
- Guia de Vigilância em Saúde, 6ª edição revisada, 2024 – Ministério da Saúde.
- Portaria nº 6.161/2024-GAB/SEMUS – São Luís/MA.

## Aviso de uso

Este aplicativo é uma ferramenta de apoio à orientação e não substitui avaliação clínica presencial, investigação epidemiológica ou decisão técnica do serviço de saúde.

## Arquivos principais

- `index.html`: aplicativo principal.
- `manifest.json`: configuração para instalação como PWA.
- `service-worker.js`: cache para funcionamento offline.
- `assets/`: logos e barra institucional.
- `icons/`: ícones do aplicativo.


## Estatísticas de acesso

O GitHub Pages não fornece estatísticas detalhadas de acesso nativamente. Caso a gestão deseje acompanhar uso do app, recomenda-se avaliar posteriormente uma ferramenta de analytics com cuidado para não coletar dados pessoais sensíveis.

## Atualização desta versão

- Corrigido o layout de impressão/PDF para evitar corte de respostas longas.
- As respostas agora fazem quebra automática de linha e respeitam a largura da página A4.
- Mantido fundo majoritariamente branco para facilitar impressão.


## Observação sobre logos no GitHub Pages

Nesta versão, as logos exibidas na página foram incorporadas diretamente ao `index.html` para evitar erro de caminho, letras maiúsculas/minúsculas ou ausência da pasta `assets` no GitHub Pages. Ainda assim, mantenha as pastas `assets/` e `icons/` no repositório para organização e para o PWA.

Após substituir arquivos no GitHub, limpe o cache do navegador ou abra em janela anônima caso apareça uma versão antiga.

## Estrutura sem subpastas

Esta versão foi preparada para evitar erro de caminho no GitHub Pages. Todos os arquivos necessários ficam na raiz do repositório/pasta publicada:

```
index.html
manifest.json
service-worker.js
README.md
icon-192.png
icon-512.png
apple-touch-icon.png
```

As logos institucionais da página estão incorporadas diretamente no `index.html`, portanto não dependem da pasta `assets`.

## Como publicar no GitHub Pages

1. Apague/substitua os arquivos antigos do repositório ou pasta `antirrabica`.
2. Suba todos os arquivos desta versão diretamente na raiz da pasta/repositório.
3. Aguarde alguns minutos e atualize a página com `Ctrl + F5`.
4. Se já tiver aberto a versão anterior, limpe o cache do app: Chrome > F12 > Application > Service Workers > Unregister; depois Clear storage > Clear site data.
