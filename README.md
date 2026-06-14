# 📊 Análise Estratégica de Vendas | 2024

Projeto de análise exploratória de dados de vendas fictícios, desenvolvido com **Python** e **MySQL**, com visualizações geradas via **Matplotlib** e dashboard interativo no **Power BI**.  
O objetivo é simular um pipeline analítico real — da extração dos dados até a geração de insights de negócio.

---

## 📸 Dashboard Power BI

![Dashboard Análise Estratégica de Vendas](https://github.com/user-attachments/assets/d1cf2bd2-add8-443b-851d-3f8f50225726)

---

## 📌 Principais Insights

- 💰 **Faturamento total:** R$ 71 mil
- 📈 **Lucro bruto:** R$ 30 mil
- 📅 **Pico de vendas** concentrado na segunda quinzena de janeiro
- 🥧 **Mês 2** respondeu por **64,46%** do custo total, contra 35,54% do mês 1

---

## 🎯 Perguntas de Negócio Respondidas

- Quais são os **top 10 clientes** que mais geram receita?
- Quais **categorias de produto** têm maior lucro bruto?
- Quais são os **produtos mais lucrativos**?
- Como se distribui a **receita por cidade**?
- Qual é a **evolução da receita** ao longo do tempo?
- Qual é o **perfil de idade** dos clientes e sua relação com a receita?

---

## 🗂️ Estrutura do Repositório

```
Analise-de-dados-vendas/
│
├── Dados Venda.xlsx       # Base de dados fictícia utilizada nas análises
├── consulta.sql           # Queries SQL utilizadas nas análises
├── analise.py             # Script principal com toda a análise em Python
├── LICENSE
└── README.md
```

---

## 🛠️ Tecnologias Utilizadas

| Ferramenta | Finalidade |
|---|---|
| Python 3 | Linguagem principal |
| MySQL | Banco de dados relacional |
| Pandas | Manipulação e análise de dados |
| Matplotlib | Visualização de dados |
| PyMySQL | Conexão Python ↔ MySQL |
| Power BI | Dashboard interativo |
| Excel | Base de dados (.xlsx) |

---

## 🗄️ Modelagem do Banco de Dados

```
clientes          vendas              custos_produtos
─────────         ──────────────      ───────────────
customer_id  ──►  customer_id         produto
nome              invoice_id          custo
cidade            produto    ─────►
idade             categoria
                  quantidade
                  preco_unitario
                  data_venda
```

---

## ▶️ Como Executar

**Pré-requisitos:**
- Python 3.8+
- MySQL rodando localmente
- Bibliotecas: `pandas`, `matplotlib`, `pymysql`, `openpyxl`

**Instalação das dependências:**
```bash
pip install pandas matplotlib pymysql openpyxl
```

**Passos:**
1. Clone o repositório
```bash
git clone https://github.com/GabrielCruz079/Analise-de-dados-vendas.git
```
2. Importe os dados do arquivo `Dados Venda.xlsx` para o MySQL e execute o `consulta.sql`
3. Ajuste as credenciais no `analise.py`:
```python
conn = pymysql.connect(
    host='localhost',
    user='root',
    password='sua_senha',
    database='projeto'
)
```
4. Execute o script:
```bash
python analise.py
```

---

## 👨‍💻 Autor

**Gabriel Cruz**  
Estudante de Ciência da Computação | Universidade Cruzeiro do Sul  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/gabriel-ramos-50a081357)
[![GitHub](https://img.shields.io/badge/GitHub-black?style=flat&logo=github)](https://github.com/GabrielCruz079)
