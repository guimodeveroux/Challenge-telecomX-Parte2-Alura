# Challenge-telecomX-Parte2-Alura

Relatório de Análise de Evasão de Clientes

Com base na análise dos dados dos clientes e no desempenho do modelo LGBMClassifier, os seguintes fatores têm a influência mais significativa na evasão de clientes:

Principais Fatores de Evasão (Com Base na Importância de Atributos e Valores SHAP)

Tempo de Permanência (Tenure): A duração do tempo que um cliente está com a empresa é um forte indicador de evasão. Clientes com menor tempo de permanência são mais propensos a sair. Isso é evidente tanto na importância dos atributos quanto nos valores SHAP, onde tenure consistentemente ocupa uma posição alta.

Serviço de Internet (Fibra Óptica vs. Sem Serviço de Internet): O tipo de serviço de internet impacta significativamente a evasão. Clientes com internet de Fibra Óptica são mais propensos a sair em comparação com aqueles sem serviço de internet. Os atributos InternetService_Fiber optic e InternetService_No têm alta importância e valores SHAP.

Tipo de Contrato (Mês a Mês vs. Dois Anos): Clientes com contratos mês a mês têm uma taxa de evasão muito maior do que aqueles com contratos de um ou dois anos. Isso é claramente mostrado pela alta importância e valores SHAP de Contract_Two year e Contract_One year.

Método de Pagamento (Cheque Eletrônico): Clientes que usam cheques eletrônicos como método de pagamento são mais propensos à evasão. O atributo PaymentMethod_Electronic check é um preditor significativo de evasão.

Cobranças (Mensal e Total): Tanto as cobranças mensais quanto as totais têm um impacto notável na evasão. Cobranças mensais mais altas e cobranças totais mais baixas tendem a estar associadas à evasão.

Segurança Online e Suporte Técnico: Clientes que não possuem serviços de segurança online ou suporte técnico são mais propensos a sair. A ausência desses serviços (OnlineSecurity_No internet service, TechSupport_No internet service, OnlineSecurity_Yes e TechSupport_Yes) são fatores importantes.

Conta Sem Papel (Paperless Billing): Clientes com conta sem papel são ligeiramente mais propensos a sair.

Idoso (Senior Citizen): Clientes idosos parecem ter uma propensão ligeiramente maior à evasão.

Desempenho do Modelo

O modelo LGBMClassifier alcançou uma acurácia de validação de aproximadamente 79.42% e um score ROC AUC de 0.8448. O relatório de classificação mostra que o modelo tem maior precisão e recall para prever clientes que não sairão (classe 0) em comparação com clientes que sairão (classe 1). Isso indica um desequilíbrio no conjunto de dados, que também é refletido nas contagens de valores da variável alvo (cerca de 73% não evasão e 27% evasão).

Estratégias de Retenção Com base nesses resultados, aqui estão algumas estratégias de retenção propostas:

Foco no Engajamento Inicial: Implementar estratégias para engajar novos clientes com menor tempo de permanência para construir lealdade e reduzir a evasão inicial.

Melhorar o Serviço de Fibra Óptica e Suporte: Investigar possíveis problemas com o serviço de internet de Fibra Óptica que possam estar causando evasão e melhorar o suporte técnico para esses clientes.

Promover Contratos de Longo Prazo: Oferecer incentivos e benefícios para encorajar os clientes a mudarem de contratos mês a mês para contratos de maior duração.

Analisar Problemas com Pagamento por Cheque Eletrônico: Investigar se existem problemas específicos ou frustrações associadas ao método de pagamento por cheque eletrônico que contribuem para a evasão.

Revisar Preços e Pacotes: Analisar a relação entre altas cobranças mensais e evasão para garantir preços competitivos e considerar a oferta de pacotes mais flexíveis ou combinados.

Destacar os Benefícios de Segurança e Suporte: Promover ativamente os benefícios dos serviços de segurança online e suporte técnico aos clientes, especialmente aqueles que atualmente não os assinam.

Avaliar a Experiência da Conta Sem Papel: Coletar feedback sobre a experiência da conta sem papel e fazer melhorias, se necessário, para reduzir qualquer evasão associada.

Personalizar Ofertas para Idosos: Desenvolver programas de retenção ou ofertas direcionadas especificamente para clientes idosos.

Ao abordar esses fatores-chave e implementar estratégias de retenção direcionadas, a empresa pode potencialmente reduzir a evasão de clientes e melhorar o valor geral do tempo de vida do cliente.
