##### Dicionário de Dados: Connecta Telecom



Tabelas de densão (Contexto)

Organizadores do modelo que filtram os eventos.





**Tabela,Descrição,Chaves e Campos Principais**



dCalendar,Calendário corporativo.,"Date, Year, Month, IsHoliday, IsBlackFriday, IsSummer, IsBackToSchool"



dCustomers,Perfil demográfico e de valor do cliente.,"CustomerID, Segmento, Sexo, Idade, Distrito, CanalPreferencial"



dProducts,"Catálogo de serviços (Móvel, Fibra, TV).","ProductID, Nome, Categoria, PrecoBase, MargemEstimada, Tecnologia"



dStores,Pontos de venda físicos.,"StoreID, Nome, Tipo"



dRegions,Distribuição geográfica e peso populacional.,"RegionID, Distrito, Weight"



dCallCenters,Centros de atendento remoto.,"CallCenterID, Localização, Tipo"



dTechCenters,Polos de suporte e manutenção de rede.,"TechCenterID, RegiaoPrincipal"



dChannels,Canais de aquisição e suporte.,"ChannelID, Canal (Ex: Loja Física, Online)"



dPaymentMethods,Formas de pagamento aceites.,"PayMethodID, Método"



dNetworkTechnology,Infraestruturas de rede disponíveis.,"NetID, Tecnologia (Ex: 5G, FTTH)"



dCampaigns,Campanhas de Marketing ativas.,"CampID, Nome, CustoEstimado"





**Tabelas de fatos (Eventos de Negócio)**

**Registos históricos e quantitativos das operações.**



**Tabela,Descrição,Métricas e Chaves Estrangeiras**



fSubscriptions,Registo de novos contratos e fidelizações.,"SubscriptionID, CustomerID, ProductID, StartDate, EndDate, FidelizacaoMeses"



fBilling,Faturação mensal e estado de cobrança.,"BillID, SubscriptionID, CustomerID, BillDate, ValorCobrado, StatusPagamento"



fUsage,Consumo diário de rede (Dados e Voz).,"UsageID, CustomerID, Date, DadosConsumidosGB, MinutosVoz"



fTickets,Registo de apoio ao cliente e falhas.,"TicketID, CustomerID, Date, Motivo, TempoResolucaoHoras, FCR (First Call Resolution)"



fNPS,Inquéritos de satisfação do cliente.,"CustomerID, TicketID, Date, NPS\_Score, Categoria (Promotor/Detrator)"



fChurn,Registo de cancelamentos de serviço.,"ChurnID, CustomerID, Date, Motivo"



fIncidents,Quebras de serviço na infraestrutura.,"IncidentID, Date, NetID, RegionID, TempoIndisponibilidadeMin, ClientesAfetados"





