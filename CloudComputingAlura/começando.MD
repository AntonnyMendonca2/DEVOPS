# Começando com cloud

## O que é a nuvem?
Uma nuvem pode ser entendida como um conjunto de aplicações, armazenamento e computação que tem como base a internet como plataforma de funcionamento. E esse pool de serviços possui capacidade suficiente para dar suporte à maioria das necessidades de grande parte dos usuários.

![image](./imagens/cloud.png)


## Matera
empresa especializada em bancos e fintecs.
> curiosidade do PIX: disponível 24/7, confiabilidade de 99.9%, pagamentos tem que responder em até 1.9 segundo e recebimento em até 2.3 segundos.

O pix é baseado em microsserviços. Utiliza kubernets

**helm charts** é basicamente uma infraestrutura para códigos para coisas que estão dentro do kubernets, dentro do kubernets temos os pods e regras para conversar entre eles, no helm charts podemos automatizar a criação dessas construções em um script único que podem ser parametrizados, o helm charts é basicamente um template para configurações do kubernets. (minhas palavras: é como se fosse um dockercompose, dizendo beeeem forçadamente.)

No matera, vários tipos de testes e mocks foram criados, o que é normal em uma empresa grande.

## Desvantagens do CLOUD!!!
- Dependência da rede.
- Falhas na estrutura do data center ou em algum servidor podem impedir o trabalho ou uso do recurso oferecido pela nuvel.
- Falhas no acesso podem ocorrer por recursos compartilhados entre empresas (pode acontecer em alguns provedores)
- Perda ou sequestro dos dados podem ocorrer (difícil)


## Modelos de cloud
![image](./imagens/modeloCloud.png)

### **IaaS** - Infrastructure as a Service
Esse modelo disponibiliza um ambiente com uma infraestrutura virtualizada, possibilitando o uso de recursos de computação, armazenamento e rede.

Serviços que utilizam:

>Amazon Web Service

>Google Compute Engine

<br>

### **PaaS** - Plataform as a Service

No PaaS, é criado um ambiente para **programação** e o desenvolvimento de alguma solução, temos um programa ou serviço entregue com o objetivo de facilitar a implementação de algum serviço.

Exemplos de PaaS:
>Heroku

>Red Hat OpenShift

<br>

### **SaaS** - Software as a Service

O software é executado em um servidor, tirando a necessidade do cliente tê-lo instalado em sua máquina.

Exemplo de SaaS:
>Gupy

>Trello

Alguns desafios para esse tipo de modelo são a dificuldade da integração dos recursos internos da organização, disponibilidade e segurança da informação.


## Tipos de CLOUD

Atualmente, temos três tipos de cloud, assim como na imagem abaixo:
![image](./imagens/tiposDeCloud.png)

**Cloud Pública**: É o tipo que mais vemos sendo utilizados por empresas. Basicamente, a cloud pública compartilha, através de uma gama de servidores interconectados, recursos e serviços entre usuários.

**Cloud Privada**: Diferente da Cloud Pública, os recursos e serviços utilizados por uma empresa é de exclusividade da mesma, sendo assim, um data center é alocado somente para esse objetivo, podendo ser cuidado pela própria empresa.

**Cloud Hibrida**: A nuvem hibrida é a junção da nuvem privada com a nuvem pública, uma empresa pode manter sua aplicação rodando em uma nuvem pública e seus dados em uma nuvem privada, por exemplo.

> Um termo muito utilizado nesse ramo é o *On Promise*, trata-se de um ambiente onde fica as máquinas em um espaço físico da empresa, em contrapartida temos  um ambiente em nuvem.


# Case BancoPAN
O case aborda a introdução da Cloud no banco pan. Principal dificuldade era o monitoramento e a dificuldade para identificar erros na hora de subir mudanças, antes eram on-premise, ou seja, rodando local, agora está hibrido com a nuvem.

termos utilizados:
- **On-premise:** software local é instalado e executado em computadores nas instalações da pessoa ou organização que usa o software, em vez de em uma instalação remota, como um farm de servidores ou nuvem.
- **Monolíto:** Arquitetura Monolítica é um sistema único, não dividido, que roda em um único processo, uma aplicação de software em que diferentes componentes estão ligados a um único programa dentro de uma única plataforma.
- **Microsserviços:** Microsserviços são uma abordagem arquitetônica e organizacional do desenvolvimento de software na qual o software consiste em pequenos serviços independentes que se comunicam usando APIs bem definidas. Esses serviços pertencem a pequenas equipes autossuficientes.
- **arquitetura orientada a eventos ( EDA ):** É um padrão de design de software que permite a uma organização detectar "eventos" ou momentos de negócios importantes (como uma transação, visita ao local, abandono do carrinho de compras, etc.) e agir sobre eles em tempo real ou quase real.


## Multicloud
Em uma multicloud, encontramos a utilização de mais de um serviço de provedores de nuvem publica ou privada, por definição, "toda nuvem híbrida é uma multicloud, mas nem toda multicloud é uma nuvem híbrida".

![image](./imagens/multicloud.png)
 A escolha de uma abordagem multicloud, combinando a utilização de mais de um provedor de serviço de nuvem, pode favorecer estratégias que possibilitam:

- **Diminuir a indisponibilidade:** Replicando dados e serviços.

- **Redução de custos:** Distribuira a carga de trabalho entre as nuvens contratadas.

- **Melhor resposta a desastres:** Sistema pode não cair totalmente, podemndo conter cópias de segurança em cada cloud.

- **Flexibilização geográfica:** Podemos ter diferentes servidores localizados em diferentes países ou regiões.

- **Utilizando o melhor de cada um:** Cada Cloud tem um ponto forte que se destaca dos demais, podemos utilizar isso ao nosso favor.

# Principais plataformas de cloud

### **AWS ou Amazon Web Services**
É a plataforma de cloud da Amazon. Lançada em 2006, provê uma série de serviços para desenvolvedores e empresas hospedarem e manterem aplicações e infraestrutura.

### **Azure**
A Microsoft também possui sua plataforma de nuvem com a oferta de produtos e serviços em tecnologia, o Azure. Ele foi apresentado ao mundo em 2008 com o nome de Windows Azure, mas somente em 2010 teve o seu lançamento oficial para o mercado. Em 2014, passou a ser chamado de Microsoft Azure, como é conhecido até hoje.

### **Google Cloud**
Plataforma do Google que entrega uma suite (conjunto de ferramentas) para computação em nuvem, o que possibilita criar, implantar e gerenciar aplicativos na nuvem, além de oferecer infraestrutura para hospedagem de sites, máquinas virtuais, bancos de dados, entre outros.



# Microsoft Azure - Hipsters Ponto Tech

> Multicloud, Hybrid cloud and Edge Computing são palavras chaves.


- **Lift and Shift:** O modelo Lift and shift, também conhecido como rehosting, é uma abordagem para migrar aplicativos para a nuvem. Esta estratégia não envolve alterações na arquitetura do aplicativo e quase nenhuma (ou nenhuma) alteração no código do aplicativo, possibilitando consequentemente uma migração mais rápida e barata.

O tipo de cloud mais procurado por empresas são os **IaaS**, mais especificamente, as máquinas virtuais onde fazer o *lift and shift* das suas aplicações que rodam *on premise* são essenciais para a migração pra nuvem.

<iframe width="544" height="304" src="https://www.youtube.com/embed/yKnkK4HxW8E" title="Terraform e máquinas virtuais no Google Cloud | #AluraMais" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

    