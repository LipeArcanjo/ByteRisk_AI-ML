# 🦷 ByteRisk - Sistema de Redução de Sinistros Odontológicos para OdontoPrev

## 📚 Visão Geral

**ByteRisk** é uma solução desenvolvida para a **OdontoPrev**, com o objetivo de reduzir custos com sinistros odontológicos por meio de intervenções preventivas e automáticas, usando técnicas de machine learning. Classificando beneficiários em rankings de risco (S a F), o ByteRisk automatiza o envio de mensagens de conscientização, convites para consultas preventivas e agendamentos de exames detalhados, ajudando a prevenir problemas de saúde bucal.

---
## 🎥 Apresentação em Vídeo

[Assista à apresentação do ByteRisk no YouTube](https://youtu.be/RmGpEU9h0dw)

---

## 🎯 Objetivo Principal

A entrega desta versão **Beta** do ByteRisk é apresentar a capacidade inicial de classificação dos beneficiários com base em dados simulados, demonstrando as funcionalidades e integrações principais que foram aprimoradas nas sprints recentes.

---

## ⚡️ Diferenças Entre a Versão Beta e a Sprint 3

Na **Sprint 3**, avançamos significativamente na implementação e avaliação do modelo. As melhorias incluem:

1. **📊 Avaliação do Modelo**:
   - Implementamos a **Matriz de Confusão** para verificar a performance do modelo.
   - Geramos um **Relatório de Classificação** para medir a precisão do modelo.
   - Criamos uma visualização da **Importância das Features**, ajudando a identificar quais variáveis têm maior impacto na previsão de risco.

2. **🛠️ Melhorias no Pipeline de Dados**:
   - Padronização do **LabelEncoder** para evitar inconsistências na codificação das variáveis categóricas.
   - Melhor tratamento na divisão dos dados entre treino (65%) e teste (35%).

3. **🌐 Integração e Implantação**:
   - O modelo treinado e o encoder foram **salvos utilizando pickle**, facilitando sua reutilização e integração.
   - Criamos um **protótipo de API com Flask**, permitindo que o modelo receba novos dados e retorne previsões em tempo real.
   
4. **🌍 Testes de Predição**:
   - Foram realizados testes com três perfis de beneficiários: **alto, médio e baixo risco**.
   - O modelo demonstrou boa capacidade preditiva, confirmando a viabilidade para futuras versões com dados reais.

---

## 🛠️ Frameworks, Bibliotecas e Ferramentas Utilizadas

As principais ferramentas para o desenvolvimento do ByteRisk incluem:

- **Scikit-Learn**: 🧠 Construção do modelo de machine learning para classificação dos beneficiários.
- **Pandas e NumPy**: 📊 Manipulação e processamento de dados coletados e simulados.
- **Matplotlib / Seaborn**: 📉 Visualização dos dados para identificar padrões e insights iniciais.
- **Flask**: 🛠️ Criação da API para integração do modelo com aplicações externas.

---

## 📂 Dados Utilizados no Modelo

A base de dados utilizada nesta sprint continua sendo composta por dados fictícios, que representam informações essenciais para a classificação de risco dos beneficiários.

**Principais Variáveis**:

- **tipo_plano**: 📝 Tipo de plano (Premium ou Básico).
- **valor_mensal**: 💸 Custo mensal do plano.
- **idade**: 👤 Faixa etária do beneficiário.
- **num_sinistros e valor_total_sinistros**: 🔍 Número e valor total dos sinistros ocorridos.
- **num_consultas e num_exames**: 🏥 Quantidade de consultas e exames realizados.
- **ranking**: 🔢 Classificação do beneficiário quanto ao risco (alto, médio e baixo risco).

---

## 🧠 Treinamento e Teste do Modelo

O modelo utilizado continua sendo o **RandomForestClassifier**, devido à sua robustez e capacidade de lidar com variáveis complexas.

- **Métricas de Avaliação**:
  - Matriz de confusão.
  - Relatório de classificação.
  - Importância das features.

- **Divisão dos Dados**:
  - 65% para treinamento.
  - 35% para testes.

---

## 🚶‍♂️ Próximos Passos

1. **Testes Adicionais**: Avaliar a performance do modelo com novos conjuntos de dados para validar sua robustez.
2. **Refinamento do Modelo**: Melhorar a análise visual e o pré-processamento para aumentar a precisão das predições.
3. **Integração com Ambiente de Produção**: Desenvolver um ambiente escalável para implantação da API com Flask.

---

## 📄 Conclusão

O ByteRisk continua evoluindo como uma solução eficiente para redução de sinistros odontológicos. Nesta sprint, avançamos na avaliação do modelo, na preparação para integração e na organização do pipeline. A próxima etapa focará na escalabilidade e nos testes com dados reais.

---

