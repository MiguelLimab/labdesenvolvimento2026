# labdesenvolvimento2026

## Histórias de Usuário

### US01 - Fazer Login

**Como** usuário do sistema (aluno, professor ou secretaria),  
**Quero** realizar login com minha senha,  
**Para que** eu possa acessar as funcionalidades do sistema de matrículas de acordo com meu perfil.

**Critérios de Aceitação:**
- O sistema deve validar o login e a senha do usuário.
- Caso as credenciais sejam inválidas, o sistema deve exibir uma mensagem de erro.
- Após o login, o sistema deve direcionar o usuário para a tela correspondente ao seu perfil (aluno, professor ou secretaria).

---

### US02 - Gerar Currículo do Semestre

**Como** secretaria da universidade,  
**Quero** gerar o currículo para cada semestre,  
**Para que** as disciplinas, professores e informações acadêmicas estejam organizadas e disponíveis para o período letivo.

**Critérios de Aceitação:**
- O currículo deve conter as disciplinas oferecidas no semestre, com seus respectivos professores.
- Cada disciplina deve estar vinculada a um curso.
- O sistema deve permitir a definição do período de matrículas associado ao semestre.

---

### US03 - Manter Informações de Disciplinas

**Como** secretaria da universidade,  
**Quero** cadastrar, editar e remover disciplinas,  
**Para que** o sistema mantenha as informações acadêmicas atualizadas.

**Critérios de Aceitação:**
- Cada disciplina deve possuir nome, número de créditos e estar vinculada a um curso.
- Deve ser possível associar um professor a uma disciplina.
- O sistema deve impedir a exclusão de disciplinas que possuam alunos matriculados.

---

### US04 - Manter Informações de Professores

**Como** secretaria da universidade,  
**Quero** cadastrar, editar e remover professores,  
**Para que** o corpo docente esteja registrado corretamente no sistema.

**Critérios de Aceitação:**
- O cadastro do professor deve conter nome, senha e demais dados necessários.
- Deve ser possível vincular professores a disciplinas.

---

### US05 - Manter Informações de Alunos

**Como** secretaria da universidade,  
**Quero** cadastrar, editar e remover alunos,  
**Para que** os dados dos estudantes estejam atualizados no sistema.

**Critérios de Aceitação:**
- O cadastro do aluno deve conter nome, matrícula, curso, senha e demais dados necessários.
- O aluno deve estar vinculado a um curso.

---

### US06 - Realizar Matrícula em Disciplinas

**Como** aluno,  
**Quero** me matricular em disciplinas durante o período de matrículas,  
**Para que** eu possa cursar as disciplinas no próximo semestre.

**Critérios de Aceitação:**
- O aluno só pode realizar matrícula durante o período de matrículas definido.
- O aluno pode se matricular em até **4 disciplinas obrigatórias** (1ª opção) e até **2 disciplinas optativas**.
- O sistema deve impedir a matrícula caso a disciplina já tenha atingido o limite de **60 alunos**.
- Após a matrícula, o **sistema de cobranças** deve ser notificado para que o aluno seja cobrado pelas disciplinas do semestre.

---

### US07 - Cancelar Matrícula em Disciplina

**Como** aluno,  
**Quero** cancelar matrículas feitas anteriormente durante o período de matrículas,  
**Para que** eu possa ajustar minha grade de disciplinas conforme necessário.

**Critérios de Aceitação:**
- O cancelamento só pode ser realizado durante o período de matrículas.
- O sistema deve atualizar a contagem de alunos matriculados na disciplina após o cancelamento.
- O sistema de cobranças deve ser notificado sobre o cancelamento.

---

### US08 - Consultar Alunos Matriculados

**Como** professor,  
**Quero** consultar quais alunos estão matriculados em cada disciplina que leciono,  
**Para que** eu possa organizar minhas aulas e conhecer meus alunos.

**Critérios de Aceitação:**
- O professor deve visualizar a lista de alunos matriculados por disciplina.
- A consulta deve estar disponível somente após o login do professor.

---

### US09 - Ativar ou Cancelar Disciplina ao Final do Período de Matrículas

**Como** secretaria da universidade,  
**Quero** que o sistema verifique, ao final do período de matrículas, se cada disciplina atingiu o número mínimo de alunos,  
**Para que** disciplinas com menos de 3 alunos sejam canceladas e somente disciplinas viáveis prossigam no semestre.

**Critérios de Aceitação:**
- Uma disciplina só fica **ativa** se tiver pelo menos **3 alunos matriculados** ao final do período de matrículas.
- Disciplinas com menos de 3 alunos devem ser **canceladas** automaticamente.
- Alunos matriculados em disciplinas canceladas devem ser notificados.

---

### US10 - Notificar Sistema de Cobranças

**Como** sistema de matrículas,  
**Quero** notificar o sistema de cobranças após a inscrição de um aluno,  
**Para que** o aluno possa ser cobrado pelas disciplinas do semestre.

**Critérios de Aceitação:**
- A notificação deve ser enviada ao sistema de cobranças após a confirmação da matrícula.
- A notificação deve conter os dados do aluno e as disciplinas nas quais está matriculado.
