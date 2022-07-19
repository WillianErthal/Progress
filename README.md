# Progress
Projetos em Progress 4GL


Informativo:
Utilitário PRODB(Utilizado para criar bancos em modo caractere)

Cria um novo banco de dados Progress.
O PRODB cria um novo banco de dados a partir de um banco de dados de origem especificado. 
PRODB cria um novo banco de dados usando a estrutura do banco de dados de origem e coloca todas as extensões no banco de dados atual
diretório de trabalho. 
Você pode usar o PRODB para fazer uma cópia de qualquer demonstração de banco ou zerar Bancos de dados Progress.

****Não use palavras-chave Progress 4GL ou caracteres especiais, como vírgulas ou ponto e vírgula.


Além do banco de dados vazio padrão, o PRODB permite que você crie outros
estruturas de banco de dados com diferentes tamanhos de bloco:
• empty (padrão)
• empty1 (tamanho do bloco 1K) 
• empty2 (tamanho do bloco 2K)
• empty4 (tamanho do bloco 4K)
• empty8 (tamanho do bloco 8K)


Estrutura de Arquivos do Banco:
.db - Arquivo principal do banco de dados. Contém o esquema do banco de dados
.lg - Arquivo de log do banco de dados. Contém informações de log em formato de texto
.st - Arquivo da estrutura do banco de dados. 
.d? - Os dados gravados.
.b? - Arquivos antes da imagem. Contém informações sobre transações em processo.
.lk - Arquivo de Lock do banco significa que o banco esta em uso.

**Lista de Comandos:

**Modelo
FOR EACH nomeTabela NO-LOCK WHERE nomeTabela.nomeCampo = "" :
END.

FOR EACH Customer NO-LOCK:
    DISPLAY Customer.Name.
END.


FOR EACH Customer NO-LOCK WHERE Customer.NAME = 'Lift tours' :
    DISPLAY Customer.Name.
END.
