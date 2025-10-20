🌐 Projeto IoT – Monitoramento com Arduino UNO

👥 Integrantes

Bernardo Moreira, rm: 564103;

Bruna Sadi, rm: 561870;

Francisco Nogueira: 566309;

Rhariel, rm:566310;

Sara Maragon, rm:563807.

🧠 Descrição do Projeto

Este projeto apresenta uma Prova de Conceito (PoC) de um sistema IoT utilizando Arduino UNO, com um sensor DHT11 e dois botões físicos.
Os dados coletados (temperatura e umidade) são enviados a um servidor web, que os armazena e exibe em um site interativo.

Os botões permitem simular interações do usuário, como seleção de modos de operação ou envio manual de dados.

⚙️ Detalhes da Implementação
🔌 Hardware Utilizado

Arduino UNO (microcontrolador principal)

Sensor DHT11 – leitura de temperatura e umidade

Dois botões (push buttons) – interação manual

Cabo USB – alimentação e comunicação serial com o computador

🧩 Software e Integração

Código Arduino: escrito em C++ usando a IDE Arduino

Biblioteca utilizada:

DHT.h para leitura do sensor DHT11

Comunicação IoT:

Envio de dados via Serial

Backend (servidor): Node.js + Express

🔬 Resultados da PoC

Leitura precisa de temperatura e umidade pelo DHT11

Envio bem-sucedido dos dados para o servidor web

Exibição em tempo real dos valores no site

Funcionamento dos dois botões para controle local das ações do sistema

🖼️ Prints de Integração IoT com o Site
<img width="1190" height="577" alt="image" src="https://github.com/user-attachments/assets/190f9960-30b1-4f22-b8a0-5d2e330506b4" />
<img width="834" height="476" alt="image" src="https://github.com/user-attachments/assets/afc99e8e-a332-40a2-953d-1de77df06bfc" />

