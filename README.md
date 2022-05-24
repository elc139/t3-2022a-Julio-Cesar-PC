# T3: Profiling de algoritmos de machine learning do Weka / wekaPython  

Nome: Julio Cesar Polmann Cuencas 

---

# Testes 
| Algorítmo  | dataset | n_jobs |
|---|---|---|
| XGBoost | GMSC | 1-4-8 |
| XGBoost | Covertype | 1-4-8 |
| RandomForest | GMSC | 1-4-8 |
| RandomForest | Covertype | 1-4-8 |

---
# Questões
1. Qual o efeito do parâmetro `n_jobs` sobre o tempo de execução de cada algoritmo e dataset?
    - De acordo com os resultados do teste com o dataset GMSC, observamos que, com o algoritimo XGBoost, a diferença de 1 n_jobs para 4 é muito significativa, mais de 3 vezes mais rápido para a execução com 4 threads em paralelo. Observei tambem no JMC, que a execução em paralelo ultiliza mais da CPU. A diferença de 4 para 8 já não teve tanta significância, visto que algumas vezes a execução com apenas 4 threads foi mais rápida que a com 8. Já com o algorítimo RandomForestClassifier a diferença foi menor, mas ainda sim muito significativa.
    - De maneira geral, o salto de desempenho da execução com 1 para 4 threads é entre 3 a 2 vezes mais rápido, já o salto de 4 para 8 threads muitas vezes diminui o desempenho.
---

2. Usando o JMC, como o tempo de execução se divide entre os diversos métodos invocados em cada caso? (veja Method Profiling no JMC)
    - TODO
