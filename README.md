# Kaggle-competition
![diamonds](input/diamonds.jpeg)

1 Se obtiene una dataset de los diamantes que consta de dos archivos: train/test.

2 Se limpian los datos del archivo train,eliminando posibles nulos,standarizando,normalizando y convirtiendo aquellas columnas categóricas a numéricas(para ello se usa la libreria sklearn).

3 Una vez convertidos todos los datos se realiza un split,con los datos del train (80%entrenamiento y 20%test),para entrenar el modelo.

4 Se eligen diversos modelos de regresión,y se evaluan sus principales metricas,siendo estas R2,MSE y MAE.

5 Dentro de cada modelo,se ajustaran los hiperparametros,es decir,se optimizaran,para encontrar los mejores de ese modelo.

6 Una vez encontrados se llevará acabo un cross_value score para que entrene las distintas porciones 20/80 del train,y por último se realizará un testeo con el 100% de los datos del train.

7 Una vez entrenado el módelo,se testeará con el los datos de test(previamente limpiados y acondicionados), con el fin de encontrar el ground truth,que en este caso será el precio de los diamantes.

8 Este ground truth será exportado a outputs,en forma de csv,y será el archivo que se subirá a Kaggle.