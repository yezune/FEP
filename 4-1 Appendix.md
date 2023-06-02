## Appendix A: Stratonovich path integrals - 첨부 A: 슈트라토노비치 경로 적분

다음은 확률적 미분방정식의 Stratonovich 해석하에서 발산항의 기원에 대한 직관을 제공합니다. 완전한 처리를 위해서는 (Cugliandolo and Lecomte, 2017)를 참조하십시오. 이산화된 경로를 상상해보세요. 여기서 각 구간의 확률은 그 중간점에서의 첫 번째 도함수와 예상 흐름의 차이에 기반합니다:

$$
\begin{equation}\tag{11.1}
\begin{aligned}
\dot x_{\tau+\tfrac{\Delta\tau}{2}}
  &= f(x_{\tau+\tfrac{\Delta\tau}{2}})+ \Delta(\omega_\tau)\\
p(\Delta(\omega_\tau))
  &= |\partial_\omega \Delta|^{-1} p(\omega_\tau)\\
p(\omega_\tau)
  &= \cal N(0,\tfrac{2\Gamma}{\Delta\tau}) \\
\end{aligned}
\end{equation}
$$

이 차이는 각 구간의 시작부에서의 흐름에서 무작위 요동의 함수로, 그 분산은 구간 길이 $\Delta\tau$가 감소함에 따라 감소합니다. 두 번째 방정식은 변수의 변화에서 따르는 것입니다; 즉, 구간의 시작에서의 무작위 요동으로부터 중간점에서의 첫 번째 도함수에 대한 기여입니다. 랑주뱅 방정식의 해를 사용하여, 우리는 흐름의 발산에 따라 (11.1)에서의 야코비안의 행렬식을 다음과 같이 표현할 수 있습니다:

$$
\begin{equation}\tag{11.2}
\begin{aligned}
\Delta(\omega_\tau)
  &= \dot x_{\tau+\tfrac{\Delta\tau}{2}}-f(x_{\tau+\tfrac{\Delta\tau}{2}})\\
\dot x_{\tau+\tfrac{\Delta\tau}{2}}
  &= e^{\tfrac{\Delta\tau}{2}\partial_xf} \dot x_\tau
   = e^{\tfrac{\Delta\tau}{2}\partial_xf}(f(x_\tau)+\omega_\tau) \Rightarrow \\
|\partial_\omega\Delta|
  &= e^{\tfrac{\Delta\tau}{2}\nabla\cdot f}

\end{aligned}
\end{equation}
$$

이를 통해 우리는 연속적인 경로의 액션 (즉, 놀라움)을 짧은 간격의 한계로 표현할 수 있습니다.

