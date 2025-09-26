É possivel acessar o menu do EntraID buscando o nome na barra de pesquisa ou na aba de Serviços.
Observações: 
  Autenticação != Autorização. Autenticação: Garante acesso a recursos mediante verificação de identidade. / Autorização: Permissão para interagir/modificar recursos.
  Usuarios criados na nuvem não são automaticamente sincronizados no ambiente on-premise.
  Permissionamento é herdável!!!
Na pagina do EntraID, no menu latera esquerdo, é possivel acessar as opções relacionadas ao EntraID.

Na pagina de Users é possível: 
  Acessar lista de usuários com detalhamento de informações sbre eles.
  Adicionar/deleta usuários (É possivel criar um novo ou adicionar um ja existente externo)
  Ver logs de acesso
  Atendimento relacionado a Senha

  Em New User:
    1 - Por padrão, o dominio usado é o email pelo qual usao Azure. Para modificar, tenha o dominio cadastrado na azure como da organização. 
    2 - Em basics, configure como desejar o usuário. Siga para Properties.
    3 - Em Properties, configure de acordo com a role e informações do usuário. Siga para Assignments.
    4 - Em Assignments é possível adicionar uma role/grupo ao user
    5 - REVIEW+CREATE

Também é possivel fazer operações em Bulk. Para tal, selecione a opção Bulk Operations na mesma barra de navegação onde tem New User.
Em Roles and Administrator é possivel atribuir regras ja existentes ou criar novas Roles (em um plano premium)


Em Entra Connect é possível replicar recursos On-premise no Cloud.
Na pagina Custom Domain Name, abaixo do menu do Entra Connect, é possível gerenciar dominios.

Ao acessar a pagina de um recurso/grupo de recursos, no IAM é possível tratar do RBAC ( Role Based Acess Control) e permissionamentos.

Defender for Cloud avalia compliance de segurança. Faz recomendações para melhorar a avaliação de recursos ou ferramentas/plataformas associadas.

Referência:
https://learn.microsoft.com/en-us/entra/fundamentals/new-name
