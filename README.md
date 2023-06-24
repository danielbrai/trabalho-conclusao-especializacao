# Sobre
O presente template foi criado para servir de modelo para a elaboração de trabalhos acadêmicos segundo a Norma Técnica que rege tais publicações (ABNT). Como base, utilizou-se o projeto elaborado pelo autor [Michael Vornes](https://github.com/mvornes), que criou um modelo que atendesse às normas utilizadas pele Universidade Tecnológica Federal do Paraná, o qual pode ser encontrado [neste link](https://github.com/mvornes/latex-utfpr-proposta-tcc).

Este modelo, assim como aquele no qual o mesmo foi baseado, é uma adaptação da classe [abnTeX2](https://github.com/abntex/abntex2), e pode - e deve - ser estendido e modificado conforme a necessidade de cada publicação, em conformidade com os requisitos da instituição de ensino em questão; atualmente, o modelo está configurado para as necessidades das normas apresentadas pelo [Instituto Federal de Educação, ciência e Tecnologia de São Paulo (IFSP) - Campus Campinas](https://portal.cmp.ifsp.edu.br).

# Instruções de Uso
Para utilizar este modelo, siga conforme o proposto:

1. Dentro do diretório **configuracoes** é onde o modelo foi parametrizado; o arquivo `ifsp_campinas-abntex2.cls` contém a definição dos comandos criados para a construção do template.

2. Ainda no diretório **configuracoes**, há um subdiretório nomeado **variaveis**; em seu interior, há um conjunto de arquivos nomeados com o prefixo `dados-`: tais arquivos se prestam a servir como variáveis para parametrização dos comandos definidos no arquivo mencionado no tópico anterior, e é neles que deverá ser realizada a alteração para atender à necessidade de cada trabalho, tais como o nome do autor, título do artigo, curso, etc

3. O arquivo `ifsp_campinas-tcc.tex` orquestra como o LaTex estruturá o arquivo pdf final; caso haja necessidade de se alterar tal estrutura, este é o local onde essa alteração deverá ser executada.

4. Cada parte do artigo foi separada em diretórios que correspondem à como se estrutura um trabalho acadêmico; assim, dentro do diretório **estrutura** há 3 subdiretórios, que representam as seções de elementos pré-textuais, textuais e pós-textuais (os nomes condizem a que seção se referem); para o diretório de elementos textuais, há um subdiretório para cada capítulo.

5. Cada capítulo é composto por um arquivo principal e diversos outros secudários, representando subseções, que são gerenciados dentro do arquivo `root.tex`; para adicionar ou remover tais subseções, basta comentar ou descomentar as linhas na qual eles são incluídos no arquivo `root.tex`; além disso, para criar novas subseções, aconselha-se manter o padrão demonstrado, alocando as novas seções em arquivos apartados e fazendo sua inclusão através do comando `input`.