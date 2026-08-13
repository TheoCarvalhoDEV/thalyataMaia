# Thalyta Maia — Arquitetura

Site institucional, estático, sem build. Abrir `index.html` no navegador já roda.

## Estrutura

```
index.html            página única (todas as seções)
css/styles.css        estilos
js/main.js            navegação, reveals, galeria/lightbox
assets/images/        logos, hero, retrato, ícones
assets/pinterest/     fotos de referência usadas em seções e projetos
assets/projetos/<projeto>/NN.webp   fotos de cada projeto
```

## Imagens

Tudo em `.webp`. Duas exceções propositais: `og-thalyta-maia.jpg` (preview do
WhatsApp/Facebook não lê webp) e `apple-touch-icon.png` (Safari só aceita PNG).

Para adicionar fotos: salve em `assets/projetos/<projeto>/` numeradas
(`01.webp`, `02.webp`, …) e replique o bloco `.project__media--destaque` de um
projeto existente no `index.html`.

## Publicação

Branch `deploy` → Netlify. `git push origin deploy` publica.
