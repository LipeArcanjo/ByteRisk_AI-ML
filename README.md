# 🦷 ByteRisk - Sistema de Redução de Sinistros Odontológicos para OdontoPrev

## 📖 Visão Geral

**ByteRisk** é uma solução desenvolvida para a **OdontoPrev**, com o objetivo de reduzir custos com sinistros odontológicos por meio de intervenções preventivas e automáticas, usando técnicas de machine learning. Classificando beneficiários em rankings de risco (S a F), o ByteRisk automatiza o envio de mensagens de conscientização, convites para consultas preventivas e agendamentos de exames detalhados, ajudando a prevenir problemas de saúde bucal.

---
## 🎥 Apresentação em Vídeo

[Assista à apresentação do ByteRisk no YouTube](https://youtu.be/Z0gSnLEw6cA)

---

## 🎯 Objetivo Principal

A entrega desta versão **Beta** do ByteRisk é apresentar a capacidade inicial de classificação dos beneficiários com base em dados simulados, demonstrando as funcionalidades e integrações principais que serão aprimoradas nas próximas versões.

---

## ⚡️ Diferenças Entre a Primeira e a Versão Beta

A primeira versão do ByteRisk focava em estruturar e organizar a base de dados e projetar a arquitetura inicial do sistema. 

Na **versão Beta**, os seguintes avanços foram realizados:

1. **🚀 Implementação de um Modelo de Classificação Inicial**: Utilizando o **Scikit-Learn**, desenvolvemos um modelo básico para prever o ranking de risco dos beneficiários. Nesta versão, o modelo utiliza dados simulados para treinar e testar a eficácia da classificação, mostrando como a solução ByteRisk aplicará a classificação em uma base de dados real no futuro.

2. **🔗 Integração de Dados e Funcionalidades**: Dados simulados (ver seção de Dados Utilizados no Modelo) foram incluídos para treinamento e testes do modelo. Esses dados refletem a **volumetria** e diversidade esperadas no banco de dados da ByteRisk, que centraliza informações valiosas de sinistros, consultas e perfis de saúde dos beneficiários.

3. **📄 Documentação Estruturada no GitHub**: O repositório já inclui o **notebook Python** com o modelo, os dados simulados e a documentação detalhada do projeto. Essa documentação acompanha o progresso do projeto desde a primeira entrega (SP1) até esta fase (SP2), detalhando as funcionalidades implementadas e suas origens.

4. **📊 Visualização de Dados**: A inclusão de gráficos e visualizações com **Matplotlib** e **Seaborn** possibilita uma análise inicial dos dados, oferecendo insights sobre o perfil dos beneficiários.

---

## 🛠 Frameworks, Bibliotecas e Ferramentas Utilizadas

As principais ferramentas para o desenvolvimento do ByteRisk incluem:

- **Scikit-Learn**: 🧠 Construção do modelo de machine learning para classificação dos beneficiários.
- **Pandas e NumPy**: 📊 Manipulação e processamento de dados coletados e simulados.
- **Matplotlib / Seaborn**: 📉 Visualização dos dados para identificar padrões e insights iniciais.

---

## 🗄 Dados Utilizados no Modelo

Os dados simulados nesta versão representam as principais variáveis que o ByteRisk usará para classificar o risco dos beneficiários. Estes dados foram criados para refletir a volumetria e diversidade de informações reais, as quais são armazenadas no banco de dados centralizado da ByteRisk, com dados detalhados de sinistros, consultas e perfis de saúde dos beneficiários. 

**Principais Variáveis**:

- **Tipo de Plano**: 📃 Diferentes categorias de planos odontológicos.
- **Valor Mensal**: 💰 O custo mensal do plano.
- **Idade do Beneficiário**: 👤 Dados demográficos dos beneficiários.
- **Número e Valor Total de Sinistros**: 🔍 Histórico de sinistros, servindo como indicativo de risco.
- **Número de Consultas e Exames**: 🏥 Histórico de consultas e exames realizados.

---

## 🔧 Preparação dos Dados Simulados

Para criar o modelo de machine learning, geramos dados fictícios que simulam as principais características dos beneficiários, possibilitando a construção e teste do modelo nesta versão.

### 🔄 Transformação dos Dados

Variáveis categóricas, como o tipo de plano, foram convertidas para valores numéricos usando **LabelEncoder**, permitindo que o modelo interprete esses dados.

---

## 🧪 Treinamento e Teste do Modelo

Foi utilizado o **RandomForestClassifier** do Scikit-Learn para treinar e testar o modelo. A divisão dos dados entre treino e teste garante que o modelo tenha uma base para validação e ajuste.

- **Divisão dos Dados**: 📑 Realizamos uma divisão equilibrada dos dados para treino e teste.
- **Acurácia**: 📈 Os testes iniciais mostraram boa performance na classificação dos beneficiários, com base nas variáveis disponíveis.

---

## 🛤 Próximos Passos

1. **Refinamento do Modelo**: Com dados reais, planejamos utilizar frameworks mais robustos, como o TensorFlow, para aprimorar a acurácia do modelo.
2. **Ampliação do Banco de Dados**: Integração de mais informações dos beneficiários para melhorar a classificação e segmentação dos perfis de risco.

---

## 📝 Conclusão

O ByteRisk é uma solução em evolução para reduzir custos de sinistros e promover saúde bucal preventiva. A versão Beta demonstra as principais funcionalidades e se alinha com a visão de automatizar intervenções com inteligência artificial, oferecendo um preview de como o sistema final funcionará com dados reais.

Este README, juntamente com o notebook Python e os dados simulados, estão disponíveis no GitHub para consulta.

---
