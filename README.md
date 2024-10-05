# Introdução

Este projeto, desenvolvido no âmbito do Mestrado em Engenharia Informática do Instituto Superior de Engenharia do Porto, visa explorar o controlo de versões através da utilização do Git, uma ferramenta essencial na gestão de código em projetos colaborativos. Dividido em duas partes, o trabalho foca-se inicialmente na utilização da branch principal, sem ramificações, para a implementação de uma funcionalidade básica. Na segunda fase, é introduzida a criação e a gestão de branches para o desenvolvimento de novas funcionalidades e correção de erros.
Adicionalmente, o projeto desafia os alunos a proporem uma solução tecnológica alternativa ao Git, analisando comparativamente as suas características e implementando um design que possa cumprir os requisitos apresentados.
Os resultados deste trabalho serão documentados num ficheiro readme.md no repositório do grupo, com uma explicação detalhada dos passos e decisões tomadas durante o desenvolvimento, facilitando a sua reprodutibilidade.

# Tutorial
## 1º Passo - Criar o Repositório
Como ponto inicial, o primeiro objetivo é a criação do repositório para o desenvolvimento do projeto.

    git clone https://github.com/rubenrodrigues19/cogsi2425_1210693_1231423_1240490.git

Este comando faz uma cópia do repositório remoto especificado no GitHub para o teu computador, criando uma cópia local do projeto.

    echo " cogsi2425_1210693_1231423_1240490" >> README.md

Este comando adiciona o texto "cogsi2425_1210693_1231423_1240490" ao ficheiro README.md. Se o ficheiro não existir, ele será criado automaticamente. O README.md serve como um documento principal para descrever o projeto.

    git init

Inicializa um novo repositório Git no diretório atual, tornando-o um repositório Git local (caso ainda não tenha sido inicializado).
  
    git add README.md

Adiciona o ficheiro README.md à "staging area", preparando-o para ser incluído no próximo commit.

    git commit -m "Readme"

Este comando grava as mudanças registadas na "staging area" com uma mensagem de commit, neste caso, "Readme", descrevendo a alteração feita.

    git branch -M main

Muda o nome da branch atual (que, por defeito, pode ser master) para main, estabelecendo-a como a branch principal do repositório.

    git push -u origin main

Envia as mudanças locais (o commit feito anteriormente) para o repositório remoto (no GitHub), especificando a branch main como a branch para envio padrão no futuro.

## 2º Passo – Criar a Pasta CA1

Após se concluir o primeiro passo, o segundo objetivo é criar uma pasta (CA1) onde irá ser copiado e armazenado uma versão do projeto Building REST

    cd /caminho/para/o/repositório/local

Navega até o diretório local onde o repositório Git está armazenado. Este é o local onde a nova pasta CA1 será criada.

    mkdir CA1

Cria uma nova pasta chamada CA1 dentro do repositório local. Esta pasta será usada para organizar os ficheiros relacionados ao primeiro trabalho da disciplina.

    cp /caminho/de/origem/* /caminho/de/destino/CA1

Copia todos os ficheiros da origem especificada para a nova pasta CA1.
    
    git status

Exibe o estado atual do repositório, mostrando quais ficheiros foram modificados ou adicionados e estão prontos para levarem commit, ou se há ficheiros não rastreados.

    git add . 

Adiciona todos os ficheiros e alterações na pasta atual (neste caso, incluindo a nova pasta CA1 e os ficheiros dentro dela) à "staging area", preparando-os para o commit.

    git commit -m "Pasta CA1"

Grava um snapshot do estado atual dos ficheiros adicionados, com uma mensagem de commit descrevendo as alterações feitas. Aqui, a mensagem indica que a pasta CA1 foi criada e adicionada.
    
    git push -u origin main

Envia as alterações locais para o repositório remoto (GitHub), na branch main. O parâmetro -u define origin/main como o destino padrão para futuros git push, facilitando o envio de futuras alterações.

## 3º Passo - Criar Tag

Neste passo, o objetivo é desenvolver uma tag para marcar a primeira versão do projeto

    git tag 1.1.0

Este comando cria uma nova tag chamada 1.1.0 no repositório local. As tags são usadas para marcar versões específicas de um projeto, servindo como referências importantes. Neste caso, a tag 1.1.0 indica que esta versão é a primeira grande versão.

    git push origin 1.1.0

Este comando envia a tag 1.1.0 para o repositório remoto (GitHub). Assim, a tag criada localmente será também visível e acessível para qualquer pessoa que tenha acesso ao repositório remoto, marcando esta versão como um ponto importante do desenvolvimento.

    git fetch –tags

Este comando faz o download de todas as tags do repositório remoto para o repositório local. Garante que todas as tags remotas sejam atualizadas e disponíveis localmente.

## 4º Passo – Criação da Nova Feature (jobYears)

Ao longo deste ponto o objetivo é desenvolver a feature jobYears, para isso, deve ser adicionado um novo campo para registar os anos de serviço do empregado na empresa (por exemplo, jobYears). O suporte para este novo campo deve ser implementado, garantindo que apenas valores inteiros são permitidos. Além disso, devem ser criados testes unitários para validar a criação de empregados e verificar os seus atributos, assegurando que não há valores nulos ou vazios. Após a conclusão e testagem da nova funcionalidade, o código deve ser comprometido e enviado, seguido da criação de uma nova tag (ex.: v1.2.0).

![Teste](img/Imagem1.png)
