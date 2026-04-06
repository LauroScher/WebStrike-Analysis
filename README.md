🛡️ Cyber Defense Operations Report: WebStrike Incident

Este repositório contém o relatório final de Resposta a Incidentes (IR) sobre um ataque focado na exploração de aplicações web, desenvolvido como parte das avaliações práticas de Blue Team na plataforma CyberDefenders.

O projeto consistiu em analisar capturas de tráfego de rede (PCAP) para dissecar a anatomia de um ataque de Unrestricted File Upload, mapear as táticas do invasor no framework MITRE ATT&CK e propor mitigações arquiteturais baseadas na ISO/IEC 27002 e no framework de contenção do NIST.

🔍 Escopo da Análise (Blue Team)

Vetor Inicial: Exploração de vulnerabilidade de upload de arquivos (CWE-434) utilizando a técnica de evasão por dupla extensão (.jpg.php).

Execução e Evasão: Execução de artefato malicioso (Web Shell) burlando os filtros primários de segurança do servidor Apache.

Comando e Controle (C2): Estabelecimento de Reverse Shell via Netcat em porta não padronizada (8080) visando contornar regras básicas de Firewall.

Impacto e Exfiltração: Acesso não autorizado ao terminal interativo e exfiltração do arquivo de mapeamento de usuários do sistema (/etc/passwd) através de protocolos alternativos (HTTPS/443).

🛠️ Metodologia e Ferramentas

Wireshark: Inspeção profunda de pacotes (DPI), análise de fluxos TCP/HTTP e extração de artefatos maliciosos de rede.

OSINT (IP2Location): Rastreamento e geolocalização do IP do atacante.

Governança & TTPs: MITRE ATT&CK, NIST SP 800-61 (Ciclo de Vida de IR) e ISO/IEC 27002 (Controles de Segurança).

👥 Analista Responsável

Lauro Scher - Análise Forense de Rede, Triagem de Incidentes e Documentação Técnica.

📄 Relatório Técnico Completo

Para visualizar as evidências completas, a extração dos payloads de Comando e Controle e as recomendações de segurança detalhadas:

👉 **[Clique aqui para ler o relatório completo em PDF]([https://drive.google.com/file/d/1XeWMdU4x2T7onbCwS1KLpEmmbcccO29N/view?usp=sharing](https://drive.google.com/file/d/1cQDwcAHgjHo0B_qs-HQ0-eqt4iHZK5GY/view?usp=sharing))**

Nota: O PDF está hospedado nativamente neste repositório para garantir uma visualização segura, protegendo a integridade dos artefatos de código analisados em laboratório isolado.
