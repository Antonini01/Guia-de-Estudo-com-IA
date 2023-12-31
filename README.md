# **Guia de Estudo Interativo com IA**

## **Visão Geral**

Este projeto é um aplicativo interativo de estudo desenvolvido em Python, utilizando **Streamlit** para a interface do usuário e **LangChain** para a integração com o modelo `Llama-2-7B` de linguagem de grande escala (LLM). Ele oferece uma experiência personalizada de aprendizado, permitindo aos usuários explorar diferentes matérias, fazer perguntas e receber respostas geradas por IA, além de testar seus conhecimentos através de um sistema de perguntas e respostas.

## **Funcionalidades**

-   **Seleção de Matéria**: Os usuários podem escolher entre várias matérias, como Matemática, Química, Física e Gramática.
-   **Geração de Respostas com IA**: Utilizando o modelo `Llama-2-7B` da LangChain, disponível no repositório [Hugging Face](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML), o aplicativo gera respostas para perguntas específicas dos usuários e também escreve redações com temas personalizados.
-   **Análise Sintática**: Para a matéria de Gramática, o aplicativo oferece uma análise sintática de textos usando spaCy.
-   **Visualização de Desempenho**: Um gráfico de desempenho é gerado usando matplotlib, permitindo aos usuários visualizar seu progresso nas diferentes matérias.
-   **Sistema de Perguntas e Respostas**: Um jogo interativo de perguntas e respostas para testar o conhecimento do usuário, com feedback instantâneo e uma barra de progresso.

## **Tecnologias Utilizadas**

-   **Python**: Linguagem de programação principal.
-   **Streamlit**: Para criar a interface do usuário web.
-   **LangChain**: Para integração com modelos de linguagem de grande escala, especificamente o `Llama-2-7B`.
-   **spaCy**: Para processamento de linguagem natural, especificamente para análise sintática em português.
-   **matplotlib**: Para a criação de gráficos de desempenho.

## **Configuração e execução**
Para configurar e executar este projeto localmente, siga estas etapas:

**Configuração do Modelo LLM**

Este projeto utiliza o modelo `Llama-2-7B` do Hugging Face. Para configurar o modelo no seu ambiente local, siga estas etapas:

1. Visite a página do modelo [Llama-2-7B no Hugging Face](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML).
2. Baixe o modelo para o seu sistema no formato bin.
3. Coloque-o no diretório principal do projeto (o mesmo diretório onde o `main.py` está localizado).
4. Certifique-se de que o caminho para o modelo está correto no código do projeto em `main.py`.

**Executando o Projeto**

Certifique-se de ter todas as dependências necessárias instaladas. Você pode instalá-las usando:
```bash
pip install -r requirements.txt
```
Em seguida, instale o modelo de linguagem português para o spaCy:
```bash
python -m spacy download pt_core_news_lg
```
Após configurar o modelo, você pode executar o projeto com o seguinte comando:

```bash
streamlit run main.py
```

## **Créditos**

Este projeto foi desenvolvido por Antonini Chiquetto como parte de um processo seletivo para estágio e iniciação científica na área de AI/ML com foco em LLM, utilizando o modelo `Llama-2-7B` do repositório do Hugging Face.



## **Referências**
Para consultar as referências utilizadas nesse projeto, consulte o arquivo `Referencias.pdf` incluído neste repositório.

## **Licença**

Este projeto está sob a [Licença MIT](https://github.com/git/git-scm.com/blob/main/MIT-LICENSE.txt). Veja o arquivo `LICENSE` para mais detalhes.
