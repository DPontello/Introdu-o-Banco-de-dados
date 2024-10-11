 Defina: banco de dados, sistema de banco de dados e sistema de gerência de banco de
dados.
2. (a) Cite algumas das informações armazenadas no catálogo do sistema, chamadas de
metadados.
(b) Mostre um exemplo dessas informações.
(c) Como essas informações são armazenadas em um sistema de arquivos tradicional?
3. Quatro características importantes da abordagem de banco de dados são: redução de
redundância de dados, abstração de dados, suporte a múltiplas visões de dados e
isolamento entre programas e dados. Descreva as vantagens proporcionadas por essas
características em relação à abordagem tradicional de sistemas em arquivos.
4. Dê um exemplo de visão de dados.
5. Dê um exemplo de um problema que poderia acontecer se o SGBD não possuísse um
controle de concorrência.
6. Explique, através de um exemplo, o que é redundância de dados e quais são os
problemas que isso pode gerar.
7. Cite alguns exemplos de restrições de integridade.
8. Diferencie modelo de dados, esquema e instância. Dê exemplos de cada um deles.
9. Descreva a arquitetura de três níveis (ANSI/SPARC) de um sistema de banco de dados.
Explique como essa arquitetura proporciona a independência de dados.
10. Dê exemplos de mudanças no banco de dados que continuam a manter a independência
de dados lógica e a independência de dados física.
11. Descreva os componentes básicos de um sistema de gerência de banco de dados.
12. Explique as principais fases de um projeto de banco de dados: coleta e análise de
requisitos, projeto conceitual, projeto lógico e projeto físico.
13. Faça os Exercícios (e Perguntas de Revisão) do livro texto (Elmasri & Navathe) dos
Capítulos 1 e 2.


## RESPOSTAS

1- Banco de dados: Coleção de dados relacionados que seguem as seguintes propriedades implícitas -> 01- representa algum aspecto do mundo real / 02- é uma coleção logica e coerente dos dados / 03- é projetado, construído para um proposito especifico.
Sistema de banco de dados: Refere-se ao conjunto completo, incluindo tanto o SGBD quanto o bando de dados(dados e estruturas).
Sistema de gerencia de banco de dados (SGBD): é um software de proposito geral que facilita processos de definição, construção, manipulação e compartilhamento de banco de dados. Ou seja é um coleção de programas que visam ao usuário criar e manter um banco de dados.

2- a) Metadados são a explicação do que cada dado representa. Isso é, em um banco de dados, "nome" é um metadado que auxilia no entendimento do dado "hugo". Alguns outros exemplos são: Nome das tabelas, nome dos atributos, tipo
b) Estudante 
	Nome/CódigoEstudante/tipoAluno/DepartamentoPrincipal
   Disciplina
	Nome/CodigoDisciplina/Creditos/departamento
c)Cada usuário define e implementa os arquivos necessários para uma aplicação de software específica como parte da programação da aplicação. Exemplo: Em um hospital, a secretária e o médico podem ter necessidades diferentes em relação aos dados dos pacientes, levando à criação de arquivos separados.


3- redução de redundância de dados: projeto que armazena cada item de dados lógico - como o nome ou a data de nascimento de um aluno - em apenas um lugar no banco de dados. O que faria que uma mudança não precisaria ser alterada em dois locais.
abstração de dados: o modelo de dados oculta (isto é, abstrai) os detalhes de armazenamento e implementação que não são do interesse da maioria dos usuários de banco de dados.
suporte a múltiplas visões de dados: Isso inclui linguagens de consulta para usuários casuais, interfaces de programação para desenvolvedores de aplicações, e interfaces gráficas (GUIs), como formulários e menus, para usuários que preferem uma interação mais visual e simplificada. Ou seja oferece vantagem em como cada usuário pretende usar o banco de dados.
isolamento entre programas e dados: No processamento de arquivos tradicional, a estrutura dos arquivos de dados está embutida nos programas de aplicação, assim, se houver uma mudança nessa estrutura, pode haver uma exigência de mudança em todos os programas que acessam esse arquivo. Já em programas que acessam o SGBD isso é mais incomum, visto que a estrutura dos arquivos de dados é armazenada no catálogo (separadamente dos programas de acesso).


4- Por exemplo, uma secretaria que agenda consultas para pacientes precisa de saber de informações de contato, como, onde mora, numero de contato entre outros já o próprio medico não precisa dessas informações.


5- 