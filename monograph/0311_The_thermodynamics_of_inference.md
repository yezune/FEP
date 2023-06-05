### 추론의 열역학

자주 묻는 질문 중 하나는 열역학적 자유 에너지와 변분 자유 에너지 사이에 정량적인 관계가 있는지 여부입니다. 위의 베이지안 역학 공식은 이 질문에 대한 명확한 답을 제공합니다. 변분 자유 에너지는 입자의 상태 함수이기 때문에 (8.4) 열역학적 퍼텐셜에 해당합니다. 반면 열역학적 자유 에너지는 입자 앙상블에 대한 기대값입니다. (6.6 참조). 즉, 열역학적 자유 에너지는 앙상블의 속성이지만 변분 자유 에너지는 단일 입자의 속성입니다. 구체적으로, 앙상블이 무작위 동적 끌개에 수렴함에 따라 열역학적 자유 에너지는 감소합니다. 앙상블이 비평형 안정상태에 도달하면, 각 입자의 변분 자유 에너지는 놀라움 또는 비평형 안정상태 퍼텐셜의 (상한)을 구성하며, 결과적으로 열역학적 퍼텐셜 에너지를 구성합니다.
#### 퍼텐셜과 놀라움

비평형 안정상태에서, 변분 자유 에너지와 입자의 열역학적 퍼텐셜 사이에는 명확한 관계가 있습니다. (6.5)와 (8.6)에서:

$$
\begin{equation}\tag{10.10}
\begin{aligned}
\begin{rcases}
U(\pi)
  &= k_B T \cdot\Im(\pi) + F_m \\
\Im(\pi)
  &= F(\pmb \alpha,s) \leq F(\pmb \mu,b) \\
\end{rcases}
  &\Rightarrow
\begin{cases}
U(\pi)
  &= k_B T \cdot F(\pmb \alpha,s) + F_m \\
  &\leq k_B t \cdot F(\pmb \mu, b) + F_m \\
\end{cases}
\\
\end{aligned}
\end{equation}
$$

이 표현들은 특정 상태의 열역학적 퍼텐셜이 특정 자유 에너지에 비례함을 보여줍니다. 여기서 $F_m$은 파티션 함수에 기반한 정규화 상수입니다. 이 관계의 흥미로운 부분은 입자의 온도 또는 무작위 요동의 진폭에 따라 달라지는 비례 상수입니다:$\Gamma_{\pi\pi}\triangleq\mu_m k_B T$. 이 관계는 특정 상태의 경로에 의해 생성된 열을 평가하는 데 사용할 수 있습니다. (6.2)와 (6.7)에서 시간에 따라 변하는 열역학적 퍼텐셜과 힘을 무시하면 다음과 같습니다:

$$
\begin{equation}\tag{10.11}
\begin{aligned}
f_m(\pi,\tau)
  &\triangleq -\nabla U(\pi,\tau) \\
\pmb q(\pi,\tau)
  &= \int_0^t\pmb{\dot q}d\tau
   = \int_0^t f_m \cdot \dot \pi d \tau
   = -\int_0^t \dot U d \tau \\
  &= U(\pi_0) - U(\pi_\tau)
   = -\Delta U \\
  &= -k_B T \cdot \Delta F(\pmb \alpha,s)
\end{aligned}
\end{equation}
$$

