# NeuralKinetics

Site conceitual de uma empresa de tecnologia, criado como projeto de portfólio. A experiência reúne apresentação institucional, serviços, projetos, perguntas frequentes e um formulário demonstrativo de briefing. A marca e os projetos exibidos são fictícios.

![Prévia do NeuralKinetics](img/social-preview.png)

## Como foi construído

- Interface renderizada com **React**. O arquivo `script.js` contém a versão compilada da aplicação e da biblioteca de movimento usada na interface; o código fonte original e o projeto de build não fazem parte deste pacote.
- **HTML** de entrada em `index.html`, **CSS** responsivo em `style.css` e assets locais em `img/` e `assets/`.
- Tipografia **Inter** carregada pelo Google Fonts, com fonte alternativa definida no CSS.
- Vídeo de abertura em `assets/hero.mp4`, com imagem de apoio e fallback remoto previstos na interface.
- Estrutura estática que pode ser servida sem Node.js ou backend.

## Interações e animações

- Vídeo no hero com controle de reprodução.
- Faixa contínua em movimento, ilustrações orbitais e detalhes animados criados em CSS.
- Entradas de conteúdo, transições de cartões, botões e navegação ao longo da página.
- Indicador de progresso da rolagem, menu adaptado para telas menores e CTA de contato móvel.
- Perguntas frequentes e janelas de conteúdo interativas.
- Suporte à preferência do sistema por movimento reduzido (`prefers-reduced-motion`).

O formulário organiza os dados informados e gera um arquivo `.txt` para download no próprio navegador. Ele **não envia e-mails nem grava os dados em um servidor**.

## Estrutura

```text
index.html          Entrada da aplicação
style.css           Layout, responsividade e animações
script.js           Aplicação React compilada
img/                Imagens e ícones
assets/hero.mp4     Vídeo local de abertura
404.html            Página de erro
robots.txt          Regra de rastreamento da demonstração
```

## Executar e publicar

Abra `index.html` no navegador ou sirva a pasta com um servidor estático. Para hospedagem compartilhada, envie os arquivos desta pasta para a pasta pública mantendo a estrutura de diretórios. O arquivo `.htaccess` configura a página 404 em Apache na raiz do domínio.

Esta versão foi preparada como demonstração e inclui `noindex, nofollow` e bloqueio em `robots.txt`. Revise essas regras, a URL de compartilhamento social e o fallback remoto do vídeo antes de usar um domínio público. Para alterar a lógica React de forma sustentável, é necessário recuperar o projeto fonte que gerou `script.js`.
