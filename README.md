# DIO Bootcamp - Nexa Engenharia de Prompts
Desafio Bootcamp DIO - Nexa Engenharia de Prompts -> AWS - Step Functions

 
## 🤔 O que é?

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
Orquestrador de execução de Serviços da AWS (200+ Serviços).

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Ferramenta Low Code para criar Workflows (Maquinas de Estado) de execução de Serviços da AWS.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
<img width="300" alt="image" src="https://github.com/user-attachments/assets/237064d4-856e-41b1-abff-ac27aeaa961b">


## 👷‍♂️ Construção

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
Para a criação/interligação dos Steps (passos) dos Workflows/Fluxo (maquinas de estado), disponibiliza:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
1 - **Ações**:   Serviços da AWS e respectivas ações pré-definidas destes serviços;

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
2 - **Fluxos**:  Steps de apoio no direcionamento do fluxo, como por exemplo: 
                   - *Choice* - decisão (lógica if/then/else);
                   - *Parallel* - execução em paralelo; 
                   - *Map* - loop de execução;
                   - *Wait* - aguarda determinado tempo (configurável) para execução do próximo step;
                   - *Success* - para o fluxo e indica "Sucesso" na execução;
                   - *Fail* - para o fluxo e indica "Falha" na execução;

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
3 - **Padrões**: Sub-fluxos pré-definidos, usados com frequencia. Exemplos:
                   - *Process S3 objects* - Usa o Maquina de Estado com o AWS Lambda para processar objetos num bucket S3;
                   - *Process JSON file in S3* - Usa o Maquina de Estado com o AWS Lambda para processar dados de um arquivo JSON no S3;
                   - *Process CSV file in S3* - Usa o Maquina de Estado com o AWS Lambda para processar dados de um arquivo CSV no S3;

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
<img width="317" alt="image" src="https://github.com/user-attachments/assets/0cf351e9-210b-4ff0-b8d6-61e3e666cdc7"> &nbsp; <img width="286" alt="image" src="https://github.com/user-attachments/assets/40001278-6be4-4a56-9c9b-f34a4be8f2db"> &nbsp; <img width="290" alt="image" src="https://github.com/user-attachments/assets/51954454-684c-4527-902a-2083c0ba9306">



## ⚙️ Configurações / Informações Adicionais

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
1 - Você não paga pela utilização do Step Functions, mas é **muito importante** lembrar que *estará utilizando* **Serviços Pagos** então verifique os custos;

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
2 - Como o Steps Functions, utiliza Serviços da AWS, **o acesso** a estes Serviços devem ser Configurados;

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
3 - Determinados Serviços necessitam de Configurações Adicionais. 
    Exemplo: AWS Bedrock, necessita da configuração da LLM que será utilizada, então além de você garantir (configurar) a utilização da LLM em sua Região, deverá configurar o Step do Bedrock, informando a utilização da LLM;
    

## ▶️ Execução / 📝 Log de Execução

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
Ao executar a Maquina de Estado, você terá a visão da execução de 2 maneiras:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
1 - **State View**: Log de Execução por Step/Task - você terá o Status e Tempo de Execução e conseguirá detalhar as informações de Entrada e Saída;

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img width="618" alt="image" src="https://github.com/user-attachments/assets/db52af7d-d362-4b86-8176-4d7b1240c738">

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
2 - **Event View**: Log de Execução por Ações dentro de cada Task;


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img width="618" alt="image" src="https://github.com/user-attachments/assets/e9472116-31a5-4223-85c1-c92f429f9d8b">





