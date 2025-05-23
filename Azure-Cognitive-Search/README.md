
# 🔍 Azure Cognitive Search - Utilizando AI Search para Indexação e Consulta de Dados

## 📚 Descrição

O **Azure Cognitive Search** é uma solução de **mineração de conhecimento** que permite encontrar **insights em escala** a partir de grandes volumes de dados não estruturados, como documentos, PDFs, imagens e notas manuscritas. Ele permite que organizações transformem seus arquivos em fontes pesquisáveis e inteligentes utilizando inteligência artificial.

---

## 🤖 O Que é Mineração de Conhecimento?

- Organizações acumulam grandes volumes de documentos ao longo do tempo.
- A busca manual e a preservação desses documentos se tornam desafios significativos.
- Dados geralmente estão "bloqueados" em formatos como PDFs, imagens e documentos.
- A **mineração de conhecimento** permite extrair insights desses dados não estruturados.

> 💡 O **Azure Cognitive Search** é a plataforma de mineração de conhecimento baseada em IA da Microsoft Azure.

---

## 🔥 Soluções de Pesquisa com Azure Cognitive Search

### 🔗 **Ingestão de Dados**
- **Azure Blob Storage Containers**
- **Azure Data Lake Storage Gen2**
- **Azure Table Stores**

### 💡 **Enriquecimento de IA e Indexação**
- Compreensão profunda dos dados usando IA.
- Aplicação de visão computacional, processamento de linguagem natural (NLP) e outros modelos.
- Geração de índices que tornam o conteúdo pesquisável.

### 🔍 **Exploração e Pesquisa**
- Pesquisa diretamente em índices através de aplicativos.
- Criação de visualizações e dashboards.
- Consultas baseadas em texto, filtros, localização e sentimentos.

---

## 🧠 Enriquecimento Cognitivo

O **enriquecimento de IA** torna os dados mais úteis e relevantes para pesquisa.

### ✅ Funcionalidades do Enriquecimento:
- Reconhecimento de entidades no texto (nomes, locais, organizações).
- Tradução de textos.
- Análise e avaliação de sentimentos.

### 🔄 Processo:
1. Um **conjunto de habilidades (skills)** processa e enriquece os documentos.
2. Os dados enriquecidos são utilizados na criação dos índices.
3. Estes índices são consumidos pela ferramenta de busca para consultas rápidas e precisas.

---

## 🧪 Laboratório - Exemplo Prático

### 🔧 **Situação-Problema**
Uma rede nacional de café no Brasil está recebendo diversas reclamações. É necessário identificar:
- **De onde** estão vindo essas reclamações.
- **Quais tipos** de problemas estão sendo reportados.

---

## 🏗️ **Solução Passo a Passo**

### 1️⃣ **Criar o Serviço de AI Search**
- Acesse o portal do Azure.
- Crie um **Search Service**.
- Informe:
  - **Resource Group** (grupo de recursos).
  - **Nome da Instância**.
  - **Pricing Tier:** **Basic** (ou outro conforme necessidade).
- Configure se necessário:
  - **Scale**, **Networking**, **Tags**.
- Revise e conclua a criação.

### 2️⃣ **Criar o Serviço Azure AI Language**
- Crie um recurso de **AI Service** como feito no laboratório anterior:
  - 👉 [Link do exemplo anterior](https://github.com/JoaoV-A01/dio-trilha-ia/tree/main/Analise-Sentimentos)

### 3️⃣ **Criar um Storage Account**
- Defina:
  - **Subscription**.
  - **Resource Group**.
  - **Nome**.
  - **Região**.
  - **Performance:** **Standard**.
  - **Redundância:** **Locally-Redundant Storage (LRS)**.
- Opções adicionais nas abas:
  - **Avançado**, **Networking**, **Data Protection**, **Encryption** e **Tags**.
- Revise e conclua.

### 4️⃣ **Configurar Segurança no Storage**
- No storage criado, altere as configurações para **permitir acessos anônimos de BLOB**.

### 5️⃣ **Adicionar Container de Dados**
- Acesse **Data Storage → Containers**.
- Crie um novo container:
  - Defina um **nome**.
  - Defina o nível de acesso: **Container (anonymous read access for containers and blobs)**.

### 6️⃣ **Alimentar o Container**
- Faça o upload de arquivos contendo **reviews de clientes**, preferencialmente variados (localizações, tipos de feedback, etc.).

### 7️⃣ **Conectar Storage ao AI Search**
- No serviço de **AI Search**, selecione o **Storage Account** com os dados.
- Preencha os dados necessários para estabelecer a conexão.

### 8️⃣ **Realizar Pesquisas**
- Exemplos de consultas:

#### 🔎 Por Localização:
```plaintext
search=location:'Chicago'
```
→ Retorna todos os comentários da região de **Chicago**.

#### 🔎 Por Sentimento:
```plaintext
search=sentiment:'negative'
```
→ Retorna todos os comentários com **sentimento negativo**.

---

## 🔗 Referências
- [Documentação do Azure Cognitive Search](https://learn.microsoft.com/pt-br/azure/search/)
- [Azure AI Search](https://azure.microsoft.com/pt-br/products/ai-services/search/)
- [Exemplo no GitHub](https://github.com/JoaoV-A01/dio-trilha-ia/tree/main/Analise-Sentimentos)
