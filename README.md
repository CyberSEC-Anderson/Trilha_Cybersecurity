_Autor: Anderson Silva Lima (www.linkedin.com/in/ls-anderson)_

# INTRODUÇÃO - RESUMO

Security Operation Center (SOC) é o nome dado ao time de segurança da informação responsável por monitorar o ambiente organizacional. Sua finalidade é detectar, analizar e responder aos incidentes de cibersegurança com o apoio de tecnologias, pessoas e processos.

Existem diferentes modelos de SOC que uma empresa pode adotar dependendo de seus requisitos e orçamento disponível.

Alguns deles são:

* In-house SOC
  * A empresa dispõe do seu próprio time de cybersecurity que terá a função de SOC, neste caso o orçamento é um ponto de atenção para a empresa.
  
* Virtual SOC
  * O time de cybersecurity não possui um ambiente próprio de trabalho, sendo assim, trabalham remotamente em diferentes localidades.
  
* Co-managed SOC
  * Consiste em um SOC interno trabalhando em conjunto com um Managed Security Service Privider (MSSP) externo à organização, neste modelo a coordenação das equipes internas e externas é muito importante.

* Command SOC
  * Neste modelo, um grupo de analistas seniores supervisionam SOC's menores numa grande região, modelo utilizado principalmente em Provedores de Telecomunicação e Agências de Defesa.


Para possuir um SOC de sucesso é necessário que haja uma forte relação entre pessoas, processos e tecnologia:

* **_Pessoas_**

Os analistas que fazem parte do SOC precisam ser treinados e familiarizados com diferentes tipos de alertas e cenários de ataque, além de serem totalmente adaptáveis as ameaças que surgem diariamente e dispostos a demandar algum tempo realizando pesquisas eficazes.

* **_Processos_**

Para ganhar maturidade é preciso estar alinhado com diferentes tipos de requisitos de segurança, como: NIST, PCI e HIPAA. Processos exigem extrema padronização de ações para garantir que nada passe despercebido e nenhum ponto que deveria haver atenção está sendo deixado de lado.

* **_Tecnologias_**

É necessário acompanhar o mercado e as movimentações tecnológicas para encontrar a melhor solução de segurança para a realidade do negócio em que está inserido.


Os papéis de cada analista do time SOC e sua Matriz de responsabilidade, precisam ser bem estabelecidos:

* **_SOC Analyst_**

Geralmente divididos por níveis (N1, N2, N3), de acordo com a estrutura do SOC e capacidade técnica dos analistas. Sua responsabilidade principal é classificar um alerta, buscar sua causa raiz e recomendar medidas corretivas.

* **_Incident Responder_**

O Incident Response Officer é o analista que participará da tecção de ameaças, realiza a avaliação inicial de violações de segurança.

* **_Threat Hunter_**

Este membro da equipe tem o propósito de encontrar vulnerabilidades antes que um hacker (Black-hat, Gray-hat) possa explorá-lo.

* **_Security Engineer_**

Mantém a infraestrutura da solução de SIEM (Security Information and Event Management) e produtos do SOC, esta pessoa é responsável por realizar as configurações de integração entre as soluções, por exemplo, preparar a conexão entre SIEM e SOAR (Security orchestration, automation and response).

* **_SOC Manager_**

Tem função de gestão, reunindo algumas responsabilidades principais, como, orçamentárias, estratégicas, liderança e gestão da operação, este nível não lida com a parte técnica e sim com a parte executiva.

# SOC ANALYST - RESPONSABILIDADES

Analistas do SOC são os primeiros a investigar as ameaças identificadas nos sistemas/rede organizacionais, quando necessário realiza o escalonamento dos incidentes para analistas de níveis técnicos superiores tornando possível a contenção da ameaça.

Algumas de suas funções de rotina são:
Examinar alertas do SIEM determinando quais ameaças são reais ou falsos positivos, utilizando diferentes produtos, serviços e soluções de segurança como: Endpoint Detection and Response (EDR), Extended Detection and Response (XDR) Log Management e SOAR.

