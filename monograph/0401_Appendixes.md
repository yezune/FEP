## 부록 A: 슈트라토노비치 경로 적분

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

## 부록 B: 보조정리와 증명

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

## 부록 C: 비평형 정상상태 에너지 함수

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

## 부록 D: 포커-프랑크 연산자

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

## 부록 E: 보편 운동

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

## 부록 F: 이산 상태공간 모형

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
