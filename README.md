# disponibilidade-de-um-servi-o-replicado-em-m-ltiplos-servidores


Fórmula matemática que calcula a disponibilidade de um serviço replicado em vários servidores

    n – número de servidores (n > 0)
    k – número mínimo de servidores disponíveis necessário para o serviço ser acessado de forma consistente (0 < k ≤ n)
    p – probabilidade de cada servidor estar disponível em um dado instante (0 ≤ p ≤ 1)

∑(i=0 to k) [C(n,i) * p^i * (1-p)^(n-i)]

onde:

C(n,i) representa o número de maneiras de escolher i servidores dentre n servidores. p^i representa a probabilidade de que exatamente i servidores estejam disponíveis em um determinado momento. (1-p)^(n-i) representa a probabilidade de que os n-i servidores restantes não estejam disponíveis.

Essa fórmula pode ser usada para calcular a probabilidade de ter pelo menos k servidores disponíveis de n servidores para uma determinada probabilidade p. Se o resultado dessa fórmula for maior que um determinado limite, o serviço poderá ser acessado de forma consistente.
