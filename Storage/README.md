Acesse a Conta de Armazenamento para o grupo de recursos E SIGA A SEQUÊNCIA DE PASSOS B.
Caso não tenha, siga a sequência de passos A:

A - Configurar conta nova

Em CRIAR RECURSOS, escolha Conta de Armazenamento.

Aba Basico:

Subscription é automatico
1- Escolha o Grupo de Recursos ou Crie um caso não exista
2 - Crie um Nome da Conta de armazenamento ÚNICA (Não deve existir nenhuma conta com memso nome, deve ter letras emcaixa baixa e numeros apenas. Ele será usado nos End Points ex: contastoragedio.blob.core.windows.net)
3 - Região
4 - Desempenho: Standard para uso geral, Premium para baixa latência
5 - Redundância: LRS para testes apenas, evite se for ambiente de produção. Faça, no mínimo, GRS. Escolha dependendo da criticidade do sistema e recursos disponíveis.

Avançado/Rede/Segurança/Criptografia: 
Configure de acordo com Caso de uso. Porém lembre de configurar de acordo com a segurança/privacidade dos recursos NECESSÁRIA/caso de uso.
Ex: Recursos expostos publicamente em ambientes de produção

6 - Criar e revisar

B - Conta já criada

Após acessar a pagina da conta, é possivel acessar recursos de Armazenamento no menu de rolagem localizado na lateral esquerda da página.
Ao criar um, um endpoint url do tipo contastorage.serviço.core.windows.net é gerado.
É possivel configurar o IAM para garantir/restringir acesso de usuários ao recurso.


C - Migrações
Para o DataBox:
Na aba de busca, escreva Migrate e selecione a opção Azure Migrate

Na pagina do Migrate há 3 opções: Aplicativos/Servior/Bds, Database only e Explore more scenarios
A primeira opção é uma versão prévia (em desenvolvimento). Não há SLA ainda para ela, então evite usar em ambiente de produção.
Escolha uma das opções e depois criar projeto.
Escolha o grupo de recursos, dê o nome conforme as retrições do Azure e escolha a geografia. 
Decida a exposição do endpoint e prossiga.
Ao criar, no menu lateral há a seção Migration Goals.
Lá é possivel selecionar o DataBox e configurar de acordo. (Recomendado para grandes volumes de dados a serem migrados)

Para o AZCopy:
AZCopy é um executável compativel com Windows/Linux/Mac, volumes menores. Suporta Blobs/Arquivos.
    - Crie ou selecione um container. 
    - Em configurações do Container, clique em Tokens de acesso compartilhado, adicione as permissões e gere o sas token.
    - Guarde o token.
    - Tenha tbm o caminho do que será migrado e o comando de linha AZCopy.
    - Abra o terminal, faca cd caminhodoexecutaveldoAzCopy
    - Use o comando com o caminho do conteudo a ser enviado pro container e o token

  Para o Gerenciador de armazenamento windows:

  Siga o manual dele

