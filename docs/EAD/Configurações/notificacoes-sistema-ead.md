# Notificações de conclusão

??? abstract "Clique aqui e assista o vídeo"

    <iframe allow="autoplay; fullscreen" allowfullscreen="" frameborder="0" height="300" src="https://player.vimeo.com/video/663452654?h=8243f85cd8" width="640"></iframe>

## **Configurando Notificações por E-mail para Conclusão de Curso EAD**

Este documento detalha o procedimento para configurar o envio automático de notificações por e-mail sempre que um aluno concluir um curso na modalidade EAD. Esta funcionalidade é útil para alertar a equipe administrativa ou pedagógica sobre a necessidade de realizar ações subsequentes, como a emissão de históricos ou a preparação de documentos.

## **1. O Papel Fundamental da "Regra de Conclusão"**

É crucial compreender que o disparo da notificação por e-mail está diretamente vinculado à **"Regra de Conclusão"** definida nas configurações do curso. O sistema utilizará este critério para determinar o momento exato em que um aluno é considerado "concluído".

A seguir, detalhamos cada uma das regras disponíveis:

### **Regra 1: "Se estiver com todas as notas lançadas em todas as disciplinas..."**

- **Lógica:** O sistema verifica a matriz curricular do curso (`Aba Pedagógico > Ver matriz`) e confirma se o aluno possui uma nota lançada em **todas as disciplinas** listadas.
- **Condição Adicional:** Além de ter as notas, o aluno deve ter atingido a média mínima para aprovação em cada uma dessas disciplinas. A média exigida pode ser consultada no **Sistema Avaliativo** vinculado ao curso.
- **Aplicação:** Ideal para cursos com uma estrutura curricular formal, incluindo cursos semipresenciais onde as notas de disciplinas presenciais também precisam ser lançadas para que a conclusão seja validada.

### **Regra 2: "Ao finalizar todas as aulas EAD em que o aluno está habilitado"**

- **Lógica:** O sistema verifica se o aluno completou 100% das aulas EAD designadas para ele.
- **Condição Adicional:** O status do aluno em cada uma dessas aulas deve ser "Aprovado". A aprovação em uma aula pode depender da obtenção de uma nota mínima em avaliações internas da própria aula.
- **Aplicação:** Recomendado para cursos totalmente online ou cursos que não se baseiam em uma matriz de disciplinas tradicional, mas sim em uma sequência de aulas com avaliações próprias.

### **Regra 3: "Sempre aprovar ao finalizar todas as aulas..."**

- **Lógica:** O sistema verifica unicamente se o aluno completou 100% das aulas EAD.
- **Condição Adicional:** Nenhuma. O sistema **não** verifica notas, médias ou status de aprovação em aulas ou disciplinas. A simples finalização de todas as aulas é suficiente para acionar a conclusão.
- **Aplicação:** Perfeito para cursos livres, de participação ou que não possuem um sistema de avaliação formal.

## **2. Passo a Passo para Configuração da Notificação**

1.  No menu lateral, navegue para `Cursos > Gestão de Cursos`.
2.  Localize o curso EAD que deseja configurar e clique em **Atualizar**.
3.  Acesse a aba **EAD**.
4.  Dentro da sub-aba **Configurações**, localize o campo **"Notificar conclusão de alunos"**.
5.  Insira um ou mais endereços de e-mail que deverão receber a notificação. Para múltiplos e-mails, separe-os por vírgula.
6.  Revise a **"Regra de Conclusão"** selecionada para garantir que ela corresponda ao critério desejado para o disparo do e-mail.
7.  Clique em **Alterar** no final da página para salvar as configurações.

## **3. Método Alternativo: Consulta Manual de Alunos Aprovados**

Além da notificação automática, é possível gerar relatórios de alunos que concluíram o curso em um determinado período.

1.  No menu lateral, navegue para `Matrículas > Gestão de Matrículas`.
2.  Utilize os filtros para selecionar o curso EAD desejado.
3.  Localize o filtro **"Com data de aprovação entre"** e defina o intervalo de datas (inicial e final) que deseja consultar.
4.  O sistema listará todos os alunos que foram aprovados no curso dentro do período especificado.

Este método é útil para auditorias e para gerar listas consolidadas de concluintes (mensais, semanais, etc.).

---

_Para dúvidas adicionais, entre em contato com o suporte do sistema._
