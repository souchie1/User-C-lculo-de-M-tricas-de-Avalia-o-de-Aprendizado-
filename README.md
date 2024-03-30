Para calcular as métricas de avaliação de modelos de classificação (acurácia, sensibilidade, especificidade, precisão e F-score), primeiro precisamos definir uma matriz de confusão. Vou escolher uma matriz de confusão arbitrária para fins de demonstração:

sql
Copy code
|        | Predito Positivo | Predito Negativo |
|--------|------------------|------------------|
| Real Positivo   |       50         |        10         |
| Real Negativo   |       5           |        80         |
A partir dessa matriz de confusão, podemos calcular as métricas conforme as fórmulas da Tabela 1:

Acurácia (Accuracy):
Accuracy
=
�
�
+
�
�
�
Accuracy= 
N
VP+VN
​
 

Sensibilidade (Recall):
Sensibilidade
=
�
�
�
�
+
�
�
Sensibilidade= 
VP+FN
VP
​
 

Especificidade (Specificity):
Especificidade
=
�
�
�
�
+
�
�
Especificidade= 
VN+FP
VN
​
 

Precisão (Precision):
Precis
a
˜
o
=
�
�
�
�
+
�
�
Precis 
a
˜
 o= 
VP+FP
VP
​
 

F-score:
F-score
=
2
×
Precis
a
˜
o
×
Sensibilidade
Precis
a
˜
o
+
Sensibilidade
F-score= 
Precis 
a
˜
 o+Sensibilidade
2×Precis 
a
˜
 o×Sensibilidade
​
 

Agora, vamos calcular essas métricas com os valores da matriz de confusão:

VP = 50
VN = 80
FP = 10
FN = 5
N = 50 + 80 + 10 + 5 = 145
Vamos agora realizar os cálculos:

Acurácia (Accuracy):
Accuracy
=
50
+
80
145
=
130
145
≈
0.8966
Accuracy= 
145
50+80
​
 = 
145
130
​
 ≈0.8966

Sensibilidade (Recall):
Sensibilidade
=
50
50
+
5
=
50
55
≈
0.9091
Sensibilidade= 
50+5
50
​
 = 
55
50
​
 ≈0.9091

Especificidade (Specificity):
Especificidade
=
80
80
+
10
=
80
90
≈
0.8889
Especificidade= 
80+10
80
​
 = 
90
80
​
 ≈0.8889

Precisão (Precision):
Precis
a
˜
o
=
50
50
+
10
=
50
60
≈
0.8333
Precis 
a
˜
 o= 
50+10
50
​
 = 
60
50
​
 ≈0.8333

F-score:
Primeiro, vamos calcular a precisão e a sensibilidade:
Precis
a
˜
o
=
0.8333
Precis 
a
˜
 o=0.8333
Sensibilidade
=
0.9091
Sensibilidade=0.9091

Em seguida, podemos calcular o F-score:
F-score
=
2
×
0.8333
×
0.9091
0.8333
+
0.9091
≈
0.8693
F-score= 
0.8333+0.9091
2×0.8333×0.9091
​
 ≈0.8693

Esses são os valores calculados para as métricas de avaliação de modelos de classificação com base na matriz de confusão fornecida.
