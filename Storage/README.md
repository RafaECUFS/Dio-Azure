Tenha uma Conta de Storage para o grupo de recursos.
Caso não tenha, em CRIAR RECURSOS, escolha Conta de Armazenamento.

Aba Basico:

Subscription é automatico
1- Escolha o Grupo de Recursos ou Crie um caso não exista
2 - Crie um Nome da Conta de armazenamento ÚNICA (Não deve existir nenhuma conta com memso nome, deve ter letras emcaixa baixa e numeros apenas. Ele será usado nos End Points ex: contastoragedio.blob....)
3 - Região
4 - Desempenho: Standard para uso geral, Premium para baixa latência
5 - Redundância: LRS para testes apenas, evite se for ambiente de produção. Faça, no mínimo, GRS. Escolha dependendo da criticidade do sistema e recursos disponíveis.

Avançado/Rede/Segurança/Criptografia: 
Configure de acordo com Caso de uso. Porém lembre de configurar de acordo com a segurança/privacidade dos recursos NECESSÁRIA/caso de uso.
Ex: Recursos expostos publicamente em ambientes de produção


6 - Criar e revisar
