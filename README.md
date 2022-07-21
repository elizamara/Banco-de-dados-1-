Trabalho 2 de Banco de Dados 1 ( =* . *= )

O trabalho 2 da disciplina Banco de dados 1 tem o objetivo de implementar e simular o comportamento de acessos a dados armazenados em memória secundária.
A implementação será feita utilizando programas de armazenamento e estruturas de arquivo de dados e índice. 



* Conceitos que precisam ser entendidos:

    **Registros:** uma coleção de itens ralcionados. Podem ter tamanho e formato fixo ou variável.

    **Formato:** pode ser referir ao tamanho e organização dos campos de um registro.
    
    **Campos:** os itens são chamados de campos

    **Arquivos:** coleções de registros de mesmo tipo. Os registros podem ter tamanho e formatos iguais.

     **Blocos:** são a menor unidade de transferência para a memória principal. Os blocos são representações lógicas e são mapeados de forma sequêncial.
                 Um bloco pode conter um ou mais setores do disco e de maneira sequencial. 
                 Os blocos armazenam fisicamente registros de um arquivo, ou de arquivos diferentes.
                 
    Exemplo:

* Disco Magnéticos:

    *Prato:* é basicamente um disco, onde são armazenados os dados. 
    
    *Trilhas:* são as organizações do patro no disco. "O prato é divido em regiões anulares chamadas de trilhas."  
    
    *Setores:* é adivisão da trilha, ou seja, uma trilha é divida em setores, setores são denominadas a menor unidade física do disco.  


* Registros:

    **Alocação Não-Espalhada:** preenche os blocos com todos os registros possíveis e deixa um espaço sobrando se não couber outro registro.

    **Alocação Espalhada:** possui um apontador para parte de um ragistro **R** no **Bloco 2** que não coube no **Bloco 1**. 



* Buffers:
    **Buffers:** os buffers contem cópias dos blocos que estão no disco. Os buffers itermediam os acessos aos blocos de disco e, os blocos são lidos do disco, armazenado em buffers em memória principal. 