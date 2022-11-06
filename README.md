
<h1 align="center"> Send.Me - Sprint 3: 17/10/2022 à 06/11/2022 </h1>

            
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
A partir da apresentação do desafio enfrentado pela empresa parceira, parte das soluções foram desenvolvidas nas sprints anteriores, onde você pode conferir mais [clicando aqui](https://github.com/The-Seven-DSM/Send.me-Documentacao-2022-2/)! Durante essa terceira sprint o foco foi o desenvolvimento de melhorias e correções do projeto, focando principalmente em melhorar e adiantar o terreno para atualizações futuras!

<div align="center">

![User Story 3](https://user-images.githubusercontent.com/101061910/200188777-28275ffb-d1a3-48e2-be8f-03ca3a0e2da8.jpg)

</div>

→ [Voltar ao topo](#topo)

<span id="entrega">

## :heavy_check_mark: Entregas

Este GIF do sistema mostra a entrega dos requisitos confirmados para a sprint, onde suas descrições podem ser checadas a seguir:
    
### Geração PDF 


### Cadastro do Backoffice

    
→ [Voltar ao topo](#topo)

<span id="metrica">

## :chart_with_upwards_trend: Métricas do time
Para melhorar o aproveitamento da equipe e das habilidades individuais de cada integrante, separamos a equipe de desenvolivmento em duas frentes: Front-End e Back-end, onde para essa primeira sprint a equipe de front-end foi encarregada de criar os componentes e páginas que seriam utilizadas, já a equipe de back-end ficou responsável por criar o crawler(Programa de navegação na Web que cria uma base de dados) para os PDFs, o CRUD, o banco de dados e o envio dos email. Ao final da sprint as duas equipes se juntaram para a integração do sistema de forma que se tornasse funcional e atendesse aos requisitos solicitados pelo cliente.

- Para acompanhar as atividades, foi criado e atualiazado pelo Scrum Mastes ao longo da sprint, um gráfico de burndown onde podemos visualizar de forma tangivel os esforços de tempo e a progressão ao longo dos dias da sprint, incluindo as atividades desenvolvidas e seus responsáveis.

<br>
<div align="center">
            
![Burndown Chart](https://user-images.githubusercontent.com/92696799/200189384-d23ab72e-0e95-488f-9120-2f85d68c5725.png)

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
| 01 | Entrar na lista de associados pela navbar | ✔️ | 
| 02 | Entrar pelo perfil do associado selecionando no nome do associado | ✔️ | 
| 03 | Mostrar a lista de todos os associados | ✔️ |
| 04 | Acessar o perfil através da lista | ✔️ |
| 05 | Mostrar dados do associado no perfil | ✔️ |
| 06 | Apagar associado pelo perfil | ✔️ | 
| 07 | Mostrar histórico contendo email enviados e não enviados | ✔️ | 
| 08 | Redirecionar para o relatório a partir da tabela histórico | ✔️ |           
| 09 | Apagar associado pela lista através do botão| ✔️ |
| 10 | Sistema diário para verificação | ✔️ |
| 11 | Melhoria na filtragem de mensagens recolhidas automaticamente | ✔️ |
| 12 | Acesso do Backoffice ao sistema caso os campos estejam preechidos corretamente | ✔️ |
| 13 | Falha ao entrar caso os dados estejam errados ou vazios | ✔️ |

</div>

### Correções

<div align="center">

| Nº | Descrição | Status |
|:--:|:----------:|:----------------:|
| 1 | Bloqueio das rotas | ❌ ✔️|

 </div> 
 
→ [Voltar ao topo](#topo)
