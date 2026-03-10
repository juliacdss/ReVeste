# Projeto Integrador - ReVeste
*ReVeste*

*ReVeste é um sistema web de brechó digital que permite os usuários anunciar e vender roupas de forma simples e organizada. A plataforma incentiva a moda sustentável e o reaproveitamento de peças, oferecendo um ambiente prático e intuitivo para compra e venda.*

**IMPORTANTE**: [**Cadastre seu projeto nesta planilha**](https://docs.google.com/spreadsheets/d/1bSb1-S9qOf46fNH8quyoFpcjcTuBMj_EdSPchOuFULY/edit?usp=sharing).

Professor: [Marco André Mendes](github.com/marcoandre)

Equipe:
- [Amanda Eduarda Andrade dos Santos](https://github.com/amandastss)
- [Anna Luiza Carvalho Araujo](https://github.com/annaaraujoifc).
- [Julia Costa da Silva](https://github.com/juliacdss).
- [Thayná de Oliveira Becker](https://github.com/thaynabecker)

Links do projeto:
(*Coloque aqui os links para a documentação do projeto e os repositórios e plubicação do backend e frontend.*)
-   [Documentação](https://github.com/juliacdss/ReVeste?tab=readme-ov-file#projeto-integrador---modelo)
-   Backend: [Repositório](github.com/marcoandre/pi-frontend) e [Publicação](https://pi-backend.herokuapp.com/)
-   Frontend: [Repositório](https://github.com/juliacdss/ReVeste.git) e [Publicação](https://pi-frontend.herokuapp.com/)

# 1. Desenvolvimento

**1.1 Modelo do Sistema**

O sistema escolhido para o projeto é um Ponto de Vendas (PDV) voltado para um brechó digital chamado ReVeste. O sistema permitirá o cadastro de produtos, o registro de vendas e o controle das peças disponíveis e já vendidas.

A escolha desse modelo se deu por ser uma ideia ligada ao cotidiano, já que a compra e venda de roupas usadas é comum atualmente, além de ser um tema interessante e fácil de compreender. Também foi escolhido por possibilitar o desenvolvimento de um sistema funcional e prático, adequado ao nível do curso.

# 2. Situação Problema

![Ciclo da Venda](docs/ciclo_da_venda.webp "Ciclo da Venda")

-   **Introdução**: O ReVeste é um brechó digital que atua por meio de uma plataforma web, permitindo que usuários anunciem e vendam roupas de forma prática. A empresa é recente e foi criada com o objetivo de incentivar a moda sustentável, promovendo o reaproveitamento de peças de vestuário. Atualmente, o funcionamento do sistema depende de processos simples e pouco automatizados, contando com uma pequena equipe responsável por organizar os anúncios e acompanhar as vendas realizadas na plataforma.
   
-   **Situação-problema**: No funcionamento atual do ReVeste, os usuários realizam o cadastro de suas peças manualmente, inserindo informações como nome do produto, descrição, preço e imagens. Essas informações ficam armazenadas de maneira básica, sem um padrão bem definido, o que pode gerar inconsistências nos dados e dificultar a organização dos anúncios dentro da plataforma.
   
Após o cadastro, as roupas ficam disponíveis para visualização de outros usuários, que podem demonstrar interesse e realizar a compra. No entanto, o controle dessas vendas não é feito de forma automatizada. Quando uma peça é vendida, é necessário que alguém registre manualmente essa informação, o que nem sempre acontece de forma imediata ou correta.
Como consequência, é comum que produtos já vendidos continuem aparecendo como disponíveis, causando confusão para os usuários e possíveis problemas nas negociações. Além disso, não existe um sistema eficiente para acompanhar o histórico de vendas, dificultando a análise do desempenho da plataforma e a tomada de decisões.

Outro ponto relevante é que, com o aumento do número de usuários e de anúncios, o controle manual se torna cada vez mais complexo. A equipe encontra dificuldades para organizar quais peças ainda estão disponíveis, quais já foram vendidas e manter uma visão geral do funcionamento da plataforma. Isso impacta diretamente na eficiência do serviço e na experiência dos usuários.

-   **Conclusão**: Diante desse cenário, fica evidente a necessidade de um sistema de Ponto de Vendas (PDV) que automatize o controle de produtos e vendas. A implementação de um software permitiria o cadastro padronizado das peças, a atualização automática do status dos produtos após cada venda e o registro organizado das transações realizadas. Dessa forma, o ReVeste poderia melhorar sua gestão interna, reduzir erros operacionais e oferecer uma experiência mais confiável e eficiente para seus usuários.

# 3. Descrição da proposta

A proposta do sistema ReVeste é desenvolver um software para organizar e facilitar o funcionamento de um brechó digital, permitindo que usuários anunciem e vendam roupas de forma prática dentro da plataforma. O foco principal do sistema é possibilitar o cadastro de produtos, o registro de vendas e o controle automático das peças disponíveis e já vendidas.

No sistema, existirão dois níveis principais de usuários: os usuários da plataforma e os administradores. Os usuários poderão criar uma conta, cadastrar roupas para venda e visualizar as peças anunciadas por outras pessoas. Ao cadastrar um produto, o usuário deverá informar dados como nome da peça, descrição, preço e imagem. Essas informações ficarão disponíveis para visualização dentro da plataforma.

Quando uma peça for vendida, o sistema registrará automaticamente essa venda e atualizará o status do produto, indicando que ele não está mais disponível. Isso evitará que itens já vendidos continuem aparecendo como disponíveis para outros usuários.

Os administradores do sistema terão acesso a funções de gerenciamento da plataforma, podendo acompanhar os produtos cadastrados, visualizar vendas realizadas e manter a organização geral do sistema.

Com a implementação do software, o ReVeste terá um processo mais organizado para o controle de anúncios e vendas, reduzindo erros no gerenciamento manual e proporcionando uma experiência mais eficiente para os usuários da plataforma.


# 4. Modelagem de Dados

(*Nessa parte a equipe deve descrever a modelagem de dados que será implementada no sistema. O texto abaixo descreve o que essa etapa deve conter e pode ser apagado depois.*)

Defina as entidades e relacionamentos que farão parte do sistema. Desenhe o diagrama de entidade-relacionamento (DER) e descreva as entidades e relacionamentos que farão parte do sistema.

# 4. Regras de negócio

As regras de negócio definem como o sistema deve funcionar e quais condições precisam ser seguidas para que as operações aconteçam corretamente. Elas ajudam a organizar os processos da plataforma, garantindo que o cadastro de produtos, as vendas e o controle das peças sejam realizados de forma padronizada e segura dentro do sistema ReVeste.

* Regras de Negócio do Sistema*

**RN01 – Cadastro de Usuário:**
Para utilizar as funcionalidades do sistema, o usuário deve realizar um cadastro informando seus dados básicos, como nome, e-mail, senha, telefone e CPF.

**RN02 – Login no Sistema:**
O acesso ao sistema só poderá ser realizado por usuários que possuam cadastro e informem corretamente e-mail e senha.

**RN03 – Cadastro de Produto:**
Para anunciar uma peça de roupa no sistema, o usuário deve cadastrar o produto informando pelo menos nome da peça, descrição, preço, marca e estado da peça.

**RN04 – Disponibilidade do Produto:**
Um produto só poderá ser exibido para compra se estiver com o status marcado como “disponível”.

**RN05 – Registro de Venda:**
Quando uma peça for vendida, o sistema deverá registrar automaticamente a venda e alterar o status do produto para “vendido”.

**RN06 – Atualização de Status do Produto:**
Após o registro da venda, o produto não poderá mais ser exibido como disponível para outros usuários.

**RN07 – Visualização de Produtos:**
Todos os usuários poderão visualizar as roupas anunciadas na plataforma.

**RN08 – Gerenciamento do Sistema:**
Administradores terão acesso a funções de gerenciamento, podendo visualizar todos os produtos cadastrados e acompanhar as vendas realizadas no sistema.

**RN09 – Integridade das Informações:**
O sistema não permitirá o cadastro de produtos com campos obrigatórios vazios, garantindo que as informações necessárias estejam sempre registradas.

# 5. Requisitos funcionais

Os requisitos funcionais definem as funcionalidades que o sistema ReVeste deverá possuir para atender às necessidades dos usuários da plataforma. Eles descrevem o que o sistema deve fazer para permitir o cadastro de usuários, o anúncio de roupas, o registro de vendas e a visualização das informações dentro do brechó digital.

*Entradas*

**R.F. 01 - Cadastro de Usuário:**
Permite que novos usuários criem uma conta no sistema para acessar a plataforma e utilizar suas funcionalidades, como anunciar e comprar roupas.
Dados necessários: nome, e-mail, cpf, telefone (opcional) e senha.
Usuários: visitantes da plataforma.

**R.F. 02 - Login de Usuário:**
Permite que usuários cadastrados acessem o sistema por meio de autenticação utilizando seus dados de login.
Dados necessários: e-mail, senha.
Usuários: usuários cadastrados e administradores.

**R.F. 03 - Cadastro de Produto:**
Permite que os usuários registrem uma peça de roupa para venda dentro da plataforma.
Dados necessários: nome do produto, descrição, preço, imagem, marca e status do produto.
Usuários: usuários cadastrados.

*Processos*

**R.F. 04 - Registro de Venda:**
Permite registrar quando um produto foi vendido dentro da plataforma, atualizando automaticamente o status da peça.
Dados necessários: produto, data da venda, status do produto.
Usuários: usuários e administradores.

**R.F. 05 - Atualização de Status do Produto:**
Atualiza automaticamente o status do produto após a realização de uma venda, alterando de “disponível” para “vendido”.
Dados necessários: produto, status do produto.
Usuários: sistema.

*Saídas*

**R.F. 06 - Visualização de Produtos:**
Permite que os usuários visualizem as roupas disponíveis para compra dentro da plataforma.
Dados necessários: nome do produto, descrição, preço, imagem, status do produto.
Usuários: todos os usuários.

**R.F. 07 - Visualização de Produtos do Usuário:**
Permite que o usuário visualize as roupas que ele anunciou na plataforma.
Dados necessários: nome do produto, descrição, preço, status do produto.
Usuários: usuários cadastrados.

**R.F. 08 - Visualização de Vendas:**
Permite que os administradores acompanhem as vendas realizadas na plataforma.
Dados necessários: produto vendido, vendedor, data da venda, status do produto.
Usuários: administradores.

# 6. Requisitos não funcionais

Requisitos não funcionais (**RNFs**) são as restrições impostas a um sistema que definem seus atributos de qualidade.

Eles geralmente são indicados por adjetivos como **segurança**, **desempenho** e **escalabilidade**.

**6.1 Categorias de requisitos não funcionais**

Os requisitos não funcionais são importantes porque ajudam a garantir que o sistema atenda às necessidades do usuário.

Os Requisitos Não Funcionais explicam as limitações e restrições do sistema a ser projetado. **Esses requisitos não têm nenhum
impacto na funcionalidade do aplicativo.** Além disso, existe uma prática comum de subclassificar os requisitos não funcionais em várias categorias:

- Interface de Usuário
- Confiabilidade
- Segurança
- Atuação
- Manutenção

Os requisitos não funcionais podem ser divididos em duas categorias:

1. **Atributos de qualidade:** Estas são as características do sistema que determinam sua qualidade geral. Exemplos de atributos de qualidade incluem segurança, desempenho e usabilidade.
2. **Restrições:** Estas são as limitações impostas ao sistema.
Exemplos de restrições incluem tempo, recursos e ambiente.

**6.2 Vantagens dos requisitos não funcionais**

Os requisitos não funcionais ajudam a garantir que o sistema seja:

1. Adaptado às necessidades do usuário.
2. Adequado à finalidade.
3. Escalável, seguro e confiável.
4. Fácil de usar e manter.

**6.3 Exemplos de requisitos não funcionais**

Aqui estão alguns exemplos de requisitos não funcionais:
1. **Segurança**: O sistema deve ser protegido contra acesso não
autorizado.
2. **Atuação**: O sistema deve ser capaz de lidar com o número necessário
de usuários sem qualquer degradação no desempenho.
3. **Escalabilidade**: O sistema deve ser capaz de aumentar ou diminuir
conforme necessário.
4. **Disponibilidade**: O sistema deve estar disponível quando necessário.
5. **Manutenção**: O sistema deve ser fácil de manter e atualizar.
6. **Portabilidade**: O sistema deve ser capaz de rodar em diferentes
plataformas com alterações mínimas.
7. **Confiabilidade**: O sistema deve ser confiável e atender aos requisitos
do usuário.
8. **Usabilidade**: O sistema deve ser fácil de usar e entender.
9. **Compatibilidade**: O sistema deve ser compatível com outros sistemas.
10. **Conformidade**: O sistema deve cumprir todas as leis e regulamentos
aplicáveis.

**6.4 Exemplo de organização dos requisitos não funcionais**

(_A seguir, um exemplo de organização de requisitos não funcionais._)

**Requisitos não funcionais:**

- **R.N.F. 01 - Nome do requisito não funcional:** descrição do requisito.
- **R.N.F. 02 - Nome do requisito não funcional:** descrição do requisito.

**Exemplos de requisitos não funcionais:**


**Sistema de Padaria**:
- **R.N.F. 01 - Navegador homologado:** O sistema deverá ser homologado para os navegadores Google Chrome e Mozilla Firefox.
- **R.N.F. 02 - Processador:** É recomendado para o sistema  no mínimo um processador Intel i3, similar ou superior a geração 7100 ou AMD Ryzen 3 da geração similar ou superior ao 3100, para que o servidor funcione em sua melhor performance.
- **R.N.F. 03 - Memória RAM:** é recomendável que o sistema possua no mínimo 2GB de RAM para melhor performance.
- **R.N.F. 04 - Arquitetura:** Será utilizada a arquitetiura MVC para o desenvolvimento do sistema, com uso de uma API REST para comunicação com o banco de dados.
- **R.N.F. 05 - Banco de dados:** O sistema será implementado com o banco de dados MySQL.
- **R.N.F. 06 - Conexão com banco de dados:** Para conexão com o banco de dados, o sistema utilizará a ferramenta de MySQL Connector.
- **R.N.F. 07 - Implementação:** O sistema deverá ser desenvolvido com linguagem Python, Javascript, HTML5, CSS3 e SQL.
- **R.N.F. 08 - Segurança:** Ficará a critério do responsável do estabelecimento a segurança dos acessos ao sistema, tendo consciência das pessoas que possua permissão para acesso.
- **R.N.F. 09 - Ambiente de Desenvolvimento Integrado (IDE):** Para criação do sistema, será utilizado o editor de texto Visual Studio Code.
- **R.N.F. 10 - Disponibilidade:** O sistema irá atender 99% do tempo de uso, somente ocorreria problemas de cadastro, remoção, inserção ou alteração em casos de falta de rede ou energia.
- **R.N.F. 11 - Legais:** O sistema deve atender às exigências da LGPD (Leis Gerais da Proteção de Dados).

**Sistema de Ordem de Serviço:**
- **R.N.F. 01 - Navegadores homologados:** o sistema deverá ser homologado para os navegadores Google Chrome e Mozilla Firefox.
- **R.N.F. 02 - Tecnologia Front-end:** Para a exibição em front-end, o software utilizará o CSS3 e o HTML5, além do framework Vue.js.
- **R.N.F. 03- Tecnologia Back-end:** O software será desenvolvido pela linguagem de programação Python, com o framework Django e a API REST com Django REST Framework.
- **R.N.F. 04 - Interoperabilidade:** O banco de dados será o MySQL, com a linguagem SQL de banco, sendo todo produzido através do MySQL Workbench .
- **R.N.F. 05 - Forma de uso do software:** O sistema por fazer parte de um ambiente interno, provavelmente será utilizado de acordo com as horas de trabalho da empresa, mas estará ativo 24 horas por dia em 7 dias por semana.
- **R.N.F. 06 - Desempenho:** Para a utilização correta e com uma qualidade e eficiência melhor, é recomendado que se use o SO mais atualizado, com recursos de hardware equivalentes a um processador intel i3 5°Gen ou semelhante, e 8GB de memória RAM, assim como os navegadores homologados.
- **R.N.F. 07- Autenticação:** Para realizar o acesso ao sistema é necessário ter um usuário de autenticação criado pelo administrador, além da possibilidade de solicitar um envio de redefinição de senha.
- **R.N.F. 08 - Web Server:** O servidor web utilizado será o Apache Tomcat, nas versões mais atualizadas.
- **R.N.F. 09 - Níveis de segurança:** O software terá diferentes tipos de acesso para cada tipo de login, tendo as permissões ideais a função de cada um.

**6.6 Conclusão**

Requisitos não funcionais são essenciais para qualquer sistema. Eles ajudam a garantir que o sistema atenda às necessidades do usuário e seja capaz de funcionar como pretendido.

É importante considerar cuidadosamente todos os requisitos não funcionais antes de projetar e desenvolver um sistema.
Eles ajudam a garantir que o sistema atenda às necessidades do usuário e seja capaz de funcionar como pretendido.

# 7. Diagrama de Caso de Uso

**Estrutura do Diagrama (como ficará)**

```
+----------------------+
|       Sistema        |
|       ReVeste        |
+----------------------+

Usuário
   |---- Criar conta
   |---- Fazer login
   |---- Cadastrar produto
   |---- Editar produto
   |---- Excluir produto
   |---- Visualizar produtos
   |---- Comprar produto
   |---- Visualizar status do produto
   |---- Ver histórico de vendas

Administrador
   |---- Fazer login
   |---- Gerenciar produtos
   |---- Visualizar usuários
   |---- Visualizar vendas
   |---- Gerar relatório de vendas
```

**Ideia visual do diagrama**

```
           Usuário
              |
   -------------------------
   |        ReVeste        |
   -------------------------
   | Criar conta           |
   | Fazer login           |
   | Cadastrar produto     |
   | Comprar produto       |
   | Visualizar produtos   |
   | Ver histórico         |
   -------------------------

           Administrador
                |
        ----------------
        | Gerenciar     |
        | produtos      |
        | vendas        |
        | usuários      |
        ----------------
```
