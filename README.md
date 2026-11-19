# um cantinho só seu

Página estática feita para a minha prima: um "computadorzinho" retrô (nanda.os) com janelas que abrem pelos ícones do desktop ou pelo menu iniciar.

- **vitrola.exe**: estante com 5 álbuns do One Direction; o disco sai da capa, encaixa na vitrola e toca pelo YouTube
- **cats.exe**: vídeo de gatos e uma chuva de gatos com erro de "gatos demais"
- **dwight.jpg**: o Dwight meditando
- **frases.txt**: frases de livros e poemas, com um rascunho que fica salvo no navegador
- **abraco.exe**: abraço sob demanda
- **correio**: cartinhas trancadas até o fim da contagem (25/11, 17h, horário de Brasília)
- janelas arrastáveis, janela principal com minimizar, tela cheia e fechar, sons gerados com a Web Audio API

A versão original (recuperada da Netlify) está na tag `v1`.

## Stack

- HTML, CSS e JavaScript puros, num único `index.html`
- Sem build, sem dependências
- Embeds: Spotify e YouTube (IFrame API)
- Ícones: Fluent Emoji, da Microsoft (MIT), via jsDelivr

## Rodar localmente

Sirva a pasta (o player do YouTube não funciona abrindo o arquivo direto):

```bash
python -m http.server 8000
```

Para ver as cartinhas abertas antes da hora, acesse `http://localhost:8000/?abrir`.

## Deploy

Hospedado na Vercel como site estático (sem framework, sem build command). Todo push na `main` publica.
