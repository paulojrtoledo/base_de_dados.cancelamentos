# Python Insights - Cancelamento de Clientes
Este projeto foi desenvolvido com o objetivo de **analisar uma base de dados de clientes e entender os principais motivos pelos quais muitos deles cancelaram o serviço**. A análise foi feita com a linguagem Python, utilizando bibliotecas como `pandas` e `plotly`.

---

## Base de Dados

A base utilizada contém **50 mil registros de clientes**, com informações como idade, frequência de uso, número de ligações para o call center, dias de atraso, tipo de assinatura e contrato, entre outros.

🔗 A base está disponível no Google Drive:  
[Base de Dados - Cancelamentos](https://drive.google.com/drive/folders/1uDesZePdkhiraJmiyeZ-w5tfc8XsNYFZ?usp=drive_link)

---

## Etapas do Projeto

###  Passo 1: Importar base de dados  
Utilizamos o `pandas` para carregar o arquivo `.csv`.

###  Passo 2: Visualizar a base de dados  
Analisamos as informações para entender os dados e remover colunas irrelevantes, como `CustomerID`.

###  Passo 3: Tratar os dados  
Remoção de valores nulos e conferência dos tipos de dados para garantir uma análise mais precisa.

###  Passo 4: Análise Inicial  
Verificamos quantos clientes cancelaram e qual a porcentagem em relação ao total.

📉 Resultado:
- 56,8% dos clientes cancelaram
- 43,2% continuaram ativos

###  Passo 5: Identificar causas de cancelamento  
Foram criados gráficos com a biblioteca `plotly` para verificar o impacto de cada variável no cancelamento.

📌 **Principais conclusões:**
- Clientes que ligaram mais de 4 vezes para o call center geralmente cancelam
- Todos os clientes com contrato mensal cancelaram
- Atrasos acima de 20 dias também estão associados a cancelamentos

---

## 🎯 Estratégias de Redução de Cancelamentos

Com base na análise, propusemos três ações:
1. Alertar após 3 ligações ao call center
2. Oferecer benefícios para contratos não mensais
3. Avisar a equipe de cobrança ao atingir 10 dias de atraso

📉 **Nova taxa de cancelamento após simulações:**  
➡️ Apenas **18,4% dos clientes cancelariam** seguindo as estratégias acima  
➡️ Um salto de **43,2% para 81,6% de retenção de clientes**

---

## 🛠️ Tecnologias Utilizadas

- Python
- Pandas
- Plotly
- Jupyter Notebook

---

## 📚 Aprendizados

Este projeto foi criado com base em aulas práticas, e me permitiu colocar em prática:
- Leitura e limpeza de bases de dados
- Análise de comportamento de clientes
- Visualização de dados com gráficos interativos
- Propostas baseadas em evidências

---

## 📌 Como usar este projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/seuusuario/cancelamento-clientes.git
