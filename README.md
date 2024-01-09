# Anotações do Curso "Build Progressive Web Apps from Scratch: Frontend Masters"

- **Introdução**
  - PWA é uma aplicação da web que funciona tanto na web quanto como um aplicativo em dispositivos móveis.
  - SDK (Software Development Kit), também conhecido como "kit de desenvolvimento de software", é um conjunto de ferramentas de desenvolvimento de software, como bibliotecas.
  - PWA oferece facilidade na manutenção, deploy e desenvolvimento por ser uma aplicação web.
  - É possível usar PWA com diferentes stacks (por exemplo, React, jQuery, Vue, etc.).
  - Oferece desempenho comparável a aplicativos nativos.
  - Suporte para notificações push através do Web Push.
  - Exemplos: [app.starbucks.com](http://app.starbucks.com) (PWA), adicionar o ícone na tela inicial sem precisar baixar pelas lojas de aplicativos convencionais (por exemplo, Tinder).
  - Identificação de uma aplicação web como PWA é possível pela presença de um ícone na barra para instalação.
  - Suporte a partir do Windows 7.
  - 93% de suporte nos navegadores e 86% para instalação via ícone.

- **Componentes do PWA**
  - **Project Setup**
    - Comando para executar: `npx serve .` (cria um servidor).
  
  - **Web Manifest**
    - Arquivo JSON que é essencial para o PWA, contendo suas configurações. Cada PWA possui apenas um manifesto.
    - Recomenda-se criar na raiz do projeto.
    - Configurações incluem nome, short_name, título para SEO, orientação, tema e configurações de exibição.
    - Definição da cor do tema no manifesto e na tag `<meta>` no index.html (para o navegador). Alterações podem não ser atualizadas instantaneamente, podendo exigir reinstalação.
    - Definição do escopo da aplicação e páginas consideradas como PWA.
    - Display: Modo primário de exibição da aplicação, geralmente utilizado o `standalone`.
    - Configurações de ícones (com recomendações de tamanhos) e uso de "maskable icons".
  
  - **Service Workers**
    - Arquivo JavaScript responsável por gerenciar um servidor web no lado do cliente.
    - Usado para melhorar o desempenho e permitir o armazenamento de recursos offline.
    - Registrado no index.html para ativação.
    - Requer verificação de disponibilidade da API.
    - Cache local para armazenamento de assets.
    - Necessidade de instruções no código para funcionamento adequado.