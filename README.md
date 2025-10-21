🌐 Projeto IoT – Monitoramento com Arduino UNO
👥 Integrantes

Bernardo Moreira, RM: 564103

Bruna Sadi, RM: 561870

Francisco Nogueira, RM: 566309

Rhariel, RM: 566310

Sara Maragon, RM: 563807

🧠 Descrição do Projeto

Este projeto é uma Prova de Conceito (PoC) de um sistema IoT (Internet das Coisas) utilizando o Arduino UNO com um sensor DHT11 para monitoramento de temperatura e umidade. O sistema também utiliza dois botões físicos para interação manual.

Os dados coletados, como:

Temperatura e Umidade (sensor DHT11)

Tempo de posse de bola e Distância percorrida (simulados pelos botões)

São enviados a um servidor Node-RED, onde são processados e exibidos em tempo real em uma interface interativa. O uso do Node-RED permite a criação visual de fluxos para o processamento dos dados, facilitando a integração e exibição dos resultados.

⚙️ Detalhes da Implementação
🔌 Hardware Utilizado

Arduino UNO: Microcontrolador principal

Sensor DHT11: Para medir temperatura e umidade

Dois Botões Push (Botões Físicos): Para interações manuais

Cabo USB: Para alimentação e comunicação com o computador

🧩 Software e Integração

Código Arduino: Programado em C++ usando a IDE Arduino

Bibliotecas Utilizadas:

DHT.h: Para leitura do sensor DHT11

Comunicação IoT:

Envio de dados via Serial para comunicação com o Node-RED

Backend:

Node-RED: Para processar, armazenar e exibir os dados em tempo real

🔗 Fluxo de Dados

O Arduino UNO coleta os dados de temperatura e umidade do sensor DHT11.

O Arduino também coleta informações simuladas pelos botões, como tempo de posse e distância percorrida.

O Arduino envia os dados para o Node-RED via Serial (ou através de MQTT, caso seja configurado).

O Node-RED processa esses dados e os exibe em um dashboard interativo em tempo real.

O Node-RED pode também realizar outras tarefas, como enviar alertas ou controlar outros dispositivos IoT.

🔬 Resultados da PoC

Leitura precisa de temperatura e umidade com o sensor DHT11.

Envio bem-sucedido dos dados para o Node-RED.

Exibição em tempo real dos valores no Node-RED Dashboard.

Funcionamento dos botões para interação manual com o sistema.

Interface interativa criada no Node-RED para visualização dos dados.

🖼️ Prints de Integração IoT com o Site
<img width="1190" height="577" alt="image" src="https://github.com/user-attachments/assets/190f9960-30b1-4f22-b8a0-5d2e330506b4" />
<img width="834" height="476" alt="image" src="https://github.com/user-attachments/assets/afc99e8e-a332-40a2-953d-1de77df06bfc" />

📋 Instruções de Execução
🛠️ Pré-requisitos

Arduino IDE para carregar o código no Arduino UNO

Node-RED instalado e em execução no seu sistema

Biblioteca DHT.h instalada na IDE Arduino

MQTT Broker (se você for utilizar MQTT para a comunicação entre Arduino e Node-RED)

🔄 Passos para Execução

Carregar o código no Arduino:

Abra o código na IDE Arduino.

Selecione a porta COM correta.

Faça o upload para o Arduino UNO.

Configurar o Node-RED:

Instale o Node-RED se ainda não o fez. (Siga a documentação oficial
).

Inicie o Node-RED com node-red-start.

Abra o painel de administração do Node-RED em http://localhost:1880.

Criar o fluxo no Node-RED:

No Node-RED, crie um fluxo para receber os dados do Arduino (usando a entrada serial ou MQTT).

Adicione um nó para exibir os dados em tempo real no Node-RED Dashboard.

Conecte os nós para garantir que os dados de temperatura, umidade e informações dos botões sejam exibidos corretamente.

Visualizar os Dados:

Abra o painel de Dashboard do Node-RED.

Os dados de temperatura, umidade, tempo de posse e distância percorrida serão exibidos em tempo real na interface.
