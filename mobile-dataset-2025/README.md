
# 📱 Análise e Previsão de Preços de Dispositivos Móveis

## 🎯 Objetivo
Analisar fatores que influenciam o preço de dispositivos móveis e desenvolver um modelo preditivo para estimar valores com base em suas características.

## 🛠️ Pré-processamento e Manipulação dos Dados

### Verificando valores nulos
![Verificação de nulo](images/verificacaodenulo.png)

### Normalização da Coluna RAM
![colunaram](images/1_4.png)

### Função de conversões para Dólar
![conversoes](images/imagemm.png)

*taxas de câmbio retiradas em 17/03/25*


## 📊 Análise Exploratória (EDA)

### Relação entre RAM e Preço

![ramepreco](images/colunaram1.png)

### Preços Médios por País

![precoporpais](images/__results___25_0.png)

### Correlação entre Features
![Análise de Correlação](images/fim.png)

### Principais insights:

Peso vs Bateria/Tela: Correlação muito alta (0.85-0.98) - dispositivos maiores têm baterias maiores

RAM vs Preço (EUA): Correlação moderada de 0.46 - mais RAM geralmente significa preço mais alto

Câmera Traseira vs RAM: Correlação de 0.18 - dispositivos com mais RAM tendem a ter melhores câmeras

Bateria vs Preço: Correlação negativa (-0.035) - surpreendentemente, bateria maior não significa preço maior

## 🤖 Modelagem Preditiva

### Resultados dos Modelos
![Comparação de Modelos](images/__results___31_0.png)

| Modelo | R² | MSE |
|--------|----|-----|
| **Random Forest** | **0.88** | **20.824** |
| XGBoost | 0.87 | 20.965 |
| Regressão Linear | 0.38 | 105.553 |

## 🛠️ Tecnologias Utilizadas
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
