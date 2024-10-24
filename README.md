# Assistente de Delivery com AWS Step Functions e Amazon Bedrock

[Sobre](#sobre) • [Descrição do Projeto](#descrição-do-projeto) [ que aprendi](#o-que-aprendi) • [Exemplo de Fluxo](#exemplo-de-fluxo) •  [Tecnologias Utilizadas](#tecnologias-utilizadas) • [Referências](#referências) •  [Contato](#contato) 

## Sobre

Este projeto foi desenvolvido como parte de um desafio prático do **Bootcamp:  Nexa - Engenharia de Prompts na AWS com Claude 3**, da <a href="https://www.dio.me/sign-up?ref=2772EA2C589E462BB0C382518E0ACBA2" targer="-Blank">**DIO - Digital Innovation One**</a> em parceria com **Nexa** e **AWS**.


## Descrição do Projeto

O objetivo foi orquestrar diferentes serviços da AWS para automatizar e gerenciar um fluxo de pedidos de delivery, desde a recepção do pedido até a entrega final, proporcionando uma experiência otimizada e personalizada para o cliente.


## O que aprendi

Durante o desenvolvimento deste projeto, aprendi a:

- **Utilizar o AWS Step Functions**: Aprendi a orquestrar diferentes serviços da AWS de maneira eficiente, integrando fluxos de trabalho e automatizando processos complexos. O **Step Functions** foi utilizado para gerenciar o ciclo de um pedido de delivery.
  
- **Trabalhar com Amazon Bedrock**: O Bedrock foi uma ferramenta essencial para personalizar a experiência do cliente. Foi utilizado o **Haiku**, um modelo do Bedrock, para executar o encadeamento de prompts de IA, aprimorando a recomendação de itens de acordo com o contexto de um jantar romântico. Isso incluiu sugestões de alimentos, bebidas e até locais para complementar a experiência.

- **Modelo ASL (Amazon States Language)**: Entendi a importância do formato JSON no Step Functions, utilizado para definir os estados e suas transições no fluxo de trabalho. Foi criado prompts para guiar o assistente virtual em tempo real, como pedir sugestões de comidas, bebidas e até de um local ideal para um jantar romântico em Paris.

- **Execução de Prompts de IA**: Aprendi a implementar prompts personalizados para fornecer recomendações inteligentes durante a experiência de entrega. Por exemplo:
  - Sugestões de alimentos que complementam um jantar com macarrão.
  - Recomendações de bebidas para acompanhar a refeição.
  - Indicação de um lugar romântico em Paris para um jantar especial.


## Exemplo de Fluxo

1. **Primeiro prompt (Comida)**: 
   - "Estou programando um jantar romântico e vou pedir macarrão. Me dê uma lista de três itens que combinam com essa experiência gastronômica."
   
   **Saída**:
   ```json
   {
       "result-one.$": "$.Body.content[0].text"
   }
   ```

2. **Segundo prompt (Bebidas)**:
   - "Liste duas bebidas que acompanham um jantar romântico."

3. **Terceiro prompt (Local em Paris)**:
   - "Liste um lugar perfeito para um jantar romântico em Paris."

4. **Parâmetros Adicionados**:
   ```json
   {
       "prompt-one": "ideia de comidas",
       "prompt-two": "ideia de bebidas",
       "prompt-three": "ideia de local"
   }
   ```

## Tecnologias Utilizadas

- **AWS Step Functions**: Para orquestrar o fluxo de trabalho do assistente de delivery.
- **Amazon Bedrock**: Para personalização e sugestões de IA.


## Referências

- [AWS Step Functions](https://aws.amazon.com/pt/step-functions/)
- [Exemplos de AWS Step Functions](https://github.com/aws-samples/aws-stepfunctions-examples)
- [Serverless e Amazon Bedrock](https://aws.amazon.com/pt/blogs/aws-brasil/como-criar-um-assistente-virtual-de-baixa-latencia-com-multiplos-modelos-usando-serverless-e-amazon-bedrock/)


## Contato

👩‍💻 Patrícia Freitas

📬 brpatyfreitas@gmail.com

 <div><a href="https://www.linkedin.com/in/patyfreitasbr"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></>
  <a href="https://www.instagram.com/patyfreitasbr"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></></div>

</br>




