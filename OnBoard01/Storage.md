# **Azure Blob**
É praticamente o S3 da Azure, para começarmos, basta ir na aba "Contas de Armazenamento" e criar uma conta, após isso, você consegue deve criar um container.
![container](./imagens/container-blob.png)

### Container configurado para acesso anonimo:
![container](./imagens/containers%20(1).png)
![container](./imagens/containers%20(2).png)

# Google Cloud
No **Google Cloud**, ao invés de um blob, nós criamos um bucket, basta **selecionar o seu projeto** e ir em **Cloud Storage**. 
É bem intuitivo, na maioria das vezes é next-next, com exceção dessa opção abaixo:
![granularidade](./imagens/granularidade.png)
isso faz com que os dados não fiquem públicos.

No Google, é um pouco diferente da AWS, os arquivos ficam privados por padrão, precisando de autenticação para obter o acesso, podemos deixar público adicionando uma nova regra nessa tela:
![publico](./imagens/link-publico.png)
![publico](./imagens/link-publico(2).png)

# AWS
O mais falado, **Amazon S3**.
É bem intuitivo, basicamente next-next, a diferença é que, na criação do bucket, é possível visualizar a opção de dados públicos:
![AWS-public](./imagens/aws-public.png)
É possível desativa-la nas permissões do bucket.
Além de deixar o bucket público, é necessário mudar a permissão do arquivo individualmente, também na tela de permissões:
![public](./imagens/public%20permission.png)