이것은 시간에 따라 변하는 잠재적인 요소가 없는 경우의 자르진스키(Jarzynski) 관계 (6.19)의 극한 케이스입니다. 재미삼아, 이제 주목할 만한 것, 즉 '추론의 양자' 또는 변분 자유 에너지의 세 자연 단위의 변화(확률비 $20:1\approx exp(3):1$에 해당)를 수행함으로써 발산하는 열을 계산할 수 있습니다[^note-30]. 이는 $300^\degree K$의 체온에서 $1.24 10^{−20} J$를 생성할 것입니다. 비교를 위해, 실내 온도에서의 랜더워(Landauer) 한계치(동등한 4.32 비트의 정보에 대해)는 $1.19 10^{−20} J$입니다 (Bennett, 2003; Landauer, 1961): 또한 (Matta와 Massa, 2017)를 참조하십시오. 우리는 다소 임의적으로, 신념 업데이트의 양자- 그리고 통계적 다양체 위에서의 암묵적인 움직임 -을 세개의 nat의 (경로 독립적인) 발산 길이와 연관시켰습니다. 열역학과 신념 업데이트에 대한 관련 처리, (경로 종속적인) 정보 길이의 측면에서는 (Crooks, 2007)에서 찾을 수 있습니다. 이런 관계들은 베이지안과 확률론적 역학이 동일한 것의 동등한 공식임을 제안합니다. 베이지안 추론을 열역학의 필요한 결과 (즉, 열역학적 퍼텐셜에 대한 경사 흐름)로 볼 수 있습니다. 또는, 베이지안 역학은 열역학의 따름정리입니다. "우리는 정보가 현실을 근본적으로 어떻게 구성하는지 이해하기 전까지는 이상한 것, 양자를 이해할 수 없을 것이라고 제안합니다. 정보는 우리가 세계에 대해 '배우는' 것이 아니라, 세계를 '만드는' 것일 수 있습니다." (Wheeler, 1989)

> [^note-30]: 대개 베이즈 요인의 관점에서 표현되는 한 확률적 신념에 대한 강력한 증거로 간주됩니다. 해당하는 고전적 통계 추론은 $p <0.05$를 요구합니다.

#### 앙상블 자유 에너지

열역학적 자유 에너지가 앙상블의 속성이라면, 우리는 열역학적 자유 에너지와 (교환 가능한) 입자들의 앙상블, 예를 들어 생물학적 또는 화학적 세포의 집합의 변분 자유 에너지 사이의 관계를 확립할 수 있을까요? (6.6)에서 앙상블에 대한 평균 변분 자유 에너지가 열역학적 엔트로피가 된다는 것은 분명합니다:

$$
\begin{equation}\tag{10.12}
\begin{aligned}
F_\Im(\tau)
  &= E[U(\pi,\tau)]-T\cdot S \\
S &= k_B E[F(\pmb \alpha, s)] \\
\end{aligned}
\end{equation}
$$

여기서 기대치는 비평형 안정상태에서 입자나 에이전트들의 앙상블에 대한 것입니다. 이것은 앙상블의 각 구성원이 자신의 변분 자유 에너지를 최소화하려고 한다면, 앙상블의 열역학적 엔트로피도 최소화될 것이라는 흥미로운 함축을 가지고 있습니다. (Friston et al., 2015a)에서 이 앙상블 관점이 어떻게 앙상블의 (모의된) 세포에서 패턴 형성과 형태형성을 시뮬레이션하는 데 사용될 수 있는지에 대한 예를 보십시오.
#### 요약

베이지안 추론의 복잡성 비용에 대한 열역학적 접근법은 실용적인 관점에서 중요할 수 있습니다. 이는 통계적 효율과 열역학적 효율이 손에 손을 잡고 가는 것을 제안합니다. 이는 흥미로운 질문을 던집니다: 예를 들어, 기계 학습이나 추론 체계가 많은 양의 열을 방출한다면, 이는 통계적으로 비효율적인 것일까요? 열역학적 퍼텐셜을 놀라움 및 베이지안 모델 증거의 대리인으로 사용할 수 있을까요? 등등.

표 5는 이전 섹션에서 고려한 다양한 퍼텐셜을 놀라움의 관점에서 - 그리고 암시적으로 추론을 지지하는 변분 자유 에너지의 관점에서 - 요약합니다. 여기서 기본적인 메시지는 어떤 역학을 특징짓기 위해서는 놀라움과 무작위 요동의 크기를 지정하는 것이 충분하다는 것입니다. 이어서 나오는 동력학은 퍼텐셜에 대한 (solenoidal) 경사 흐름의 형태로 표현될 수 있으며, 이는 놀라움의 함수이거나 그 반대일 수 있습니다. 퍼텐셜의 정의에 따라, 무작위 요동의 크기는 양자 역학에서의 역 질량 또는 확률론적 역학에서의 스케일된 온도와 같은 다양한 해석을 얻게 됩니다. 보존 역학에서는 무작위 요동이 할인될 수 있으므로, 질량이나 전하와 같은 양은 놀라움과 퍼텐셜 사이의 비례 상수가 됩니다.

