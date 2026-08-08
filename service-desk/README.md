# Service Desk Acadêmico

Aplicativo web estático feito em HTML, CSS e JavaScript para demonstrar versionamento de código em aula.

## Como abrir sem servidor

Este projeto não precisa de servidor local, Node.js, Python ou instalação de dependências.

Opção mais simples:

1. Dê dois cliques no arquivo `abrir-service-desk.bat`.
2. O navegador padrão abrirá o arquivo `index.html`.

Também é possível abrir diretamente o arquivo `index.html` com dois cliques.

## Funcionalidades

- Tela do usuário para abrir chamados.
- Painel do analista para selecionar chamados.
- Alteração de status.
- Alteração de prioridade.
- Registro de correção.
- Histórico dos chamados.
- Persistência simples usando `localStorage`.

## Arquivos principais

- `index.html`: estrutura das telas.
- `styles.css`: aparência do aplicativo.
- `app.js`: regras de interação e persistência local.
- `abrir-service-desk.bat`: atalho para abrir o app no navegador sem subir servidor.

## Quatro bugs intencionais para a aula

1. A busca do painel do analista procura por ID e título, mas não procura pelo nome do solicitante, apesar do placeholder dizer que isso funciona.
2. Ao salvar alterações em um chamado, os dados aparecem atualizados na tela, mas não são persistidos no `localStorage`. Ao recarregar a página, as alterações somem.
3. O botão "Limpar base local" não limpa a lista de chamados; ele restaura os chamados de exemplo. O rótulo e o comportamento entram em conflito.
4. O histórico geral mostra apenas o estado atual de cada chamado, não a lista completa de eventos de cada chamado. Isso limita a auditoria prometida pela funcionalidade.


