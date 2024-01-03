O domínio é o problema, em termos de negocio , que precisa ser resolvido **independente  da tecnologia que será utilizada .**

O DDD se divide em duas partes

Strategic DDD (context Map) 
- **Visão geral do domínio:** concentra-se na compreensão da estrutura e relacionamentos gerais do domínio de negócios.
- **Ferramentas:**
    - **Contextos delimitados:** Dividindo o domínio complexo em áreas menores, autocontidas, com limites claros, cada uma com seu próprio modelo de domínio, terminologia e responsabilidades.
    - **Mapa de contexto:** Visualizando como os contextos delimitados interagem entre si, identificando pontos de integração e conflitos potenciais.
    - **Linguagem ubiqua:** Criando um vocabulário compartilhado entre especialistas do domínio e desenvolvedores para garantir uma representação precisa do domínio.

**Atividades principais:**

1. **Exploração do domínio:** Colaborando com especialistas do domínio para entender profundamente os conceitos, relacionamentos e regras do domínio.
2. **Identificação de contextos delimitados:** Definindo os limites de cada contexto com base na coesão e acoplamento dos conceitos de domínio.
3. **Criação de mapa de contexto:** Visualizando como os contextos interagem e se comunicam, considerando padrões de integração como núcleo compartilhado, cliente-fornecedor ou camada anticorrupção.
4. **Desenvolvimento da linguagem ubiqua:** Refinando a linguagem para garantir uma compreensão compartilhada e consistência ao longo do projeto.

 

Tatical DDD: (Domain model inside a bounded context )

**DDD Tático:**

- **Projeto e implementação detalhados de modelos de domínio dentro de contextos delimitados individuais.**
- **Ferramentas:**
    - **Entidades:** Objetos com uma identidade única que persistem ao longo do tempo, representando conceitos de domínio centrais.
    - **Objetos de valor:** Objetos que descrevem uma característica ou atributo sem uma identidade distinta, frequentemente usados para aprimorar entidades.
    - **Agregados:** Aglomerados de entidades e objetos de valor tratados como uma unidade para alterações de dados, garantindo consistência e integridade.
    - **Serviços de domínio:** Operações que não se encaixam naturalmente em entidades ou objetos de valor, encapsulando a lógica do domínio.
    - **Repositórios:** Interfaces que fornecem acesso a objetos de domínio, isolando detalhes de persistência do modelo de domínio.
    - **Eventos de domínio:** Notificações de eventos de domínio significativos, usados para comunicação entre contextos delimitados ou acionamento de ações.

**Atividades principais:**

1. **Projeto do modelo de domínio:** Criando um modelo detalhado do domínio dentro de um contexto delimitado, usando entidades, objetos de valor, agregados e serviços.
2. **Implementação da lógica do domínio:** Encapsulando regras e comportamentos do domínio dentro de objetos e serviços de domínio.
3. **Projeto de persistência:** Escolhendo estratégias de persistência apropriadas, garantindo a integridade do modelo de domínio.
4. **Teste e validação:** Garantindo que o modelo de domínio reflita com precisão os requisitos de negócios e se comporte conforme o esperado.

**Resumo:**

- **DDD Estratégico** molda a arquitetura geral de um sistema DDD, garantindo o alinhamento com as necessidades de negócios e os limites do domínio.
- **DDD Tático** concentra-se no design e implementação detalhados de modelos de domínio dentro de contextos delimitados, promovendo uma linguagem de domínio rica e expressiva.

**Juntos, eles permitem a criação de software que está intimamente alinhado com o domínio de negócios, promove uma compreensão compartilhada entre desenvolvedores e especialistas do domínio e é adaptável às necessidades de negócios em evolução.**

**Aqui estão alguns exemplos de como o DDD pode ser usado para melhorar o desenvolvimento de software:**

- **Aumentar a precisão do software:** O DDD ajuda a garantir que o software reflita com precisão o domínio de negócios, o que pode levar a um software mais preciso e confiável.
- **Melhorar a comunicação entre desenvolvedores e especialistas do domínio:** A linguagem ubiqua do DDD fornece um vocabulário comum para desenvolvedores e especialistas do domínio, o que pode facilitar a comunicação e o entendimento mútuo.
- **Facilitar a manutenção do software:** O DDD ajuda a organizar o software de forma lógica e consistente, o que pode facilitar a manutenção e a evolução do software ao longo do tempo.




