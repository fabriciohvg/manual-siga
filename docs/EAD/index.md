# Início

O Sistema SIGA conta com uma plataforma completa de EAD, que permite:

- cadastrar cursos, turmas e aulas;
- configurar a liberação de conteúdos (semanal, mensal etc.);
- inserir materiais de estudo;
- aplicar avaliações on-line ou por envio de anexos;
- disponibilizar videoaulas (YouTube, Vimeo ou hospedadas no próprio sistema);
- emitir automaticamente certificados e diplomas;
- definir períodos de acesso personalizados;
- realizar renovações com cobrança automática;
- emitir declarações e documentos diversos, entre outros recursos.

## Visão geral

Este documento oferece uma visão geral completa da funcionalidade de Ensino a Distância (EAD) do sistema SIGA. O objetivo é servir como um guia para administradores e gestores acadêmicos, detalhando desde a configuração inicial de um curso até o acompanhamento do progresso do aluno.

??? abstract "Clique aqui e assista ao vídeo: Visão Geral do ambiente EAD / Sistema SIGA"

    <iframe allow="autoplay; fullscreen" allowfullscreen="" frameborder="0" height="300" src="https://player.vimeo.com/video/663452654?h=8243f85cd8" width="640"></iframe>

## Introdução

O módulo EAD do sistema SIGA é uma ferramenta flexível projetada para gerenciar cursos em diversos formatos, incluindo:

- Cursos 100% online.
- Cursos semipresenciais.
- Cursos técnicos e profissionalizantes.
- Cursos livres e de extensão.

Este guia utilizará o curso "Pedagogia EAD" como exemplo para demonstrar as funcionalidades.

## Painel Administrativo

A configuração do EAD é realizada dentro do cadastro do curso desejado. Acesse o menu `EAD` no painel lateral do curso para gerenciar todas as suas propriedades.

### Configurações gerais

**Matrícula Online:** Defina se os alunos podem se matricular de forma autônoma (online) ou se a matrícula deve ser realizada exclusivamente por um funcionário da instituição.

**Apresentação do Curso:** Configure os elementos visuais e informativos que o aluno verá na plataforma, como categoria, imagem de capa, slides de apresentação, resumo, detalhes, público-alvo e informações sobre o certificado.

**Período de Acesso e Suporte:**

- **Acesso ao Curso:** Determine por quantos dias o aluno terá acesso ao conteúdo após a efetivação da matrícula. Para acesso vitalício, insira o valor `0`.
- **Suporte ao Curso:** Defina o período durante o qual o aluno terá direito a suporte.

**Bloqueio por Pendência Financeira:** Ative o bloqueio automático de acesso ao curso para alunos inadimplentes. É possível configurar o número de pendências e os dias de vencimento que acionarão o bloqueio.

**Regras de Conclusão do Curso:** Escolha a condição que determinará a conclusão do curso pelo aluno:

1.  Ter todas as notas lançadas em todas as disciplinas matriculadas.
2.  Finalizar todas as aulas EAD cadastradas.
3.  Aprovação automática assim que todas as aulas forem finalizadas.

**Certificado de Conclusão:** Vincule um modelo de documento (certificado) pré-cadastrado no editor de documentos do SIGA. O sistema pode preencher automaticamente campos dinâmicos (nome do aluno, carga horária, nota, assinatura digital, QR Code para validação online) e liberar o certificado para impressão assim que o aluno atender à regra de conclusão.

### Integração com Matrícula Web

