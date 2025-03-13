# Atividade Perceptron

##tarefa 1
```Python
from sklearn.linear_model import Perceptron

X=[[0,0], [0,1], [1,0], [1,1]]

Y= [0,1,1,1]

modelo= Perceptron()
modelo.fit(X,Y)

print ("Previsões:")
testes = [[0,0], [0,1], [1,0], [1,1]]
for teste in testes:
  previsao = modelo.predict([teste])
  print(f"Nuvens:{teste[0]}, previsao chuva {teste[1]} => Levar guarda-chuva? {'Sim' if previsao[0] == 1 else 'Não'}")
```

##tarefa 2
```Python
from sklearn.linear_model import Perceptron

X=[[0,0,0], [0,1,0], [1,0,0], [1,1,0], [0,0,1], [0,1,1], [1,0,1], [1,1,1]]

Y= [0,1,1,1,0,0,0,0]

modelo= Perceptron()
modelo.fit(X,Y)

print ("Decisões:")
testes = [[0,0,0], [0,1,0], [1,0,0], [1,1,0], [0,0,1], [0,1,1], [1,0,1], [1,1,1]]
for teste in testes:
  decisao = modelo.predict([teste])
  print(f"Ensolarado:{teste[0]}, Finde:{teste[1]}, Lotação:{teste[2]} decisao parque {teste[1]} => ir no parque? {'Sim' if decisao[0] == 1 else 'Não'}")
```

##tarefa 3
```Python
from sklearn.linear_model import Perceptron

X=[[0,1,1,1], [1,0,1,1], [1,1,0,1], [0,0,1,0], [1,1,1,1], [0,1,0,0], [1,0,0,1], [0,0,0,1]]

Y= [0,1,0,1,1,0,0,0]

modelo= Perceptron()
modelo.fit(X,Y)

print ("Decisões:")
testes = [[0,1,1,1], [1,0,1,1], [1,1,0,1], [0,0,1,0], [1,1,1,1], [0,1,0,0], [1,0,0,1], [0,0,0,1]]
for teste in testes:
  decisao = modelo.predict([teste])
  print(f"cansado:{teste[0]}, ingredientes:{teste[1]}, restaurante aberto:{teste[2]}, pagamento recente:{teste[3]} decisao comer {teste[0]} => comer fora? {'Sim' if decisao[0] == 1 else 'Não'}")
```
