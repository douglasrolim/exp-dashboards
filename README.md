# Dashboard de Desenvolviemnto - Descrição do Experimento

A atividade proposta no experimento consiste na utilização dos recursos do middleware de dados Smart Geo Layers (SGeoL) para construção de uma **camada Planejamento de obras** para a Prefeitura de Natal.

## Instruções

Para definir tal camada, é necessário fazer uso das APIs para Camadas e Entidades do SGeoL, incluindo o uso das APIs de segurança, conforme é apresentado o caso de uso a seguir:

![Funcionalidade para criação e entidades](/img/caso-de-uso-dev.png)

Observações:

- No SGeoL, todas as camadas devem possuir obrigatoriamente uma propriedade do tipo 'Property' chamada *path* - que indica o path a ser usado para realizar consultas, inserções, atualizações e remoções de entidades nessa camada.
- No Sgeol, Entidades com informações geograficas devem possuir obrigatoriamente uma propriedade do tipo GeoProperty chamada *location*, cujo valor é um GeoJSON.
- No Sgeol, tanto camadas como entidades, devem obrigatoriamente possuir um **name** (nome da camada ou entidade) e uma **description** (descrição da camada ou entidade).



Fluxo de chamadas da API do SGeoL:

![Fluxo de chamadas para API do Sgeol](/img/sgeol-uso-api.jpg)

## Definição da camada
  
Os seguintes passos devem ser executados:

- path: p_obras_eng_[seu_nome]
	- Exemplo: p_obras_eng_douglas
- name: Plan. de obras - [Seu Nome]
	- Exemplo: Plan. de obras - Douglas
- description: Planejamento de Obras da Prefeitura de Natal - Engenheir[a] [Seu Nome]
	- Exemplo: Planejamento de Obras da Prefeitura de Natal - Engenheiro Douglas
- crea: 123456789

Após criada a cada, salve a imagem a seguir e defina como ícone da camada:

![Funcionalidade para criação e entidades](/img/marker-obras.png)

## Definição das entidades

Para a camada criada, adicione as seguintes entidades:

**Entidade 1**
- name: Obras para a Copa do Mundo
- description: Polígono de área afetada pelas obras
- location: Usar os dados de: https://gist.github.com/douglasrolim/64f7ae9793d130a745d7ea7accc17f5f

**Entidade 2**
- name: Obras de reparo da Via Costeira
- description: Pontos da operação tapa buracos da via da Via costeira
- location: Usar os dados de: https://gist.github.com/douglasrolim/07358c4db4bceb4fec3ef62b1a43f2b3

**Entidade 3***
- name: Obras de manutenção das áreas verdes
- description: Pontos de obras para manutenção das áreas verdes
- location: Usar os dados de: https://gist.github.com/douglasrolim/aa997fcea8b9e1e6e7b1c3cd1ba28733

## Definição das entidades

Em seguida, deve-se analisar os dados adicionados fazendo uso do Dashboard de Visualização.

**Acesse o Dashboard de Visualização**: http://sgeolayers.imd.ufrn.br/signatal/

- Realize login usando as mesmas cedenciais usadas no Dashboard de desenvolvimento
- Plotar no mapa a camada criadas nas instruções anteriores
- Selecionar uma entidade apresentada do mapa e visualizar na barra de navegação.
- Editar a descrição para "Obra concluída" e salvar as modificações.
- Poltar no mapa a camada de "Equipamentos desportivos"
- Usar o controle de visualização de camadas para ocultar as camadas e ativar o mapa de calor para a camada de "Equipamentos desportivos"


## Guias e material de apoio

[Link para o Dashboard de Desenvolvimento](http://sgeolayers.imd.ufrn.br/devboard/)

[Manual do Dashboard de Desenvolvimento](https://docs.google.com/document/d/1cx7UJ0hMkUzKJ2l8DcXKeiyASrBuh_wlrdOuBIy46No/edit?usp=sharing)

Para a realização das tarefas, a documentação e guias oficiais do SGeoL podem ser consultados. 

[SGeoL - API](http://sgeolayers.imd.ufrn.br/sgeol-test-sec/operacoes-api.xhtml)

[SGeoL - API Usuários e Autenticação](http://sgeolayers.imd.ufrn.br/sgeol-test-sec/api-usuarios-autenticacao.xhtml)

[SGeol - API Camadas](http://sgeolayers.imd.ufrn.br/sgeol-test-sec/api-camadas.xhtml)

[SGeol - API Entidades](http://sgeolayers.imd.ufrn.br/sgeol-test-sec/api-entidades.xhtml)

[Tutorial - Postman](https://documenter.getpostman.com/view/4390317/SWTBfJQ9?version=latest)

## Formulário Final

Ao final da realização das atividades, favor responder o link em anexo para finalização da participação no experimento:

[Link do formulário do experimento](https://docs.google.com/forms/d/e/1FAIpQLSeuVhewdsU04atKJAapF0MuxEYHOVY0K4ev0dh9jSOkVSxamA/viewform?usp=sf_link)