Porém, é importante que um analista de SOC não dependa de ferramentas ou produtos de segurança para analisar corretamente as ameaças. Para que isso seja possível o profissional deve buscar competências em uma gama de setores, sendo alguns deles:

* **_Operating Systems (O.S.)_**

Para detectar um comportamento anormal no sistema é necessário que primeiramente o analista possa identificar um comportamento normal, por isso, é importante conhecer o básico da lógica de funcionamento de Sistemas Operacionais Windows/Linux.

* **_Network_**

No dia-a-dia, o analista terá contato uma série de endereços IP's e URL's maliciosas e precisará avaliar se algum dispositivo interno está tentando realizar conexão com esses endereços, por isso é necessário entender o básico sobre rede de computadores e protocolos.

* **_Malware Analysis_**

Em algum momento o analista encontrará um software malicioso na rede, para entender seu objetivo será necessário ter certas habilidades relacionadas a Malware Analysis e principalmente uma boa lógica de programação para entender o mínimo de seu comportamento e exploração.

* **_Thinking outside the box_**

Uma das habilidades que considero mais importantes para um analista de SOC é pensar de forma criativa, pois os vetores de ataques mudam frequentemente, e pensar fora da caixa na maioria das vezes traz linhas de pensamento e soluções que não poderiam ser encontradas de outra forma.

# SOLUÇÕES E SERVIÇOS DE SEGURANÇA UTILIZADAS

Na profissão de SOC algumas soluções e serviços de segurança são frequentemente utilizadas em sua rotina de trabalho, entre elas temos: SIEM, SOAR, EDR, XDR, LOG MANAGEMENT, Threat Inteligence, etc. Embora existam diversas fabricantes de softwares o funcionamento básico de cada um não diferem um do outro, portanto neste momento entender seu conceito é o suficiente.

* **_SIEM_**
É uma solução de segurança que provê logs em tempo real de eventos ocorridos no ambiente para que a partir de regras já configuradas seja possível detectar ameaças à segurança, os logs coletados podem ser filtrados para trazer melhor visualização de um evento específico ou série de eventos relacionados, a partir da análise desses logs, um analista de SOC determina quais deles são ameaças reais ou falsos positivos.

* Algumas soluções conhecidas são: IBM QRadar, ArcSight ESM, FortiSIEM, Splunk, entre outros.
  * (ArcSight ESM)

