# Relatório - Desafio Módulo 3 – Processamento de Dados Simplificado com Power BI

## Introdução

Neste relatório, descreverei as etapas e diretrizes que segui para lidar com o desafio proposto neste módulo. O desafio envolveu a criação de uma instância na Azure para MySQL, a importação de um banco de dados disponível no GitHub e a integração do Power BI com o MySQL na Azure. Além disso, realizei a verificação de problemas na base de dados e a transformação dos dados conforme as diretrizes fornecidas.

## Diretrizes para Transformação dos Dados

### 1. Verificação dos Cabeçalhos e Tipos de Dados

Iniciei verificando os nomes das colunas e os tipos de dados em cada uma delas para garantir a consistência e compreensão dos dados.

### 2. Modificação dos Valores Monetários para o Tipo Double Preciso

Realizei a modificação dos valores monetários para o tipo de dado "double preciso" a fim de garantir a precisão das informações financeiras.

### 3. Verificação da Existência de Nulos e Análise da Remoção

Identifiquei e analisei os valores nulos na base de dados, decidindo se deveriam ser mantidos ou removidos com base na relevância dos registros.

### 4. Identificação de Colaboradores sem Gerente

Identifiquei colaboradores com valores nulos na coluna "Super_ssn" como possíveis gerentes e verifiquei se algum colaborador não tinha um gerente associado.

### 5. Verificação de Departamentos sem Gerente

Verifiquei se havia departamentos sem gerentes e, caso encontrasse algum, preenchi essas lacunas com os dados disponíveis.

### 6. Separação de Colunas Complexas

Realizei a separação das colunas complexas para facilitar a manipulação dos dados e garantir a consistência.

### 7. Mescla de Consultas Employee e Department

Mesclei as consultas de "employee" e "department" para criar uma tabela que associava o nome dos departamentos aos colaboradores. Essa mescla foi feita com base na tabela "employee".

### 8. Eliminação de Colunas Desnecessárias

Removi as colunas que não eram relevantes para o relatório final, mantendo apenas as informações essenciais.

### 9. Junção de Colaboradores e Respectivos Nomes de Gerentes

Realizei a junção dos colaboradores com os respectivos nomes dos gerentes, seja por meio de consulta SQL ou pela mescla de tabelas no Power BI.

### 10. Mescla de Colunas de Nome e Sobrenome

Realizei a mescla das colunas de nome e sobrenome para criar uma única coluna que continha os nomes completos dos colaboradores.

### 11. Mescla de Nomes de Departamentos e Localizações

Mesclei os nomes de departamentos e localizações para criar combinações únicas, o que facilitaria a criação de um modelo estrela em módulos futuros.

### 12. Agrupamento de Dados por Gerente

Agrupei os dados para determinar quantos colaboradores estavam associados a cada gerente.

### 13. Eliminação de Colunas Desnecessárias

Finalizei eliminando todas as colunas que não seriam utilizadas no relatório final, mantendo-o limpo e conciso.

## Por que Usar Mesclar em Vez de Atribuir?

A escolha de usar a operação de mesclar em vez de atribuir se deve na necessidade de criar conexões significativas entre os dados. A mesclagem permite a combinação inteligente de tabelas com base em colunas comuns, criando uma nova tabela que integra as informações relevantes de maneira coerente. Contudo, a atribuição simplesmente empilharia as tabelas umas sobre as outras, resultando em uma sobreposição de dados sem lógica. Para o sucesso deste projeto, é crucial estabelecer relações eficazes e não simplesmente empilhar informações de forma desorganizada.

## Conclusão

Em resumo, este desafio envolveu a integração de dados, análise e transformação para preparar a base de dados para relatórios futuros. As etapas descritas acima foram essenciais para garantir a qualidade e a utilidade dos dados no Power BI.

Este relatório resume o processo que segui no desafio do Módulo 3 e serve como documentação das etapas realizadas. Agradeço novamente à nossa professora pelo seu ensinamento e orientação durante este curso.
