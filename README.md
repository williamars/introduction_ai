# Inteligência Artificial

Este projeto possui o material da disciplina sobre Inteligência Artificial.

Este projeto possui dois diretórios: 

* [code](code/): onde você irá encontrar todo o código fonte em Python necessário para o andamento desta disciplina. 
* [docs](docs/): pasta com todo o material adicional, slides, exercícios e outros documentos.

## Setup do ambiente para execução dos exercícios

Configurando um ambiente virtual:

````bash
python3 -m virtualenv venv
source venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
````

## Publicar nova versão da página web

Para publicar o novo conteúdo da página web basta fazer um `push` para o branch gh-pages:

````bash
mkdocs gh-deploy
````

No repositório existe uma action configurada para fazer o deploy do conteúdo na página [http://fbarth.net.br/agents/](http://fbarth.net.br/agents/).

## Compilando material escrito em Markdown

Segue um exemplo sobre como compilar os materiais que estão em markdown: 

````bash
pandoc -t beamer slides.md -o slides.pdf
````
