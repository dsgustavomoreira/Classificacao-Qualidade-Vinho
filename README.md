# Previsão de Doenças Renais
Classificação da Qualidade do Vinho com Algoritmos Random Forest e Support Vector Machine

# Conclusões
1. O melhor resultado para o trabalho foi obtido com o algoritmo SVC, com a utilização da técnica Random Search.
2. O primeiro ponto a ser observado é que há ligeira alteração dos valores de f1-score e accuracy entre os modelos, por isso, buscou-se avaliar Matriz de Confusão a fim de identificar qual erro seria mais tolerável para este caso.
3. Dito isto, buscou-se identificar a Matriz de Confusão com o menor Falso Negativo (previsão de boa qualidade sendo na verdade ruim), já que neste caso haverá desapontamento na experiência de degustação. Por outro lado, a incidência de Falso Positivo (previsão de vinho ruim, sendo na verdade um bom vinho) tende a ser menos prejudicial à reputação da empresa, já que um rótulo 'teoricamente' inferior irá se apresentar superior ao previamente oferecido, causando ao cliente uma 'boa surpresa' na experiência gastronômica.

# Sugestões

Sugerem-se algumas variações na metodologia deste estudo a fim de verificar o aumento da assertividade, como:

1. Divisão da categoria 'target' em 3 classes (3 e 4; 5 e 6; e, 7 e 8), ao invés de somente duas (3, 4, 5; e 6, 7, 8);
2. Aplicação de outros algoritmos, como XGBoost, haja vista a sua robustez;
3. Utilizar limite superior e inferior para outliers de 1,5 ou 2 (neste estudo considerou-se 3);
4. Manter os outliers, uma vez que não há argumentos convincentes para a sua exclusão.
