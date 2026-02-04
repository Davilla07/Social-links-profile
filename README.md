# Frontend Mentor - Solução do perfil de links sociais

Esta é uma solução para o [desafio Social links profile do Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). Os desafios do Frontend Mentor ajudam você a aprimorar suas habilidades de codificação construindo projetos realistas.

## Sumário

- [Visão geral](#visão-geral)
  - [O desafio](#o-desafio)
  - [Captura de tela](#captura-de-tela)
  - [Links](#links)
- [Meu processo](#meu-processo)
  - [Ferramentas utilizadas](#ferramentas-utilizadas)
  - [O que aprendi](#o-que-aprendi)
  - [Desenvolvimento futuro](#desenvolvimento-futuro)
  - [Recursos úteis](#recursos-úteis)
- [Autor](#autor)

## Visão geral

### O desafio

Os usuários devem conseguir:

- Ver estados de hover e focus para todos os elementos interativos da página
- Visualizar o layout ideal dependendo do tamanho da tela do dispositivo
- Ver o perfil estilizado de acordo com as especificações do design

### Captura de tela

![./screenshot.jpg](./screenshot.jpg)


### Links

- URL da solução: [https://github.com/seuusername/social-links-profile](https://github.com/seuusername/social-links-profile)
- URL do site ao vivo: [https://seuusername.github.io/social-links-profile](https://seuusername.github.io/social-links-profile)

## Meu processo

### Ferramentas utilizadas

- HTML5 semântico
- Variáveis CSS (Custom Properties)
- Flexbox
- Workflow mobile-first
- CSS Reset
- Google Fonts (Inter)
- Estados de hover e focus

### O que aprendi

Neste projeto, aprimorei meus conhecimentos em CSS moderno e boas práticas de desenvolvimento web. Aqui estão alguns dos principais aprendizados:

**CSS Custom Properties (Variáveis)**
Aprendi a organizar e utilizar variáveis CSS no seletor `:root` para facilitar a manutenção do código. Isso permitiu centralizar cores, fontes e medidas em um único local.

```css
:root {
  --color-background: hsl(0, 0%, 8%);
  --color-card: hsl(0, 0%, 12%);
  --color-list: hsl(0, 0%, 20%);
  --color-name-avatar: hsl(0, 0%, 100%);
  --color-location-avatar: hsl(75, 94%, 57%);
  --font-size-paragraph: 14px;
  --font-weight-paragraphs: 400;
  --font-weight-list: 600;
  --font-weight-name: 700;
  --border-radius: 10px;
}

**Flexbox para Layout**
Dominei o uso do Flexbox para centralizar o card na página, utilizando display: flex combinado com justify-content: center e align-items: center para alinhamento perfeito.

body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-color: var(--color-background);
}

**Estados Interativos (Hover e Focus)**
Implementei estados de :hover e :focus para elementos interativos, aprendendo a importância da semântica correta dos seletores. Descobri que li a:hover é diferente de li :hover (com espaço), onde o espaço muda completamente o comportamento do seletor.

.links-list li a:hover {
  background-color: hsl(0, 0%, 25%);
  transform: translateY(-2px);
  transition: all 0.3s ease;
}

.links-list li a:focus {
  outline: 3px solid var(--color-location-avatar);
  outline-offset: 3px;
}

**Estrutura Semântica de Listas**
Aprendi a estruturar corretamente uma lista de links usando <ul> → <li> → <a>, garantindo acessibilidade e semântica adequada.

<ul class="links-list">
  <li><a href="#">GitHub</a></li>
  <li><a href="#">Frontend Mentor</a></li>
  <li><a href="#">LinkedIn</a></li>
  <li><a href="#">Twitter</a></li>
  <li><a href="#">Instagram</a></li>
</ul>

**Responsividade Mobile-First**
Implementei um design responsivo utilizando max-width: 340px combinado com width: 100%, garantindo que o card se adapte corretamente a diferentes tamanhos de tela.


**CSS Reset**
Apliquei um reset universal para garantir estilos consistentes entre diferentes navegadores, uma prática profissional essencial.

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

**Desenvolvimento futuro**

Áreas que quero focar em projetos futuros:

*Transições CSS mais avançadas: Explorar animações complexas e micro-interações

*Acessibilidade (a11y): Aprimorar contrastes e adicionar atributos ARIA para usuários de leitores de tela

*Metodologia BEM: Adotar uma convenção de nomenclatura para CSS mais escalável e organizado

*CSS Grid: Explorar Grid como alternativa ao Flexbox para layouts mais complexos

*Media Queries personalizadas: Criar variáveis para breakpoints para melhorar a responsividade em diferentes dispositivos

Recursos úteis
MDN Web Docs - CSS Custom Properties - Guia essencial para entender variáveis CSS
CSS-Tricks - Guia Completo do Flexbox - Recurso definitivo para dominar Flexbox
Google Fonts - Inter - Documentação oficial da fonte utilizada
MDN - Pseudo-classes :hover e :focus - Entendendo seletores de estado interativo
WebAIM - Acessibilidade com Teclado - Diretrizes para navegação com teclado e estados de focus
Autor

Frontend Mentor - @Davilla07
GitHub - @Davilla07