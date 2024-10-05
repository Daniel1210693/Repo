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
