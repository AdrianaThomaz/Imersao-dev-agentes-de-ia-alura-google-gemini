🤲🏼❤️ 🚀  🥊 🥊  🙏🏼       # Imersao-dev-agentes-de-ia-alura-google-gemini    🙏🏼  🥊 🥊  🚀 ❤️🤲🏼


Demonstração do conhecimento adquirido na Alura,na imersão agentes de IA com Google Gemini 
Com os mestres da tecnologia Carol Carneiro, Vinicius Carida e Fabrício Carraro!



Desenvolvi um assistente superinteligente, um sistema de Recuperação de Aumento de Geração (RAG) em Python, focado em atuar como um assistente de políticas internas para RH e TI. 


Um sistema RAG (Retrieval-Augmented Generation) é como um assistente inteligente. Ele não se baseia apenas em um conhecimento pré-existente (como faria uma IA tradicional), mas consegue ir buscar e ler informações em documentos, para depois gerar respostas com base no que aprendeu.

Neste caso, o assistente funciona assim:

Fonte de informações: Na aula prática foi nos fornecido PDFs com todas as políticas internas de RH e TI.

Preparação: O sistema usa um programa chamado PyMuPDFLoader para abrir e ler esses PDFs. Depois, ele usa o RecursiveCharacterTextSplitter para dividir o conteúdo desses documentos em pequenos pedaços. Isso é feito para facilitar a busca e a leitura de informações relevantes.

Orquestração: O LangChain atua como o maestro do processo. Ele gerencia o fluxo de trabalho, garantindo que tudo funcione na ordem certa: primeiro, ele lê os PDFs, depois divide o conteúdo em pedaços e, por fim, quando alguém faz uma pergunta, ele busca a resposta nesses pedaços e a formula de uma forma compreensível.

sistema RAG funciona como um bibliotecário super-rápido: ele lê todos os documentos de políticas, memoriza onde está cada pedacinho de informação e, quando você faz uma pergunta, ele encontra a resposta exata e a explica de forma clara.

Então para que esse assistente superinteligente consiga entender e responder suas perguntas, ele precisa de algumas "ferramentas".

Preparação do Conhecimento
O assistente pega toda a informação (seus documentos) e a transforma em um código secreto. Esse código é chamado de embeddings. É como se cada pedaço de informação virasse um número, e o assistente usa a inteligência da Google (a mesma do Gemini) para criar esses números.

Organização e Busca
Esses códigos (os números) são guardados em uma espécie de "super-agenda" chamada FAISS. Essa agenda é incrivelmente rápida para encontrar informações parecidas.

Quando você faz uma pergunta, o assistente transforma a sua pergunta em um código também. Ele, então, vai na "super-agenda" e encontra os códigos que mais se parecem com o da sua pergunta.

A Resposta
Com os trechos de informação que mais se parecem com a sua pergunta, o assistente monta a resposta. Ele não inventa nada, ele usa a informação que ele encontrou, dando o crédito (a citação) de onde ele tirou aquela informação.


Eu utilizei o Google Colab, Alun para baixar os PDF's, plataforma da Alura e o GitHub.

❤️ 🚀  🥊 🥊 No Google Colab:❤️ 🚀  🥊 🥊 

Dependências e Ferramentas Técnicas

langchain_community: Componentes da LangChain para trabalhar com diferentes tipos de documentos e integrações.

langchain-text-splitters: Utilizado para dividir os documentos em pedaços (chunks) de tamanho gerenciável, usando RecursiveCharacterTextSplitter para preservar o contexto.

pymupdf: Carrega e extrai o texto de arquivos PDF, permitindo que o sistema leia os documentos de políticas internas.

faiss-cpu: Um banco de dados vetorial de alta performance, utilizado para armazenar os embeddings dos documentos e realizar a busca por similaridade de forma eficiente.

langchain-google-genai: Integração com a API do Google, especificamente para gerar embeddings (GoogleGenerativeAIEmbeddings) que representam o significado do texto. O modelo gemini-embedding-001 é usado para essa tarefa.

langchain_core: Fornece os componentes básicos como ChatPromptTemplate para criar prompts de forma estruturada.

langchain.chains: Onde a lógica da cadeia de documentos (create_stuff_documents_chain) é definida, ligando a pergunta do usuário, o contexto recuperado e o modelo de linguagem para gerar a resposta final.

RegEx (re) e pathlib: Bibliotecas nativas do Python para manipulação de strings e caminhos de arquivos, usadas na função de formatação para extrair trechos de texto e citar as fontes.

 Este projeto foi uma imersão valiosa nos conceitos de LLMs, engenharia de prompts e arquiteturas de RAG.

❤️ 🚀  🥊 🥊 Agradecimentos aos mestres Carol Carneiro, Vinicius Carida e Fabricio Carraro por compartilharem seu conhecimento.❤️ 🚀  🥊 🥊 


🙏🏼  🥊  🥊 🚀 ❤️🤲🏼❤️ 🚀  🥊 🥊 🤲🏼🙏🏼  🥊  🥊 🚀 ❤️🤲🏼❤️ 🚀  🥊 🥊 🤲🏼🙏🏼  🥊  🥊 🚀 ❤️🤲🏼❤️ 🚀  🥊 🥊 🤲🏼🙏🏼  🥊  🥊 🚀 ❤️🤲🏼❤️ 🚀  🥊 🥊 🤲🏼
