# Network Fundamentals - TryHackMe

**Módulo:** Pre Security > Network Fundamentals  
**Status:** Em andamento

---

## O que é o módulo
O módulo fala sobre os fundamentos básicos da internet, protocolos e envio de dados entre dispositivos.

---

## O que aprendi

Aprendi que o TCP é a maneira mais eficiente e segura de se enviar arquivos para um requisitante quando se trata de informações sensíveis e/ou que não podem ser perdidas. O TCP envia os pacotes de forma separada e os reúne no ponto de chegada exibindo ao usuário a informação final. A diferença entre ele e o UDP é que o TCP checa se os arquivos foram recebidos corretamente e caso não tenham sido, reenvia-os. O UDP em contrapartida é mais rápido e é uma alternativa perfeita para casos em que o usuário não se importa com a perda de alguns pacotes pelo caminho já que o UDP não faz esse "double-check". Alguns exemplos são vídeos, chamadas de voz, jogos online. É menos seguro, mas mais veloz e perfeito pra ocasiões onde a velocidade é prioridade e a perda de alguns pacotes não prejudica o produto final.

Além disso, aprendi sobre a importância do Three-way Handshake no envio de pacotes via TCP e de como conceitos importantes como SYN e ACK funcionam na hora em que o usuário tenta fazer uma conexão em algum site. O Three-way Handshake é a primeira checagem pra ver se a conexão foi devidamente estabelecida entre ambas as partes.

O conhecimento sobre as portas acabou de ser iniciado mas já aprendi alguns conceitos básicos sobre como funciona o uso de algumas delas e sobre como algumas são utilizadas por padrão a depender do serviço (como a porta 80 para HTTP e 443 para HTTPS).

---

## O que foi mais difícil
Entender sobre os pacotes de dados e como eles funcionam exatamente nesse processo de envio e recebimento.

---

## Aplicação em Cybersecurity
Esse conhecimento é aplicável em segurança pelo entendimento que me deu sobre como funcionam as portas de acesso e o Three-way Handshake. Me dando uma visão mais ampla de como funcionam alguns tipos de ataques como DoS e DDoS, e como portas abertas como SSH podem ser alvos diretos de invasão.
