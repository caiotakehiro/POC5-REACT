## Andreas Caycedo Martinez 10435302
## Caio Takehiro Magnoli Igari 10437809
### Sistemas de Informação, 02J L12
## POC 5-React
Esta Prova de Conceito mostra como utilizar o o funcionamento de alguns conceitos de REACT, usando Next.js. Eles são:

## Estrutura Next.js 14+
Esta POC foca no uso do Next.js 14+. As principais características desta estrutura são:

- Roteamento Automático: O diretório "app/" organiza as páginas e rotas de forma automática.
- Renderização Híbrida: Suporte a renderização no lado do servidor (SSR) e geração de páginas estáticas (SSG), permitindo otimização de desempenho de acordo com a necessidade de cada página.
- Componentização: Componentes reutilizáveis, como Header.tsx, são organizados em app/components/, promovendo a modularização e facilitando a manutenção.
- Estilo CSS(Global e Módulo): Suporte a CSS Modules para estilos locais em componentes e a estilos globais, com "globals.css", para configurações universais de estilo.
- Fontes Customizadas: Fontes personalizadas estão localizadas em "fonts/", permitindo customização visual otimizada.
  
A estrutura Next.js 14+ permite desenvolver aplicações React de maneira eficiente, promovendo performance e simplicidade.

## Componentes Simples (Sem Estado)
Os componentes simples são simples porém muito eficientes, eles são utilizados apenas para renderizam de dados estáticos. Seu funcionamento é bem claro, ele recebe uma propriedade e em seguida retornam JSX, durante essa POC esse elemento é aplicado várias vezes como por exemplo no componente Header, que tem a função de exibir o titulo da página
```jsx
const Header: React.FC<HeaderProps> = ({ title }) => {
  return (
    <header className={styles.header}>
      <h1 className={styles.title}>{title}</h1>
    </header>
  );
};
```
O código acima é um componente simples pois assim como ja foi dito ele não possuí ciclo de vida, ele apenas recebe uma prop e a renderiza dentro de umm elemento.
## Estilo CSS (Global e Módulo)
- Global:
Os estilos definidos no CSS global são aplicados a toda a aplicação, ou seja, eles afetam qualquer elemento que corresponda ao seletor CSS, independentemente de onde esse elemento esteja, a seguir tem um exemplo de como aplicamos o estilo global em nosso trabalho.
```css
/* src/styles/globals.css */
body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
  }
  
  h1 {
    color: #0070f3;
  }
```

- Módulo:
Os estilos definidos em um módulo CSS afetam apenas o componente no qual são importados. Isso evita interferência de estilos entre componentes, a seguir tem um exeplo de como foi aplicado o estilo no trabalho.
```css
/* src/components/Header.module.css */
.header {
    background-color: #f0f0f0;
    padding: 20px;
  }
  
  .title {
    color: #0070f3;
    font-size: 24px;
  }
```
## Como acessar o resultado
Para acessar o resultado do código apresentado ao longo desse ReadMe basta seguir os seguintes passos:
![380027049-61c8c4d4-bbfb-45d7-99aa-8ca96f4d0488](https://github.com/user-attachments/assets/79bf4e7f-0c66-4018-9cc8-7053f16bdeea)
- Acessar o terminal do arquivo
- Digitar " npm run dev "
- "ctlr + click" no link ao lado de "- Local:"


## Resultado visual 
O código apresentado durante esse ReadMe, quando executado resulta na imagem a seguir:
![380009896-c9a1ccb3-bfd5-4a72-94ea-5a22d5001252](https://github.com/user-attachments/assets/f6c49652-375c-40df-a873-0114086d2d1d)

## Conclusão 
Esta POC é uma demonstração de aplicação de conceitos fundamentais do React, visto que o projeto usa elementos da estrutura Next.js 14, utiliza componentes simples sem estado e o uso de estilos como CSS global e módulo.