$$
\begin{equation}\tag{11.3}
\begin{aligned}
\Im(x[\tau]
  &= \lim_{\Delta\tau \to 0}\sum_\tau\Im(\Delta(\omega_\tau))\\
  &= \lim_{\Delta\tau \to 0}\sum_\tau\tfrac 1 2 (\dot x-f)\cdot \tfrac{\Delta\tau}{2\Gamma}(\dot x-f) + \tfrac{\Delta\tau}{2}\nabla\cdot f \\
  &= \tfrac 1 2 \int[(\dot x-f)\cdot\tfrac{1}{2\Gamma}(\dot x-f)+\nabla\cdot f]dt\\
\end{aligned}
\end{equation}
$$

이것은 라그랑지안의 액션 또는 경로 적분입니다. 직관적으로, 발산은 시간에 따라 무작위 요동이 얼마나 빠르게 지수적으로 '기억되거나' '잊혀지는지'를 결정합니다. 즉, 발산이 낮을 때는 흐름에 대한 요동이 빠르게 감소하고 더 넓은 범위의 무작위 요동이 후속 흐름에서 유사한 차이를 생성하여 그들을 더 가능성 있거나 덜 놀랍게 만듭니다.

## Appendix B: lemmas and proofs - 첨부 B: 보조정리와 증명

**보조정리** (비평형 정상상태 밀도): 비평형 정상상태의 무작위 동적 시스템의 밀도는 흐름이 $f=(Q−\Gamma)\nabla\Im$ 이고 관련된 Fokker Planck 연산자가 $\pmb L\triangleq\nabla\cdot(\Gamma\nabla-f)$인 경우에는 다음과 같이 주어집니다:

$$
\begin{equation}\tag{12.1}
\begin{aligned}
p(x)
  &= exp(-\Im(x)) \\
  &\Rightarrow \nabla p = -p(x)\nabla\Im(x) \\
  &\Rightarrow \dot p(x) = \pmb L p(x) = 0 \\
  &\Rightarrow f(x) = (\Gamma - Q)\nabla\ln p(x) \\
\end{aligned}
\end{equation}
$$

**증명**: 포커-프랑크 연산자에 $\nabla p=-p\nabla\Im$와 $f=Q\nabla\Im-\Gamma\nabla\Im$를 대입하면 다음과 같이 됩니다:

$$
\begin{equation}\tag{12.2}
\begin{aligned}
\pmb L p
  &= \nabla\cdot\Gamma\nabla p-\nabla\cdot(fp) \\
  &= -\nabla\cdot(p\Gamma\nabla\Im)-\nabla\cdot(pQ\nabla\Im)+\nabla\cdot(p\Gamma\nabla\Im) \\
  &= -p\nabla\cdot(Q\nabla\Im)-(Q\nabla\Im)\cdot\nabla p \\
  &= -p(\nabla\cdot(Q\nabla\Im)-\nabla\Im\cdot(Q\nabla\Im)) \\
\end{aligned}
\end{equation}
$$

(12.1)은 솔레노이 흐름 성분 $Q\nabla\Im$이 발산이 없고 $\nabla\Im$에 직교할 때 만족됩니다. 두 조건이 만족되는 것을 쉽게 확인할 수 있습니다. 그러한 조건은 다음과 같습니다:
$$
\begin{equation}\tag{12.3}
\begin{aligned}
Q &= -Q^t 
  \Rightarrow 
\begin{cases}
  \nabla\cdot(Q\nabla\Im) &= tr(Q\nabla_{xx}\Im) = 0 \\
  \nabla\Im\cdot(Q\nabla\Im) &= tr(Q\nabla\Im\nabla\Im^T) = 0 \\
\end{cases}
\end{aligned}
\end{equation}
$$

이는 $p=exp(-\Im)$가 평형 밀도 또는 포커-프랑크 연산자가 묘사하는 밀도 동역학의 고유해 $\pmb L p=0$임을 의미합니다.


**따름정리** *(마르코프 담요): 만약 한 (외부) 상태의 부분집합 $\eta\subset x$이 그들의 마르코프 담요 $b\subset x$에 조건부로 다른 (내부) 부분집합 $\eta\subset x$와 조건부로 독립적이며 – 그리고 부분집합이 솔레노이드 흐름을 통해 연결되지 않는다면 – 내부 상태의 흐름은 외부 상태에 의존하지 않고, 반대도 마찬가지입니다.*

$$
\begin{equation}\tag{12.4}
\begin{aligned}
\begin{rcases}
p(x|m)
  &= p(\eta|b)p(\mu|b)p(b) \\
Q_{\eta\mu} 
  &= 0 \\
Q_{\eta b} 
  &= 0 \\
Q_{\mu b} 
  &= 0 \\
\end{rcases} 
  &\Rightarrow 
\begin{cases}
\nabla_\mu f_\eta(x)
  &= 0 \\
\nabla_\eta f_\mu(x)
  &= 0 \\
\end{cases} 
\end{aligned}
\end{equation}
$$

**증명**: 상기 방정식의 분할에 따라 흐름을 표현하면 다음과 같습니다:

$$
\begin{equation}\tag{12.5}
\begin{aligned}
\begin{bmatrix}
  f_\eta(x) \\
  f_b(x) \\
  f_\mu(x) \\
\end{bmatrix}
  &=
\begin{bmatrix}
  \Gamma_{\eta\eta}-Q_{\eta\eta}& -Q_{\eta b}        & -Q_{\eta\mu} \\
  Q_{\eta b}^T                  & \Gamma_{bb}-Q_{bb} & -Q_{b\mu} \\
  Q_{\eta\mu}^T                 & Q_{b\mu}^T         & \Gamma_{\mu\mu}-Q_{\mu\mu} \\
\end{bmatrix}
\begin{bmatrix}
  \nabla_\eta \ln p \\
  \nabla_b \ln p \\
  \nabla_\mu \ln p \\
\end{bmatrix}
  =
\begin{bmatrix}
  (\Gamma_{\eta\eta} - Q_{\eta\eta})\nabla_\eta \ln p \\
  (\Gamma_{bb}       - Q_{bb})      \nabla_b \ln p \\
  (\Gamma_{\mu\mu}   - Q_{\mu\mu})  \nabla_\mu \ln p \\
\end{bmatrix} \\
\end{aligned}
\end{equation}
$$

여기서 (그리고 전체적으로) 무작위 요동이 독립적이며 동일하게 분포하고 있다고 가정합니다 (즉, 그들의 공분산이 주대각선 형태를 가집니다). 상기의 조건부 독립성에 따라서

$$
\begin{equation}\tag{12.6}
\begin{aligned}
\nabla_{\mu\eta}\ln p(x)
  &= \nabla_{\mu\eta}(\ln p(\eta|b)+\ln p(\mu|b)+\ln p(b)) 
   = 0 \\
\end{aligned}
\end{equation}
$$

그리고

$$
\begin{equation}\tag{12.7}
\begin{aligned}
\nabla_\mu f_\eta(x)
  &= (\Gamma_{\eta\eta}-Q_{\eta\eta})\nabla_{\mu\eta}\ln p(x) = 0 \\
\nabla_\eta f_\mu(x)
  &= (\Gamma_{\mu\mu}-Q_{\mu\mu})\nabla_{\eta\mu}\ln p(x) = 0 \\
\end{aligned}
\end{equation}
$$

이것은 내부 상태의 흐름이 외부 상태에 의존하지 않음을, 그리고 그 반대도 마찬가지임을 의미합니다.

**참고**: 마르코프 담요 따름정리는 (일반화된) 마르코프 담요 분할에 내재된 조건부 독립성의 결과로 외부와 내부 상태의 분리를 표현합니다. 다른 구성은 흐름 제약 조건을 기반으로 마르코프 담요 (및 솔레노이드 결합의 억제)를 이끌어내는 것을 시작합니다. 예를 들어, 우리는 다음과 같이 야코비안을 이용하여 결합되지 않은 흐름을 표현할 수 있습니다: (12.5)에서

$$
\begin{equation}\tag{12.8}
\begin{aligned}
\begin{rcases}
  \nabla_\mu f_\eta(x) \\
  \nabla_\eta f_\mu(x) \\
\end{rcases}
  &=
\begin{Bmatrix}
  (Q_{\eta\eta}-\Gamma_{\eta\eta})\nabla_{\mu\eta}\Im+Q_{\eta b}\nabla_{\mu b}\Im+Q_{\eta\mu}\nabla_{\mu\mu}\Im \\
  (Q_{\mu\mu}-\Gamma_{\mu\mu})\nabla_{\eta\mu}\Im+Q_{b \mu}^T\nabla_{\eta b}\Im+Q_{\eta\mu}^T\nabla_{\eta\eta}\Im \\
\end{Bmatrix}
   = 0 \\
\end{aligned}
\end{equation}
$$

$\Gamma_{\eta\eta},\Gamma_{\mu\mu}$이 양의 정부호이므로, 놀라움의 연관된 미분은 반드시 0이어야 하며, 우리는 마르코프 담요 분해를 다시 얻게 됩니다:

$$
\begin{equation}\tag{12.9}
\begin{aligned}
\begin{rcases}
  \nabla_{\mu\eta} \\
  \nabla_{\eta\mu} \\
\end{rcases}
  &= 0 \Rightarrow
\begin{Bmatrix}
  \Im(\eta|b,\mu) \\
  \Im(\mu|b,\eta) \\
\end{Bmatrix}
   =
\begin{Bmatrix}
  \Im(\eta|b) \\
  \Im(\mu|b) \\
\end{Bmatrix}
    \Rightarrow p(x)
   = p(\eta|b)p(\mu|b)p(b) \\
\\
\end{aligned}
\end{equation}
$$

또한, $\nabla_{\mu\mu}\Im,\nabla_{\eta\eta}\Im$이 양의 반정부호이므로, 외부와 내부 상태 사이의 솔레노이드 결합을 제거할 수 있습니다: $Q_{\eta\mu}=0$. 그래서, 담요 상태와의 솔레노이드 결합은 다음을 만족해야 합니다:

$$
\begin{equation}\tag{12.10}
\begin{aligned}
\begin{rcases}
  Q_{\eta b}\nabla_{\mu b}\Im \\
  Q_{b \mu}^T\nabla\Im \\
\end{rcases}
  &= 0 \Leftarrow 
\begin{Bmatrix}
  Q_{\eta b} \\
  Q_{\mu b} \\
\end{Bmatrix}
   = 0 \\
\\
\end{aligned}
\end{equation}
$$

담요 상태와의 솔레노이드 결합이 없는 것은 흐름 제약조건을 만족하는 데 충분하지만 필요하지는 않다는 점을 유의하십시오. 예를 들어, 담요 상태를 활성화 상태와 감각 상태로 나누어 위의 분석을 반복하고, 따르는 (완전한) 흐름 제약조건을 가지면, 다음과 같이 표현할 수 있습니다:

$$
\begin{equation}\tag{12.11}
\begin{aligned}
f(x)
   = 
\begin{bmatrix}
  f_\eta(\eta,b) \\
  f_s(\eta,b) \\
  f_\mu(\mu,b) \\
  f_a(\mu,b) \\
\end{bmatrix}
  &\Leftrightarrow 
\begin{Bmatrix}
  \nabla_\mu f_\eta \\
  \nabla_\mu f_s \\
  \nabla_\eta f_\mu \\
  \nabla_\eta f_a \\
\end{Bmatrix}
   =
\begin{Bmatrix}
  (Q_{\eta\eta} -\Gamma_{\eta\eta})\nabla_{\mu\eta}\Im 
    + Q_{\eta a}\nabla_{\mu a}\Im 
    + Q_{\eta s}\nabla_{\mu s}\Im 
    + Q_{\eta\mu}\nabla_{\mu\mu}\Im \\
  (Q_{ss} -\Gamma_{ss})\nabla_{\mu s}\Im 
    + Q_{sa}\nabla_{\mu a}\Im 
    - Q_{\eta s}^T\nabla_{\mu\eta}\Im 
    + Q_{s\mu}\nabla_{\mu\mu}\Im \\
  (Q_{\mu\mu} -\Gamma_{\mu\mu})\nabla_{\eta\mu}\Im 
    - Q_{a\mu}^T\nabla_{\eta a}\Im 
    - Q_{s\mu}^T\nabla_{\eta s}\Im 
    - Q_{\eta\mu}^T\nabla_{\eta\eta}\Im \\
  (Q_{aa} -\Gamma_{aa})\nabla_{\eta a}\Im 
    + Q_{a \mu}\nabla_{\eta\mu}\Im 
    - Q_{sa}^T\nabla_{\eta s}\Im 
    - Q_{\eta a}^T\nabla_{\eta\eta}\Im \\
\end{Bmatrix}
   = 0 \\
  &\Rightarrow
\begin{Bmatrix}
  \nabla_{\mu\eta}\Im \\
  \nabla_{\mu s}\Im \\
  \nabla_{\eta\mu}\Im \\
  \nabla_{\eta a}\Im \\
\end{Bmatrix}
   = 0 \Rightarrow
\begin{bmatrix}
  Q_{\eta a} & Q_{\eta\mu} \\
  Q_{sa} & Q_{s\mu} \\
\end{bmatrix}
   =
\begin{bmatrix}
 Q_{\eta\alpha} \\
 Q_{s\alpha} \\
\end{bmatrix}
   = 0 \\
\end{aligned}
\end{equation}
$$

이러한 제약조건에 의해 내포된 특정한 흐름의 분리는 내부 상태와 외부 상태 사이, 그리고 자율적 상태와 비자율적 상태 사이의 솔레노이드 결합을 배제합니다. 이것은 일반화된 상태에 대한 마르코프 담요을 유도하며, 그것은 그림 23에서 보여주는 것처럼 나타납니다.

![FIGURE 23](./img/23.png)
<p style="text-align: center;">FIGURE 23</p>

*일반화된 마르코프 담요*. 이 종속성 그래프 또는 베이지안 네트워크는 일반화된 상태, 즉 상태와 그들의 운동을 포함하는 그림 1의 세부적인 버전입니다. 내부 상태의 마르코프 담요은 파란색으로 강조된 일반화된 상태로 구성되며, 해당 운동의 마르코프 담요을 구성하는 일반화된 상태는 분홍색 원으로 그려져 있습니다. 이 그림에서 중요한 점은 일반화된 내부 상태의 마르코프 담요이 일반화된 담요 상태(감각 운동 제외)를 포함한다는 것입니다. 이 일반화된 담요은 내부 상태와 외부 상태 사이, 그리고 자율적 상태와 비자율적 상태 사이에 솔레노이드 결합이 없어야 합니다.

**보조정리** (marginal flow): _어떤 약한 혼합 랜덤 동적 시스템에 대해, 상태의 어떤 부분 집합 $\eta\in X$의 주변 흐름 $f\eta(\mu)$은 다른 $\mu\in X$의 보완하에 평균화 될 수 있으며, 해당하는 주변 놀라움 $\Im(\mu)=−\ln p(\mu)$의 기울기를 통해 표현될 수 있습니다_:

$$
\begin{equation}\tag{12.12}
\begin{aligned}
f_\eta(\mu)
  &\triangleq E_{p(\tilde \mu|\mu)}[f_\eta(\mu,\tilde \mu)]
   = (\Gamma_{\eta\eta} - Q_{\eta\eta})\nabla_\eta\ln p(\mu) - Q_{\eta \tilde \eta} \nabla_{\tilde \eta} \ln p(\mu) \\
\end{aligned}
\end{equation}
$$

**증명**: 상태의 부분 집합과 그 보완집합으로 상태를 분할한다고 합시다: $x=(\mu,\tilde\mu)$. 이에 상응하는 (비평형 정상상태) 흐름의 분할은 다음과 같이 표현될 수 있습니다:
$$
\begin{equation}\tag{12.13}
\begin{aligned}
\begin{bmatrix}
  f_\eta(x) \\
  f_{\tilde \eta}(x) \\
\end{bmatrix}
  &=
\begin{bmatrix}
  \Gamma_{\eta\eta}-Q_{\eta\eta} & -Q_{\eta\tilde\eta} \\
  Q^T_{\eta\tilde\eta}           & \Gamma_{\tilde\eta\tilde\eta} - Q_{\tilde\eta\tilde\eta} \\
\end{bmatrix}
\begin{bmatrix}
  \nabla_\eta\ln p(x) \\
  \nabla_{\tilde\eta}\ln p(x) \\
\end{bmatrix}
\end{aligned}
\end{equation}
$$

이를 바탕으로, $x=(\mu,\tilde\mu)$에서 $\tilde\mu$에 대한 기대값으로 흐름을 정의할 수 있습니다:

$$
\begin{equation}\tag{12.14}
\begin{aligned}
f_\eta(\mu)
  &\triangleq E_{p(\tilde\mu|\mu)}[f_\eta(\mu,\tilde\mu)] 
   = \int f_\eta(x)p(\tilde\mu|\mu)d\tilde\mu \\
  &= \int(\Gamma_{\eta\eta} -Q_{\eta\eta})\nabla_\eta \ln p(x) -Q_{\eta\tilde\eta}\nabla_{\tilde\eta}\ln p(x))p(\tilde\mu|\mu)d\tilde\mu \\
  &= \int\Big((\Gamma_{\eta\eta} -Q_{\eta\eta})\nabla_\eta p(\tilde\mu|\mu)p(\mu) -Q_{\eta\tilde\eta}\nabla_{\tilde\eta}p(\tilde\mu|\mu)\Big)p(\mu)\frac{p(\tilde\mu|\mu)}{p(\tilde\mu,\mu)}d\tilde\mu \\
  &= (\Gamma_{\eta\eta} - Q_{\eta\eta})\left(\frac{\nabla_\eta p(\mu)}{p(\mu)} + \int\nabla_\eta p(\tilde\mu|\mu)d\tilde\mu \right) 
     - Q_{\eta\tilde\eta}\left( \frac{\nabla_{\tilde\eta}p(\mu)}{p(\mu)} + \int\nabla_{\tilde\eta} p(\tilde\mu|\mu)d\tilde\mu \right)\\
  \\
  &= (\Gamma_{\eta\eta} - Q_{\eta\eta})\nabla_\eta \ln p(\mu) - Q_{\eta\tilde\eta}\nabla_{\tilde\eta}\ln p(\mu) \\
\end{aligned}
\end{equation}
$$


확률 기울기의 적분은 확률 밀도의 평균 변화가 0이기 때문에 사라집니다.

