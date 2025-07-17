# 🧪 Gerador de Casos de Teste

A ideia do projeto vem de uma necesidade de otimizar o tempo e automatizar os planos de testes com base nas tarefas descritas utilizando api do chatGPT (OpenIA)

---

## Funcionalidades

* Geração automática de **casos de teste completos**, baseados em técnicas como:

  * Particionamento de Equivalência
  * Valor Limite
  * Estado
  * Casos positivos e negativos
* Gera um **documento `.docx` em modo paisagem** (facilitar a visualização da tabela), com:
  * Logo do projeto/ empresa
  * Tabela com os casos de teste
* Interface gráfica (Tkinter)
* Preserva a chave da API via `.env` - [Gere sua chave OpenIA](https://platform.openai.com/docs/api-reference/authentication). 

<img width="935" height="600" alt="image" src="https://github.com/user-attachments/assets/29ddd9de-b9cf-4dfd-bc52-6adbe482c52b" />

_Exemplo de documento no repositório_


<img width="697" height="504" alt="image" src="https://github.com/user-attachments/assets/5f7de185-4563-4726-a388-b612acfec0d8" />


---


## Como Usar?

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/gerador-casos-teste-ia.git
cd gerador-casos-teste-ia
```

### 2. Instale as dependências

Recomenda-se o uso de um ambiente virtual.

```bash
pip install -r requirements.txt
```

### 3. Configure o arquivo `.env`

Crie um arquivo `.env` na raiz do projeto com o seguinte conteúdo:

```
OPENAI_API_KEY=sua_chave_api_aqui
```

> **Importante:** sua chave da OpenAI será mantida privada. Não compartilhe o `.env`.

### 4. Execute o projeto

```bash
python gerador-Plano-Teste.py
```

---

## Como Funciona?

O projeto utiliza a OpenAI GPT para interpretar a tarefa escrita (Quanto mais detalhado, melhor) e, a partir dela, gerar um plano de testes com:

* Resumo da Tarefa
* Pré-condições
* Técnicas de Teste
* Casos de Teste completos no formato:

Tabela:
```
Caso de Teste;Descrição;Passos;Resultado Esperado;Status;Observação do teste
```

---


Esse projeto nasceu de uma **necessidade real no ambiente de desenvolvimento**, onde havia carência de tempo e padronização para a geração de casos de teste de qualidade.


