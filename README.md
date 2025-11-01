# Aprendendo-Lambda-Function-e-S3
Este repositório demonstra como **automatizar tarefas na AWS** utilizando **Lambda Functions** e **S3

# ⚡ Tarefas Automatizadas com AWS Lambda e Amazon S3
Quando um arquivo é enviado a um bucket S3, a função Lambda é automaticamente acionada para processar o evento — sem necessidade de servidores!

---

## 🎯 Objetivo

Mostrar como criar uma **automação serverless** na AWS com CloudFormation, Lambda e S3.  
Exemplo prático: ao fazer upload de um arquivo no S3, o Lambda registra o nome do arquivo e o horário do upload no CloudWatch Logs.

---

## 🧩 Serviços Utilizados

| Serviço | Função |
|----------|--------|
| **Amazon S3** | Armazenar os arquivos de entrada (imagens, logs, documentos, etc.) |
| **AWS Lambda** | Executar código automaticamente em resposta a eventos |
| **Amazon CloudWatch** | Registrar logs das execuções da função Lambda |
| **AWS CloudFormation** | Automatizar a criação de toda a infraestrutura |

---

⚙️ Funções Principais
| Função |	Descrição |
---
|Automação de Processos -> 	Executar código automaticamente quando algo acontece no S3 (por exemplo: upload de um arquivo).
Processamento de Dados	-> Ler, converter, validar ou mover arquivos enviados para o bucket.
Gatilho de Workflows ->	Iniciar pipelines, workflows ou funções adicionais quando um evento S3 ocorre.
Análise e Monitoramento	-> Registrar logs, métricas ou acionar alertas no CloudWatch.
Integração com outros serviços ->	Enviar dados processados para DynamoDB, SNS, SQS, API Gateway, entre outros.

---

🧠 Como a Integração Funciona
Evento no S3
→ Um arquivo é enviado, deletado ou alterado.

Trigger (Gatilho)
→ O S3 emite um evento configurado para acionar a função Lambda.

Lambda Executa o Código
→ A função processa o evento (por exemplo, lê o nome do arquivo e salva no banco).

Logs e Monitoramento
→ O resultado da execução é armazenado no CloudWatch Logs.

## ⚙️ Arquitetura

