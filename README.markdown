jQuery Fundamentals' pt-BR Translation
=======================================


Este repositório é um submódulo do [repositório original](http://github.com/rmurphey/jqfundamentals) do livro jQuery Fundamentals da[Rebecca Murphey](http://github.com/rmurphey).

Gerando html, pdf ou epub
-------------------------

Este repositório contém apenas o conteudo do livro, não tendo assim, toda a infra disponível para geração destes formatos não se encontra aqui. Pra isso, você precisa fazer o clone do repositório original, rodar uma atualização de submódulos (este repo é um submódulo do original) e logo em seguida alterar o script de build para gerar o e-book na língua correta. Vamos aos passos:

    git clone git://github.com/rmurphey/jqfundamentals.git
    cd jqfundamentals
    git submodule init
    git submodule update
    cd book
    scripts/install.sh 
    vim scripts/publish-pdf.sh #mude a primeira linha para "input=src/pt-BR/jquery-fundamentals-book.xml" (sem as aspas)
    scripts/publish-pdf.sh 

Se tiver dado tudo certo, o livro em pdf estará em book/release/pdf
