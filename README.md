# Sistema de Agentes IA para Análise de Tendência de Preço de Criptomoedas

Este projeto implementa um sistema de agentes de inteligência artificial (IA) para gerar relatórios de análise de tendência de preço de criptomoedas, focado especificamente no par BTC/USD na plataforma Bybit. O sistema utiliza o framework ADK de agentes do Google e o modelo Gemini para automatizar o processo de pesquisa, planejamento, redação e revisão desses relatórios.

## Funcionalidades

O sistema é composto por quatro agentes principais:

1.  **Agente Buscador de Notícias:**
    * Responsável por pesquisar as últimas notícias e lançamentos relevantes sobre o tópico especificado (ex: BTC/USD na Bybit).
    * Utiliza a ferramenta de busca do Google (google\_search) para coletar informações.
    * Foca em identificar os lançamentos e eventos mais relevantes e com maior repercussão.

2.  **Agente Planejador de Relatório:**
    * Analisa as notícias e lançamentos encontrados pelo Agente Buscador.
    * Cria um plano detalhado do relatório, definindo a estrutura, os pontos chave a serem abordados e as pesquisas adicionais necessárias.
    * Identifica os fatores mais importantes que influenciam a tendência de preço do ativo.

3.  **Agente Redator do Relatório:**
    * Escreve um rascunho do relatório de tendência de preço com base no plano fornecido pelo Agente Planejador.
    * Adota a perspectiva de um trader especializado em criptomoedas, considerando possíveis operações de trade (compra ou venda) na Bybit.
    * Busca fornecer um relatório objetivo, claro e informativo, com sugestões de posicionamento.

4.  **Agente Revisor de Qualidade:**
    * Revisa o rascunho do relatório gerado pelo Agente Redator.
    * Verifica a clareza, concisão, correção e tom do texto.
    * Fornece feedback e sugestões de melhorias, ou confirma que o rascunho está pronto para publicação.

## Tecnologias Utilizadas

* **Google Gemini:** Modelo de linguagem grande utilizado pelos agentes para geração de texto e análise de informações.
* **Google ADK (Agent Development Kit):** Framework para desenvolvimento e execução de agentes de IA.
* **google-genai Python SDK:** Biblioteca para interagir com os modelos Gemini.
* **Ferramenta de Busca do Google (google\_search):** Utilizada pelos agentes para pesquisar informações na web.
* **Python:** Linguagem de programação principal.
* **Bibliotecas Python:**
    * `os`
    * `google.colab.userdata`
    * `google.genai`
    * `google.adk.agents`
    * `google.adk.runners`
    * `google.adk.sessions`
    * `google.adk.tools`
    * `google.genai.types`
    * `datetime`
    * `textwrap`
    * `IPython.display`
    * `requests`
    * `warnings`

## Configuração

1.  **Instalação de Dependências:**
    ```bash
    !pip install -q google-genai google-adk
    ```

2.  **Configuração da API Key do Google Gemini:**
    * Você precisa obter uma API Key do Google Gemini e configurá-la como uma variável de ambiente.
    * O código utiliza `google.colab.userdata` para acessar a API Key de forma segura no Google Colab.

3.  **Configuração do Cliente Gemini:**
    * O código inicializa o cliente da SDK do Gemini e define o modelo a ser utilizado.

## Como Usar

1.  Execute as células do notebook para instalar as dependências e configurar o ambiente.
2.  Quando solicitado, insira o tópico sobre o qual você deseja gerar o relatório (por exemplo, "BTC/USD na Bybit nas últimas 24 horas").
3.  O sistema de agentes irá gerar o relatório em etapas, exibindo a saída de cada agente.

## Exemplo de Uso

O notebook inclui um exemplo de execução do sistema para o tópico "BTC/USD na Bybit nas últimas 48 horas". A saída demonstra o fluxo de trabalho dos agentes, desde a busca de notícias até a geração do relatório final revisado.

## Contribuição

Contribuições para este projeto são bem-vindas! Se você tiver alguma sugestão de melhoria ou encontrar algum problema, sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença

[Inserir a licença do projeto]
