#JPA

##Métodos do entity manager:
###persist -> Insert no banco 
Recebe como argumento o objeto entidade a ser inserido no banco.

###find-> Select no banco
Retorna um objeto entidade e recebo como argumento a classe entidade e o id do registro desejado na tabela.

###remove->Delete o banco
Recebe a entidade a ser removida e a remove do banco.

###begin-> Abre o entity manager para realização de operações

###close-> Fecha o entity manager

###commit -> Faz o commit das operações (essencial)

###merge->Transforma uma entidade detached em managed