**따름정리** (조건부 독립): _상태의 한 부분집합의 흐름이 다른 부분집합에 의존하지 않는다면, 그것은 두 번째 부분집합 아래에서의 마진 흐름 (예상)이 된다. 예를 들어, 마르코프 담요 파티션에 따르면, 다음과 같습니다_:

$$
\begin{equation}\tag{12.15}
\begin{aligned}
\begin{bmatrix}
  f_\eta(x) \\
  f_s(x) \\
  f_\mu(x) \\
  f_a(x) \\
\end{bmatrix}
  &= 
\begin{bmatrix}
  f_\eta(\eta,b) \\
  f_s(\eta,b) \\
  f_\mu(\mu,b) \\
  f_a(\mu,b) \\
\end{bmatrix}
  = 
\begin{bmatrix}
  (Q-_{\eta\eta}-\Gamma_{\eta})\nabla_\eta\Im \\
  (Q-_{ss}-\Gamma_{ss})\nabla_s\Im \\
  (Q-_{\mu\mu}-\Gamma_{\mu\mu})\nabla_\mu\Im \\
  (Q-_{aa}-\Gamma_{aa})\nabla_a\Im \\
\end{bmatrix}
  + 
\begin{bmatrix}
  +Q_{\eta s}\nabla_s\Im \\
  +Q_{\eta s}^T\nabla_\eta\Im \\
  +Q_{\mu a}\nabla_a\Im \\
  +Q_{\mu a}^T\nabla_\mu\Im \\
\end{bmatrix} \\ 
\end{aligned}
\end{equation}
$$

마르코프 담요 따름정리 (12.11)에 의해 많은 솔레노이드 항이 제거됩니다. 간단히 말해, 마르코프 담요에 의해 유도된 조건부 독립성은 외부 상태의 흐름이 내부 상태의 모든 값에 대해 동일하다는 것을 의미하며, 이것은 내부 상태에 대한 평균에 불과합니다 (다른 파티션에 대해서도 비슷합니다).

**따름정리** _(예상 흐름): 모든 다른 상태들에 대한 평균을 가진 부분집합 $\eta\subset x$의 마진 흐름은 그 부분집합의 마진 밀도의 기울기에만 의존하며, 그 부분집합이 보완집합과 솔레노이드 결합이 없어야 합니다:_



$$
\begin{equation}\tag{12.16}
\begin{aligned}
f_\eta(\eta)
  &= (\Gamma_{\eta\eta}-Q_{\eta\eta})\nabla_\eta\ln p(\eta)
   = (Q_{\eta\eta}-\Gamma_{\eta\eta})\nabla_\eta\Im(\eta) \\
\end{aligned}
\end{equation}
$$

이것은 $\eta=\mu$ 이고 $Q_{\eta\tilde\eta}=0$ 일 때, 마진 흐름 보조정리의 특수한 경우입니다. 이것은 모든 다른 상태들에 대한 평균을 가진 어떤 상태나 상태 부분집합의 예상 흐름이, 모든 상태를 함께 고려했을 때와 정확히 같은 방식으로 행동할 것임을 의미합니다. 즉, 그것은 그것의 (마진) 놀라움의 기울기를 따라 내려갈 것입니다.

## Appendix C: nonequilibrium steady-static energy functions - 첨부 C: 비평형 정상상태 에너지 함수

비평형 정상상태에서, 놀라움의 예상 곡률은 기울기 제곱의 예상 합입니다:

$$
\begin{equation}\tag{13.1}
\begin{aligned}
E_{p(x)}[\nabla^2\Im]
  &= \int p\nabla^2\Im dx \\
  &= \int p\Bigg(\frac{\nabla p\cdot\nabla p}{p^2}-\frac{\nabla^2 p}{p} \Bigg)dx  \\
  &= \int p\nabla\Im\cdot\nabla\Im dx \\
  &= E_{p(x)}[\nabla\Im\cdot\nabla\Im]\\
\end{aligned}
\end{equation}
$$

비평형 정상상태 밀도의 곡률의 적분이 사라지는 이유는 이것이 적절한 밀도이기 때문입니다. 이 방정식은 예상되는 슈뢰딩거 퍼텐셜, 라그랑지안, 그리고 해밀토니안에 대한 몇 가지 직관적인 표현식을 제공합니다: 단일 경로를 따라 이산적인 엔트로피 생산 (즉, 열의 소산과 관련된 자기정보의 변화)을 생각해 보겠습니다. 이는 (6.9)의 표기법을 사용하여 정의됩니다. 그에 해당하는 기대값은 이산적인 엔트로피 생산이며, 이것은 - (13.1)에 의하면 - 놀라움의 평균 곡률입니다:

$$
\begin{equation}\tag{13.2}
\begin{aligned}
\dot\Im(x,\omega)
  &\triangleq \tfrac 1 \Gamma f\cdot\dot\pi 
   = \tfrac 1 {k_b T} \pmb{\dot q}\\
\dot\Im(x)
  &\triangleq E_{p(\omega}[\dot\Im^q(x,\omega)] 
   = \Gamma\nabla\Im(x) \cdot \nabla\Im(x) \\
\dot H^q
  &\triangleq 
     E_{p(x)}[\dot\Im^q(x)]
   = E_{p(x)}[\Gamma\nabla\Im\cdot\nabla\Im]
   = E_{p(x)}[\Gamma\nabla^2\Im]
\end{aligned}
\end{equation}
$$

즉, 이산적인 엔트로피 생산은 무작위 요동의 진폭과 놀라움 또는 비평형 정상상태 퍼텐셜의 평균 곡률(또는 제곱 그라디언트의 합)과 함께 증가합니다. 차례로 이것은 자유도가 $n$인 시스템(즉, $x\in\R^n$)에 대한 다음과 같은 기대값을 이끌어냅니다:

$$
\begin{equation}\tag{13.3}
\begin{aligned}
V(x)
  &= \tfrac{\hbar}{2}[\tfrac 1 2 \Gamma\nabla\Im \cdot \Gamma\Im - \Gamma\nabla^2\Im] \\
\cal L(x,\dot x)
  &= \tfrac{1}{4\Gamma}(\omega\cdot\omega)-\tfrac 1 2 \Gamma\nabla^2\Im \\
\cal H(x,\dot x)
  &= \tfrac{1}{4\Gamma}(f+\omega)\cdot(f+\omega) - \tfrac 1 \hbar V(x) \\
  \\
\pmb V
  &\triangleq E_{p(x)}[V(x)]
   = -\tfrac \hbar 4 \dot H^q] \\
\pmb{\cal L}
  &\triangleq E_{p(x,\omega)}[\mathcal L (x,\dot x)] 
   = -\tfrac 1 2 [n - \dot H^q] \\
\pmb{\cal H}
  &\triangleq E_{p(x,\omega)}[\mathcal H (x,\dot x)]
   = -\tfrac 1 2 [n + \dot H^q] \\
\end{aligned}
\end{equation}
$$

이러한 표현들은 기대 곡률의 역할을 비평형 정상상태 동력학의 주요 (전역적) 특성화 요소로서 드러냅니다.

## Appendix D: the Fokker-Planck operator - 첨부 D: 포커-프랑크 연산자

포커-플랑크 연산자는 무한 차원 (힐베르트) 공간에서 작동합니다. 이는 즉, 밀도 동력학의 지지 공간입니다. 분명히, 이것은 실용적인 응용에서의 수치 해법에 유용하지 않습니다. 하지만, 이산적인 기저를 사용하여 밀도 동력학을 쉽게 관리할 수 있는 형태로 변환할 수 있습니다. 예를 들어, 정규직교 기저 $\ket{v_i(x)}$를 사용하면, (디랙 표기법을 사용하여):

$$
\begin{equation}\tag{14.1}
\begin{aligned}
\ket{p(x)} 
  &= \textstyle\sum_i\ket{v_i(x)} \varphi_i \\
\braket{v_i|v_k}
  &= \delta_{ik}
\end{aligned}
\end{equation}
$$

이를 통해 연관된 계수 $\varphi_i\in \Complex$의 용어로 밀도 동력학을 표현할 수 있게 됩니다.

$$
\begin{equation}\tag{14.2}
\begin{aligned}
\dot p(x)
  &= \pmb L\ket{p(x)} 
   \Rightarrow \dot\varphi 
   = \lambda \varphi \\
\lambda_{ik}
  &= \braket{v_i|\pmb L|v_k}
\end{aligned}
\end{equation}
$$

계수들은 기저와 관련된 확률 모드의 진폭입니다. 포커-프랑크 연산자의 고유함수인 기저를 자연스럽게 선택하면 밀도 동력학을 일련의 무결접 모드로 분해하고, 중요하게는 거의 순간적으로 소산되는 빠른 모드(즉, 고유값이 $\lambda_{ii}\ll 0$인 고유모드의 계수)를 무시할 수 있습니다.

실제 도전과제는, 예를 들어 날씨 예보에서, 고유모드를 찾는 것입니다(예, Harlim and Yang, 2017; Palmer and Laure, 2013). 대안으로 다항식 기저를 사용하여, 계수를 확률 밀도의 순간으로 표현할 수 있습니다. 이로 인해 밀도 동력학에 대한 저차원 근사법이 생깁니다(예, 순간의 방법). 예를 들어, 첫 번째 두 순간을 유지하는 것은 라플라스 근사에 해당합니다. 이에 대한 예는 우리의 인구 동태에 대한 동적 원인 모델링 작업에서 찾을 수 있습니다(Marreiros et al., 2009). 마지막으로, 푸리에 기저 세트를 사용할 수 있습니다. 이는 확률 진폭으로 해석할 수 있는 (푸리에) 계수를 보장하는 Plancherel 정리에 따라 파동 함수(확률 밀도와 대조적으로)를 분해함으로써 중요한 변화를 가져오는 양자역학적 형식으로 이끌어줍니다.

## Appendix E: generalised motion - 첨부 E: 보편 운동

_"마르코프 프로세스 이론의 기술을 적용하여 얻은 결과는 '대규모' 요동을 특징짓는 범위 내에서만 유용하다"_ (Stratonovich, 1967); p123.

일반적으로, 우리는 무작위 요동이 충분히 빠르기 때문에 그들의 시리얼 혹은 시간적 상관관계를 무시할 수 있다고 가정해왔습니다. 이는 그들의 시간적 도함수의 정밀도가 0이라는 것(또는 존재하지 않는다는 것)을 의미합니다. 그 결과로서, 일반화된 상태의 움직임과 일반화된 상태 자체 사이에 통계적 연결이 없습니다. 그러나, 우리가 일정한 시간적 부드러움(즉, 분석적인)을 가진 무작위 요동을 허용하면, 상황이 바뀝니다. 이 경우, 일반화된 움직임과 상태 사이의 의존성은 (1.1)의 랑주뱅 역학의 일반화된 버전을 초래합니다: 일련의 시간 도함수를 적용하면(일차까지) 다음과 같습니다:

