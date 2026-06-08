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
O desenvolvimento seguirá uma abordagem incremental, acompanhando os semestres do curso e as sprints do P.I. O protótipo inicial será um site responsivo, baseado nos conhecimentos adquiridos em sala de aula, contendo funcionalidades como login de aluno, funcionário e administrador, gestão de alunos e controle de materiais de sala de aula. 

Para o desenvolvimento do projeto serão utilizadas ferramentas como Figma para prototipação e design das interfaces, Visual Studio Code para programação e GitHub para versionamento do código. As principais tecnologias utilizadas serão HTML5, CSS3, Bootstrap e JavaScript para o desenvolvimento web. 

O projeto seguirá um modelo de desenvolvimento incremental, permitindo melhorias contínuas durante cada etapa do P.I.

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
Não presente nesta etapa do P.I. no primeiro semestre.

# 4. Modelo do banco de dados
Não presente nesta etapa do P.I. no primeiro semestre.

# 5. Banco de dados
Não presente nesta etapa do P.I. no primeiro semestre.

# 6. Diagrama de classes
Não presente nesta etapa do P.I. no primeiro semestre.

# 7. Estudo de viabilidade
<strong>Viabilidade Operacional: </strong>

O projeto será desenvolvido em sprints conforme as entregas incrementais por semestre do P.I., com divisão de tarefas entre os cinco integrantes. A metodologia ágil garante essas entregas parciais e o controle de progresso contínuo. 

<strong>Viabilidade de Mercado: </strong>

O projeto possui viabilidade de mercado por ser uma plataforma desenvolvida especificamente para atender às necessidades da instituição cliente, oferecendo funcionalidades personalizadas para gerenciamento da escola. Diferente de plataformas genéricas, o sistema será adaptado conforme as demandas reais da instituição, tornando o gerenciamento mais organizado, acessível e eficiente. 

<strong>Viabilidade Técnica: </strong>

Nosso produto é viável tecnicamente pois a equipe possui conhecimento em HTML, CSS, JavaScript e frameworks modernos. Utilizando ferramentas gratuitas e acessíveis, como VSCode, Figma e GitHub, tornamos o desenvolvimento viável dentro do contexto acadêmico. 

<strong>Viabilidade Financeira: </strong>

O projeto é viável financeiramente falando pois o custo de desenvolvimento é zero e trata-se de ambiente acadêmico. A hospedagem inicial será feita em serviços gratuitos, com escalabilidade paga somente em caso de adoção real pela escola.

# 8. Regras de negócio (Modelo canvas)

O que foi elaborado? 

<strong>Proposta de valor: </strong>

Entregamos um sistema personalizado, único e atrativo, desenvolvido especialmente para atender às necessidades do cliente, facilitando a comunicação, o acesso às informações e o acompanhamento das atividades de forma prática, moderna e eficiente, centralizando a experiência educacional da escola em uma plataforma digital, acessível, intuitiva e organizada. 

Para quem foi elaborado? 

<strong>Segmento de clientes: </strong>

Jovens em busca do primeiro emprego e pessoas que desejam se qualificar ou se recolocar no mercado de trabalho, especialmente aquelas em situação de vulnerabilidade social ou com poucas condições financeiras para custear um novo curso. O projeto também é destinado a qualquer pessoa interessada em adquirir conhecimento profissionalizante e ampliar suas oportunidades de estudo e emprego. 

<strong>Canais: </strong>

Os canais para alcançar os clientes serão principalmente as redes sociais da escola Zafra e de todas as empresas parceiras, além da divulgação boca a boca, permitindo que as informações sobre os cursos e oportunidades alcancem cada vez mais pessoas da comunidade. 

<strong>Relacionamento com clientes: </strong>

Garantir suporte educacional e acesso simplificado aos cursos profissionalizantes, promovendo inclusão social, acompanhamento dos alunos e oportunidades de ingresso no mercado de trabalho. 

Como foi elaborado? 

<strong>Atividades principais: </strong>

Pesquisa e levantamento de requisitos, criação de protótipos das interfaces, desenvolvimento das páginas e funcionalidades do sistema, testes de usabilidade, correção de erros e documentação do projeto. 

<strong>Parcerias principais: </strong>

Fatec Jahu, Zafra, Raide Jahu, Grupo Jauense, Valseg, Elringklinger, Limer Stamp, Mais RH, Papelaria Jr, Santo Antonio. 

<strong>Recursos Principais: </strong>

Computadores e internet disponibilizados pela faculdade, notebooks e computadores pessoais da equipe de desenvolvimento, sistema web para testes e validação do sistema, ferramentas de desenvolvimento como VSCode e Figma, conhecimento da equipe de desenvolvimento em linguagens de programação. 

Quanto custará? 

<strong>Fontes de receita: </strong>

O projeto possui caráter acadêmico, não apresentando fontes de receita. Futuramente, poderão existir parcerias com empresas locais e instituições apoiadoras, assim como possíveis doações e parcerias educacionais. 

<strong>Estrutura de custos: </strong>

Hospedagem do sistema, internet e infraestrutura, manutenção e atualização da plataforma, recursos computacionais utilizados no desenvolvimento, horas de trabalho da equipe de desenvolvimento.

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
Instrument Sans, Roboto

# 10. Protótipo
Link Protótipo - https://www.figma.com/design/LeJFP9L6ZnqMeJ6t9N9exC/Portal-do-aluno-zafra?node-id=0-1&t=No13j89CUywRDGzP-1

# 11. Aplicação
Link Aplicação - https://github.com/leandromello1/Equipe-Zafra-PI/tree/master
