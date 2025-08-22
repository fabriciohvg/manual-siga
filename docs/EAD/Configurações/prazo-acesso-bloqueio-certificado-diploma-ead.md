# Acesso, prazo, bloqueio e certificados

??? abstract "Clique aqui e assista o vídeo"

    <iframe allow="autoplay; fullscreen" allowfullscreen="" frameborder="0" height="300" src="https://player.vimeo.com/video/663452654?h=8243f85cd8" width="640"></iframe>

## **Configuração Estrutural de um Curso EAD**

Este guia aborda as configurações fundamentais para estruturar um curso EAD no sistema SIGA. O processo é realizado dentro do cadastro do curso e envolve desde a definição do modelo de ensino até as regras de acesso, conclusão e certificação.

## **1. Estratégia de Cadastro do Curso: Presencial, EAD ou Semipresencial**

Antes de iniciar a configuração, é crucial definir a estratégia de cadastro com base na modalidade do curso.

- **Cursos com Variação (Presencial e EAD):**

  - **Cenário:** O mesmo curso (ex: Pedagogia) é oferecido em uma versão 100% presencial e outra 100% EAD, com matrizes curriculares, sistemas avaliativos ou cargas horárias distintas.
  - **Recomendação:** Crie **dois cadastros de curso separados** (ex: "Pedagogia" e "Pedagogia EAD"). Essa abordagem simplifica a gestão de turmas, matrículas e relatórios pedagógicos, mantendo cada modalidade isolada.

- **Cursos Semipresenciais:**

  - **Cenário:** O curso possui uma única matriz curricular que mescla disciplinas presenciais e online.
  - **Recomendação:** Utilize um **único cadastro de curso**. A estrutura unificada reflete a jornada do aluno, que cursará ambas as modalidades dentro da mesma matrícula.

- **Cursos Exclusivamente Presenciais ou EAD:**
  - **Recomendação:** Utilize um **único cadastro** para cada curso, focado na sua respectiva modalidade.

> **Nota:** Este manual foca exclusivamente na configuração de cursos na modalidade EAD. Para detalhes sobre cursos presenciais, consulte a documentação específica.

## **2. Ativação e Configurações Iniciais do Módulo EAD**

### **2.1. Pré-requisitos**

Antes de configurar a aba EAD, certifique-se de que as seguintes seções do cadastro do curso já estão devidamente preenchidas:

- Dados gerais (nome, duração, carga horária).
- Dados financeiros e pedagógicos.
- **Matriz Curricular:** As disciplinas do curso devem estar cadastradas e organizadas.
- Sistema Avaliativo.

### **2.2. Ativando a Funcionalidade EAD**

1.  Acesse `Cursos > Gestão de Cursos` e abra o cadastro do curso desejado.
2.  Na aba principal, localize a opção **"Tem aulas EAD?"** e altere seu valor para **"Sim"**.
3.  Salve a alteração. A aba lateral **"EAD"** será habilitada.
4.  Acesse a aba **EAD > Configurações**.

## **3. Detalhamento das Configurações EAD**

Esta seção aborda cada campo da aba "Configurações" do módulo EAD.

### **3.1. Disponibilidade e Apresentação Visual**

- **Disponível para Compra/Matrícula Online:**
  - **Sim:** O curso poderá ser incluído na "Matrícula Web", permitindo que alunos se inscrevam de forma autônoma.
  - **Não:** A matrícula de alunos neste curso deverá ser realizada exclusivamente de forma manual por um funcionário.
- **Informações Visuais:** Os campos a seguir (categoria, imagem, slides, resumo, etc.) são utilizados para apresentar o curso de forma atrativa na plataforma. Eles não impactam o funcionamento técnico das aulas.

### **3.2. Regras de Acesso e Suporte**

- **Período de Acesso ao Curso (em dias):**
  - Define por quanto tempo o aluno poderá acessar o conteúdo do curso, contados a partir da data de matrícula.
  - Este valor é independente da duração oficial do curso ou da vigência da matrícula.
    - **Exemplo:** Um curso com duração de 3 meses (90 dias) pode ter um período de acesso de 180 dias, permitindo que o aluno revise o conteúdo por mais 3 meses após o término.
  - Para conceder **acesso vitalício**, insira o valor `0`.
- **Período de Suporte ao Curso (em dias):**
  - Define o período em que o aluno poderá enviar dúvidas e interagir com os professores. A lógica de contagem é a mesma do período de acesso.

> **Importante:** O sistema sempre considerará o maior prazo entre a **vigência da matrícula** e o **período configurado (acesso/suporte)**. Se a matrícula for vigente por 90 dias e o período de acesso for de 30 dias, o aluno terá acesso por 90 dias. Se o período de acesso for de 180 dias, ele terá acesso por 180 dias.

### **3.3. Bloqueio por Inadimplência Financeira**

- Configure o bloqueio automático de acesso ao curso para alunos com pendências financeiras.
- **Número de Parcelas Vencidas:** Defina a quantidade de parcelas em atraso que acionará o bloqueio (ex: `1` ou `2`).
- **Dias de Vencimento:** Defina o número de dias após o vencimento para que a regra seja aplicada (ex: `10` dias).
- Para **desativar** o bloqueio, insira o valor `0` no campo de parcelas.

### **3.4. Regra de Conclusão do Curso**

Selecione o critério que o sistema utilizará para determinar se um aluno concluiu o curso com sucesso.

- **Regra 1: Notas Lançadas em Todas as Disciplinas:**
  - O aluno é considerado finalizado quando tiver uma nota (ou status) em todas as disciplinas da sua matriz curricular.
  - O sistema então calculará o resultado final (aprovado/reprovado) com base nas médias obtidas e no sistema avaliativo do curso.
- **Regra 2: Finalização de Todas as Aulas EAD:**
  - O aluno é considerado finalizado ao concluir todas as aulas EAD em que está habilitado.
  - O sistema verificará o status final em cada aula (que pode depender de provas internas da aula) para definir a aprovação no curso. Esta regra é útil para cursos que não têm uma estrutura formal de disciplinas.
- **Regra 3: Sempre Aprovar ao Finalizar as Aulas:**
  - O aluno será automaticamente considerado **aprovado** assim que concluir a última aula EAD.
  - Esta regra ignora notas e disciplinas, sendo ideal para cursos livres, de participação ou que não possuem avaliações formais.

### **3.5. Documento de Conclusão (Certificado)**

- **Vincular Certificado:** Selecione um modelo de documento (previamente cadastrado) que será emitido como certificado de conclusão.
- **Cadastro do Modelo:** Os modelos de certificado são criados e gerenciados em `Documentos e Impressão > Gestão de Modelos`. Utilize campos dinâmicos para personalizar o certificado com informações do aluno e do curso (nome, carga horária, data, assinatura digital, etc.).
- **Emissão pelo Aluno:** Uma vez que o aluno atenda à regra de conclusão definida, um botão para imprimir o certificado será exibido automaticamente em seu portal (`EAD > Meus Cursos`), permitindo a emissão autônoma e 100% online.
