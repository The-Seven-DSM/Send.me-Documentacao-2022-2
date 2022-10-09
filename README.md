
<h1 align="center"> Send.Me - Sprint 2: 18/09/2022 à 09/10/2022 </h1>

            
<br id="topo">
<p align="center">
    <a href="#objetivo">Objetivo da Sprint</a>  |  
    <a href="#entrega">Entregas</a>  |
    <a href="#metrica">Métricas do Time</a> |
    <a href="#como rodar">Como Rodar</a> |
    <a href="#testes">Testes do Sistema</a> 
</p>

<span id="objetivo">

## :dart: Objetivos da Sprint
A partir da apresentação do desafio enfrentado pela empresa parceira, parte das soluções foram desenvolvidas na primeira Sprint, onde você pode conferir mais clicando aqui! Durante essa segunda sprint o foco foi o desenvolvimento de melhorias, correções e novas ferramentas para o projeto. 

<div align="center">

![Backlog 2](https://user-images.githubusercontent.com/101061910/194674948-f7b5ebfe-8052-4e0e-a978-96794056d697.jpg)

</div>

→ [Voltar ao topo](#topo)

<span id="entrega">

## :heavy_check_mark: Entregas

Este GIF do sistema mostra a entrega dos requisitos confirmados para a sprint, onde suas descrições podem ser checadas a seguir:
    
![Teste do Sistema](https://user-images.githubusercontent.com/92696799/190957283-b059e1aa-37c6-4345-a721-5e34b67e207e.gif)

<h2>RFs</h2>

### RF 04: Criação de Relatórios
Este requisito se trata do relatório e a busca de informações no diário oficial. Foi criado um filtro para busca de informação no diário oficial para evitar a superlotação do banco de dados. Este requisito foi feito na primeira sprint levando em consideração as principais funções para a utilidade geral do projeto, e será refinado na sprint 3

<h2>USs</h2>

### US 3
Esta User Story se refere a busca de informação no diário oficial, onde foi adicionado um filtro para não sobrecarregar o banco de dados. Esta User Story foi criada na primeira sprint levando em consideração as principais funções para a utilidade geral do produto.

### US 8
Esta User Story se refere ao histórico de e-mail dos associados, para melhor controle dos e-mails enviados para cada associado. Esta User Story foi criada na segunda sprint levando em consideração o progresso do projeto para a utilidade geral do produto.

### US 9
Esta User Story se refere ao login do backoffice, para que o controle do time seja mais fácil. Esta User Story foi criada na segunda sprint levando em consideração o progresso do projeto para a utilidade geral do produto.

<br>
→ [Voltar ao topo](#topo)

<span id="metrica">

## :chart_with_upwards_trend: Métricas do time
Para melhorar o aproveitamento da equipe e das habilidades individuais de cada integrante, separamos a equipe de desenvolivmento em duas frentes: Front-End e Back-end, onde para essa primeira sprint a equipe de front-end foi encarregada de criar os componentes e páginas que seriam utilizadas, já a equipe de back-end ficou responsável por criar o crawler(Programa de navegação na Web que cria uma base de dados) para os PDFs, o CRUD, o banco de dados e o envio dos email. Ao final da sprint as duas equipes se juntaram para a integração do sistema de forma que se tornasse funcional e atendesse aos requisitos solicitados pelo cliente.

- Para acompanhar as atividades, foi criado e atualiazado pelo Scrum Mastes ao longo da sprint, um gráfico de burndown onde podemos visualizar de forma tangivel os esforços de tempo e a progressão ao longo dos dias da sprint, incluindo as atividades desenvolvidas e seus responsáveis.

<br>
<div align="center">
            
![burndown](https://user-images.githubusercontent.com/101061910/190930471-4b8b8c8a-bb27-4eaa-867a-b14f37a05276.jpg)

</div>
    
→ [Voltar ao topo](#topo)

<span id="como rodar">

## :gear: Como Rodar

Para executar o projeto inteiro primeiro temos de clonar os repositorios [FrontEnd](https://github.com/The-Seven-DSM/Send.me-FrontEnd-2022-2), [BackEnd](https://github.com/The-Seven-DSM/Send.me-BackEnd-2022-2) e [Bot](https://github.com/The-Seven-DSM/Send.me-Bot-2022-2)


- Baixe ou clone estes repositório
```bash
$ git clone https://github.com/The-Seven-DSM/Send.me-Bot-2022-2.git
$ git clone https://github.com/The-Seven-DSM/Send.me-BackEnd-2022-2.git
$ git clone https://github.com/The-Seven-DSM/Send.me-FrontEnd-2022-2.git
```

OBS: O projeto deve rodar na seguinte ordem Bot -> BackEnd -> FrontEnd

- Acesse a pasta Send.me-Bot-2022-2 
```bash
#Rodando Bot

# Já dentro do projeto, localize o arquivo Database.config.ts dentro da pasta config 
# Na linha 3 altere o campo "root" e "admin" para suas credenciais do MySQL

$ cd Send.me-Bot-2022-2
$ pip install -r requirements.txt
$ Python app.py

#Espere o bot terminar sua execução e passe para o próximo 
```

- Acesse a pasta do Send.me-BackEnd-2022-2
```bash
#Rodando BackEnd
yarn install
$ yarn start
```

- Acesse a pasta do Send.me-FrontEnd-2022-2
```bash
#Rodando FrontEnd
yarn install
$ yarn start
```

- A aplicação iniciará localmente na porta 3000. Use o navegador para acessar o link [http://localhost:3000](http://localhost:3000)

Finalizado!!!

→ [Voltar ao topo](#topo)

<span id="testes">

## :clipboard: Testes do Sistema

Como solicitado pelo cliente ao fim da sprint, testamos todas as interações possiveis através da página web e sua respostas, de forma que podemos ver a eficácia

<div align="center">
    
| Nº | Descrição | Status |
|:--:|:----------:|:----------------:|
| 01 | Redirecionamento para a página de cadastro do associado | ✔️ | 
| 02 | Preenchimento dos campos de cadastro de associado | ✔️ | 
| 03 | Bloqueio do cadastro de associados caso um campo não esteja preenchido | ✔️ | 
| 04 | Cadastro de associado a partir do formulário caso os campos estejam preenchidos através do botão de cadastro| ✔️ |
| 05 | Voltar para a Home a partir da página de cadastro de associados  | ✔️ | 
| 06 | Visualização da tabela de associados presentes no PDF do dia | ✔️ | 
| 07 | Envio de email validados através do botão de envio de email geral  | ✔️ |
| 08 | Redirecionamento para a página de validação e edição de email | ✔️ |
| 09 | Edição de texto do email  | ✔️ |
| 10 | Validar o email/edição atrevés do botão de validar  | ✔️ |
| 11 | Envio do email através do botão de envio de email   | ✔️ |
| 12 | Voltar para a Home a partir da página de validação de email  | ✔️ |
| 13 | Voltar para a Home a partir do botão Send.Me (Logo)  | ✔️ | 

</div>

### Correções

<div align="center">

| Nº | Descrição | Status |
|:--:|:----------:|:----------------:|
| 1 | Envio do email através do botão de envio de email caso seja um email validado  | ✔️ |

 </div> 
 
→ [Voltar ao topo](#topo)