![image](https://user-images.githubusercontent.com/123386609/215601846-052899a9-eb89-4bfd-a492-358e7f290a36.png)

Ao verificar os detalhes de um alerta é possível ter mais informações relacionados ao evento, como: Hostname, IP address, file Hash, etc.

Um bom analista sabe que nem todos os alertas enviados realmente são ameaças concretas e precisa utilizar de suas habilidades técnicas para separar falsos positivos de ameaças reais.

* **_Log Management_**
Correlaciona logs provenientes de diferentes fontes e ambientes, como: Operating System, Firewall, Proxy, EDR, XDR, etc. permitindo o gerenciamento de diferentes tipos de logs em um só lugar.

As soluções apresentadas anteriormente são soluções de Identificação de ameaças, as próximas a serem definidas são utilizadas após a identificação, na fase de análise técnica, algumas delas são:

* **_EDR_**
É uma solução de proteção de Endpoints que combina monitoramento em real-time, coleta de dados baseada em regras, detecção, analise e resposta a incidentes em uma só solução, a partir da visualização de processos, comandos, arquivos e capacidade de isolamento dos Endpoints em situação concreta de Ataque. Mesmo com o isolamento da máquina ela ainda continua a se comunicar apenas com a console, para gerenciamento remoto por parte do analista que responde ao incidente.

* Algumas soluções disponíveis no mercado são: CarbonBlack, SentinelOne, FireEye HX, Trellix EDR (Antiga McAfee).
  * (Trellix EDR)

![image](https://user-images.githubusercontent.com/123386609/215606669-fe5ebb1e-8d98-4de0-a4e9-65e9cbd6fee4.png)

A partir de um EDR é possível ter uma visualização dos acontecimentos de forma cronológica e como cada ação se relaciona com as demais. Tudo isso visualmente a partir de mapas de correlação gerados pela ferramenta.

* **_XDR_**
Um XDR é uma evolução do EDR, como seu próprio nome induz, enquanto o EDR faz a Detecção e Resposta a incidentes de segurança o XDR possibilita Detecção e Resposta Estendidas, trazendo mais capacidades de resposta a incidentes de segurança, uma de suas grandes diferenças é a habilidade de capturar dados em camadas superiores, mais distantes do Endpoint em si.

* Algumas soluções são: Trend Micro Vision One, Cortex XDR, entre outros.
  * (Cortex XDR)

![image](https://user-images.githubusercontent.com/123386609/215608758-e7ad0319-22e0-414e-95f6-e8f799189293.png)

Um XDR tende a ser a mais completa solução de proteção de Endpoints, visto que além das assinaturas de ameaças conhecidas, ela atua com analise comportamental, fazendo com que seja possível detectar um ataque antes do mesmo se concretizar podendo bloquear as ações do hacker (Black-hat, Gray-hat).

Atualmente as soluções de Antivírus convencionais também atuam com proteção baseada em comportamento, porém as capacidades do XDR vão muito além disso, como: analise de vulnerabilidades e patches no Sistema Operacional, possibilidade de importar scripts a serem executados automaticamente nos ativos, isolamento de máquinas infectadas ou com comportamento suspeito, conseguir um live terminal do equipamento, analisar arquivos em Sandbox, etc.

* **_SOAR_**
A utilização de um SOAR pode economizar muito tempo para um analista de SOC, pois ele tem a capacidade de integrar todas as demais soluções de segurança em um só lugar. Também é utilizado para criar Playbooks, que são processos e passos já configurados para a resposta a um determinado incidente, contendo um passo a passo das ações que o analista precisa executar em sua análise.

* Algumas ferramentas de SOAR disponíveis: Splunk Phantom, IBM Resilient, Logsign, Demisto.
  * (IBM Resilient)

![image](https://user-images.githubusercontent.com/123386609/215611121-625128fa-3fb0-4da0-8de7-a016137e3db9.png)

* **_Threat Inteligence_**
Também conhecida como Threat Intel, é a varredura de sites, blogs, fóruns, ferramentas de comunicação, disponíveis na surface e dark web buscando identificar correlação de palavras chave de uma organização nesses ambientes, como por exemplo vazamento de dados ou vulnerabilidades sendo vendidas na dark web por hackers (Black-hat, Gray-hat).

# DICAS E TRUQUES PARA ANÁLISE
1. Entenda o alerta:
> Qual o motivo do alerta ter sido disparado?
> Qual o nome da regra envolvida no alerta e sua descrição?
> Qual ataque estou enfrentando?
> Quais dispositivos aparecem no tráfego?
> Qual a direção do tráfego?
> Qual é a origem e qual é o destino?
> Qual protocolo está sendo usado nessa comunicação?

2. Reúna Informações:
> Relacione os endereços IP's com os dispositivos envolvidos;
> Quem são os donos desses IP's?
> O tráfego é interno ou vem da Internet?
> Caso venha da Internet, qual a reputação do IP? (Veja links úteis)
> Caso o tráfego venha da rede interna:
> Qual o hostname do dispositivo?
> Quem é o usuário associado ao dispositivo?
> Esse equipamento é compartilhado com vários usuários diferentes?
> Quando foi o último login do usuário?

# LINKS ÚTEIS - TESTES ONLINE

* https://www.virustotal.com/
* https://talosintelligence.com/
* https://www.abuseipdb.com/
* https://www.processchecker.com/file.php
* https://sitelookup.mcafee.com/
* https://mxtoolbox.com/
* https://registro.br/tecnologia/ferramentas/whois/


_Autor: Anderson Silva Lima (www.linkedin.com/in/ls-anderson)_
