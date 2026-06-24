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

No tópico sobre VPN, aprendi sobre os benefícios de privacidade, anonimato e acesso remoto seguro a redes internas, além da diferença entre as tecnologias PPP, PPTP e IPsec. Essa foi inclusive a parte que mais me trouxe dificuldade no módulo.

Por fim, aprendi a diferença entre Switch e Router: o Router conecta meus dispositivos à rede externa, me permitindo acessar a internet, enquanto o Switch conecta meus dispositivos entre eles dentro da mesma rede local.

---

## O que foi mais difícil
Entender as diferenças entre as tecnologias de VPN (PPP, PPTP e IPsec) foi a parte mais desafiadora. Cada uma tem suas vantagens e desvantagens, e absorver isso exigiu mais atenção.

---

## Aplicação em Cybersecurity
Esse conhecimento é aplicável em segurança por me permitir entender conceitos fundamentais de defesa de rede, como Firewall e VPN. Isso me ajuda a visualizar formas eficientes de manter a segurança e privacidade de uma rede, além de entender como o Firewall pode ser importante para defesa dependendo do tipo de ataque recebido (como DDoS).

---

# How The Web Works - HTML, CSS, JS e Segurança Web

**Módulo:** Pre Security > How The Web Works  
**Status:** Em andamento

---

## O que é a sessão
A sessão aborda como uma página web é construída, cobrindo HTML, CSS e JavaScript, além de introduzir vulnerabilidades comuns relacionadas ao frontend de um site.

---

## O que aprendi

Aprendi bastante sobre como funciona o HTML de uma página e qual a diferença entre o uso do HTML (código responsável pela estrutura e exibição da página), o CSS (usado para estilização) e o JavaScript (usado para adicionar funcionalidades e interatividade à página).

Dentro do módulo, aprendi sobre Exposição de Dados Sensíveis (Sensitive Data Exposure) e sobre como é importante revisar o código HTML de um site para garantir que ele não exponha dados sensíveis, como credenciais de administradores ou de usuários deixadas acidentalmente em comentários no código.

Além disso, o tópico abordou o HTML Injection e como a sanitização de dados é fundamental para manter um site seguro. Tive um pouco de dificuldade para entender os riscos reais que isso representa, mas, estudando mais sobre o assunto, entendi que o HTML Injection pode facilmente evoluir para um XSS (Cross-Site Scripting), o que poderia levar o usuário final a um site de phishing ou resultar no roubo de cookies de sessão, sem que a vítima perceba.

---

## O que foi mais difícil
Entender a gravidade real dos riscos por trás do HTML Injection e como ele se conecta a um ataque mais amplo como o XSS.

---

## Aplicação em Cybersecurity
É importante ter esses conceitos em mente na área de cybersecurity para saber quais vulnerabilidades buscar na hora de uma análise de segurança, e saber exatamente o que corrigir em códigos HTML nesses casos. Seja removendo dados sensíveis expostos, seja implementando sanitização adequada de inputs do usuário.

---

# How The Web Works - Componentes e Infraestrutura

**Módulo:** Pre Security > How The Web Works  
**Status:** Finalizado.

---

## O que é a sessão
A sessão aborda os componentes que ajudam o funcionamento da web, como WAF, CDN, Databases, Load Balancers (e os algoritmos round-robin e weighted) e Health Check.

---

## O que aprendi

Aprendi bastante sobre como o WAF é útil para proteger contra ataques na camada de aplicação web, como XSS e SQL Injection (assuntos abordados também no módulo anterior). O WAF analisa o conteúdo da requisição HTTP, e não só IP/porta como um firewall tradicional.

Aprendi sobre como o Load Balancer é útil para garantir que um site se mantenha ativo mesmo com alto tráfego, e garante um certo "backup" caso um servidor caia. Ele atua distribuindo as requisições entre vários servidores, repartindo a carga e podendo usar algoritmos como round-robin (distribuição igual) ou weighted (distribuição baseada na capacidade/ocupação de cada servidor).

Além disso, aprendi sobre como o CDN serve para diminuir o tráfego de um site, hospedando conteúdo estático (como código JS, CSS, imagens e vídeos) em servidores espalhados pelo mundo, entregando o conteúdo a partir do servidor mais próximo do usuário. Isso é diferente de conteúdo dinâmico, como a página inicial de um blog, que muda com frequência e por isso não se beneficia da mesma forma do CDN.

---

## O que foi mais difícil
Entender como o CDN e o Load Balancer funcionam na prática foi um pouco desafiador. Mas, estudando mais a fundo, entendi que são conceitos importantes para garantir o funcionamento de um servidor mesmo diante de ataques comuns, como o DDoS.

---

## Aplicação em Cybersecurity
Isso tudo se aplica em cybersecurity de várias maneiras. O CDN é importante para diminuir o tráfego de sites e ajudar a mitigar ataques de sobrecarga de servidor, como o DDoS. O Load Balancer é fundamental para garantir que um site continue funcionando, já que distribui as requisições e evita sobrecarga em um único servidor. O WAF protege analisando o conteúdo da requisição HTTP em busca de ataques na camada de aplicação, enquanto o Health Check garante o bom funcionamento ao checar constantemente se cada servidor continua ativo e respondendo corretamente.
