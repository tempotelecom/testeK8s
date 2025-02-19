# testeK8s

## Objetivo
O propósito deste teste é verificar as habilidades do candidato a devOps nos seguintes critérios:
- docker
- k8s
- github
- habilidade de criar documentações para realização de setup
- CI/CD

## O teste
O teste deverá ser feito utilizando o seguinte projeto https://github.com/tempotelecom/conversao-temperatura
Deverá ser criada uma pipeline no github que atenda aos  seguintes critérios
- criação da imagem
- armazenamento dessa imagem em um repositorio de imagens (dockerhub)
- deploy da imagem criada automaticamente em ambiente de prod ao dar merge na master
- criação de um ambiente de preview ao subir um novo branch caso o dev adicione a label 'preview' no projeto
- ao remover o label ou fechar o PR ou dar merge no PR, o ambiente de preview deve ser destruido
- a pipeline deve rodar os testes em preview e master logo após a etapa de build.

Além da etapa da pipeline será avaliado os seguintes items
- criação do cluster k8s utilizando terraform
- versionamento do codigo do terraform em um repositorio github
- pipeline para o projeto terraform que aplica as alteraçoes no cluster ao mesclar no branch main

O teste tem um prazo de execução de uma semana a partir da data de envio.<br>
O retorno deverá ser por email junto com uma documentação no corpo do email das etapas para fazer o setup do cluster e ambientes<br>
Poderá ser utilizada uma conta gratuita free tier da aws ou até mesmo o Kind para execução do cluster<br>
O cluster deverá ter o control plain e dois nós.<br>
A pipeline a ser utilizada deverá ser o Github actions.<br>
Será avaliado a organização dos commits.<br>
Alterações após a entrega do código não serão consideradas.
