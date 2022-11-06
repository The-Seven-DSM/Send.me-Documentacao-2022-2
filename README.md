
<h1 align="center"> Send.Me - Sprint 1: 29/08/2022 à 18/09/2022 </h1>

            
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
A partir da apresentação do desafio enfrentado pela empresa parceira, a solução desenvolvida se configura em um sistema que lê o diário oficial do estado, separa as citações daqueles que forem associados da empresa e permitir que, após ter sido validado, seja enviado um e-mail para eles.

<div align="center">

![User Story 1](https://user-images.githubusercontent.com/101061910/199399181-994cf2ac-b61e-4481-b9e6-8af829559091.jpg)

</div>

→ [Voltar ao topo](#topo)

<span id="entrega">

## :heavy_check_mark: Entregas

Este GIF do sistema mostra a entrega dos requisitos confirmados para a sprint, onde suas descrições podem ser checadas a seguir:
    
![Teste do Sistema](https://user-images.githubusercontent.com/92696799/190957283-b059e1aa-37c6-4345-a721-5e34b67e207e.gif)
    

→ [Voltar ao topo](#topo)

<span id="metrica">

## :chart_with_upwards_trend: Métricas do time
Para melhorar o aproveitamento da equipe e das habilidades individuais de cada integrante, separamos a equipe de desenvolvimento em duas frentes: Front-End e Back-end, onde para essa primeira sprint a equipe de front-end foi encarregada de criar os componentes e páginas que seriam utilizadas, já a equipe de back-end ficou responsável por criar o crawler(Programa de navegação na Web que cria uma base de dados) para os PDFs, o CRUD, o banco de dados e o envio dos email. Ao final da sprint as duas equipes se juntaram para a integração do sistema de forma que se tornasse funcional e atendesse aos requisitos solicitados pelo cliente.

- Para acompanhar as atividades, foi criado e atualiazado pelo Scrum Masters ao longo da sprint, um gráfico de burndown onde podemos visualizar de forma tangível os esforços de tempo e a progressão ao longo dos dias da sprint, incluindo as atividades desenvolvidas e seus responsáveis.

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
| 11 | Envio do email através do botão de envio de email caso seja um email validado  | ❌ |
| 12 | Voltar para a Home a partir da página de validação de email  | ✔️ |
| 13 | Voltar para a Home a partir do botão Send.Me (Logo)  | ✔️ | 
    
</div>
    
→ [Voltar ao topo](#topo)
