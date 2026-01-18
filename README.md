# 🌌 Simulação do Sistema Solar (N-Body)

Este projeto implementa uma **simulação física do Sistema Solar** baseada no **problema de N corpos**, utilizando leis clássicas da física, métodos numéricos estáveis e boas práticas de computação científica.

O foco é **realismo físico**, **clareza matemática** e **arquitetura de software bem definida**, permitindo extensões futuras como visualização 3D, otimizações de desempenho e correções relativísticas.

---

## 🎯 Objetivos

* Simular o movimento de corpos celestes usando a **Lei da Gravitação Universal**
* Resolver numericamente o **problema de N corpos**
* Garantir **estabilidade orbital** e **conservação de energia**
* Separar claramente:

  * Física
  * Matemática
  * Motor de simulação
  * Visualização
* Criar uma base extensível para estudos e experimentos científicos

---

## 🧠 Fundamentos Teóricos

### Física Utilizada

* Mecânica Clássica (Newton)
* Gravitação Universal
* Sistemas dinâmicos
* Conservação de:

  * Energia
  * Momento linear
  * Momento angular

### Modelo Matemático

Para cada corpo ( i ):

[
\vec{F}*i = \sum*{j \neq i} G \frac{m_i m_j}{r_{ij}^2} \hat{r}_{ij}
]

[
\vec{a}_i = \frac{\vec{F}_i}{m_i}
]

Essas equações diferenciais ordinárias são resolvidas numericamente.

---

## 🔢 Métodos Numéricos

Métodos de integração implementados (ou planejados):

* **Velocity Verlet** (principal)
* Leapfrog
* Runge-Kutta 4 (RK4)

> O método Velocity Verlet é preferido por sua estabilidade e boa conservação de energia em sistemas orbitais.

---

## 📏 Sistema de Unidades

Para evitar problemas numéricos, são utilizadas unidades astronômicas:

| Grandeza    | Unidade                    |
| ----------- | -------------------------- |
| Distância   | Unidade Astronômica (UA)   |
| Massa       | Massa Solar                |
| Tempo       | Dias ou Anos               |
| Constante G | Normalizada para o sistema |

---

## 🧪 Validação Científica

O projeto inclui testes para:

* Conservação da energia total
* Estabilidade orbital ao longo do tempo
* Comparação com órbitas analíticas (caso de dois corpos)

---

## 🚀 Extensões Planejadas

* Visualização 3D interativa
* Correções relativísticas (précessão de Mercúrio)
* Passo de tempo adaptativo
* Otimização com Cython ou C++
* Exportação de dados para Web (JSON)

---

## 📚 Referências

* Goldstein, *Classical Mechanics*
* Press et al., *Numerical Recipes*
* NASA JPL Ephemerides
* Hairer et al., *Geometric Numerical Integration*
