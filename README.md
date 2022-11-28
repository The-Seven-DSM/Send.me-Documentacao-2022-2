
<h1 align="center"> Send.Me - Sprint 4: 07/11/2022 à 27/11/2022 </h1>

            
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
A partir da apresentação do desafio enfrentado pela empresa parceira, parte das soluções foram desenvolvidas nas sprints anteriores, onde você pode conferir mais [clicando aqui](https://github.com/The-Seven-DSM/Send.me-Documentacao-2022-2/)! Durante essa quarta sprint o foco foi o desenvolvimento de melhorias e correções do projeto, focando principalmente em melhorar e finalizar o projeto!

<div align="center">

![User Story 4](https://user-images.githubusercontent.com/101061910/204147936-d9b9125d-fa34-4715-ae26-ecf7b43d1886.jpg)

</div>

→ [Voltar ao topo](#topo)

<span id="entrega">

## :heavy_check_mark: Entregas

Este GIF do sistema mostra a entrega dos requisitos confirmados para a sprint, onde suas descrições podem ser checadas a seguir:
    
### Refatoração           
![2022-11-28 00-00-19](https://user-images.githubusercontent.com/92696799/204182369-27e5bd88-8d87-4eab-ab6a-084b44f233ee.gif)  

### Filtro por Caderno                    
![2022-11-27 23-49-09 (online-video-cutter com)](https://user-images.githubusercontent.com/92696799/204181812-06970d27-4e57-4527-9385-19950bafff8c.gif)
                        
→ [Voltar ao topo](#topo)

<span id="metrica">

## :chart_with_upwards_trend: Métricas do time
Para melhorar o aproveitamento da equipe e das habilidades individuais de cada integrante, separamos a equipe de desenvolvimento em duas frentes: Front-End e Back-end, onde para essa primeira sprint a equipe de front-end foi encarregada de criar os componentes e páginas que seriam utilizadas, já a equipe de back-end ficou responsável por criar o crawler(Programa de navegação na Web que cria uma base de dados) para os PDFs, o CRUD, o banco de dados e o envio dos email. Ao final da sprint as duas equipes se juntaram para a integração do sistema de forma que se tornasse funcional e atendesse aos requisitos solicitados pelo cliente.

- Para acompanhar as atividades, foi criado e atualiazado pelo Scrum Masters ao longo da sprint, um gráfico de burndown onde podemos visualizar de forma tangível os esforços de tempo e a progressão ao longo dos dias da sprint, incluindo as atividades desenvolvidas e seus responsáveis.

<br>
<div align="center">
            
![Burndown Chart](https://user-images.githubusercontent.com/92696799/204162011-ddcff131-8eaa-4042-8984-3707506d7653.png)

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
| 01 | Envio Automático de Email| ✔️ | 
| 02 | Envio de Todos os Email com Status Positivo| ✔️ |
| 03 | Envio de Todos os Emails | ✔️ | 
| 04 | Refatoração Completa do Código | ✔️ |
| 05 | Filtro por Caderno | ✔️ |
| 06 | Filtro por Nome | ✔️ |

</div>
