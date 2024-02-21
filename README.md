# Lab-Minera-o-de-Documentos

## Passo a passo para configurar um serviço de pesquisa dentro do Azure. 

   . primeiro passo devemos criar os recursos necessários para esta pesquisa: 
 
   . inicialmente criar um serviço de pesquisa, Azure AI Search, que será usado para gerenciarmos as informações. 
   
   . após isso criamos um recurso Azure AI, que irá fornecer soluções para enriquecer os nossos dados. 

   . e por último criamos uma conta de armazenamento, onde irão ficar alocados os nossos dados a serem analisados. 

   . salientando apenas que os 3 recursos devem estar dentro do mesmo Resource Group e estarem armazenados na mesma região. 

   # Criação de container para armazenar os nossos dados

   Após termos a nossa conta de armazenamento já criada, dentro desse recurso iremos criar um container, que será onde vamos armazenar os nossos dados. Nomeamos este container, e fazemos o upload dos dados a serem analisados e enriquecidos com AI. 

   Agora dentro do nosso recurso de AI Search, nós iremos importar os dados que já estão na nossa storage account, e é aqui que vamos definir o que queremos extrair de informações, sentimentos, geração de imagens por exemplo. Após termos importado os nossos dados o nosso serviço de pesquisa já estará configurado e podemos então a partir do nosso Azure Search Service na aba de Search Explorer pesquisa por palavras chaves através do JSON query editor e verificar qual o resultado que o nosso AI service retorna, analisando sentimentos, palavras chaves, entidades e etc. 
   Temos ainda uma outra funcionalidade que seria verificar a geração de imagens dentro do container coffee-skillset-image-projection, que foi criado durante o processo de implementação dos serviços. Ao entrarmos no container acima, podemos clicar em qualquer das pastas que irá nos abrir 2 arquivos .jpg. Clicando em qualquer um desses arquivos irá nos abrir uma nova aba, selecionamos a opção "Edit" e irá ser mostrada a imagem gerada. Aqui está o enriquecimento dos dados do nosso AI Service. 