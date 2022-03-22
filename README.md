# Consulta em WebService Banco Central

    Esse programa consulta dados de moedas do Banco Central e converte os dados em pandas.DataFrame
    
    Funcionalidades
       * Consulta dados
       * Converte em dataframe
       * Filtro no dataframe
       * Gera Gráfico

    Dados de Acesso WebService:

       * moeda = 1,"Dolar (venda)",
                10813,"Dolar (Compra)",
                21619,"Euro (venda)",
                21620,"Euro (compra)",
                21621,"Iene (venda)",
                21622,"Iene (compra)",
                21623,"Libra esterlina (venda)",
                21624,"Libra esterlina (compra)",
                21625,"Franco Suíço (venda)",
                21626,"Franco Suíço (compra)",
                21627,"Coroa Dinamarquesa (venda)",
                21628,"Coroa Dinamarquesa (compra)"
                21629,"Coroa Norueguesa (venda)",
                21630,"Coroa Norueguesa (compra)",
                21631,"Coroa Sueca (venda)",
                21632,"Coroa Sueca (compra)",
                21633,"Dolar Australiano (venda)",
                21634,"Dolar Australiano (compra)",
                21635,"Dolar Canadense (venda)",
                21636,"Dolar Canadense (compra)"
       
        * wsdl: https://www3.bcb.gov.br/sgspub/JSP/sgsgeral/FachadaWSSGS.wsdl
        * endpoint: getValor(moedas,data)

    Funções:
        
       * RetornaDados(qtd_dias) -> Dados de entrada(qtd_dias = quantidade de dias) para consultar, 
                                    retorna o dataframe .
       * Filtro(fm,dados) -> Dados de entrada (fm = Filtro Moeda "Dolar (venda)"), 
                                    retorna o dataframe filtrando por moeda.
       * GeraGrafico(dados_Filtro) -> Gera o gráfico de acordo com filtro da função  Filtro
    
    Execução:
       
       python estudo.ws.py
    
    Referência: 
        https://pandas.pydata.org/pandas-docs/stable/index.html
        https://dadosabertos.bcb.gov.br/dataset/20740-taxa-media-de-juros-das-operacoes-de-credito-com-recursos-livres---pessoas-fisicas---total/resource/c5b4c37b-10f6-4d5f-8e84-b9e8ff56e9ff
