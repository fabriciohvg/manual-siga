# Documentos obrigatórios

??? abstract "Clique aqui e assista o vídeo"

    <iframe loading="lazy" allow="autoplay; fullscreen" allowfullscreen="" frameborder="0" height="300" src="https://player.vimeo.com/video/663456426?h=8ef5fd93e9" width="640"></iframe>

## **Documentos Obrigatórios do Aluno**

Este documento descreve o processo completo para cadastrar, configurar e gerenciar os documentos obrigatórios que os alunos devem entregar à instituição. O sistema SIGA permite centralizar essa gestão e automatizar o recebimento de arquivos através do Portal do Aluno.

## **1. Visão Geral**

A funcionalidade de Documentos Obrigatórios permite:

- Criar uma biblioteca central com todos os documentos que a instituição pode solicitar.
- Definir regras específicas para cada documento, como a permissão para envio online.
- Atribuir documentos específicos para cada curso oferecido.
- Automatizar o recebimento e a aprovação de documentos enviados pelos alunos.
- Configurar bloqueios no Portal do Aluno com base na pendência de documentos críticos, como o contrato de matrícula assinado.

O processo é dividido em duas etapas principais:

1.  **Cadastro e Configuração Global:** Criação da lista mestre de todos os documentos possíveis.
2.  **Atribuição ao Curso:** Seleção dos documentos da lista mestre que se aplicam a um curso específico.

## **2. Etapa 1: Cadastro e Configuração dos Documentos (Biblioteca Central)**

Nesta etapa, você criará uma lista com todos os documentos que sua instituição pode vir a exigir, independentemente do curso.

### **2.1. Acessando o Módulo**

1.  No menu lateral, navegue para `Cursos > Documentos Obrigatórios`.
2.  Nesta tela, você pode cadastrar um novo documento ou editar um já existente clicando em **Atualizar**.

### **2.2. Configurando um Documento**

Ao cadastrar ou atualizar um documento, as seguintes opções estão disponíveis:

- **Nome do Documento:** O título que será exibido para o administrador e para o aluno (ex: "CPF", "Comprovante de Endereço", "Contrato de Matrícula Assinado").
- **Modelo/Formulário de Referência:** Permite anexar um arquivo (PDF, imagem, etc.) como modelo.
  - **Uso 1 (Explicativo):** Anexe uma imagem explicando como o documento deve ser enviado (ex: foto da CNH aberta).
  - **Uso 2 (Formulário):** Anexe um formulário que o aluno deve baixar, preencher e reenviar.
- **Permitir Envio via Anexo (Portal do Aluno):**
  - **Sim:** O aluno poderá enviar o arquivo (foto ou scan) diretamente pelo Portal do Aluno.
  - **Não:** O aluno será informado da pendência, mas não terá a opção de envio online, devendo entregar o documento presencialmente ou por outros meios.
- **Mensagem de Instrução para o Aluno:** Um campo de texto para fornecer instruções claras sobre o envio (ex: "O arquivo deve estar nítido e legível", "Envie todas as páginas em um único arquivo PDF").

## **3. Etapa 2: Configurações Avançadas e de Bloqueio**

Para documentos críticos, é possível configurar regras de bloqueio que afetam a experiência do aluno no portal.

### **3.1. Limitar o Acesso ao Portal do Aluno**

- **Opção:** `A pendência deste documento limita o acesso ao portal do aluno?`
  - **Sim:** Enquanto este documento estiver pendente (não enviado ou não aprovado pelo administrador), o aluno terá o acesso a funcionalidades-chave do portal (como EAD, boletim, comunicados) bloqueado.
  - **Não:** A pendência do documento será exibida, mas não impedirá o aluno de utilizar o portal normalmente.

### **3.2. Caso de Uso: O Contrato de Matrícula Assinado**

Esta é a aplicação mais comum para a funcionalidade de bloqueio. O objetivo é garantir que o aluno só tenha acesso total ao curso após devolver o contrato devidamente assinado.

**Configuração Recomendada:**

1.  **Crie o Documento Obrigatório:** Cadastre um documento com o nome "Contrato de Matrícula Assinado".
2.  **Habilite o Envio Online:** Marque a opção para que o aluno possa enviar o arquivo.
3.  **Ative o Bloqueio:** Na opção `Limitar o acesso ao portal do aluno?`, selecione **Sim**.
4.  **Vincule o Modelo de Contrato:** No campo `Documento Vinculado`, selecione o modelo de contrato correspondente (ex: "Contrato de Matrícula").

> **Nota Importante:** A opção `Documento Vinculado` garante que, mesmo com o portal limitado, o aluno ainda consiga acessar e imprimir o modelo de contrato que precisa assinar. Sem esse vínculo, ele não conseguiria obter o documento para cumprir a pendência.

## **4. Etapa 3: Atribuição de Documentos a um Curso Específico**

Após configurar a biblioteca de documentos, o próximo passo é definir quais deles são exigidos para cada curso.

1.  Navegue para `Cursos > Gestão de Cursos`.
2.  Localize o curso desejado (ex: "Pedagogia EAD") e abra seu cadastro.
3.  Role a tela até a seção **"Documentos obrigatórios para este curso"**.
4.  Marque a caixa de seleção de todos os documentos que os alunos matriculados neste curso deverão entregar.
5.  Salve as alterações.

### **4.1. Vinculando o Modelo de Contrato para Impressão**

Para que o aluno possa imprimir o contrato correto, é preciso vincular o modelo de documento ao curso:

1.  Dentro do cadastro do curso, localize a seção **"Reconhecimento documentação do curso"**.
2.  No campo **"Permitir que o aluno imprima o contrato através do painel do aluno?"**, selecione o modelo de documento de contrato correspondente (ex: "Contrato de Matrícula - Pedagogia").

> **Lembrete:** Os modelos de contrato são criados e editados no menu `Documentos e Impressões > Gestão de Modelos`. É possível ter um modelo de contrato diferente para cada curso.

## **5. Etapa 4: Acompanhamento e Aprovação dos Envios**

Quando um aluno envia um documento ou solicita uma atualização cadastral, a administração é notificada para realizar a aprovação.

- **Central de Aprovações:** Todas as submissões dos alunos ficam centralizadas no menu `Alunos > Atualização Cadastral`.
- **Fluxo de Aprovação:** Nesta tela, o administrador pode visualizar o arquivo enviado pelo aluno, aprovar o documento (marcando a pendência como resolvida) ou reprová-lo, caso não esteja em conformidade.

Após a aprovação de um documento que limitava o acesso, o portal do aluno é liberado automaticamente.

Manuais relacionados:

- [Como limitar o portal do aluno para alunos que não enviarem determinados documentos obrigatórios](http://manual.sistemasiga.net/2019/11/21/como-limitar-o-portal-do-aluno-para-alunos-que-nao-enviarem-determinados-documentos-obrigatorios/)

- [Como exibir no painel do aluno/responsável documentos obrigatórios pendentes/não entregues](http://manual.sistemasiga.net/2018/10/02/como-exibir-no-painel-do-alunoresponsavel-documentos-obrigatorios-pendentesnao-entregues/)

- [Cadastrar/vincular documentos necessários/obrigatórios para matrícula em curso](http://manual.sistemasiga.net/2017/03/14/documentos-necessarios-matricula/)

- [Como permitir que alunos atualizem dados pessoais, ou enviem documentos pendentes, para posterior aprovação](http://manual.sistemasiga.net/2019/08/21/como-permitir-que-alunos-atualizem-dados-pessoais-ou-enviem-documentos-pendentes-para-posterior-aprovacao/)
