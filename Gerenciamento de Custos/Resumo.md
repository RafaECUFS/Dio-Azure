Existem 6 fatores que influenciam os custos de serviços cloud na Azure:
  .Tipo de Recurso
  .Consumo
  .Manutenção/Monitoramento
  .Área Geográfica
  .Tráfego de Rede
  .Assinatura

Segue-se um exemplo de Monitoramento mostrando os custos de Grupos de recursos diferentes numa conta Free:
  <img width="1420" height="980" alt="costanalysis_charts" src="https://github.com/user-attachments/assets/65b09f66-b07b-43a5-8099-c2f49e8dd77d" />
A diferença de preço entre os recursos é nítida:
Armazenamento e Rede tem maior gasto E MAIOR CONSUMO.
Máquina Virtual, apesar de ser o primeiro recurso criado no grupo, teve o menor custo. 
Isso provavelmente se deve ao fato de ter havido pouco uso dos recursos de Máquina Virtual enquanto os outros geram custo em segundo plano.

Tags ajudam a identificar recursos/grupos de recursos em faturas. Elas utilizam pares chave/valor para identificação.
Elas não são herdáveis, o que significa que recursos filhos, de um gruopo de recursos que tem tag por exemplo, não recebem a tag do pai.
Por exemplo: AZ900_Lab (Grupo de Recursos) e AZ900_LabVNet (Virtual Network do grupo AZ900_Lab)

Azure conta com calculadoras de custo para estimar (aproximadamente) custos dos recursos cloud:

<a href="[url](https://azure.microsoft.com/en-us/pricing/calculator/)">Azure Calculator</a>


Infelizmente a Azure descontinuou o TCO Calculator, que permitia comparação de custos com Estruturas On-premise hipotéticas, e trabalha apenas com Azure Migrate para comparar com estruturas On-Premise descobertas.

