#JPA

##Métodos do entity manager:
###persist -> Transforma uma entidade transient em uma entidade managed (Insert no banco)
Recebe como argumento o objeto entidade a ser inserido no banco.

###find-> Select no banco
Retorna um objeto entidade e recebo como argumento a classe entidade e o id do registro desejado na tabela.

###remove->Delete o banco
Recebe a entidade a ser removida e a remove do banco.
Se passar uma entidade detached, ele da erro, tem que usar o find pra pegar uma entidade managed

###begin-> Abre o entity manager para realização de operações

###close-> Fecha o entity manager

###commit -> Faz o commit das operações (essencial)

###merge->Transforma uma entidade detached em managed (Insert ou update no banco)
Pode ser usado para atualizar dados na tabela, porem ha meios melhores (set)


###Para transformar duas relaçoes em uma relacao bidirecional->usar o mappedBy na anotação

###So há necessidade de abrir uma transaction se for fazer update ou insert no banco (commit) 

##Funções da query:

###sum -> retorna a soma dos valores buscados na query

###avg -> retorna a media dos valores buscados na query

###count -> retorna a quantidade de valores buscado na query