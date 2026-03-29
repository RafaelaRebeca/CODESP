# Documento de Visão

## Histórico de Revisões

| Data | Versão | Descrição | Autores |
| :--: | :----: | :-------: | :-----: |
| 29/03 | 1.0 | Versão inicial | Igor |
| - | - | - | - |

---

## 1. Visão Geral do Sistema Proposto

O sistema proposto consiste em um aplicativo mobile para gerenciamento de inscrições em turmas esportivas do IFRN. A solução visa substituir o processo manual atualmente realizado por meio de planilhas e atendimento presencial, proporcionando maior eficiência, transparência e acessibilidade.

A aplicação permitirá que estudantes realizem inscrições de forma remota, acompanhem o status de suas vagas e visualizem sua posição em listas de espera. Além disso, o sistema fornecerá aos gerentes ferramentas para criação e administração de turmas, controle de vagas e acompanhamento de inscritos.

---

## 2. Visão Geral do Produto

O produto será um aplicativo mobile que permitirá a digitalização completa do processo de inscrição em atividades esportivas institucionais.

Ele terá como principais características:
- Acesso remoto às inscrições
- Controle automático de vagas
- Lista de espera com atualização em tempo real
- Transparência para os estudantes
- Facilidade de gerenciamento para os administradores

O sistema será projetado para ser simples, intuitivo e acessível, reduzindo erros humanos e eliminando a necessidade de processos presenciais.

---

## 3. Descrição do Problema

| - | - |
| :-: | :-: |
| **Problema** | Processo manual de inscrição em turmas esportivas utilizando planilhas e atendimento presencial |
| **Afeta** | Estudantes e gerentes responsáveis pelas turmas |
| **Impacta** | Falta de transparência, dificuldade no controle de vagas, erros humanos, ausência de comunicação eficiente |
| **Solução** | Desenvolvimento de um aplicativo mobile para automatizar inscrições, gerenciar listas de espera e melhorar a comunicação |

---

## 4. Descrição dos Usuários 

| Usuário | Descrição | Responsabilidades |
| :-----: | :-------: | :--------------: |
| Sistema | Plataforma digital de gerenciamento | Processar inscrições, controlar vagas e listas de espera |
| Estudante | Aluno do IFRN interessado em participar de atividades esportivas | Realizar cadastro, inscrever-se em turmas e acompanhar status |
| Gerente | Responsável pela gestão das turmas esportivas | Criar turmas, gerenciar inscritos e controlar vagas |

---

## 5. Descrição do Ambiente dos Usuários

| Usuário | Ambiente operacional |
| :-----: | :------------------: |
| Estudante | Dispositivos móveis (smartphones) com acesso à internet |
| Gerente | Computadores ou dispositivos móveis com acesso à internet |

---

## 6. Principais Necessidades dos Usuários

1. **Estudante**
   - Realizar inscrição online em turmas esportivas
   - Visualizar status da inscrição
   - Acompanhar posição na lista de espera
   - Receber informações atualizadas sobre vagas

2. **Gerente**
   - Criar e gerenciar turmas
   - Definir quantidade de vagas
   - Visualizar lista de inscritos
   - Controlar desistências e movimentação da lista de espera

---

## 7. Alternativas Concorrentes

1. **Planilhas (Excel/Google Sheets)**
   - **Pontos fortes:**
     - Fácil de usar
     - Baixo custo
     - Amplamente conhecido
   - **Pontos fracos:**
     - Alto risco de erros manuais
     - Falta de atualização em tempo real para os alunos
     - Baixa transparência
     - Dificuldade de controle de lista de espera

2. **Inscrição presencial**
   - **Pontos fortes:**
     - Contato direto com o responsável
     - Simplicidade no processo inicial
   - **Pontos fracos:**
     - Necessidade de deslocamento
     - Falta de praticidade
     - Informação não acessível posteriormente
     - Problemas de comunicação sobre mudanças

---

## 8. Regras de Negócio

| ID  | Regra | Descrição |
| :-: | :---: | :-------: |
| RN01 | Limite de inscrições | Cada estudante pode se inscrever em no máximo 3 turmas |
| RN02 | Ordem de inscrição | As vagas são preenchidas por ordem de chegada |
| RN03 | Lista de espera | Alunos excedentes são inseridos automaticamente em lista de espera |
| RN04 | Promoção automática | Quando uma vaga é liberada, o próximo da lista de espera é promovido |
| RN05 | Dados obrigatórios | O cadastro do estudante deve conter matrícula, CPF e telefone |
| RN06 | Controle de vagas | Cada turma possui um número máximo de vagas definido pelo gerente |

---

## 9. Requisitos Funcionais

### 9.1 Cadastro e Autenticação

| Código | Nome | Descrição | Prioridade |
| :----: | :--: | :-------: | :--------: |
| RF01 | Cadastro de usuário | Permitir que o estudante se cadastre no sistema | Alta |
| RF02 | Autenticação | Permitir login de usuários | Alta |

---

### 9.2 Gerenciamento de Turmas

| Código | Nome | Descrição | Prioridade |
| :----: | :--: | :-------: | :--------: |
| RF03 | Visualizar turmas | Exibir turmas disponíveis e lotadas | Alta |
| RF04 | Criar turma | Permitir que o gerente crie novas turmas | Alta |

---

### 9.3 Inscrição

| Código | Nome | Descrição | Prioridade |
| :----: | :--: | :-------: | :--------: |
| RF05 | Inscrição em turma | Permitir inscrição em turmas | Alta |
| RF06 | Lista de espera | Inserir automaticamente em lista de espera quando não houver vagas | Alta |
| RF07 | Cancelar inscrição | Permitir desistência da turma | Média |

---

### 9.4 Acompanhamento

| Código | Nome | Descrição | Prioridade |
| :----: | :--: | :-------: | :--------: |
| RF08 | Visualizar status | Permitir ao aluno visualizar sua situação na turma | Alta |
| RF09 | Visualizar posição | Mostrar posição na lista de espera | Alta |

---

### 9.5 Administração

| Código | Nome | Descrição | Prioridade |
| :----: | :--: | :-------: | :--------: |
| RF10 | Gerenciar inscritos | Permitir visualizar e gerenciar inscritos | Média |

---

## 10. Requisitos Não-funcionais

| Código | Nome | Descrição | Categoria | Classificação |
| :----: | :--: | :-------: | :-------: | :-----------: |
| NF01 | Usabilidade | Interface simples e intuitiva para os usuários | Usabilidade | Obrigatório |
| NF02 | Disponibilidade | Sistema disponível 24/7 | Confiabilidade | Obrigatório |
| NF03 | Desempenho | Resposta rápida nas operações de inscrição | Performance | Obrigatório |
| NF04 | Segurança | Proteção dos dados pessoais dos usuários (CPF, telefone) | Confiabilidade | Obrigatório |
| NF05 | Compatibilidade | Funcionar em diferentes dispositivos móveis | Suportabilidade | Desejável |
| NF06 | Escalabilidade | Suportar múltiplos usuários simultaneamente | Performance | Desejável |

---