$$
\begin{equation}\tag{14.3}
\begin{aligned}
\begin{rcases}
\dot x
  &= f(x,v)+\omega\\
\dot x^{'}
  &= f\cdot x^{'}+\omega^{'}\\
\dot x^{''}
  &= f\cdot x^{''}+\omega^{''}\\
  &\vdots \\
\end{rcases}
  &\Rightarrow \dot{\vec x}
  = \pmb D\vec x
  = \nabla \pmb f\cdot\vec x + \vec\omega \\
  \\
\vec x
  &\triangleq (x,x^{'},x^{''},\ldots) \\
\nabla f
  &= I \otimes \nabla f
\end{aligned}
\end{equation}
$$

여기서 **D**는 일반화된 상태로부터 일반화된 움직임을 반환하는 블록 행렬 연산자입니다(아래에서 예제를 참조하십시오). 라그랑주와 뉴턴 표기법의 시간 도함수 혼합은 우리가 일반화된 움직임 좌표에서 작업하고 있다는 것을 상기시켜줍니다. 관련된 라그랑지안과 놀라움은 (일차까지) 직관적인 형태를 가집니다:

$$
\begin{equation}\tag{14.4}
\begin{aligned}
\mathcal L(\vec x)
  &= \tfrac 1 2(\tfrac 1 2 \vec x \cdot \pmb M\vec x + \nabla \cdot \pmb f(\vec x))\\
\pmb M
  &= (\pmb D - \nabla \pmb f)\cdot \pmb \Gamma^{-1}(\pmb D-\nabla\pmb f) \\
  \\
\Im(\vec x)
  &= \Im(x) + \Im(\pmb D\vec x|x ) \\
  &= \Im(x) + \mathcal L(\vec x) \\
\end{aligned}
\end{equation}
$$

(일반화된) 라그랑지안이 이 설정에서 (일반화된) 놀라움으로 흡수될 수 있다는 점을 주목하십시오. 일반화된 움직임이 실질적으로 궤적을 설명하기 때문에, 이는 놀라움이 지역 행동이 됨을 의미합니다. 즉, 무작위 요동의 상관 길이 동안의 지역 경로의 놀라움입니다. (14.4)의 라그랑지안은 흐름 기울기와 일반화된 요동의 진폭을 통합하는 *효과적인 질량 행렬* **M**에 대해 표현되었습니다. 이러한 요동의 진폭은 그들의 자기상관 함수의 함수로서, 0의 지연에서 평가됩니다:

$$
\begin{equation}\tag{14.5}
\begin{aligned}
\Gamma 
  &= 
\begin{bmatrix}
  1                      & 0                  & \partial^2_\tau\rho(0) & \cdots \\
  0                      & -\partial^2\rho(0) & 0                      & \space \\
  \partial_\tau^2\rho(0) & 0                  & \partial_\tau^4\rho(0) & \space \\
  \vdots                 & \space             & \space                 & \ddots \\
\end{bmatrix}
   \otimes \Gamma \\
\end{aligned}
\end{equation}
$$

식(14.5)는 확률 과정 이론(Cox and Miller, 1965)의 표준결과에서 나오고 운동의 일반화된 좌표에서의 무작위 요동의 진폭에 따라 시간 상관관계를 정량화할 수 있게 해줍니다. 직관적으로, 무작위 요동이 매우 빠르다고 가정하면, 상관 함수의 곡률 (상관 길이)은 무한대 (0)로 향합니다. 요동이 빠른 한계에서, 우리는 따라서 일반화된 운동의 고차항을 무시할 수 있습니다. 그러므로 (14.3)는 Wiener 가정 (1.1) 하에서 랑주뱅 형식에 귀결됩니다. 그러나 (1.1)과 같이, Delta 함수로 근사화할 수 없는 상관 함수를 수용하고자 한다면, 운동의 일반화된 좌표는 상태 공간을 유용하게 확장하여 계산적으로 그리고 분석적으로 간단한 방식으로 역학을 해결할 수 있게 해줍니다(Friston et al., 2010). 베이지안 필터링의 맥락에서 일반화된 운동의 좌표의 사용은 다음의 보조정리에 의해 특히 유용합니다:

**보조정리** (일반화된 경사 흐름):_일반화된 경사 흐름은 자유 에너지 $F(\vec\mu,b)$의 변형이 외부 상태의 일반화된 운동에 대한 변형 밀도 $q_{\vec\mu}(\vec\mu)=\mathcal N(\sigma(\vec\mu),\Sigma(\vec\mu))$ 에 대해 최소화될 때, 일반화된 내부 상태의 운동이 그들의 일반화된 운동이 된다는 것을 의미합니다:_

$$
\begin{equation}\tag{14.6}
\begin{aligned}
\delta_q F
  &= 0
   \Leftrightarrow \dot{\vec \mu}
   = \pmb D\vec\mu \\
\end{aligned}
\end{equation}
$$

**증명**: 

일반화된 운동 좌표에서, (8.21)은 Helmholtz 분해의 관점에서 표현될 수 있습니다:

$$
\begin{equation}\tag{14.7}
\begin{aligned}
\dot{\vec\mu}
  &= (Q_{\sigma\sigma} - \Gamma_{\sigma\sigma})\cdot\nabla_{\vec\mu}F(\vec\mu,b) \\
  &= \pmb D\vec\mu - \Gamma_{\sigma\sigma}\cdot \nabla_{\vec\mu}F(\vec\mu,b) \\
  \\
\pmb D\vec\mu
  &= Q_{\sigma\sigma}\cdot\nabla_{\vec\mu}F(\vec\mu,b)
   \Rightarrow \nabla_{\vec\mu}\cdot\pmb D\vec\mu = 0 \\
\vec\mu
  &= (\pmb \mu(b), \pmb \mu^{'}(b),\pmb \mu^{''}(b),\ldots)\\
\end{aligned}
\end{equation}
$$

일반화된 운동 좌표에서, 소용돌이 흐름은 **D** 라는 발산 없는 연산자(divergence-free operator)로 나타낼 수 있습니다. 이 연산자는 일반화된 시간 미분 연산자 역할을 합니다. 이 설정에서 가장 가능성이 높은 내부 상태 경로는 변분 자유 에너지를 최소화하고 일반화된 내부 상태의 운동을 (발산 없는) 일반화된 운동으로 만듭니다.

$$
\begin{equation}\tag{14.8}
\begin{aligned}
\dot{\vec\mu}
  &= \pmb D\vec\mu
   \Leftrightarrow \nabla_{\vec\mu}F(\vec\mu,b) = 0
   \Leftrightarrow \delta_q F = 0\\
\end{aligned}
\end{equation}
$$

주어진 식(14.6).

**참고**: 간단히 말해서, 일반화된 운동 $D_{\vec\mu}$는 일반화된 운동 좌표에서 보존적이고 발산 없는 흐름에 해당합니다. 직관적으로, 이것은 일반화된 운동과 함께 움직이는 기준 프레임에서 운동을 경사 흐름으로 보여줍니다.

$$
\begin{equation}\tag{14.9}
\begin{aligned}
\pmb D\vec\mu - \dot{\vec\mu}
  &= \Gamma_{\sigma\sigma}\nabla_{\vec\mu}F(\vec\mu,b)\\
\end{aligned}
\end{equation}
$$

이것은 아마도 가장 일반적이고 간결한 형태의 (일반화된 또는 변분) 베이즈 필터일 것입니다. 적절한 (계측) 변환을 선택하면 확장된 칼만-부시 필터(Friston et al., 2014)와 같은 표준 필터링 방식을 복구할 수 있습니다:

$$
\begin{equation}\tag{14.10}
\begin{aligned}
\pmb D
  &=
\begin{bmatrix}
  0 & I \\
  0 & 0 \\
\end{bmatrix},\space\space 
\vec \mu
   = (\pmb \mu(b), \mu^{'}(b))\\
\end{aligned}
\end{equation}
$$

These classical schemes generally limit generalised motion to first order.

## Appendix F: discrete state-space models - 첨부 F: 이산 상태공간 모형

계속된 상태 공간 형식에서, 기대 자유 에너지는 미래의 자율 상태와 관련된 최종 상태에 대한 예측 밀도의 함수입니다. 이산 상태 공간 형식에서, 대응하는 기대 자유 에너지는 정책의 각 시퀀스에 대한 요소가 있는 벡터가 됩니다. (즉, 정책). 그 파생은 동일한 기본 논증을 따릅니다. 그러나 기대 자유 에너지 한계는 밀도(분포)가 아닌 확률 분포의 엔트로피의 비음의(양의) 특성에서 직접 도출되며, Jensen의 불평등 대신에 도출됩니다.

**보조정리** (기대 자유 에너지 – 이산):*초기 상태 $\pi_0$ 를 가지는 $i$번째 정책 $\alpha^i=(\alpha_1^i,\ldots,\alpha_\tau^i)$의 사전 놀라움 $\Im(\alpha^i|\pi_0)$은 위험과 모호함을 포함하는 기대 자유 에너지로 상한됩니다:*
 
$$
\begin{equation}\tag{15.1}
\begin{aligned}
G(\alpha^i)
  &=
    \underbrace{
      D[Q_i(\eta_\tau|\alpha^i)||P(\eta_\tau|\alpha^i)]
    }_{Risk}
   +
    \underbrace{
      E_{Q_i}[\Im(s_\tau|\eta_\tau)]
    }_{Ambiguit}
   + \Im(\alpha^i)
   \geq \Im(\alpha^i|\pi_0)
\end{aligned}
\end{equation}
$$

*예측 밀도는 현재(특정) 상태 $\pi_0$를 기준으로 변분 밀도에 따라 정의됩니다:*

$$
\begin{equation}\tag{15.2}
\begin{aligned}
Q_i(s_\tau,\eta_\tau,\alpha^i)
  &\triangleq Q_i(s_\tau|\eta_\tau)Q_i(\eta_\tau|\alpha^i)P(\alpha^i|\pi_0)\\
Q_i(\eta_\tau|alpha^i)
  &\triangleq P(\eta_\tau|\alpha^i,\pi_0)
   = \textstyle\sum_{\eta_0} Q_\mu(\eta_0)P(\eta_\tau|\alpha^i,\pi_0,\eta_0)\\
Q_\mu(\eta_0)
  &= P(\eta_0 | \pi_0) \\
\end{aligned}
\end{equation}
$$

*여기서,* $\space Q_i(s_\tau|\eta_\tau)=P(s_\tau|\eta_\tau)=P(s_\tau|\eta_\tau,\alpha)$.

**증명**: 예측 분포(결과, 상태 및 정책에 대해)와 생성 모델에 해당하는 사전 분포(즉, 비평형 정상상태 분포)의 거리는 0보다 커야 합니다.

$$
\begin{equation}\tag{15.3}
\begin{aligned}
D[Q||P]
  &= E_Q[\pmb G(\alpha)-\Im(\alpha|\pi_0] \geq 0\\
\pmb G(\alpha^i)
  &= G(\alpha^i) - H[Q_i(s_\tau|\eta_\tau)] \\
G(\alpha^i)
  &=  E_{Q_i}[\Im(\eta_\tau,s_\tau,\alpha^i)]-H[Q_i(\eta_\tau|\alpha^i)]\\
  \\
Q_i
  &\triangleq Q_i(\eta_\tau,s_\tau,\alpha^i) \\
P_i
  &\triangleq P_i(\eta_\tau,s_\tau,\alpha^i) \\
\end{aligned}
\end{equation}
$$

예측 분포가 비평형 정상상태(즉, 사전 분포)로 수렴하면, 특정 정책의 기대 자유 에너지는 그것의 놀라움의 상한이어야 합니다.

$$
\begin{equation}\tag{15.4}
\begin{aligned}
D[Q||P]
  &= 0
   \Rightarrow \pmb G(\alpha) = \Im(\alpha|\pi_0) \\
  &\Rightarrow G(\alpha^i) = \Im(\alpha^i|\pi_0) + H[Q_i(s_\tau|\eta_\tau)]\\
  &\Rightarrow G(\alpha^i) = \Im(\alpha^i|\pi_0)\\
\end{aligned}
\end{equation}
$$

마지막 부방정식은 이산 상태에 대한 분포의 조건부 엔트로피가 0보다 작을 수 없기 때문입니다. 따라서 수렴 시에 기대 자유 에너지는 경로의 놀라움(15.1)에 대한 상한을 제공하며, 모호함이 없을 때는 동일합니다.

**참고**: 위험이 최소화되면 – 예측 분포가 사전 분포 $Q_i\approx P(\eta_\tau,s_\tau|\alpha^i)$ – 에 수렴하면 – 기대 자유 에너지는 지적 가치와 도구적 가치의 혼합이 됩니다. 즉, 정보 획득과 기대 로그의 증거입니다. (15.1)에서 위험이 없을 때:

$$
\begin{equation}\tag{15.5}
\begin{aligned}
G(\alpha^i)
  &= E_{Q_i}[\Im(s_\tau|\eta_\tau)] + \Im(\alpha^i)\\
  &= E_{Q_i}[\Im(s_\tau|\eta_\tau,\alpha^i) + \Im(\alpha^i)] \\
  &= E_{Q_i}[\ln P(\eta_\tau|\alpha^i) - \ln P(\eta_\tau|s_\tau,\alpha^i) - \ln P(s_\tau,\alpha^i)] \\
  &= E_{Q_i}
    [-
     \underbrace{
       D[P(\eta_\tau|s_\tau,\alpha^i)|P(\eta_\tau|\alpha^i)]
     }_{\text{epistemic value}}
     -
     \underbrace{
       ln P(s_\tau,\alpha^i)
     }_{\text{instrumental value}}
   ] \\
\end{aligned}
\end{equation}
$$

이것은 정보 획득 또는 주의력 측면에서 모호함의 대안적인 공식으로 간주될 수 있습니다.

소프트웨어 참고: 이 모노그래프에 설명된 시뮬레이션은 http://www.fil.ion.ucl.ac.uk/spm/software/ 에서 제공되는 학술 소프트웨어를 사용하여 재현할 수 있습니다. Matlab 프롬프트에서 DEM을 입력하면 그래픽 사용자 인터페이스가 호출됩니다. 위의 시뮬레이션은 A physics of life 버튼을 선택하여 재현할 수 있습니다. 이렇게 하면 사용자는 코드와 서브루틴을 검사하고 자신의 재량에 따라 사용자 지정할 수 있습니다.

감사의 말: 이 모노그래프를 작성할 당시 KF는 Wellcome Principal Research Fellow (Ref: 088130/Z/09/Z)였습니다. 이 모노그래프에 설명된 아이디어에 기여한 수십 명의 친구와 동료들이 있습니다. 토마스 파(Thomas Parr)를 명시적으로 언급하겠습니다. 토마스는 이 책을 쓰는 동안 저의 박사 과정 학생이었고 능동 추론 공식화에 실질적인 기여를 했습니다. 또한 그는 저희 런던 동료들을 위해 모노그래프의 공식적인 논쟁과 감독을 해부하는 귀중한 주간 세미나를 준비했습니다: https://www.fil.ion.ucl.ac.uk/~tparr/Physics/Slides%20Stochastic%20dynamics.htm
## Appendix G: Glossary of terms and expressions - 첨부 G: 용어 및 표현어 주석

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

## Apendix H: Translation Glossory - 첨부 H: 번역 용어

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

>  [한국물리학회 물리학용어집](https://www.kps.or.kr/content/voca/search.php) \
>  [대한수학회 수학용어](https://www.kms.or.kr/mathdict/list.html) \
>  [Google Bard](https://bard.google.com/?hl=kr)\
>  [ChatGPT](https://chat.openai.com/?model=gpt-4-browsing)


## References - 참고자료

Adams, R.A., Shipp, S., Friston, K.J., 2013. Predictions not commands: active inference in the motor system. Brain Struct Funct. 218, 611-643.\
Agarwal, S., Wettlaufer, J.S., 2016. Maximal stochastic transport in the Lorenz equations. Physics Letters A 380, 142-146.\
Alhambra, A.M., Masanes, L., Oppenheim, J., Perry, C., 2016a. Fluctuating Work: From Quantum Thermodynamical Identities to a Second Law Equality. Physical Review X 6.\
Alhambra, A.M., Oppenheim, J., Perry, C., 2016b. Fluctuating States: What is the Probability of a Thermodynamical Transition? Physical Review X 6.\
Amari, S., 1998. Natural gradient works efficiently in learning. Neural Computation 10, 251-276.\
Ao, P., 2004. Potential in stochastic differential equations: novel construction. J Phys. A: Math Gen. 37, L25–30.\
Ao, P., 2008. Emerging of Stochastic Dynamical Equalities and Steady State Thermodynamics. Commun. Theor. Phys. (Beijing, China) 49, 1073-1090.\
Arnold, L., 2003. Random Dynamical Systems (Springer Monographs in Mathematics). Springer- Verlag, Berlin.\
Arsenović, D., Burić, N., Davidović, D.M., Prvanović, S., 2014. Lagrangian form of Schrödinger equation. Foundations of Physics 44, 725-735.\
Ashby, W.R., 1947. Principles of the self-organizing dynamic system. J Gen Psychology. 37, 125-128.\
Attias, H., 2003. Planning by Probabilistic Inference, Proc. of the 9th Int. Workshop on Artificial Intelligence and Statistics.\
Ay, N., 2015. Information Geometry on Complexity and Stochastic Interaction. Entropy 17, 2432.\
Ayala, F., Dobzhansky, T., 1974. Studies in the philosophy of biology: reduction and related problems. University of California Press, Berkeley and Los Angeles.\
Bak, P., Tang, C., Wiesenfeld, K., 1987. Self-organized criticality: an explanation of 1/f noise. Phys Rev Lett. 59, 381–384.\
Bak, P., Tang, C., Wiesenfeld, K., 1988. Self-organized criticality. Physical review. A, General physics 38, 364-374.\
Balleine, B.W., Dickinson, A., 1998. Goal-directed instrumental action: contingency and incentive learning and their cortical substrates. Neuropharmacology 37, 407-419.\
Ballentine, L.E., 1970. The Statistical Interpretation of Quantum Mechanics. Reviews of Modern Physics 42, 358-381.\
Baranes, A., Oudeyer, P.Y., 2009. R-IAC: Robust Intrinsically Motivated Exploration and Active Learning. Ieee Transactions on Autonomous Mental Development 1, 155-169.\
Barlow, H., 1961. Possible principles underlying the transformations of sensory messages, in: Rosenblith, W. (Ed.), Sensory Communication. MIT Press, Cambridge, MA, pp. 217-234.\
Barlow, H.B., 1974. Inductive inference, coding, perception, and language. Perception 3, 123-134.\
Barreto, E., Josic, K., Morales, C.J., Sander, E., So, P., 2003. The geometry of chaos synchronization. Chaos 13, 151-164.\
Barrow, J.D., Tipler, F.J., Wheeler, J.A., 2015. The anthropic cosmological principle. Oxford University Press, Oxford; New York.\
Bastos, A.M., Usrey, W.M., Adams, R.A., Mangun, G.R., Fries, P., Friston, K.J., 2012. Canonical microcircuits for predictive coding. Neuron 76, 695-711.\
Batterman, R.W., 2001. The devil in the details: Asymptotic reasoning in explanation, reduction, and emergence. Oxford University Press.\
Beal, M.J., 2003. Variational Algorithms for Approximate Bayesian Inference. PhD. Thesis, University College London.\
Bechtel, W., Richardson, R.C., 2010. Discovering complexity: Decomposition and localization as strategies in scientific research. MIT press.\
Bedau, M., 2002. Downward causation and the autonomy of weak emergence. Principia: an international journal of epistemology 6, 5-50.\
Bedau, M.A., Humphreys, P.E., 2008. Emergence: Contemporary readings in philosophy and science. MIT press.\
Beggs, J.M., Plenz, D., 2003. Neuronal avalanches in neocortical circuits. J Neurosci. 23, 11167-11177.\
Belousov, B.P., 1959. "Периодически действующая реакция и ее механизм [Periodically acting reaction and its mechanism]. Сборнрефератов по радиационной медицине [Collection of Abstracts on Radiation Medicine], 145-147.\
Bennett, C.H., 2003. Notes on Landauer's principle, reversible computation, and Maxwell's Demon. Studies in History and Philosophy of Science Part B: Studies in History and Philosophy of Modern Physics 34, 501-510.\
Berlyne, D.E., 1950. Novelty and curiosity as determinants of explanatory behaviour. British Journal of Psychology-General Section 41, 68-80.\
Bernard, C., 1974. Lectures on the phenomena common to animals and plants. Charles C Thomas, Springfield, IL.\
Bialek, W., Nemenman, I., Tishby, N., 2001. Predictability, complexity, and learning. Neural Computat. 13, 2409-2463.\
Birkhoff, G.D., 1927. Dynamical systems. American Mathematical Society, New York.\
Boccaletti, S., Kurths, J., Osipov, G., Valladares, D.L., Zhou, C.S., 2002. The synchronization of chaotic systems. Physics Reports-Review Section of Physics Letters 366, 1-101.\
Bohm, D., 1952. A Suggested Interpretation of the Quantum Theory in Terms of "Hidden" Variables. I. Physical Review 85, 166-179.\
Botvinick, M., Toussaint, M., 2012. Planning as inference. Trends Cogn Sci. 16, 485-488.\
Breakspear, M., Heitmann, S., Daffertshofer, A., 2010. Generative Models of Cortical Oscillations: Neurobiological Implications of the Kuramoto Model. Frontiers in Human Neuroscience 4.\
Breakspear, M., Stam, C.J., 2005. Dynamics of a neural system with a multiscale architecture. Philos Trans R Soc Lond B Biol Sci. 360, 1051-1074.\
Bressloff, P.C., Newby, J.M., 2013. Stochastic models of intracellular transport. Reviews of Modern Physics 85, 135-196.\
Bridgman, P.W., 1954. Remarks on the Present State of Operationalism. Scientific Monthly 79, 224- 226.\
Brookes, J.C., 2017. Quantum effects in biology: golden rule in enzymes, olfaction, photosynthesis and magnetodetection. Proceedings. Mathematical, physical, and engineering sciences 473, 20160822.\
Bruineberg, J., Rietveld, E., 2014. Self-organization, free energy minimization, and optimal grip on a field of affordances. Frontiers in Human Neuroscience 8, 599.\
Burgess, N., Barry, C., O'Keefe, J., 2007. An oscillatory interference model of grid cell firing. Hippocampus 17, 801-812.\
Buzsaki, G., 1998. Memory consolidation during sleep: a neurophysiological perspective. Journal of sleep research 7 Suppl 1, 17-23.\
Buzsaki, G., Moser, E.I., 2013. Memory, navigation and theta rhythm in the hippocampal-entorhinal system. Nature Neuroscience 16, 130-138.\
Calvo, P., Friston, K., 2017. Predicting green: really radical (plant) predictive processing. Journal of The Royal Society Interface 14.\
Campbell, D.T., 1974. ‘Downward causation’in hierarchically organised biological systems, Studies in the Philosophy of Biology. Springer, pp. 179-186.\
Capozziello, S., De Laurentis, M., 2011. Extended Theories of Gravity. Physics Reports-Review Section of Physics Letters 509, 167-320.\
Cardy, J.L., 2015. Scaling and renormalization in statistical physics.\
Carr, J., 1981. Applications of Centre Manifold Theory. Springer-Verlag, Berlin.\
Caticha, A., 2015a. The basics of information geometry. AIP Conference Proceedings 1641, 15-26. Caticha, A., 2015b. Entropic Dynamics. Entropy 17, 6110.\
Cessac, B., Blanchard, P., Krüger, T., 2001. Lyapunov exponents and transport in the Zhang model of Self-Organized Criticality. Phys Rev E Stat Nonlin Soft Matter Phys. 64, 016133.\
Clark, A., 2017. How to Knit Your Own markov blanket, in: Metzinger, T.K., Wiese, W. (Eds.), Philosophy and Predictive Processing. MIND Group, Frankfurt am Main.\
Clarke, S.E., Longtin, A., Maler, L., 2015. Contrast coding in the electrosensory system: parallels with visual computation. Nat Rev Neurosci 16, 733-744.\
Conant, R.C., Ashby, W.R., 1970. Every Good Regulator of a system must be a model of that system. Int. J. Systems Sci. 1, 89-97.\
Constant, A., Ramstead, M.J.D., Veissiere, S.P.L., Campbell, J.O., Friston, K.J., 2018. A variational approach to niche construction. J R Soc Interface 15.\
Cook, A., 1994. The observational foundations of physics. Cambridge University Press, Cambridge. Cox, D.R., Miller, H.D., 1965. The theory of stochastic processes. Methuen, London.\
Crauel, H., 1999. Global random attractors are uniquely determined by attracting deterministic compact sets. Ann. Mat. Pura Appl. 4, 57-72.\
Crauel, H., Debussche, A., Flandoli, F., 1997. Random attractors. Journal of Dynamics and Differential Equations 9, 307-341.\
Crauel, H., Flandoli, F., 1994. Attractors for random dynamical systems. Probab Theory Relat Fields 100, 365-393.\
Craver, C.F., Bechtel, W., 2007. Top-down causation without top-down causes. Biology & Philosophy 22, 547-563.\
Crooks, G.E., 2007. Measuring thermodynamic length. Phys Rev Lett 99, 100602.\
Cugliandolo, L.F., Lecomte, V., 2017. Rules of calculus in the path integral representation of white noise Langevin equations: the Onsager–Machlup approach. Journal of Physics A: Mathematical and Theoretical 50, 345001.\
D'Alessio, L., Kafri, Y., Polkovnikov, A., Rigol, M., 2016. From quantum chaos and eigenstate thermalization to statistical mechanics and thermodynamics. Advances in Physics 65, 239-362.\
Dauwels, J., 2007. On Variational Message Passing on Factor Graphs, 2007 IEEE International Symposium on Information Theory, pp. 2546-2550.\
Davis, M.J., 2006. Low-dimensional manifolds in reaction-diffusion equations. 1. Fundamental aspects. J Phys Chem A. 110, 5235-5256.\
Demirdjian, D., Taycher, L., Shakhnarovich, G., Grauman, K., Darrell, T., Ieee Computer, S.O.C., 2005. Avoiding the "streetlight effect": Tracking by exploring likelihood modes, Tenth Ieee International Conference on Computer Vision, Vols 1 and 2, Proceedings, pp. 357-364.\
Deyle, E.R., Sugihara, G., 2011. Generalized Theorems for Nonlinear State Space Reconstruction. PLOS ONE 6, e18295.\
Dezfouli, A., Balleine, B.W., 2013. Actions, action sequences and habits: evidence that goal-directed and habitual action control are hierarchically organized. PLoS Comput Biol 9, e1003364.\
Dolan, R.J., Dayan, P., 2013. Goals and habits in the brain. Neuron 80, 312-325.\
Einstein, A., 2013. Principle of Relativity. Dover Publications.\
England, J.L., 2015. Dissipative adaptation in driven self-assembly. Nature nanotechnology 10, 919- 923.\
Esposito, M., Harbola, U., Mukamel, S., 2009. Nonequilibrium fluctuations, fluctuation theorems, and counting statistics in quantum systems. Reviews of Modern Physics 81, 1665-1702.\
Evans, D.J., Searles, D.J., 2002. The fluctuation theorem. Advances in Physics 51, 1529-1585. Feynman, R.P., 1948. Space-Time Approach to Non-Relativistic Quantum Mechanics. Reviews of Modern Physics 20, 367-387.\
Feynman, R.P., 1972. Statistical mechanics. Benjamin, Reading MA.\
Fierro, A., Franzese, G., de Candia, A., Coniglio, A., 1999. Percolation transition and the onset of nonexponential relaxation in fully frustrated models. Physical Review E 59, 60-66.\
FitzGerald, T.H., Schwartenbeck, P., Moutoussis, M., Dolan, R.J., Friston, K., 2015. Active inference, evidence accumulation, and the urn task. Neural Comput 27, 306-328.\
Fleming, W.H., Sheu, S.J., 2002. Risk-sensitive control and an optimal investment model II. Ann. Appl. Probab. 12, 730-767.\
Fox, C., Roberts, S., 2011. A tutorial on variational Bayes. Artificial Intelligence Review 38, 1-11.\
Frank, T.D., 2004. Nonlinear Fokker-Planck Equations: Fundamentals and Applications. Springer Series in Synergetics. Springer, Berlin.\
Freeman, W.J., 1994. Characterization of state transitions in spatially distributed, chaotic, nonlinear, dynamical systems in cerebral cortex. Integr Physiol Behav Sci. 29, 294-306.\
Freeman, W.J., 1995. The kiss of chaos and the sleeping beauty of psychology, in: Abraham, F.D., Gilgen, A.R. (Eds.), Chaos theory in psychology. Praeger Publishers/Greenwood Publishing Group, Westport, CT, pp. 19-29.\
Friston, K., 2013. Life as we know it. J R Soc Interface 10, 20130475.\
Friston, K., Adams, R.A., Perrinet, L., Breakspear, M., 2012. Perceptions as hypotheses: saccades as experiments. Front Psychol. 3, 151.\
Friston, K., Ao, P., 2012. Free energy, value, and attractors. Comput Math Methods Med 2012, 937860.\
Friston, K., FitzGerald, T., Rigoli, F., Schwartenbeck, P., Pezzulo, G., 2017a. Active Inference: A Process Theory. Neural Comput 29, 1-49.\
Friston, K., Frith, C., 2015. A Duet for one. Conscious Cogn 36, 390-405.\
Friston, K., Kilner, J., Harrison, L., 2006. A free energy principle for the brain. Journal of physiology, Paris 100, 70-87.\
Friston, K., Levin, M., Sengupta, B., Pezzulo, G., 2015a. Knowing one's place: a free-energy approach to pattern regulation. J R Soc Interface 12.\
Friston, K., Mattout, J., Kilner, J., 2011. Action understanding and active inference. Biol Cybern. 104, 137–160.\
Friston, K., Mattout, J., Trujillo-Barreto, N., Ashburner, J., Penny, W., 2007. Variational free energy and the Laplace approximation. NeuroImage 34, 220-234.\
Friston, K., Rigoli, F., Ognibene, D., Mathys, C., Fitzgerald, T., Pezzulo, G., 2015b. Active inference and epistemic value. Cogn Neurosci 6, 187-214.\
Friston, K., Sengupta, B., Auletta, G., 2014. Cognitive Dynamics: From Attractors to Active Inference. Proceedings of the IEEE 102, 427-445.\
Friston, K., Stephan, K., Li, B., Daunizeau, J., 2010. Generalised Filtering. Mathematical Problems in Engineering vol., 2010, 621670.\
Friston, K.J., Lin, M., Frith, C.D., Pezzulo, G., Hobson, J.A., Ondobaka, S., 2017b. Active Inference, Curiosity and Insight. Neural Comput 29, 2633-2683.\
Friston, K.J., Parr, T., de Vries, B., 2017c. The graphical brain: Belief propagation and active inference. Network Neuroscience 0, 1-34.\
Friston, K.J., Rosch, R., Parr, T., Price, C., Bowman, H., 2017d. Deep temporal models and active inference. Neuroscience and biobehavioral reviews 77, 388-402.\
Fuster, J.M., 2004. Upper processing stages of the perception-action cycle. Trends Cogn Sci. 8, 143- 145.\
Gallese, V., Goldman, A., 1998. Mirror neurons and the simulation theory of mind-reading. Trends in Cognitive Sciences 2, 493-501.\
Garriga, J., Vilenkin, A., 2001. Many worlds in one. Physical Review D 64.\
Gershman, S.J., Daw, N.D., 2017. Reinforcement Learning and Episodic Memory in Humans and Animals: An Integrative Framework. Annual review of psychology 68, 101-128.\
Ginzburg, V.L., 1987. Solitons and instantons, operator quantization. Nova Science Publishers, Commack, N.Y.\
Giraud, A.L., Poeppel, D., 2012. Cortical oscillations and speech processing: emerging computational principles and operations. Nat Neurosci 15, 511-517.\
Goldstone, J., Salam, A., Weinberg, S., 1962. Broken Symmetries. Physical Review 127, 965-970.\
Goold, J., Huber, M., Riera, A., Rio, L.d., Skrzypczyk, P., 2016. The role of quantum information in thermodynamics—a topical review. Journal of Physics A: Mathematical and Theoretical 49, 143001.\
Haken, H., 1983. Synergetics: an introduction. Non-equilibrium phase transition and self- selforganisation in physics, chemistry and biology. Springer-Verlag, Berlin.\
Harlim, J., Yang, H., 2017. Diffusion Forecasting Model with Basis Functions from QR- Decomposition. Journal of Nonlinear Science.\
Helgaker, T., Jorgensen, P., Olsen, J., 2014. Molecular electronic-structure theory. John Wiley & Sons.\
Helmholtz, H., 1866/1962. Concerning the perceptions in general, Treatise on physiological optics, vol. III. Dover, New York.\
Helmholtz, H., 1878 (1971). The Facts of Perception, in: Middletown, R.K. (Ed.), The Selected Writings of Hermann von Helmholtz. Wesleyan University Press, Connecticut, p. 384.\
Hinton, G.E., Zemel, R.S., 1993. Autoencoders, minimum description length and Helmholtz free energy, Proceedings of the 6th International Conference on Neural Information Processing Systems. Morgan Kaufmann Publishers Inc., Denver, Colorado, pp. 3-10.\
Hohwy, J., 2016. The Self-Evidencing Brain. Noûs 50, 259-285.\
Holmes, Z., Weidt, S., Jennings, D., Anders, J., Mintert, F., 2019. Coherent fluctuation relations: from the abstract to the concrete. Quantum-Austria 3.\
Hu, A., Xu, Z., Guo, L., 2010. The existence of generalized synchronization of chaotic systems in complex networks. Chaos 20, 013112.\
Hunt, B., Ott, E., Yorke, J., 1997. Differentiable synchronisation of chaos. Phys Rev E 55, 4029-4034. \
Hutter, M., 2006. Universal Artificial Intellegence : Sequential Decisions Based on Algorithmic Probability. Springer-Verlag Berlin and Heidelberg & Co. KG, Dordrecht.\
Itti, L., Baldi, P., 2009. Bayesian Surprise Attracts Human Attention. Vision Res. 49, 1295-1306. Jarzynski, C., 1997. Nonequilibrium Equality for Free Energy Differences. Physical Review Letters 78, 2690-2693.\
Jaynes, E.T., 1957. Information Theory and Statistical Mechanics. Physical Review Series II 106, 620– 630.\
Jensen, O., Gips, B., Bergmann, T.O., Bonnefond, M., 2014. Temporal coding organized by coupled alpha and gamma oscillations prioritize visual processing. Trends Neurosci 37, 357-369.\
Jones, D.S., 1979. Elementary information theory. Clarendon Press, Oxford.\
Kaluza, P., Meyer-Ortmanns, H., 2010. On the role of frustration in excitable systems. Chaos 20, 043111.\
Kappen, H.J., 2005. Path integrals and symmetry breaking for optimal control theory. Journal of Statistical Mechanics: Theory and Experiment 11, P11011.\
Kappen, H.J., Gomez, Y., Opper, M., 2012. Optimal control as a graphical model inference problem. Machine learning 87, 159-182.\
Kauffman, S.A., Johnsen, S., 1991. Coevolution to the edge of chaos: coupled fitness landscapes, poised states, and coevolutionary avalanches. Journal of theoretical biology 149, 467-505.\
Kayser, C., Ermentrout, B., 2010. Complex times for earthquakes, stocks, and the brain's activity. Neuron 66, 329-331.\
Keber, F.C., Loiseau, E., Sanchez, T., DeCamp, S.J., Giomi, L., Bowick, M.J., Marchetti, M.C., Dogic, Z., Bausch, A.R., 2014. Topology and dynamics of active nematic vesicles. Science 345, 1135-1139.\
Kerr, W.C., Graham, A.J., 2000. Generalized phase space version of Langevin equations and associated Fokker-Planck equations. European Physical Journal B 15, 305-311.\
Khadka, U., Holubec, V., Yang, H., Cichos, F., 2018. Active particles bound by information flows. Nature Communications 9, 3864.\
Kilner, J.M., Friston, K.J., Frith, C.D., 2007. Predictive coding: an account of the mirror neuron system. Cognitive processing 8, 159-166.\
Kim, E.-j., 2018. Investigating Information Geometry in Classical and Quantum Systems through Information Length. Entropy 20, 574.\
Kim, J., 1999. Making sense of emergence. Philosophical studies 95, 3-36.\
Kleeman, R., 2014. A Path Integral Formalism for Non-equilibrium Hamiltonian Statistical Systems. Journal of Statistical Physics 158, 1271-1297.\
Knill, D.C., Pouget, A., 2004. The Bayesian brain: the role of uncertainty in neural coding and computation. Trends Neurosci. 27, 712-719.\
Koide, T., 2017. Perturbative expansion of irreversible work in Fokker–Planck equation à la quantum mechanics. Journal of Physics A: Mathematical and Theoretical 50, 325001.\
Kwapien, J., Drozdz, S., 2012. Physical approach to complex systems. Physics Reports-Review Section of Physics Letters 515, 115-226.\
Landauer, R., 1961. Irreversibility and Heat Generation in the Computing Process. IBM Journal of Research and Development 5, 183-191.\
LeCun, Y., Bengio, Y., Hinton, G., 2015. Deep learning. Nature 521, 436-444.\
Lin, H.W., Tegmark, M., Rolnick, D., 2017. Why Does Deep and Cheap Learning Work So Well? Journal of Statistical Physics 168, 1223-1247.\
Linsker, R., 1990. Perceptual neural organization: some approaches based on network models and information theory. Annu Rev Neurosci. 13, 257-281.\
Lisman, J., 2012. Excitation, inhibition, local oscillations, or large-scale loops: what causes the symptoms of schizophrenia? Curr Opin Neurobiol. 22, 537-544.\
Littlejohn, R.G., Reinsch, M., 1997. Gauge fields in the separation of rotations and internal motions in the n-body problem. Reviews of Modern Physics 69, 213-275.\
Lopes da Silva, F., 1991. Neural mechanisms underlying brain waves: from neural membranes to networks. Electroencephalography and Clinical Neurophysiology 79, 81-93.\
Lorenz, E.N., 1963. Deterministic nonperiodic flow. J Atmos Sci. 20, 130-141.\
Lyapunov, A.M., Fuller, A.T., 1992. The general problem of the stability of motion. Taylor & Francis, London.\
MacKay, D.J., 1995. Free-energy minimisation algorithm for decoding and cryptoanalysis. Electronics Letters 31, 445-447.\
Marreiros, A.C., Kiebel, S.J., Daunizeau, J., Harrison, L.M., Friston, K.J., 2009. Population dynamics under the Laplace assumption. Neuroimage 44, 701-714.\
Matsuda, H., 2000. Physical nature of higher-order mutual information: intrinsic correlations and frustration. Physical review. E, Statistical physics, plasmas, fluids, and related interdisciplinary topics 62, 3096-3102.\
Matta, C.F., Massa, L., 2017. Notes on The Energy Equivalence of Information. The journal of physical chemistry. A 121, 9131-9135.\
Maturana, H.R., Varela, F., 1980. Autopoiesis: the organization of the living, in: Maturana HR, V.F. (Ed.), Autopoiesis and Cognition. Reidel, Dordrecht, Netherlands.\
Mirza, M.B., Adams, R.A., Mathys, C.D., Friston, K.J., 2016. Scene Construction, Visual Foraging, and Active Inference. Frontiers in computational neuroscience 10, 56.\
Modi, M.E., Sahin, M., 2017. Translational use of event-related potentials to assess circuit integrity in ASD. Nat Rev Neurol 13, 160-170.\
Nagel, E., 1961. The Structure of Science. Harcourt, Brace and World., New York.\
Namikawa, J., 2005. Chaotic itinerancy and power-law residence time distribution in stochastic dynamical systems. Phys. Rev. E 72, 026204.\
Nara, S., 2003. Can potentially useful dynamics to solve complex problems emerge from constrained chaos and/or chaotic itinerancy? Chaos 13, 1110-1121.\
Newman, M.E.J., 2005. Power laws, Pareto distributions and Zipf's law. Contemporary Physics 46, 323-351.\
Nicolis, G., Prigogine, I., 1977. Self-organization in non-equilibrium systems. John Wiley, New York.\
Oudeyer, P.-Y., Kaplan, F., 2007. What is intrinsic motivation? a typology of computational approaches. Frontiers in Neurorobotics 1, 6.\
Ovchinnikov, I., 2016. Introduction to Supersymmetric Theory of Stochastics. Entropy 18, 108.\
Palacios, E.R., Razi, A., Parr, T., Kirchhoff, M., Friston, K., 2017. Biological Self-organisation and markov blankets. bioRxiv.\
Palmer, T.N., Laure, Z., 2013. Singular vectors, predictability and ensemble forecasting for weather and climate. Journal of Physics A: Mathematical and Theoretical 46, 254018.\
Parisi, G., Sourlas, N., 1982. Supersymmetric field theories and stochastic differential equations. Nuclear Physics B 206, 321-332.\
Parrondo, J.M.R., Horowitz, J.M., Sagawa, T., 2015. Thermodynamics of information. Nature Physics 11, 131-139.\
Pavlos, G.P., Karakatsanis, L.P., Xenakis, M.N., 2012. Tsallis non-extensive statistics, intermittent turbulence, SOC and chaos in the solar plasma, Part one: Sunspot dynamics. Physica A: Statistical Mechanics and its Applications 391, 6287-6319.\
Pearl, J., 1988. Probabilistic Reasoning In Intelligent Systems: Networks of Plausible Inference. Morgan Kaufmann, San Fransisco, CA, USA.\
Penny, W.D., Stephan, K.E., Mechelli, A., Friston, K.J., 2004. Comparing dynamic causal models. Neuroimage 22, 1157-1172.\
Plenz, D., Thiagarajan, T.C., 2007. The organizing principles of neuronal avalanches: cell assemblies in the cortex? Trends Neurosci. 30, 101-110.\
Poland, D., 1993. Cooperative catalysis and chemical chaos: a chemical model for the Lorenz equations. Physica D 65 86–99.\
Prigogine, I., 1978. Time, Structure, and Fluctuations. Science 201, 777-785.\
Proust, J., 2015. The philosophy of metacognition mental agency and self-awareness. Oxford University Press, Oxford.\
Pyragas, K., 1997. Conditional Lyapunov exponents from time series. Physical Review E 56, 5183- 5187.\
Ramaswamy, S., 2010. The Mechanics and Statistics of Active Matter, in: Langer, J.S. (Ed.), Annual Review of Condensed Matter Physics, Vol 1, vol. 1, pp. 323-345.\
Ramsay, D.S., Woods, S.C., 2014. Clarifying the Roles of Homeostasis and Allostasis in Physiological Regulation. Psychological review 121, 225-247.\
Ramstead, M.J.D., Badcock, P.B., Friston, K.J., 2017. Answering Schrodinger's question: A free-energy formulation. Phys Life Rev.\
Rao, R.P., Ballard, D.H., 1999. Predictive coding in the visual cortex: a functional interpretation of some extra-classical receptive-field effects. Nat Neurosci. 2, 79-87.\
Rényi, A., 2007. Probability theory. Dover Publications, Mineola, N.Y.\
Rizzolatti, G., Craighero, L., 2004. The mirror-neuron system. Annu Rev Neurosci. 27, 169-192. Roweis, S., Ghahramani, Z., 1999. A unifying review of linear gaussian models. Neural Computation 11, 305-345.\
Rulkov, N.F., Sushchik, M.M., Tsimring, L.S., Abarbanel, H.D., 1995. Generalized synchronization of chaos in directionally coupled chaotic systems. Physical review. E, Statistical physics, plasmas, fluids, and related interdisciplinary topics 51, 980-994.\
Schilpp, P.A., 2000. Albert Einstein : philosopher-scientist. MFJ Books, New York.\
Schlosshauer, M., 2004. Decoherence, the measurement problem, and interpretations of quantum mechanics. Reviews of Modern Physics 76, 1267-1305.\
Schmidhuber, J., 2006. Developmental robotics, optimal artificial curiosity, creativity, music, and the fine arts. Connection Science 18, 173-187.\
Schmidhuber, J., 2010. Formal Theory of Creativity, Fun, and Intrinsic Motivation (1990-2010). Ieee Transactions on Autonomous Mental Development 2, 230-247.\
슈뢰딩거, E., 1944. What Is Life? : The Physical Aspect of the Living Cell. Trinity College, Dublin, Dublin, pp. 1-32.\
Schumacher, J., Haslinger, R., Pipa, G., 2012. Statistical modeling approach for detecting generalized synchronization. Physical review. E, Statistical, nonlinear, and soft matter physics 85, 056215.\
Schwabl, F., 2002. Phase Transitions, Scale Invariance, Renormalization Group Theory , and Percolation, Statistical Mechanics. Springer Berlin Heidelberg, Berlin, Heidelberg, pp. 327-404.\
Schwartenbeck, P., FitzGerald, T.H., Mathys, C., Dolan, R., Kronbichler, M., Friston, K., 2015. Evidence for surprise minimization over value maximization in choice behavior. Scientific reports 5, 16575.\
Seifert, U., 2012. Stochastic thermodynamics, fluctuation theorems and molecular machines. Reports on progress in physics. Physical Society (Great Britain) 75, 126001.\
Sejnowski, T., Paulsen, O., 2006. Network oscillations: emerging computational principles. J. Neurosci. 26, 1673-1676.\
Sekimoto, K., 1998. Langevin Equation and Thermodynamics. Progress of Theoretical Physics Supplement 130, 17-27.\
Sengupta, B., Friston, K., 2017. Sentient Self-Organization: Minimal dynamics and circular causality, arXiv:1705.08265, pp. 1-9.\
Seth, A., 2014. The cybernetic brain: from interoceptive inference to sensorimotor contingencies, MINDS project. MINDS, Metzinger, T; Windt, JM.\
Seth, A.K., 2015. Inference to the Best Prediction, in: Metzinger, T.K., Windt, J.M. (Eds.), Open MIND. MIND Group, Frankfurt am Main.\
Shew, W.L., Yang, H., Yu, S., Roy, R., Plenz, D., 2011. Information capacity and transmission are maximized in balanced cortical networks with neuronal avalanches. J Neurosci 31, 55-63. Spiegelhalter, D.J., Best, N.G., Carlin, B.P., van der Linde, A., 2002. Bayesian measures of model complexity and fit. J. Royal Statist. Society Series B 64, 583-639.\
Stephan, K.E., Manjaly, Z.M., Mathys, C.D., Weber, L.A.E., Paliwal, S., Gard, T., Tittgemeyer, M., Fleming, S.M., Haker, H., Seth, A.K., Petzschner, F.H., 2016. Allostatic Self-efficacy: A Metacognitive Theory of Dyshomeostasis-Induced Fatigue and Depression. Frontiers in Human Neuroscience 10, 550. Sterling, P., Eyer, J., 1988. Allostasis: A new paradigm to explain arousal pathology, Handbook of Life Stress, Cognition and Health. John Wiley & Sons, New York, pp. 629-649.\
Still, S., Precup, D., 2012. An information-theoretic approach to curiosity-driven reinforcement learning. Theory in biosciences = Theorie in den Biowissenschaften 131, 139-148.\
Stratonovich, R.L., 1967. Topics in the theory of random noise. Gordon and Breach, New York.\
Sun, Y., Gomez, F., Schmidhuber, J., 2011. Planning to Be Surprised: Optimal Bayesian Exploration in Dynamic Environments, in: Schmidhuber, J., Thórisson, K.R., Looks, M. (Eds.), Artificial General Intelligence: 4th International Conference, AGI 2011, Mountain View, CA, USA, August 3-6, 2011. Proceedings. Springer Berlin Heidelberg, Berlin, Heidelberg, pp. 41-51.\
Sutton, R.S., Precup, D., Singh, S., 1999. Between MDPs and semi-MDPs: A framework for temporal abstraction in reinforcement learning. Artificial Intelligence 112, 181-211.\
Takens, F., 1980. Detecting strange attractors in turbulence. Rijksuniversiteit Groningen. Mathematisch Instituut, Groningen.Theise, N.D., Kafatos, M.C., 2013. Complementarity in biological systems: A complexity view. Complexity 18, 11-20.
Thompson, E., 2010. Mind in life: Biology, phenomenology, and the sciences of mind. Harvard University Press.\
Thompson, E., Varela, F., 2001. Radical embodiment: neural dynamics and consciousness. Trends Cogn Sci. 5, 418-425.\
Tishby, N., Polani, D., 2010. Information Theory of Decisions and Actions, in: Cutsuridis, V., Hussain, A., and Taylor, J. (Eds.), Perception-reason-action cycle: Models, algorithms and systems. Springer, Berlin.\
Tononi, G., Sporns, O., Edelman, G.M., 1994. A measure for brain complexity: relating functional segregation and integration in the nervous system. Proc Natl Acad Sci U S A 91, 5033-5037. Toussaint, M., Storkey, A., 2006. Probabilistic inference for solving discrete and continuous state Markov Decision Processes, Proc. of the 23nd Int. Conf. on Machine Learning, pp. 945–952.\
Tribus, M., 1961. Thermodynamics and Thermostatics: An Introduction to Energy, Information and States of Matter, with Engineering Applications. D. Van Nostrand Company Inc, New York, USA. Tschacher, W., Haken, H., 2007. Intentionality in non-equilibrium systems? The functional aspects of self-organised pattern formation. New Ideas in Psychology 25, 1-15.\
Tsuda, I., 2001. Toward an interpretation of dynamic neural activity in terms of chaotic dynamical systems. Behav Brain Sci. 24, 793-810.\
Tsuda, I., Fujii, H., 2004. A Complex Systems Approach to an Interpretation of Dynamic Brain Activity I: Chaotic Itinerancy Can Provide a Mathematical Basis for Information Processing in Cortical Transitory and Nonstationary Dynamics. Lecture notes in computer science ISSU 3146, 109-128. Turing, A.M., 1952. The Chemical Basis of Morphogenesis. Phil Trans Royal Society of London, series B 237 37–72.\
Uhlhaas, P.J., Singer, W., 2010. Abnormal neural oscillations and synchrony in schizophrenia. Nature Reviews Neuroscience 11, 100-113.\
van den Broek, J.L., Wiegerinck, W.A.J.J., Kappen, H.J., 2010. Risk-sensitive path integral control. UAI 6, 1–8.\
Vespignani, A., Zapperi, S., 1998. How self-organized criticality works: A unified mean-field picture. Physical Review E 57, 6345-6362.\
Wallace, C.S., Dowe, D.L., 1999. Minimum Message Length and Kolmogorov Complexity. The Computer Journal 42, 270-283.\
Wang, X.M., 2009. From Dirac Notation to Probability Bracket Notation: Time Evolution and Path Integral under Wick Rotations. ArXiv e-prints.\
Wheeler, J.A., 1989. Information, Physics, Quantum: The Search for Links, Proceedings III International Symposium on Foundations of Quantum Mechanics, pp. 354-358.\
Wissner-Gross, A.D., Freer, C.E., 2013. Causal Entropic Forces. Physical Review Letters 110, 168702. Yan, H., Zhao, L., Hu, L., Wang, X., Wang, E., Wang, J., 2013. Nonequilibrium landscape theory of neural networks. Proceedings of the National Academy of Sciences 110, E4185-E4194.\
Yuan, R., Ma, Y., Yuan, B., Ao, P., 2011. Potential function in dynamical systems and the relation with Lyapunov function, Proceedings of the 30th Chinese Control Conference, pp. 6573-6580.\
Yuan, R., Ma, Y., Yuan, B., Ping, A., 2010. Bridging Engineering and Physics: Lyapunov Function as Potential Function. arXiv:1012.2721v1 [nlin.CD].\
Zurek, W.H., 2003. Decoherence, einselection, and the quantum origins of the classical. Reviews of Modern Physics 75, 715-775.\
Zurek, W.H., 2009. Quantum Darwinism. Nat Phys 5, 181-188.
