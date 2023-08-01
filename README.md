<h1>API Gateway para Comunicação e Registro de Requisições entre Microservices</h1>

  <h2>Descrição do Projeto</h2>
    <p>Este projeto é um API Gateway desenvolvido em Java 11, utilizando as tecnologias JPA, Spring Cloud, Hibernate e Lombok, que tem como principal função facilitar a comunicação entre microservices em uma arquitetura distribuída. O API Gateway é responsável por receber as requisições dos clientes e direcioná-las aos microservices apropriados, além de registrar os dados das requisições em um banco de dados para fins de auditoria.</p>

  <h3>Principais Funcionalidades</h3>
    <ol>
        <li><strong>Roteamento de Requisições:</strong> O API Gateway gerencia a rota das requisições recebidas dos clientes para os respectivos microservices, facilitando o controle de endpoints e evitando a necessidade de conhecimento detalhado da estrutura interna dos microservices.</li>
        <li><strong>Armazenamento de Requisições:</strong> A cada requisição recebida pelo API Gateway, os dados são registrados e salvos no banco de dados. Isso permite a posterior análise e auditoria das requisições realizadas ao sistema.</li>
        <li><strong>Backup de Requisições:</strong> O projeto inclui um job schedule que é executado diariamente às 3h da manhã. Esse job é responsável por gerar um backup das requisições armazenadas no banco de dados, garantindo que esses registros estejam disponíveis para fins de auditoria mesmo em situações de falhas ou perda de dados.</li>
    </ol>

  <h3>Tecnologias Utilizadas</h3>
    <p>O projeto foi desenvolvido utilizando as seguintes tecnologias e bibliotecas:</p>
    <ul>
        <li>Java 11: Linguagem de programação principal do projeto, garantindo o uso de recursos mais modernos e eficientes.</li>
        <li>JPA (Java Persistence API): Utilizado para facilitar a persistência dos dados no banco de dados relacional, fornecendo uma camada de abstração sobre o Hibernate.</li>
        <li>Spring Cloud: Framework que fornece ferramentas e bibliotecas para o desenvolvimento de sistemas distribuídos em uma arquitetura de microservices.</li>
        <li>Hibernate: Framework de mapeamento objeto-relacional que simplifica a integração entre o Java e o banco de dados.</li>
        <li>Lombok: Biblioteca que reduz a verbosidade do código Java através de anotações, tornando o código mais limpo e conciso.</li>
    </ul>

  <h3>Próximos Passos</h3>
    <p>O projeto está em constante evolução, e os próximos passos incluem:</p>
    <ul>
        <li><strong>Integração com Microservices:</strong> A integração completa com todos os microservices do sistema, garantindo um fluxo de comunicação eficiente e seguro.</li>
        <li><strong>Jenkins ou RabbitMQ:</strong> A integração de ferramentas como Jenkins ou RabbitMQ para melhorar a eficiência e escalabilidade do sistema, bem como otimizar a integração contínua e a troca de mensagens assíncronas entre os microservices.</li>
        <li><strong>Documentação Detalhada:</strong> A criação de uma documentação detalhada do projeto, incluindo informações sobre a arquitetura, endpoints disponíveis, configuração do banco de dados e instruções de implantação.</li>
    </ul>

  <h3>Como Contribuir</h3>
    <p>Contribuições são bem-vindas! Se você deseja contribuir para o projeto, siga os passos abaixo:</p>
    <ol>
        <li>Faça um fork deste repositório.</li>
        <li>Crie uma branch com um nome descritivo para a sua contribuição.</li>
        <li>Implemente suas melhorias ou correções.</li>
        <li>Crie testes para garantir a integridade das mudanças.</li>
        <li>Abra um Pull Request detalhando suas alterações e aguarde a revisão.</li>
    </ol>

  <h3>Licença</h3>
    <p>Este projeto está licenciado sob a licença <a href="link_para_licenca.txt">MIT</a>. Você é livre para usar, modificar e distribuir o código conforme os termos da licença.</p>
