# Equipe-Zafra-PI
Projeto Interdisciplinar do curso de Desenvolvimento de Software Multiplataforma - Fatec Jahu
<br/><br/>

<p>Grupo 7</p>
<p>Ana Luisa Zaratin Fria</p>
<p>Arthur Canzian</p>
<p>Leandro Prado de Mello Gusmão</p>
<p>Luiz Henrique de Araújo</p>
<p>Renan de Azevedo e Silva</p>
<br/><br/>

<p align="left" style="font-size:28px;"><strong><em>Documentação do PI</em></strong></p>
<details>
  <summary><strong>📑 Sumário</strong></summary>

- [1. Introdução](#1-introdução)
  - [Objetivos](#-objetivos)
  - [Metodologia](#-metodologia)
- [2. Requisitos](#2-requisitos)
  - [Requisitos funcionais](#-requisitos-funcionais)
  - [Requisitos não funcionais](#-requisitos-não-funcionais)
- [3. Modelo de casos de uso](#3-modelo-de-casos-de-uso)
- [4. Modelo do banco de dados](#4-modelo-do-banco-de-dados)
- [5. Banco de dados](#5-banco-de-dados)
- [6. Diagrama de classes](#6-diagrama-de-classes)
- [7. Estudo de viabilidade](#7-estudo-de-viabilidade)
- [8. Regras de negócio (Modelo canvas)](#8-regras-de-negócio-modelo-canvas)
- [9. Design](#9-design)
- [10. Protótipo](#10-protótipo)
- [11. Aplicação](#11-aplicação)

</details>

Para cada semestre, do 1º ao 6º, iremos utilizar este template para documentar o PI - incrementalmente.

# 1. Introdução
O Projeto descreve o desenvolvimento de um portal acadêmico para a Escola Zafra, fundada em 2025. O projeto visa disponibilizar ferramentas para a criação auxiliar a gestão da escola e a captação e alunos.
Como uma instituição de fundação recente, a Escola Zafra identifica a necessidade estratégica de implementar uma infraestrutura tecnológica própria, tornando essencial a transição para uma plataforma digital personalizada.
Com base nisso, o sistema busca:
- Facilitar o processo de inscrição e cadastro de alunos
- Oferecer ferramentas para a criação e gerenciamento de atividades acadêmicas, questionários e testes vocacionais
- ⁠Providenciar um canal de comunicação entre alunos e o corpo docente da escola

## • Objetivos
Criar uma plataforma website que seja gratuita e voltada à educação, captação e inclusão de pessoas, realocando-as para o mercado de trabalho.  Criação de um site básico, bem elaborado, responsivo e funcional para poder gerenciar todas as etapas da capacitação.

## • Metodologia
(Que métodos, tecnologias, modelos de processo, ferramentas irá utilizar?  
Responde à pergunta: Como? Com o que? Onde? Quando?)  

O desenvolvimento seguirá uma abordagem incremental, acompanhando os semestres do curso e sprints do P.I. O protótipo inicial será um site responsivo, baseado em materiais e aprendizagens em sala de aula, e terá como principais funções o login de aluno, funcionário ou administrador; gestão de alunos e controle de materiais de sala de aula.

# 2. Requisitos

Documento de requisitos de um sistema é um documento essencial que descreve os requisitos funcionais e não funcionais de um projeto de software. Serve como um modelo para o design, desenvolvimento e implementação do sistema, garantindo que todas as partes interessadas, desde analistas de negócios e desenvolvedores até usuários finais, tenham uma compreensão clara dos objetivos e escopo do sistema.

## • Requisitos funcionais
Atores do sistema: administrador (responsável pela gestão completa da plataforma), professor/voluntário (responsável por ministrar cursos e acompanhar os alunos), aluno (usuário que se inscreve e participa dos cursos), visitante (usuário não autenticado que acessa informação sobre o curso e realiza inscrições).

<strong>- Requisitos Funcionais para Administrador do Sistema</strong>

RF1 – Cadastrar cursos
<p>O sistema deve permitir que o diretor cadastre, edite e exclua cursos.</p>

RF2 – Cadastrar professores
<p>O sistema deve permitir que o diretor cadastre, edite e exclua professores.</p>

RF3 – Visualizar todos os alunos
<p>O sistema deve permitir que o diretor visualize todos os alunos cadastrados.</p>

RF4 – Acompanhar inscrições
<p>O sistema deve permitir que o diretor acompanhe as inscrições nos cursos.</p>

RF5 – Gerenciar links
<p>O sistema deve permitir que o diretor gerencie links de inscrição.</p>

<strong>- Requisitos Funcionais para Professor</strong>

RF6 – Visualizar cursos
<p>O sistema deve permitir que o professor visualize os cursos que ministra.</p>

RF7 – Visualizar alunos
<p>O sistema deve permitir que o professor visualize os alunos inscritos em seus cursos.</p>

RF8 – Registrar informações dos alunos
<p>O sistema deve permitir que o professor registre informações sobre os alunos (ex.: presença, notas, etc.).</p>

<strong>- Requisitos Funcionais para Aluno</strong>

RF9 – Cadastrar na plataforma
<p>O sistema deve permitir que o aluno se cadastre na plataforma.</p>

RF10 – Visualizar cursos disponíveis
<p>O sistema deve permitir que o aluno visualize cursos disponíveis.</p>

RF11 – Inscrever em cursos
<p>O sistema deve permitir que o aluno se inscreva em cursos.</p>

RF12 – Acessar área do aluno
<p>O sistema deve permitir que o aluno acesse sua área (plataforma do aluno).</p>

RF13 – Visualizar inscrições ativas
<p>O sistema deve permitir que o aluno visualize suas inscrições.</p>

<strong>- Requisitos Funcionais para Visitante</strong>

RF14 – Visualizar cursos disponíveis
<p>O sistema deve permitir que visitantes visualizem cursos disponíveis.</p>

RF15 – Inscrever em cursos
<p>O sistema deve disponibilizar um link de inscrição para os cursos.</p>

## • Requisitos não funcionais
Qualidade do sistema

<strong>- Requisitos de usabilidade</strong>

RNF1 – Interface intuitiva
<p>O sistema deve possuir interface simples e intuitiva.</p>

RNF2 – Responsividade
<p>O sistema deve ser responsivo (funcionar em celular, tablet, computador).</p>

<strong>- Requisitos de segurança</strong>

RNF3 – Autenticação
<p>O sistema deve exigir autenticação para acesso às áreas restritas.</p>

RNF4 – Dados seguros
<p>Os dados dos usuários devem ser armazenados de forma segura.</p>

<strong>- Requisitos de desempenho</strong>

RNF5 – Carregar páginas
<p>O sistema deve carregar páginas em até 3 segundos.</p>

RNF6 – Múltiplos usuários
<p>O sistema deve suportar múltiplos usuários simultâneos.</p>

<strong>- Requisito de disponibilidade</strong>

RNF7 – Disponível 24h
<p>O sistema deve estar disponível 24/7, salvo manutenções.</p>

<strong>- Requisito de manutenção</strong>

RNF8 – Desenvolvimento em módulos
<p>O sistema deve ser desenvolvido de forma modular para facilitar manutenção.</p>

# 3. Modelo de casos de uso

# 4. Modelo do banco de dados
(Modelo conceitual, Modelo lógico, Físico)

# 5. Banco de dados

# 6. Diagrama de classes

# 7. Estudo de viabilidade

<strong>- Análise:</strong>
Criaremos um sistema como projeto universitário com parceria com a Zafra. Todos os recursos serão fornecidos pela Fatec. 

<strong>- Viabilidade de Mercado:</strong>
Temos parceria com uma empresa já estabelecida, então não precisamos nos preocupar com a viabilidade de mercado do produto pois essa empresa é nosso cliente. 

<strong>- Viabilidade Técnica:</strong>
Já temos uma equipe formada e a Fatec fornecerá os recursos necessários para a criação e desenvolvimento do programa. 

<strong>- Viabilidade Financeira:</strong>
Não haverá fonte de receita com a criação do projeto, porém qualquer custo será cobrado pela Fatec. 

<strong>- Riscos:</strong>
Não haverá riscos para a criação do projeto.

# 8. Regras de negócio (Modelo canvas)

<strong>- O que foi elaborado?</strong>

Proposta de valor:
Desenvolver um sistema para cadastrar alunos e disponibilizar ferramentas para ajudar a comunicação entre professores e estudantes, agindo como um portal para alunos. 

<strong>- Para quem foi elaborado?</strong>

Segmento de clientes:
Jovens e interessados com poucas condições financeiras em busca de um curso profissionalizante gratuito para entrar no mercado de trabalho. 

Canais:
O sistema deve servir como canal de comunicação entre a empresa e os usuários. 

Relacionamento com clientes:
Garantir ensino profissionalizante e condições básicas para os alunos, com o objetivo de colocar essas pessoas no mercado de trabalho. 

<strong>- Como foi elaborado?</strong>

Atividades principais:
Desenvolver um portal do aluno, com sistema de cadastro e ferramentas para auxiliar o ensino. 

Parcerias principais:
Fatec Jahu 

Recursos Principais:
Computadores e internet fornecidos pela Fatec e máquinas (notebook/pc) domésticas voltadas para uso pessoal. 

<strong>- Quanto custará?</strong>

Fontes de receita:
Esse é um trabalho acadêmico voluntário e não haverá fonte de receita.

Estrutura de custos:
Não haverá custos pois o trabalho é voluntário e os recursos são fornecidos pela Fatec.

# 9. Design
Paleta de cor:
Azul escuro (#1E3983)
Azul marinho (#0F2563)
Ciano (#6DABBC)
Ciano Escuro (#60A1AF)
Azul bebê (#E7F0F9)
Cinza (#CFCFCF)
Branco (#FFFFFF)
Preto (#000000)

Tipografia:
Instrument Sans
Roboto

# 10. Protótipo
(Gere um protótipo funcional na ferramenta que se sentir mais confortável (Figma, por exemplo) e apresente aqui, indicando o link).

# 11. Aplicação
