# 📬 Classificador de SPAM (Naive Bayes Style)

Já recebeu aquele e-mail prometendo **dinheiro rápido** ou um **prêmio especial**?  
Pois é... nosso modelo aqui foi feito para **denunciar os picaretas da internet**.  

## 🤖 Como funciona?

1. Pegamos um dataset de nome spam_or_not_spam.csv.  
2. Dizemos ao modelo:  
   - "Isso aqui é **Não spam** (1)"  
   - "Isso aqui é **Spam** (0)"  
3. Ele aprende que palavras como **money**, **promotion**, **prize** = suspeito.  
4. Quando chega um e-mail novo, ele faz as contas de probabilidade e grita:  
   - `É SPAM! 🚨`  
   - ou `Relaxa, é Não é 😎`.  

## 📊 O segredo (shhh 🤫)

A mágica acontece com **Naive Bayes**, um algoritmo que usa **probabilidade**.  
É tipo um amigo fofoqueiro:  
- Viu a palavra "promoção"? → 80% de chance de ser spam.  
- Viu "relatório"? → 95% de chance de ser sério.  

Ele junta tudo e dá o veredito.  

## 🚀 Rodando o projeto

```bash
# rodar no terminal do seu IDE
pip install scikit-learn
import pandas as pd
import numpy as np
# arquivo Para jupyter notebook
python classificacao-spam-naospam.ipynb

# Testar modelo
exemplo = ["Meeting with the board."] <-- Aqui esta o input para testar o modelo, não vou me preocupar em criar um interface gráfica, deixo para dev frontend 🤦‍♂️. 
Minhas preocupaçoes são com Bag of Words, TF-IDF e Naïve Bayes e muito outros.

X_exemplo = vetorizador.transform(exemplo)
# 1 = spam, 0 = não spam
print("É spam?", modelo.predict(X_exemplo)[0]) 