<p style="text-align:center">TABLE 5 <br/>
Potentials and surprisal (conditional dependencies on external states are omitted for clarity)
</p>

|$\begin{aligned}&\text{Mechanics(1.8)}\\ & f(x)=(Q-\Gamma)\cdot\nabla\Im(x)\end{aligned}$  | $\begin{aligned}&\text{NESS Potential or suprisal}\\ &\Im(x) \end{aligned}$ | $\begin{aligned}&\text{Amplitude of fluctuation}\\ &\Gamma \end{aligned}$ |
|:-------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------:|:-------------------------------------------:|
| $\begin{aligned}&\text{Quantum mechanics(5.4)}\\        & i\hbar\dot\Psi=\pmb H\Psi\end{aligned}$       | $\begin{aligned}&\text{Schrödinger potential}\\ &V(x)=\tfrac{\hbar^2}{4m}(\tfrac 1 2\nabla\Im\cdot\nabla\Im-\nabla^2\Im)\end{aligned}$| $\Gamma=\tfrac \hbar {2m}$ |
| $\begin{aligned}&\text{Stochastic mechanics (6.2)}\\    & f(\pi)=(Q_m-\mu_m)\nabla U(\pi)\end{aligned}$ | $\begin{aligned}&\text{Thermodynamic potential} U(s,\alpha)\\ &\Im(s,\alpha)=\tfrac{1}{k_B T}U(s,\alpha)+\ln Z\end{aligned}$ | $\Gamma=\mu_m K_B T$|
| $\begin{aligned}&\text{Newtonian mechanics (7.11)}\\    &\begin{Bmatrix}\pmb{\dot a}\\\pmb{\dot s}\end{Bmatrix}=\begin{Bmatrix}+\nabla_{\pmb s}\Im(\pmb b)\\-\nabla_{\pmb a}\Im(\pmb b)\end{Bmatrix} \end{aligned}$ | $\begin{aligned}&\text{Newtonian potential}\space\Im(\pmb a)\\ &\Im(\pmb s, \pmb a)=\Im(\pmb a)+\tfrac{\hbar}{2m}\pmb s\cdot\pmb s\end{aligned}$ |$\Gamma=0$|
| $\begin{aligned}&\text{Classical mechanics (7.12)}\\    &\begin{Bmatrix}\pmb{\dot a}\\\pmb{\dot s}\end{Bmatrix}=\begin{Bmatrix}+\nabla_{\pmb s}\Im(\pmb b)\\-\nabla_{\pmb a}\Im(\pmb b)\end{Bmatrix} \end{aligned}$ | $\begin{aligned}&\text{Electrical potential}\space \varphi(\pmb a)\\ & \Im(\pmb s,\pmb a)=z\varphi(\pmb a)+\tfrac{\hbar}{2m}(\pmb s-zA(\pmb a))\cdot(\pmb s-zA(\pmb a))\end{aligned}$ |$\Gamma=0$|
| $\begin{aligned}&\text{Relativistic mechanics (7.14)}\\ &\begin{Bmatrix}\pmb{\dot a}\\\pmb{\dot s}\end{Bmatrix}=\begin{Bmatrix}+\nabla_{\pmb s}\Im(\pmb b)\\-\nabla_{\pmb a}\Im(\pmb b)\end{Bmatrix} \end{aligned}$| $\begin{aligned}&\text{Gravitational potential}\space V(\pmb a)\\ &\Im(\pmb s, \pmb a)=V(\pmb a)+\sqrt{m^2c^4+\pmb s^2 c^2} \end{aligned}$ |$\Gamma=0$|
| $\begin{aligned}&\text{Bayesian mechanics (8.5)}\\      & \pmb{\dot\alpha}=(Q_{\alpha\alpha}-\Gamma_{\alpha\alpha})-\nabla_\alpha F(\pmb \alpha, s) \end{aligned}$ | $\begin{aligned}&\text{Variational free energy}\\ &\Im(s,\pmb \alpha)=F(\pmb \alpha, s) \end{aligned}$ |$\Gamma_{\alpha\alpha}$|


[TABLE 5](./img/t5.png)

