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

# Network Fundamentals - TryHackMe (Parte 2)

**Módulo:** Pre Security > Network Fundamentals  
**Status:** Finalizado

---

## O que é a sessão
A sessão fala sobre Port Forwarding, Firewalls, VPN, Router e Switch, abordando como cada um opera e quais benefícios oferece.

---

## O que aprendi

Aprendi sobre Port Forwarding e como ele serve pra configurar dispositivos pessoais a receber informações externas, permitindo que serviços dentro de uma rede privada sejam acessados pela internet.

Aprendi também sobre Firewalls e a diferença entre Stateless e Stateful. O Stateless usa um conjunto de regras fixas e analisa pacote por pacote, sem guardar informação sobre a conexão. O Stateful analisa o comportamento da conexão inteira, sendo dinâmico nas suas decisões. Por consumir menos recursos, o Stateless é uma opção mais resistente contra ataques DDoS, já que não precisa rastrear o estado de milhares de conexões simultâneas.

No tópico sobre VPN, aprendi sobre os benefícios de privacidade, anonimato e acesso remoto seguro a redes internas, além da diferença entre as tecnologias PPP, PPTP e IPsec — essa foi inclusive a parte que mais me trouxe dificuldade no módulo.

Por fim, aprendi a diferença entre Switch e Router: o Router conecta meus dispositivos à rede externa, me permitindo acessar a internet, enquanto o Switch conecta meus dispositivos entre eles dentro da mesma rede local.

---

## O que foi mais difícil
Entender as diferenças entre as tecnologias de VPN (PPP, PPTP e IPsec) foi a parte mais desafiadora. Cada uma tem suas vantagens e desvantagens, e absorver isso exigiu mais atenção.

---

## Aplicação em Cybersecurity
Esse conhecimento é aplicável em segurança por me permitir entender conceitos fundamentais de defesa de rede, como Firewall e VPN. Isso me ajuda a visualizar formas eficientes de manter a segurança e privacidade de uma rede, além de entender como o Firewall pode ser importante para defesa dependendo do tipo de ataque recebido (como DDoS).
