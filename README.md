# IACIT · Landing page conceitual

Landing page imersiva para a **IACIT Soluções Tecnológicas**, Empresa Estratégica de Defesa sediada em São José dos Campos (SP).
Conteúdo baseado nas informações públicas de [iacit.com.br](https://www.iacit.com.br/).

## Destaques

- Radar PPI animado em canvas no hero, com varredura e alvos em tempo real
- Rolagem horizontal fixada com os quatro mercados da IACIT
- **Radar OTH 0100 em 3D**: costa gaúcha, setor de 120°, curvatura da Terra e navios sem AIS, tudo conduzido pelo scroll
- **Radar RMT 0200 em 3D**: radome, varredura volumétrica de 600 km, dupla polarização H/V e classificação de hidrometeoros
- Portfólio filtrável com prévia que segue o cursor
- Linha do tempo com ano fixo e efeito de embaralhamento
- Tema claro e escuro, layout responsivo e suporte a movimento reduzido

## Tecnologias

Arquivo único (`index.html`), sem etapa de build. Bibliotecas carregadas por CDN:

- [GSAP 3.13](https://gsap.com/) com ScrollTrigger, ScrambleText e Flip
- [Lenis](https://lenis.darkroom.engineering/) para rolagem suave
- [three.js r128](https://threejs.org/) para as cenas 3D
- Fontes Saira, IBM Plex Sans e IBM Plex Mono (Google Fonts)

## Rodar localmente

Abra o `index.html` no navegador, ou sirva a pasta:

```bash
npx serve .
# ou
python3 -m http.server 8080
```

## Publicar com GitHub Pages

1. Envie os arquivos para a branch `main`.
2. Em **Settings → Pages**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`.
3. O site fica disponível em `https://<seu-usuario>.github.io/<nome-do-repositorio>/`.

## Aviso

Projeto conceitual, não oficial. Marcas, nomes de produtos e informações pertencem à IACIT Soluções Tecnológicas S.A.
As cenas 3D usam posições e escalas ilustrativas; os dados técnicos citados vêm do site oficial.
