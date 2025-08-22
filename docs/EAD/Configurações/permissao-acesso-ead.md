# Permissões de acesso

??? abstract "Clique aqui e assista o vídeo"

    <iframe allow="autoplay; fullscreen" allowfullscreen="" frameborder="0" height="300" src="https://player.vimeo.com/video/663452654?h=8243f85cd8" width="640"></iframe>

## **Permissões para o Módulo EAD**

Este documento detalha o procedimento para configurar as permissões de acesso dos colaboradores às funcionalidades de Ensino a Distância (EAD) no sistema SIGA. Uma gestão adequada de permissões é fundamental para garantir a segurança e a correta operação do módulo.

## **1. Introdução ao Gerenciamento de Acessos**

Para que os usuários (colaboradores, coordenadores, etc.) possam gerenciar cursos, aulas e alunos no ambiente EAD, é necessário que seus perfis de acesso contenham as permissões apropriadas.

O sistema SIGA permite o gerenciamento de permissões de duas formas:

1.  **Via Perfis de Acesso:** Método recomendado, onde as permissões são configuradas em um perfil que pode ser atribuído a múltiplos usuários. Alterações no perfil são replicadas para todos os usuários vinculados.
2.  **Via Gestão de Usuários (Individual):** Permite alterar as permissões de um único usuário. Este método deve ser utilizado principalmente para conferência ou para exceções específicas, pois não garante a padronização.

> **Prática Recomendada:** Utilize sempre os **Perfis de Acesso** (`Administração > Perfis de Acesso`) para editar permissões. Isso garante consistência e facilita a manutenção, aplicando as mesmas regras a todos os colaboradores que desempenham a mesma função.

## **2. Configurando um Perfil de Acesso para o EAD**

O procedimento a seguir descreve como editar um perfil existente para incluir as permissões do módulo EAD.

### **2.1. Acessando os Perfis de Acesso**

1.  No menu lateral do sistema, navegue para `Administração > Perfis de Acesso`.
2.  O sistema listará todos os perfis cadastrados. Localize o perfil que deseja modificar (ex: "Perfil Colaborador") e clique em **Atualizar**.

### **2.2. Atribuindo Permissões Gerais de EAD**

1.  Dentro da tela de edição do perfil, utilize o campo **Filtro** e digite `EAD` para exibir todas as permissões relacionadas ao módulo.
2.  Marque as caixas de seleção correspondentes às funcionalidades que os usuários deste perfil poderão acessar.
3.  Analise a permissão específica: **"Permitir visualizar todos os arquivos da biblioteca ou somente os enviados pelo próprio usuário"**.
    - **Marcada:** O usuário poderá visualizar todos os arquivos da biblioteca, incluindo materiais enviados por outros professores e administradores. Recomendado para perfis de coordenação.
    - **Desmarcada:** O usuário visualizará apenas os arquivos (vídeos, documentos, etc.) que ele mesmo enviou.

### **2.3. Configurando a Permissão de Bloqueio de Renovação Manual**

O sistema possui uma permissão de segurança crítica para turmas EAD que operam com matrículas de vigência definida (ex: acesso por 6 meses).

- **Permissão:** `Bloquear alteração da vigência e renovação manual em matrículas onde a turma principal é turma EAD`.

**Funcionalidade:**

- **Se marcada (Bloqueio ATIVO):**

  - O colaborador com este perfil **não poderá** estender manualmente a data de vigência da matrícula de um aluno.
  - A renovação do acesso só poderá ser realizada pelo próprio aluno através do **Portal do Aluno**, via **Requerimento de Serviço**.
  - Neste fluxo, o sistema gera uma cobrança (ex: boleto de R$ 100,00) para o aluno. A renovação e a liberação do acesso por mais tempo são feitas **automaticamente** pelo sistema SIGA após a identificação do pagamento.
  - Este método aumenta a segurança financeira e a automação dos processos.

- **Se desmarcada (Bloqueio INATIVO):**
  - O colaborador com este perfil **poderá** renovar manualmente o acesso de um aluno, sem a necessidade de um processo financeiro atrelado via sistema.
  - Esta configuração pode abrir brechas para negociações financeiras não registradas e deve ser atribuída apenas a usuários de alta confiança (ex: perfil "Administrativo EAD").

Após definir as configurações desejadas, clique em **Salvar** para aplicar as alterações ao perfil.

## **3. Atribuindo o Perfil a Usuários**

Uma vez que o perfil de acesso esteja configurado, o passo final é atribuí-lo aos colaboradores correspondentes.

1.  Na tela de listagem de perfis (`Administração > Perfis de Acesso`), localize o perfil configurado.
2.  Na coluna **Usuários**, clique no ícone correspondente.
3.  A tela será dividida em duas colunas:
    - À esquerda, estarão listados todos os usuários cadastrados no sistema.
    - À direita, estarão os usuários que já utilizam este perfil.
4.  Para vincular um novo usuário, clique sobre o nome dele na lista da esquerda e, em seguida, clique no botão **Adicionar**.
5.  Após mover todos os usuários desejados para a coluna da direita, clique em **Salvar**.

Os usuários selecionados herdarão imediatamente todas as permissões configuradas no perfil e poderão acessar as funcionalidades do módulo EAD.

---

_Para dúvidas adicionais ou cenários específicos, entre em contato com o suporte do sistema._

---

## Manuais relacionados

- [Como utilizar/configurar perfis de acesso](http://manual.sistemasiga.net/2019/03/08/como-aplicar-perfil-de-acesso-para-colaboradores-limitacao-de-acesso-ao-menu-lateralfuncoes/)
