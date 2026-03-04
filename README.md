# analise-trafego-wireshark.
Projeto prático de análise de protocolos DNS, TCP e HTTP.
# 🛡️ Análise de Tráfego de Rede (Base Fundamental)

## 📋 Objetivo
Este projeto foi desenvolvido como parte do meu aprendizado em **Segurança da Informação**. O objetivo é identificar e analisar os principais protocolos de comunicação em uma rede doméstica utilizando o **Wireshark**.

---

## 🔬 Metodologia
A captura foi realizada em ambiente controlado, filtrando o tráfego gerado pelo acesso ao domínio `example.com`.

### 1. Resolução DNS
Identifiquei a requisição do meu host (`192.168.15.88`) consultando o servidor da Cloudflare (`1.1.1.1`).
![DNS Query]

### 2. Handshake TCP
Observei o estabelecimento de conexão (Three-way Handshake). Notei o uso da porta 443, indicando uma tentativa de conexão segura (HTTPS).
![TCP Handshake])



### 3. Requisição HTTP
Diferente das capturas anteriores, aqui consegui visualizar o método `GET` em texto claro. 
> **Análise de Segurança:** A visibilidade desses dados reforça o risco de ataques do tipo *Sniffing* em redes que não utilizam criptografia (TLS/SSL).
![HTTP GET]

---

## 🏁 Conclusão
Através deste projeto, compreendi a ordem lógica da comunicação cliente-servidor e a importância vital de protocolos seguros para a integridade e privacidade dos dados.