Vincule o curso a uma [Matrícula Web](#) para automatizar o processo de inscrição. Nesta função, é possível:

- Definir uma taxa de matrícula e as formas de pagamento (boleto bancário, transferência, PagSeguro/cartão de crédito).
- Receber notificações automáticas quando o pagamento da taxa for confirmado.
- Exigir o envio online de documentos (ex: identidade, comprovante de endereço).
- Permitir que o aluno preencha seus dados cadastrais, otimizando o processo de efetivação da matrícula.

### Estrutura de aulas

**O Conceito de Configuração de Aulas:** O sistema permite criar diferentes "configurações de aulas" para o mesmo curso. Isso é útil para gerenciar turmas de anos letivos distintos que possam ter estruturas curriculares diferentes.

!!! example "Exemplo de configuração de aulas"

    A turma de 2020 pode ter 3 aulas, enquanto a turma de 2021 pode ter 5 aulas. Ao criar uma nova configuração para 2021 e vincular a nova turma a ela, as alterações não afetarão o histórico dos alunos de 2020.

**Duplicando Configurações de Aulas:** Para otimizar o tempo, é possível duplicar uma configuração existente e apenas realizar as alterações necessárias, sem precisar cadastrar todas as aulas novamente.

### Cadastro / configuração de aulas

Cada aula possui um conjunto detalhado de configurações para controlar o processo de aprendizagem do aluno.

**Informações Básicas:**

- **Módulo/Período:** Associe a aula a um módulo ou período específico da matriz curricular.
- **Título e Descrição:** Defina o nome e uma breve descrição da aula.
- **Disciplina e Professor:** Vincule a aula a uma disciplina (para lançamento de notas no histórico) e a um ou mais professores responsáveis. O professor vinculado será o destinatário das dúvidas enviadas pelos alunos.

**Permissões e Propriedades:**

- **Aula Ativa:** Controla a visibilidade da aula para os alunos.
- **Aula Padrão:** Se "Sim", todos os alunos matriculados no curso serão automaticamente habilitados nesta aula. Se "Não", os alunos deverão ser inseridos manualmente.
- **Aula Demonstrativa:** Permite que a aula seja acessada por qualquer pessoa, mesmo sem login, ideal para fins de marketing e divulgação.

**Regras de Sequenciamento e Liberação:**

**Requisito:**

- **Sim (Escada):** O aluno só pode acessar a aula seguinte após concluir a atual.
- **Não:** O aluno pode acessar qualquer aula a qualquer momento.
- **Geral:** O aluno precisa concluir esta aula (ex: uma aula de nivelamento) para que todas as outras aulas do curso sejam liberadas.

**Liberação da Aula:**

- **Liberada:** A aula está sempre disponível (respeitando a regra de requisito).
- **Liberada a partir de:** Defina uma data fixa para a liberação da aula.
- **Liberação Personalizada:** Libere a aula após um número de dias a contar da data de matrícula de cada aluno.
- **Bloqueio da Aula:** De forma similar à liberação, é possível bloquear o acesso a uma aula após uma data específica ou após um determinado número de dias da conclusão da mesma.

**Controles de Acesso:**

- **Permanência Obrigatória:** Defina um tempo mínimo (em minutos) que o aluno deve permanecer na tela da aula para poder finalizá-la.
- **Visualizações Permitidas:** Limite o número de vezes que um aluno pode acessar uma mesma aula. Insira `0` para não utilizar.

**Avaliações da Aula (Opcional):**

**Prova / Questionário Online:**

- Crie um questionário com múltiplas questões.
- Tipos de questão: escolha única, múltipla escolha ou resposta textual.
- Configure as alternativas, a resposta correta e a pontuação de cada questão.
- Exija uma porcentagem ou pontuação mínima para aprovação.
- Permita que o aluno refaça a prova um número definido de vezes.
- Vincule a nota obtida diretamente a uma avaliação no boletim do aluno.

**Avaliação por Envio de Anexo:**

- Solicite que o aluno envie um arquivo (ex: redação, resumo, trabalho).
- A avaliação deste envio é manual, realizada por um professor ou administrador.
- A nota atribuída também pode ser vinculada ao boletim do aluno.

**Conteúdo e Material de Apoio:**

- **Material da Aula:** Anexe arquivos de apoio como PDF, Word, PowerPoint, áudio (MP3), etc. Os arquivos são gerenciados através de uma biblioteca central, permitindo reutilizá-los em outras aulas ou cursos. O limite de upload por arquivo é de 700 MB.
- **Conteúdo da Aula:** Utilize o editor de texto para inserir o conteúdo principal, incluindo textos, imagens e vídeos. É possível incorporar vídeos do YouTube ou Vimeo; fazer o upload de um arquivo de vídeo (ex: MP4) para a biblioteca do sistema e incorporá-lo na aula. Vídeos hospedados no SIGA podem exibir uma marca d'água automática com o nome, código e data/hora de acesso do aluno.

## Portal do Aluno

Após a matrícula, o aluno recebe seus dados de acesso ao portal, onde pode gerenciar sua vida acadêmica.

### Funcionalidades do aluno

O aluno tem acesso a diversas funcionalidades, como:

- **Documentos Pendentes:** Visualizar e enviar arquivos de documentos exigidos pela instituição.
- **Financeiro:** Acompanhar cobranças, imprimir boletos e visualizar o extrato financeiro.
- **Atualização Cadastral:** Solicitar a alteração de dados pessoais (sujeito à aprovação administrativa).
- **Contrato:** Visualizar e imprimir o contrato de matrícula.
- **Boletim:** Acompanhar suas notas e o desempenho acadêmico.
- **EAD > Meus Cursos:** Ponto de acesso central para todos os cursos EAD em que está matriculado.

### Acesso e navegação no curso

Dentro da área do curso, o aluno visualiza uma lista de todas as aulas, com informações como:

- Status (não realizado, cursando, aprovado).
- Necessidade de avaliação (prova ou anexo).
- Botão de acesso à aula.

O sistema respeita as regras de requisito e liberação, exibindo aulas futuras como "indisponíveis" até que as condições sejam atendidas.

### Interação com a aula

Ao abrir uma aula, o aluno encontra:

- **Conteúdo e Vídeos:** O corpo principal da aula para estudo.
- **Material da Aula:** Links para baixar os arquivos de apoio.
- **Questionário:** Botão para iniciar a prova online, caso exista. O resultado é exibido imediatamente após a conclusão.
- **Avaliação por Anexo:** Campo para fazer o upload do arquivo solicitado.
- **Dúvidas:** Um formulário para enviar perguntas diretamente ao professor responsável pela aula.

O aluno deve clicar em "Finalizar Aula" para registrar seu progresso e, se for o caso, liberar a próxima aula da sequência.

## Acompanhamento e avaliações

O administrador possui ferramentas para monitorar e avaliar o progresso dos alunos.

### Gestão de aulas

Esta tela centraliza o acompanhamento (menu **EAD** / **Gestão de aulas**). É possível buscar por um aluno específico e visualizar o status de cada aula cursada por ele.

**Verificar Desempenho em Questionários:** É possível visualizar as respostas que o aluno deu em cada questão da prova, além da nota final obtida.

**Avaliar Envios de Anexos:**

1.  Clique para visualizar o arquivo enviado pelo aluno.
2.  Atribua um status ("Aprovado" ou "Reprovado") e uma nota.
3.  Escreva uma observação ou feedback para o aluno.
4.  Caso reprovado, defina se o aluno terá a permissão para reenviar o arquivo.

Após a avaliação manual, o status da aula é atualizado automaticamente no portal do aluno, liberando as aulas seguintes se os requisitos forem cumpridos.

## Conclusão

O módulo EAD do Sistema SIGA oferece um ecossistema completo para a gestão de cursos a distância. Com configurações robustas de controle de acesso, avaliações flexíveis e portais intuitivos para administradores e alunos, a plataforma se adapta às mais diversas necessidades pedagógicas e administrativas. Para funcionalidades específicas ou dúvidas não abordadas neste guia, entre em contato com a equipe de suporte através do [sistema de chamnados :octicons-link-external-16:](https://cliente.agenciavmc.net.br/).
