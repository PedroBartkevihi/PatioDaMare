# Pátio da Maré — Landing Page (projeto de estudo)

**Ver online:** https://pedrobartkevihi.github.io/PatioDaMare/

Landing page **fictícia** de divulgação do empreendimento residencial
**Pátio da Maré**, da incorporadora **Pátio Sul Incorporações**, criada **para
fins de estudo**. Partindo de um exercício de curso feito só com HTML e CSS, o
objetivo foi modernizar o visual — layout, tipografia, cores, espaçamentos,
botões, cards, responsividade e pequenas interações — mantendo o estilo de
escrita do código original.

O empreendimento, a incorporadora e os textos são inventados para este projeto
e não correspondem a nenhuma empresa ou imóvel real. As fotos são ilustrativas.

## Tecnologias

- HTML5
- CSS3 (variáveis em `:root`, flexbox, `clamp()` e media queries)
- JavaScript (vanilla, sem dependências)
- [Google Fonts](https://fonts.google.com/) — Open Sans (Apache 2.0) e Playfair Display (OFL)

Sem frameworks e sem etapa de build: é só abrir o `index.html`.

## Estrutura

```
Projeto2/
├── index.html
├── css/
│   └── style.css
├── js/
│   └── script.js
└── imagens/
    ├── bg-form.jpg      (foto da capa)
    ├── seta.svg         (seta da seção de chamada)
    └── mosaico1..4.jpg  (fotos da seção Estrutura)
```

As logos do Pátio da Maré e da Pátio Sul são texto com as fontes do site e um
ícone de ondas em SVG, desenhado direto no `index.html`.

## Seções

1. **Header** — logos e menu (vira dropdown no mobile).
2. **Capa** — foto, chamada principal e formulário de contato.
3. **Chamada** — faixa de destaque com seta e botão para o formulário.
4. **Estrutura (mosaico)** — quatro cards alternando foto e texto.
5. **Rodapé** — marca, slogan e links.

## Interações (`js/script.js`)

- Abre/fecha o menu no mobile (com `Esc`, clique fora e clique em link).
- Sombra no header ao rolar a página.
- Elementos `[data-revelar]` surgem ao entrar na tela (`IntersectionObserver`).
- Feedback ao enviar o formulário (não há back-end).
- Respeita `prefers-reduced-motion` e funciona sem JavaScript.

## Como executar

Abra o `index.html` no navegador, ou rode um servidor estático na pasta do
projeto:

```bash
python -m http.server 8080
```

E acesse `http://localhost:8080`.

## Créditos das imagens

As fotos vêm do [Pexels](https://www.pexels.com/) (licença livre, sem
necessidade de atribuição) e foram apenas redimensionadas, recortadas e
salvas sem metadados: [capa](https://www.pexels.com/photo/24807133/),
[1](https://www.pexels.com/photo/27051764/),
[2](https://www.pexels.com/photo/6775268/),
[3](https://www.pexels.com/photo/6957107/) e
[4](https://www.pexels.com/photo/18822579/). A seta e o ícone das ondas são
SVGs simples, desenhados para este projeto.

## Uso

Repositório de **estudo de front-end, sem fins comerciais**. O código-fonte
(HTML, CSS e JavaScript) é de autoria de **Pedro Farias** e pode ser
reaproveitado livremente. Toda a identidade (empreendimento, incorporadora,
textos e slogan) é fictícia.
