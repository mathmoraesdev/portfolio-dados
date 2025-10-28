
# 📱 Análise e Previsão de Preços de Dispositivos Móveis

## 🎯 Objetivo
Analisar fatores que influenciam o preço de dispositivos móveis e desenvolver um modelo preditivo para estimar valores com base em suas características.

## 🛠️ Pré-processamento e Manipulação dos Dados

### Verificando valores nulos
<img width="774" height="464" alt="Image" src="https://github.com/user-attachments/assets/30b5ce8f-1e0c-4815-b790-c5669d17a1d9" />

### Normalização da Coluna RAM
<img width="835" height="365" alt="Image" src="https://github.com/user-attachments/assets/66579b33-5fa1-4e47-a37a-bc8d76343e29" />

### Função de conversões para Dólar
<img width="840" height="763" alt="Image" src="https://github.com/user-attachments/assets/d9aa0f7d-1d9e-40ac-a6ab-5779083bd7fb" />

*taxas de câmbio retiradas em 17/03/25*


## 📊 Análise Exploratória (EDA)

### Relação entre RAM e Preço

<img width="580" height="455" alt="Image" src="https://github.com/user-attachments/assets/4cfe3566-7192-41d4-8994-8d466b4366be" />

### Preços Médios por País

<img width="977" height="590" alt="Image" src="https://github.com/user-attachments/assets/f5ab8fc6-b360-4afa-ad64-ede5206aff57" />

### Correlação entre Features
<img width="1032" height="819" alt="Image" src="https://github.com/user-attachments/assets/c79faab2-f995-4cae-a0df-2e56891f36ef" />


### Principais insights:

Peso vs Bateria/Tela: Correlação muito alta (0.85-0.98) - dispositivos maiores têm baterias maiores

RAM vs Preço (EUA): Correlação moderada de 0.46 - mais RAM geralmente significa preço mais alto

Câmera Traseira vs RAM: Correlação de 0.18 - dispositivos com mais RAM tendem a ter melhores câmeras

Bateria vs Preço: Correlação negativa (-0.035) - surpreendentemente, bateria maior não significa preço maior

## 🤖 Modelagem Preditiva

### Resultados dos Modelos
<img width="1189" height="590" alt="Image" src="https://github.com/user-attachments/assets/97967df1-3ad6-4be6-951b-ed245a053e96" />

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
