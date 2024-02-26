<h1>
     <span> Azure Cognitive Search: Utilizando AI Search para indexação e consulta de dados</span>
</h1>

## O que precisa ser feito?

O desafio propõe que seja criada uma pesquisa que funcione juntamente com um serviço de inteligência artificial para identificar palavras chave e sentimentos 

[Documentação](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)

## Primeira etapa: Criando recurso do Azure AI Search   

01 - Clique em "Azure AI Search", opção "Criar" e no "Pricing Tier", selecionar o nível "Basic".

02 - Aguarde terminar a implantação

## Segunda etapa: Criando recurso do Azure AI Services  

01 - Clique em "Serviços Cognitivos" e faça a configuração, para esse serviço o Pricing Tier poderá ser o "Standard $ 0 e marcar o campo checkBox.

02 - Aguarde implantação

## Terceira etapa: Criando o armazenamento (storage) 

01 - Clique na opção "Storage acount"

02 - Em seguida, vamos na opção "create"

03 - Storage acount name: precisa ser um nome único e com no mínimo 3 caracteres e no máximo de 24 caracteres.

04 - Performace - Escolha a opção "Standard"

05 - Redundancy - Escolha a opção: "Locally-reduntand storage - LRS"

06 - Aguarde implantação

## Quarta etapa: Permitindo acesso anônimo ao Blob  
 
Para fins didáticos permita o acesso anônimo ao blob para simplificar e facilitar nossas implementações, essa etapa é necessária apenas para o caso de estudos e jamais é indicadado para ambientes de produção.

01 - Após criar o armazenamento, entre no mesmo e navegue até a guia "Configurações" e clique em "Configuração", marcando as opções "Allow Blob anonimous access", como Enabled. Logo após, clique em "Salvar":

## Quinta etapa: Criando o container 

01 -  Dentro do armazenamento que foi criado, navegue até a aba "Armazenamento de dados" e selecione a opção "contêineres". E então, clique na opção "+Contêiner":

02 - Logo em seguida, preencha a aba "Nome" com "coffeereviews" e configure 

## Sexta etapa: Carregar o Blob

01 - Selecione o contêiner que foi criado ("coffeereviews"):

02 - Na nova página, vá na opção "Carregar": 

03 - Faça o download dos arquivos da documentação acima em seguida, faça o upload dos arquivos baixados

## Sétima etapa: Importação e indexação dos dados

01 - Voltamos para o AI Search, selecione o elemento criado e então clique na opção "Importar dados":

02 - Na próxima etapa, em "Conectar a seus dados", na parte "Fonte de dados", selecione "Armazenamento de Blob do Azure":

03 - Selecione o elemento:

04 - Em seguida, selecione novamente o contêiner ("coffeereviews") e, depois de selecionado, clique na opção azul embaixo:


05 - Daqui para frente, recomendo que siga a [documentação](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html) para facilitar a compreensão dos passos necessários! Vá até o passo 17 e então volte para continuarmos :)

## Última etapa: Consulta ao índice

01 - Depois de importamos os dados, chegou o momento da última etapa. Vamos na opção "Gerenciador de pesquisa"

02 - Logo em seguida, vamos utilizar um comando que vai verificar se a indexação foi feita corretamente e mostra os documentos.

## O que foi aprendido:  

O uso das ferramentas do Microsoft Azure facilitam a análise de documentos em grande quantidade, facilitando a consulta, pesquisas e o processo de filtragem das situações que queremos validar. 