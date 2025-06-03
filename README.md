Formulário de Avaliação de Maturidade de Segurança OWASP SAMM

Visão Geral
Esta é uma aplicação web de página única projetada para facilitar a avaliação da maturidade de segurança de squads de desenvolvimento de software, utilizando o modelo OWASP SAMM (Software Assurance Maturity Model). A ferramenta permite que as equipes (squads) autoavaliem as suas práticas de segurança em diversas funções de negócio, selecionem níveis de maturidade para cada prática e exportem os resultados para um arquivo CSV.

O objetivo principal é ajudar as equipes a entender o seu nível atual de maturidade em segurança, identificar áreas de melhoria e planear a evolução das suas práticas de segurança.

Funcionalidades Principais
Informações da Squad: Permite inserir detalhes básicos sobre a squad que está a ser avaliada, como nome, avaliador, data, tamanho e comentários adicionais.

Avaliação Interativa: Para cada prática de segurança dentro das funções de negócio do SAMM, o utilizador pode selecionar um dos quatro níveis de maturidade (0 a 3).

A seleção de um nível é visualmente destacada.

Cada nível apresenta um título, uma descrição detalhada e exemplos práticos.

Barra de Progresso: Indica visualmente a percentagem de práticas de segurança já avaliadas.

Preenchimento Automático da Data: O campo "Data da Avaliação" é preenchido automaticamente com a data atual, mas pode ser alterado.

Exportação para CSV:

Gera um arquivo CSV com todas as informações da squad e os detalhes de cada prática avaliada (Função de Negócios, Prática de Segurança, Código da Prática, Nível Selecionado, Título do Nível e Descrição do Nível).

Utiliza ponto e vírgula (;) como delimitador para melhor compatibilidade com o Microsoft Excel em configurações regionais que o utilizam como padrão (ex: Português do Brasil).

O nome do arquivo CSV gerado inclui o nome da squad e um timestamp para fácil identificação (ex: Avaliacao_SAMM_NomeDaSquad_YYYYMMDDTHHMMSS.csv).

O botão de exportação fica desabilitado até que pelo menos uma prática seja avaliada.

Cálculo de Pontuação (Placeholder): Um botão "Submeter Avaliação" calcula e exibe uma pontuação média com base nas práticas avaliadas. Esta funcionalidade é um placeholder e pode ser expandida.

Design Responsivo (Básico): A interface é desenhada para ser visualmente agradável e funcional em diferentes tamanhos de ecrã, embora otimizações mais avançadas possam ser implementadas.

Como Utilizar
Abrir a Aplicação: Abra o arquivo Formulário OWASP SAMM - Avaliação de Maturidade de Segurança.html num navegador web moderno ou acesse https://lrosario.com.br/owasp-samm/

Preencher Informações da Squad:

Insira o "Nome da Squad".

Insira o "Nome do Avaliador".

Verifique ou ajuste a "Data da Avaliação".

Selecione o "Tamanho da Squad".

Adicione quaisquer "Comentários Adicionais" relevantes.

Realizar a Avaliação:

Navegue por cada Função de Negócios (Governança, Projeto, Implementação, Verificação, Operações).

Para cada "Prática de Segurança" listada:

Leia a descrição da prática e os exemplos.

Clique no "Nível de Maturidade" (0, 1, 2 ou 3) que melhor representa a situação atual da sua squad. A seleção será destacada.

A barra de progresso será atualizada à medida que avalia as práticas.

Exportar os Resultados:

Após avaliar pelo menos uma prática (idealmente todas), o botão "Exportar para CSV" será habilitado.

Clique no botão "Exportar para CSV".

Um arquivo CSV será gerado e descarregado automaticamente pelo seu navegador.

Submeter Avaliação (Opcional/Placeholder):

Clique no botão "Submeter Avaliação" para ver uma pontuação média placeholder.

Estrutura da Avaliação SAMM
A avaliação está organizada de acordo com as cinco Funções de Negócios do OWASP SAMM:

Governança: Como a squad organiza, planeia e gere as atividades de segurança.

Estratégia e Métricas de Segurança (SM)

Políticas e Conformidade (PC)

Educação e Treinamento em Segurança (EG)

Projeto: Como a squad planeia a segurança desde o início do ciclo de vida do desenvolvimento.

Análise de Ameaças (TA)

Requisitos de Segurança (SR)

Arquitetura de Segurança (SA)

Implementação: Como a squad constrói e entrega software seguro.

Build Seguro (SB)

Deploy Seguro (SD)

Gerenciamento de Defeitos (DM)

Verificação: Como a squad testa e valida a segurança do software.

Revisão de Requisitos de Segurança (SRV)

Testes de Segurança (ST)

Revisão de Código Seguro (SCR)

Operações: Como a squad mantém a segurança do software em produção.

Gerenciamento de Incidentes (IM)

Gerenciamento de Configurações de Segurança (SCM)

Gerenciamento de Vulnerabilidades (VM)

Detalhes da Exportação CSV
O arquivo CSV gerado contém as seguintes colunas:

Nome da Squad

Nome do Avaliador

Data da Avaliação

Tamanho da Squad

Comentários Adicionais

Função de Negócios SAMM

Prática de Segurança SAMM

Código da Prática

Nível Selecionado (0-3, ou "N/A" se não avaliado)

Título do Nível (ou "Não Avaliado")

Descrição do Nível (ou "Não Avaliado")

Detalhes Técnicos
Frontend: HTML5, CSS3, JavaScript (Vanilla JS).

Estrutura: Página única, sem dependências de frameworks externos para a lógica principal.

Estilização: CSS puro para apresentação visual.

Possíveis Melhorias Futuras
Implementar uma lógica de pontuação mais detalhada e visualização gráfica dos resultados.

Adicionar persistência de dados (ex: localStorage ou integração com backend/base de dados).

Melhorar a acessibilidade (WCAG).

Adicionar funcionalidades de comparação entre avaliações.

Permitir a personalização das práticas e níveis de maturidade.

Internacionalização para outros idiomas.

Substituir os alert() por modais customizados para uma melhor experiência do utilizador.