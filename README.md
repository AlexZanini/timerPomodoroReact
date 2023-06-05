# React Pomodoro Timer
Este projeto baseado na técnica Pomodoro. Esta aplicação permite que você defina um timer para suas tarefas e interrompa-as se necessário. Você pode ver o histórico das suas tarefas concluídas, interrompidas ou ainda em andamento.

## Funcionalidades
Adicionar um novo ciclo com um nome de tarefa e uma quantidade de minutos
Interromper um ciclo atual
Visualizar o tempo restante no ciclo atual
Visualizar um histórico de todos os ciclos, incluindo a tarefa, a duração, a data de início e o status (concluído, interrompido ou em andamento)

## Tecnologias Utilizadas
React.js
TypeScript
Styled-components
React Router
Date-fns
React Hook Form

## Estrutura dos Arquivos

Aqui está a estrutura de alguns dos principais arquivos e pastas deste projeto:

- `src/App.tsx`: Este é o ponto de entrada principal da aplicação. Ele é responsável por renderizar os componentes principais e gerenciar os contextos globais. Todos os componentes da aplicação são chamados a partir deste arquivo.

- `src/contexts/CyclesContext.tsx`: Este arquivo contém o contexto CyclesContext que é usado para gerenciar os ciclos do timer. Ele contém a lógica para adicionar, interromper e manter o histórico dos ciclos. Cada ciclo é um objeto que inclui um identificador único, o nome da tarefa, a duração da tarefa, e o status do ciclo.

- `src/pages/Home`: Esta pasta contém os componentes da página principal da aplicação. A página Home é o lugar onde os usuários podem iniciar um novo ciclo, ver a contagem regressiva do ciclo atual e interromper o ciclo se necessário.

- `src/pages/Home/components/Countdown`: Este é o componente que exibe a contagem regressiva do ciclo ativo. Ele recebe a duração do ciclo atual como propriedade e atualiza a exibição a cada segundo.

- `src/pages/Home/components/NewCycleForm`: Este componente permite ao usuário iniciar um novo ciclo. Ele inclui um formulário onde os usuários podem inserir o nome da tarefa e a duração desejada. Quando o formulário é submetido, um novo ciclo é adicionado ao CyclesContext.

- `src/pages/History`: Esta pasta contém a página que exibe o histórico de ciclos do usuário. Cada ciclo é listado com seu nome de tarefa, duração e status. Os ciclos podem estar em um de três estados: concluído, interrompido ou em andamento.
