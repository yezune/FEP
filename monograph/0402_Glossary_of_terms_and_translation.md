## Glossary of terms and expressions - 용어 및 표현어 주석

*(a.u.: arbitrary units; e.g., metres (m), radians (rad), etc)*

| Expression(표현식)                                        | Description(설멸)                                                      | Units(단위)              |
|---------------------------------------------------------|:----------------------------------------------------------------------|-------------------------|
|                                                         | **Variables(변수)**                                                    |                         |
| $\tau$                                                  | 시간                                                                   | s(seconds)              |
| $x[\tau]=\{x(t):t\in(0,\tau)\}$                         | 상태공간에서 궤적이나 패스                                                   | a.u. (m)                |
| $\omega(\tau)$                                          | 무작위 요동                                                              | a.u. (m)                |
| $\begin{aligned}x^{(i)}&=\{x_1^{(i)},x_2^{(i)},\ldots,x_N^{(i)}\} \\x_n^{(i)}&=\{x_{n_1}^{(i)},x_{n_2}^{(i)},\ldots,x_{n_M}^{(i)}\} \end{aligned}$| $i$ 번째 설명 수준의 벡터 상태 | a.u. (m) |
| $x=\{\eta,s,a,\mu\}\in X$                               | 마르코프 분할은 외부, 감각, 활동 및 내부 상태로 나눔                              | a.u. (m)                |
| $\tilde\eta\in X\backslash E:x=\{\eta,\tilde\eta\}\in X$| 상태 부분 집합의 여집합                                                     | a.u. (m)                |
| $\dot x=\frac{dx}{dt}$                                  | 시간 미분(뉴턴 표기법)                                                     | m/s                     |
| $\vec x=(x,x^{'},x^{''},\ldots)$                        | 일반화된 운동(라그랑지안 표기법)                                              | (m,m/s,...)             |
| $\alpha=\{a,\mu\}\in A$                                 | 자율 상태                                                               | a.u. (m)                |
| $b=\{s,a\}\in B$                                        | 담요 상태                                                               | a.u. (m)                |
| $\pi=\{b,\mu\}\in P$                                    | 특정 상태                                                               | a.u. (m)                |
| $\eta\in E$                                             | 외부 상태                                                               | a.u. (m)                |
| $\Gamma=\tfrac h{2m}=\mu_m k_B T$                       | 무작위 요동의 진폭 (즉, 분산의 절반)                                          | $m^2$/s or J$\cdot$s/kg |
| $\mathcal Q$                                            | 솔레노이드 흐름의 정도                                                      | $m^2$/s or J$\cdot$s/kg |
| $m=\tfrac{\hbar}{2\mu_m k_b T}=\tfrac{\hbar}{2\Gamma}$  | (감소된) 질량                                                            | kg(kilogram)            |
| $\mu_m=\tfrac{\hbar}{2mk_B T}=\tfrac{1}{k_B T}\Gamma$   | 이동성 계수                                                              | s/kg                    |
| $T$                                                     | 온도                                                                   | K(Kelvin)               |
| $\ell=\int d\ell :d\ell^2=g_{ij}d\lambda^j d\lambda^i$  | 정보 길이                                                               | nats                    |
| $D(\tau)=D[p(x,\tau\vert\pi_0)\parallel p(x,\infty\vert pi_0)]$ | 발산 길이                                                       | nats                    |
| $\pmb\tau=d\ell(\tau\geq\pmb\tau)\approx 0$             | 임계 시간                                                               | s                       |
| $g_{ij}=E\lbrack\frac{\partial\Im}{\partial\lambda^i}\frac{\partial\Im}{\partial\lambda^i}\rbrack$| 피셔(정보 메트릭)텐서            | a.u.                    |
|                                                         | **Functions(함수), functionals(함수적) and potentials(퍼텐셜)**            |                         |
| $E[x]=[E_p[x]=\int xp_\lambda(x)dx$                     | 기대치 또는 평균                                                          |                         |
| $p_\lambda(x):Pr[X\in A]=\int_A p_\lambda(x)dx$         | 충분한 통계에 의해 매개변수화된 확율 밀도 함수 $\lambda$                         |                         |
| $p_\tau(x)\equiv p(x,\tau)$                             | 시간에 의해 매개변수화된 시간의존 확율 밀도 함수                                  |                         |
| $\begin{aligned}p(x)&\triangleq p_\infty(x)=\lim_{\tau\to\infty}(p(x,\tau)\\ &\Leftrightarrow \pmb L p(x)= 0\end{aligned}$ | 비평형 정상상태 밀도 - 포커-프랑크 연산자의 고유해 ||
| $q_mu(\eta)$                                            | 변분 밀도 - 내부상태의 매개변수화된 외부 상태의 (거의 후반) 밀도                     |                         |
| $f(x)=E[\dot x]$                                        | 흐름 - 상태공간에서 기대 운동                                                |                         |
| $j(x)=f(x)p(x)-\Gamma\nabla p(x)$                       | 확율 흐름                                                               |                         |
| $\begin{aligned}\Psi(x,t)&=\Psi(x)e^{-i\omega t}\\p(x)&=\Psi(x)\cdot\Psi(x)^\dagger\end{aligned}$ | Wave function - the complex root of the NESS density ||
| $\mathcal L(x,\dot x)=\tfrac 1 2[(\dot x-f)\cdot\tfrac 1 {2\Gamma}(\dot x-f)+\nabla\cdot f]$ | Lagrangian (Legendre transform of the Hamiltonian)        ||
| $\mathcal H(x,\dot x)=\dot x\cdot \tfrac{\partial\mathcal L}{\partial\dot x}-\mathcal L(x,\dot x)$ | Hamiltonian (Legendre transform of the Lagrangian)  ||
| $\mathcal A(x[\tau])=\Im(x[\tau])=\int_0^t\mathcal(x,\dot x)d\tau$ | Action: the surprisal of a path;i.e., path integral of the Lagrangian               ||
| $V(x)=\tfrac m 2 f\cdot f+\tfrac \hbar 2 \nabla\cdot f$ | Schrödinger potential                                                 | J(Joules)               |
| $U(\pi)=k_B T\cdot\Im(\pi)+F_m$                         | Thermodynamic potential                                               | J or kg $m^2$/$s^2$     |
| $F_\Im(\tau)\triangleq E[U(\pi,\tau)]-E[k_B T\cdot\Im(\pi)]$ | Thermodynamic free energy                                        | J or kg $m^2$/$s^2$     |
| $F(\pi)\geq\Im(\pi)$ | Variational free energy - an upper bound on the suprisal of the paticular states                         | nats                    |
| $G(\alpha_\tau)\geq\Im_\tau(\alpha_\tau\vert\pi_0))$| Expected free energy - an upper bound on the surprisal of an autonomous state ini the future | nats |
| $\Omega(x[\tau])$                                       | Path-dependent measurement                                            | a.u.                    |
| $\pmb\sigma(u_i)=\frac{exp(-u_i)}{\sum_i exp(-u_i)}$    | Normalised exponential (softmax) function of a vector                 | a.u.                    |
|                                                         |**Operators**                                                          |                         |
| $u\cdot v= u^T v = \braket{u\vert v}=u_i v^i$           | Inner product using do, Dirac and summation notation                  |                         |
| $u\times v=uv^T = \ket{u}\bra{v}$                       | Outer product using cross and Dirac notation                          |                         |
| $\nabla_x\Im(x)=\frac{\partial\Im}{\partial x}=\big( \frac{\partial\Im}{\partial x_1}, \frac{\partial\Im}{\partial x_2},\cdots\big)$ | Differential or gradient operator (on a scalar field)||
| $\nabla_{xx}\Im(x)=\frac{\partial^2\Im}{\partial x^2}$  | Curvature operator (on a scalar field)                                |                         |
| $\nabla\cdot f(x) = \sum_i\frac{\partial f_i}{\partial x_i}$ | Divergence operator (on a vector field)                          |                         |
| $\nabla^2\Im(x)=\nabla\cdot\nabla\Im=\Delta\Im$         | Laplace operator - the divergence of a gradient                       |                         |
| $\begin{aligned}\pmb L&=\nabla\cdot(\Gamma\nabla-f) \\ \dot x&=\pmb L p(x)\end{aligned}$ | Fokker-Planck operator               |                         |
| $\begin{aligned}\pmb H&=V(x)-\tfrac{\hbar^2}{2m}\nabla^2 \\ i\hbar\dot\Psi(x)&=\pmb H\Psi(x)\end{aligned}$ | Hamiltonian operator |                       |
| $\pmb T = -\tfrac{\hbar^2}{2m}\nabla^2$                 | Kinetic operator                                                      |                         |
| $\Im(x)=-\ln p(x)$                                      | Surprisal or self-information                                         | nats                    |
| $H(X)=H[p(x)]=E[\Im(x)]$                                | Entropy or expected surprisal                                         | nats                    |
| $H(X\vert Y) = E_{p(x,y)}[\Im(x\vert y)]$               | Conditional entropy                                                   | nats                    |
| $D[q(x)\parallel p(x)]=E_q[\ln q(x)-\ln p(x)]$          | Relative entropy or Kullback-Leibler divergence                       | nats                    |
| $\begin{aligned}I(X,Y)&=H(X)-H(X\vert Y)\\&=H(X)+H(Y)-H(X,Y)\\&=D[p(x,y)\parallel p(x)p(y)]\geq0\end{aligned}$ | Mutual information | nats or natural units 1 nat $\approx$ 1.44 bits |
| $S\triangleq=k_B H(X)$                                  | Thermodynamic entropy                                                 | J/K or $m^2$kg $s^{-2}$ /K |
|                                                         |**Constants and coefficients**                                         |                         |
| $Z$                                                     | Partition function or normalisation constant                          | a.u                     |
| $\hbar=\tfrac \hbar {2\pi}$                             | (Reduced) Planck constant (or Dirac constant) $1.05457\times 10^{-34}$| $m^2$ kg/s or J$\cdot$ s|
| $k_B$                                                   | Boltzmann constant $1.39\times 10^{-23}$                              | $m^2$ kg $s^{-2}$/K or J/K |
| c                                                       | Speed of light 299,792,458                                            | m/s                     |

## Translation Glossory - 번역 용어

| 영어                           | 한국어                  | 참고                       |
|-------------------------------|------------------------|---------------------------|
| autopoiesis                   | 자기생성                 | ChatGPT                   |
| blanket state                 | 담요 상태                | Google Bard               |
| corollary                     | 따름정리                 | 대한수학회 수학용어           |
| ensenble                      | 앙상블                  | 한국물리학회 물리학용어집        |
| entropy                       | 엔트로피                 | 한국물리학회 물리학용어집       |
| equation                      | 방정식, 식(문맥에 따라)     | 한국물리학회 물리학용어집       |
| fluctuation                   | 요동                    | 한국물리학회 물리학용어집      |
| formulation                   |	수식화, 공식화            | 한국물리학회 물리학용어집       |
| lemma                         | 보조정리                 | 대한수학회 수학용어           |
| Markov blanket                | 마르코프 담요             | Google Bard              |
| potential                     | 퍼텐셜                  | 한국물리학회 물리학용어집       |
| nonequilibrium steady-state   | 비평형 정상상태           | 한국물리학회 물리학용어집       |
| surprise, suprisal            | 놀라움                  | Google Bard              |
| symetry breaking              | 대칭 깨짐                | 한국물리학회 물리학용어집      |
| wave function                 | 파동 함수                | 한국물리학회 물리학용어집      |
| adiabatic                     | 단열                    | 한국물리학회 물리학용어집      |
| Probability current           | 확율 흐름                | 한국물리학회 물리학용어집      |

>  [한국물리학회 물리학용어집](./ref/20221216_english_korean_physics_glossory.csv) \
>  [대한수학회 수학용어](https://www.kms.or.kr/mathdict/list.html) \
>  [Google Bard](https://bard.google.com/?hl=kr)\
>  [ChatGPT](https://chat.openai.com/?model=gpt-4-browsing)
