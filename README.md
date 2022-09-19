
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

![Backlog Sprint](https://user-images.githubusercontent.com/101061910/190931394-b119e60b-934d-4b08-8ec0-64239ba638f3.jpg)

</div>

→ [Voltar ao topo](#topo)

<span id="entrega">

## :heavy_check_mark: Entregas

Este GIF do sistema mostra a entrega dos requisitos confirmados para a sprint, onde suas descrições podem ser checadas a seguir:
    
GIF    
    
### RF 01: Manipulação do PDFs  
Esse requisito se trata do sistema de donwload, tratamento e exclusão dos dos PDFs. Este requisito, como o validado, teve seu início na primeira sprint levando em consideração as principais funções para a utilidade geral do projeto. O termino desse requisito será feito em entregas futuras onde o sistema fará a exclusão dos PDFs.  
    
### RF 02: Leitura e localização de conteúdo

Este requisito se trata de um crawler, que lê os PDFs baixados e busca nomes e as informações de nossos associados, para posteriormente armazenar em uma base de dados. Este requisito, como o validado, foi desenvolvido na primeira sprint levando em consideração as principais funções para a utilidade geral do projeto, e será refinado na sprint 2.
 
### RF 03: Cadatro de Associados   
Este requisito se trata do cadastro de associados, contendo seus dados pessoais e seus contatos. Este requisito foi feito na primeira sprint levando em consideração as principais funções para a utilidade geral do projeto, e será refinado na sprint 2.    
    
### RF 04: Criação de Relatórios
Este requisito se trata do relatório, impresso ou arquivo, criado a partir das informações armazenadas pelo crawler, contendo nome, e-mail e outras informações dos associados, onde o mesmo tem de receber de forma eletrônica em sua caixa de emails. Este requisito foi feito na primeira sprint levando em consideração as principais funções para a utilidade geral do projeto, e será refinado na sprint 2
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
$ cd Send.me-Bot-2022-2
$ pip install -r requirements.txt
$ Python app.py}

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
| 04 | Cadastro de associado a partir do formulário caso os campos estejam preenchidos através od botão de cadastro| ✔️ |
| 05 | Voltar para a Home a partir da página de cadastro de associados  | ✔️ | 
| 06 | Visualização da tabela de associados presentes no PDF do dia | ✔️ | 
| 07 | Envio de email validados através do botão de envio de email geral  | ✔️ |
| 08 | Redirecionamento para a página de validação e edição de email | ✔️ |
| 09 | Edição de texto do email  | ✔️ |
| 10 | Validar o email/edição atrevés do botão de validar  | ✔️ |
| 11 | Envio do email através do botão de envio de email   | ❌ |
| 12 | Voltar para a Home a partir da página de validação de email  | ✔️ |
| 13 | Voltar para a Home a partir do botão Send.Me (Logo)  | ✔️ | 
    
</div>
    
→ [Voltar ao topo](#topo)
