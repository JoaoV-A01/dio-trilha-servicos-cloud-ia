
# Análise de Sentimentos com Language Studio no Azure AI

## 📚 Descrição

Este projeto explora os recursos de **Análise de Sentimentos** utilizando o **Language Studio**, parte do conjunto de serviços de IA da Microsoft Azure. Através deste serviço, é possível analisar textos, detectar sentimentos, identificar frases-chave, reconhecer entidades e muito mais.

---

## 🚀 Funcionalidades Principais

### 🔍 **Language Studio**
- Detecta o idioma predominante.
- Realiza análise de sentimentos (positivo, neutro e negativo).
- Extrai frases-chave.
- Identifica entidades presentes no texto.

### ❓ **Resposta a Perguntas**
- Permite criar uma base de conhecimento com pares de perguntas e respostas.
- Facilita a criação de bots de FAQ e assistentes virtuais.

### 🤖 **Serviço de Bot**
- Interpreta e-mails, chamadas e conversas utilizando palavras-chave.
- Gera respostas coerentes e contextualizadas.
- Plataforma em nuvem para desenvolvimento e gerenciamento de bots.
- Integração com o Azure AI Language e outros serviços.
- ⚠️ **Observação:** Não substitui a interação humana em casos complexos, mas reduz significativamente o volume de atendimentos simples.

### 🗣️ **Compreensão da Linguagem Coloquial**
- O serviço compreende comandos divididos em:
  - **Declaração:** Ação solicitada (Ex.: "Acenda").
  - **Entidade:** Objeto ou assunto (Ex.: "a luz").
  - **Intenção:** Ação final (Ex.: "Ligar lâmpada").

### 🧠 **Reconhecimento e Síntese de Fala**
- Transforma fala em texto (speech-to-text).
- Gera fala a partir de texto (text-to-speech).
- Suporte para legendas em tempo real e offline.
- Possibilidade de personalizar vozes e entonações.

---

## ⚙️ **Configuração do Serviço de Fala no Language Studio**

1. **Criar Novo Recurso**
   - Acesse **Configurações** → **Criar Novo Recurso**.
   - Selecione uma **Assinatura**.
   - Defina um **Nome**, escolha uma **Região**, configure o **Plano de Preço** e selecione um **Grupo de Recursos**.

2. **Configurar Conversão de Fala**
   - Na tela inicial, vá em **Conversão de Fala e Texto** → **Conversão de Fala em Texto em Tempo Real**.
   - Escolha o idioma do áudio.
   - Visualize na área de resultados: detalhes do áudio e transcrição.

3. **Cenários Comuns**
   - Legendas automáticas (tempo real ou offline).
   - Criação de falas personalizadas.

4. **Considerações**
   - Verificação de custos.
   - Leitura das diretrizes de **Uso Responsável da IA** disponibilizadas pela Microsoft.

---

## 💡 **Configuração do Serviço de Análise de Sentimentos**

1. **Criar Recurso**
   - No portal Azure, selecione **IA + Machine Learning** → **Language Service**.
   - Configure:
     - **Assinatura**
     - **Grupo de Recursos**
     - **Nome da Instância**
   - Leia e aceite os termos de **Uso Responsável de IA**.

2. **Configurações Adicionais**
   - Configure **Rede**, **Identidade**, **Tags** e revise os dados antes de criar.

3. **Utilizar o Serviço**
   - Acesse o recurso criado no **Cognitive Services**.
   - Vá em **Classificação de Texto** → **Análise de Sentimentos e Opinião**.
   - Insira um texto (Ex.: comentários de hotel) para teste.
   - O serviço retorna:
     - Palavras-chave.
     - Percentuais de **positividade**, **neutralidade** e **negatividade**.

---

## 📝 **Observações Finais**
- O Language Studio oferece recursos avançados para processamento de linguagem natural (NLP).
- As ferramentas são altamente customizáveis e podem ser integradas a outros serviços da Azure.
- Importante avaliar os custos e aderir às práticas de **IA Responsável**, conforme sugerido pela Microsoft.

---

## 🔗 **Referências Oficiais**
- [Documentação do Language Studio](https://learn.microsoft.com/pt-br/azure/ai-services/language-service/)
- [Microsoft Azure Cognitive Services](https://azure.microsoft.com/pt-br/products/ai-services/cognitive-services/)
