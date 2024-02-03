# Time Series Class Work Chapter 9

## Pooria Assarehha

### ARMA(2,2) forcast and CI

$$ \hat{Y}_t(l) = \hat{\mu} + \phi_1 \left(\hat{Y}_t(l-1) - \mu\right)  + \phi_2  \left(\hat{Y}_t(l-2) - \mu \right) - \theta_1 E[e_{t+l-1} | \bf{Y} ] - \theta_2 E[e_{t+l-2} | \bf{Y} ] $$

$$ E[e_{t+j} | \bf{Y} ] = \begin{cases} 0 & j>0 \\ e_{t+j} & j \le 0  \end{cases} $$

<!-- $$ \hat{Y}_t(l) = C_t(l) + I_t(l) \begin{cases} C_t(l) = C(\phi_1, \phi_2, \theta_1, \theta_2, \bf{Y}) \\ I_t(l) = e_{t+l} + \psi_1 e_{t+l-1} + \psi_2 e_{t+l-2} + \dots\ + \psi_{l-1} e_{t+1} & l \ge 1 \end{cases}  $$ -->


95%  C.I. : $$ Var(e_t(l)) = \sigma^2 \sum_i^{l-1} \psi_j^2 \begin{cases} \psi_0 = 1 \\ \psi_1 = \phi_1 - \theta_1 \\
\psi_2 = \phi_2 - \theta_2 \\ \vdots \end{cases} \quad  \Rightarrow \quad   \hat{Y}_t(l) \pm 1.96 \times \sqrt{\sigma^2 \sum_i^{l-1} \psi_j^2} $$ 

