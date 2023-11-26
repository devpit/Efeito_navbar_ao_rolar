# Efeito de Navbar ao Rolar

Este repositório oferece uma implementação simples, mas eficaz, de um efeito para a barra de navegação (navbar) que adiciona uma interação visual agradável quando o usuário rola a página. Esse efeito é útil para aprimorar a experiência do usuário e dar um toque de elegância à navegação.

## Funcionalidades

- **Transição de Fundo:**
  - Ao rolar a página, a barra de navegação altera seu estilo de fundo, proporcionando uma transição suave e agradável.
- **Melhoria da Experiência do Usuário:**
  - O efeito de rolagem melhora a experiência visual do usuário, adicionando um elemento dinâmico à navegação.

## Como Utilizar

1. **Inclusão do Script e Estilos:**
   - Adicione o script JavaScript e os estilos CSS à sua página HTML para incorporar o efeito à sua barra de navegação.
   ```html
   <link rel="stylesheet" href="caminho-para/seu-estilo.css">
   <script src="caminho-para/seu-script.js"></script>
   ```

2. **HTML da Barra de Navegação:**
   - Estruture sua barra de navegação no HTML com a classe `navbar` para que o script possa aplicar o efeito.
   ```html
   <nav class="navbar">
      <!-- Conteúdo da barra de navegação -->
   </nav>
   ```

3. **Configuração Personalizada (Opcional):**
   - Personalize o estilo e comportamento do efeito ajustando as classes e propriedades no seu estilo CSS.

3. **CSS navbar:**
   - Personalize o estilo e comportamento do efeito ajustando as classes e propriedades no seu estilo CSS.
   ```css
   nav {
    position: fixed;
    z-index: 1;
    opacity: 0;
    top: 0;
    left: 0;
    width: 100%;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding: 0 24px 0 15px;
    background: transparent;
    box-shadow: 0 0 20px rgb(0 0 0 / 8%);
    }

    nav.scrolled {
    background: #ff6961;
    box-shadow: 2px 3px 3px #f44336;
    opacity: 1;
    }
   ```

## Exemplo de Uso

```javascript
// Inicialização do efeito de navbar ao rolar
window.addEventListener("scroll", function () {
    var navbar = document.querySelector("nav");
    navbar.classList.toggle("scrolled", window.scrollY > 0);
});
```

## Contribuição

Contribuições são bem-vindas! Se você encontrar problemas ou tiver sugestões para melhorias, sinta-se à vontade para abrir uma *issue* ou enviar um *pull request*.

Espero que este efeito simples de navbar ao rolar adicione um toque elegante à navegação da sua página. Se precisar de suporte ou tiver dúvidas, sinta-se à vontade para entrar em contato.
