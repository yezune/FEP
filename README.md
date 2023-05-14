# A FREE ENERGY PRINCIPLE FOR A PARTICULAR PHYSICS
# 새로운 물리학을 위한 자유 에너지 원리

__Karl Friston__

*The Wellcome Centre for Human Neuroimaging, UCL Queen Square Institute of Neurology, London, UK WC1N 3AR. Email: k.friston@ucl.ac.uk
(This work is under consideration for publication by The MIT Press)*

## Abstract
이 원고는 통계적 의미에서 다른 '것'들과 구별할 수 있는 모든 '것'에 대한 이론을 시도합니다. 그 결과로 나타나는 통계적 독립성은 마르코프 담요를 통해 매개되며, 이는 공간적 및 시간적 규모가 점점 높아지는 앙상블(것들의 집합)의 재귀적 구성을 나타냅니다. 이 분해는 작은 것들의 설명을 제공합니다. 예를 들어, 슈뢰딩거 방정식을 통한 양자역학, 통계역학 및 관련 플럭투에이션 정리를 통한 작은 것들의 앙상블, 고전역학을 통한 큰 것들까지 이어집니다. 이러한 설명은 자율적이거나 활성화된 것들에 대한 베이지안 역학을 보완합니다. 이 작업이 모든 '것'의 공식을 제공하지만, 주요 기여는 마르코프 담요의 자기조직화에 대한 평형이 아닌 정상 상태에 대한 함의를 검토하는 것입니다. 간단히 말해, 우리는 정보 기하학과 함께하는 자유 에너지 원리를 되찾아 어떤 것의 내부 상태를 외부 상태에 대한 추론 또는 표현으로 해석할 수 있게 합니다. 그 결과로 나타나는 베이지안 역학은 양자, 통계, 고전 역학과 호환되며, 생명체와 같은 입자의 형식적인 설명을 제공할 수 있습니다.

**Key words**: *self-organisation; nonequilibrium steady-state; active inference; active particles; free energy; entropy; random dynamical attractor; autopoiesis; Markov blanket; Bayesian; variational.*

## Introduction

이 원고는 어떤 '것'이 다른 것과 구별되고, 아무 '것'도 아닌 것과 구별되는 전제에서 시작하여, 조금 농담스럽게 모든 '것'에 대한 이론을 시도합니다. 이 원고의 목표는 물리학(예: 양자, 통계 및 고전 역학)의 구조물에 호소하여 동적 시스템의 공식을 검증하고, 그 결과로 나오는 공식을 사용하여 동일한 틀 안에서 자기 조직에 대한 설명을 도출하는 것입니다. 우리의 시작점은 불변측도를 가진 시스템의 것들에 대한 정의입니다. 즉, 유인 집합을 가진 약 혼합 시스템입니다. 이러한 시스템의 설명은 일반적으로 무작위 동적 시스템의 형식주의를 사용하여 시작합니다. 예를 들어, 무작위 미분 방정식(예: 랑제뱅 방정식)을 기반으로 한 시스템 상태의 흐름이나 동적입니다. 여기서 현재의 처리가 시작되고, 그 후 멈춥니다. 그것은 몇 가지 분명한 질문을 하며 멈춥니다. 예를 들어, 상태란 무엇이며, 무작위 변동이 어디서 오는가? 이 질문들은 더 간단한 질문들로 이어집니다. 즉, 우리가 어떤 것의 상태를 다루고 있다면, 그 상태를 가진 것은 무엇이고, 어떻게 다른 것과 구별할 수 있는가? 이 질문들에 대한 답변은 글자 그대로 모든 것에 대한 이론으로 이어집니다.

어떤 것들의 본질을 다루기 위해, 우리는 어떻게 어떤 것이 다른 모든 것과 구별될 수 있는지 묻기 시작합니다. 자기조직의 공식을 추구하면서, 우리는 이러한 분리의 기초로 조건부 독립 개념을 사용합니다. 구체적으로, 어떤 것이 존재하려면 그것을 구성하지 않는 (외부적 또는 외재적) 상태와 통계적으로 분리될 수 있는 (내부적 또는 내재적) 상태를 가져야 한다고 가정합니다. 이러한 분리는 마르코프 담요의 존재를 시사합니다. 즉, 내부 상태와 외부 상태를 조건부로 독립적으로 만드는 상태 집합입니다. 그 것들(즉, 내부 상태와 담요)의 존재는 마르코프 담요를 활성 상태와 감각 상태로 분할해야 함을 시사합니다. 이들은 각각 외부 상태와 내부 상태의 영향을 받지 않습니다. 이것은 약간 임의적으로 들릴 수 있지만, 이것은 상태들에 대한 조건부 독립성의 최소 집합이며, 상태를 가진 것들에 대한 얘기를 허용하는 암시적인 분할입니다. 구체적으로, 이것은 자기조직에서 '자아'를 구성하는 분할을 제공합니다. 이어지는 섹션에서는 다음 분명한 질문을 다룹니다: '것'들이란 무엇인가? 이 시점에서 우리는 무작위 동적 시스템의 랑제뱅 공식을 마르코프 담요의 관점에서 재귀적으로 자기 확인할 수 있는 답안으로 사용합니다. 간단히 말해, 제안된 공식은 것들의 상태(즉, 입자)가 담요 상태의 혼합물로 구성되며, 마르코프 담요가 더 작은 규모에서 것들을 둘러싼다고 말합니다. 효과적으로 이것은 더 작은 것들의 마르코프 담요로부터 것들을 구성함으로써 "것이란 무엇인가?"라는 질문을 회피합니다. 귀납적으로, 우리는 모든 방향으로 마르코프 담요를 가지며, 이는 것들의 본질을 명시할 필요가 없음을 의미합니다.

더 구체적으로, 우리는 주어진 공간적-시간적 규모에서의 랑제뱅 동력학 공식이 마르코프 담요의 앙상블로 분해될 수 있다는 것을 알게 됩니다. 이러한 담요 상태는 더 높은 규모에서 원래 규모의 동력학과 정확히 같은 (랑제뱅) 형태를 가진 동력학을 가집니다. 한 규모에서 다음 규모로 동력학을 올릴 때, 내부 상태는 실질적으로 제거되어 담요 상태의 느린 거시적 동력학만 남깁니다. 이것들은 다음 단계의 것들의 상태가 되며, 그들만의 마르코프 담요를 가지고 있습니다. 이 형식주의의 종착점은 점진적으로 높은 공간적 및 시간적 규모에서의 모든 것에 대한 설명입니다. 암시적인 시간 규모의 분리는 후속 섹션에서 점진적으로 더 큰 것들의 동력학, 물리학 또는 역학의 종류를 검토하는 데 사용됩니다.

이 원고는 기본적인 결과를 확립하는 첫 번째 부분, 이러한 결과를 동적 시스템의 극한 사례에 적용하여 양자, 통계 및 고전 역학을 되찾는 두 번째 부분, 그리고 미립자의 행동에 영향을 주는 내부 상태를 가진 미립자에 대한 베이지안 역학을 통해 활성 또는 자율 시스템의 특수한 경우를 고려하는 세 번째 부분으로 구성된 세 부분에 걸쳐 12개의 섹션으로 구성되어 있습니다.

제1부: 첫 번째 섹션은 측정 가능한 특성을 가진 마르코프 담요의 동력학에 대한 제약을 도입하는 기초적인 처리입니다. 측정 가능성 제약 – 또는 충분히 긴 시간 동안 불변 척도를 가지고 있는 것 – 은 상태의 흐름을 비평형 정상 상태(Nonequilibrium Steady State - NESS) 밀도의 함수로 표현할 수 있게 합니다. 흐름과 NESS 밀도 간의 관계는 밀도 동력학의 폭커-플랑크 공식과 특히 그 고유 해법에서 직접적으로 따릅니다. 여기서 흥미로운 결과는 비평형 정상 상태에서 마르코프 담요로부터 물려받은 시스템의 운동 방정식에서 암시적인 의존성입니다. 그 결과로 나오는 상대적으로 간단한 보조 정리와 조건부 독립성에 관한 따름정리는 이어지는 섹션에서 긴밀한 행동의 기초를 형성합니다. 두 번째 섹션에서는 대칭성 깨짐 및 자기조직 측면에서 밀도 동력학을 특징 짓는 다양한 방법을 살펴봅니다. 이 섹션에서는 정보 이론과 기하학을 사용하여 비평형 정상 상태로의 다양한 종류의 자기조직을 특징 짓습니다. 세 번째 섹션에서는 특정 시스템(로렌츠 시스템의 앙상블에 기반한 합성 원시 스프)의 수치 분석을 사용하여 자기조직의 예시를 제공합니다. 이 시스템은 원고 전체에서 동일한 동력학에 대해 상호 보완적인 관점을 취하는 방법을 설명하는 데 사용됩니다. 네 번째 섹션에서는 중첩된 규모에서 마르코프 담요의 이 (랑제뱅) 공식의 행동을 고려합니다. 간단히 말해, 우리는 더 높은 규모로 올라감에 따라 무작위 및 본질적인 변동이 점진적으로 억제되어, 무작위 변동에 의해 지배되는 에너지 소산 동력학에서 발산이 없는 흐름에 의해 지배되는 대형 시스템의 보존 동력학으로 이동하는 결과가 나타납니다.

제2부: 섹션 5에서는 양자역학 측면에서 매우 작은 것들을 고려합니다. 이 섹션에서는 첫 번째 섹션에서 확립된 입자의 흐름과 NESS 밀도 간의 관계를 사용하여 슈뢰딩거 파동 방정식을 도출합니다. 여기서의 요령은 NESS 밀도를 파동 함수 역할을 하는 (복소수) 근으로 표현하거나 인수분해하는 것입니다. 섹션 6에서는 앙상블 동력학과 확률 열역학 측면에서 작은 것들의 집단 행동을 고려합니다. 여기서의 초점은 앙상블의 소산 동력학을 통계 역학에서의 확립된 결과와 연결하는 것으로, 즉 열역학 법칙과 Jarzynski 등식과 같은 관련 변동 정리입니다. 그런 다음 작은 진폭의 무작위 변동에 대한 극한에서 큰 것들의 물리학을 살펴봅니다. 이 극한은 고전적 라그랑지안이나 해밀턴을 사용하여 운동 방정식을 작성할 수 있게 하여, 고전 역학, 뉴턴 운동 법칙 및 맥스웰 방정식으로 이어집니다.

제3부: 무생성 입자의 밀도 동역학을 양자, 통계, 고전 역학의 극한 케이스로 설명한 후, 내부 상태를 무시할 수 없는 자율적 행동을 보이는 큰 것들(예: 우리와 같은 큰 활성 입자)의 존재론에 대해 살펴봅니다. 섹션 8은 생물학적 자기조직에 대표적이거나 추론적 능력을 부여할 수 있는 이유를 논합니다. 다시 말해, 좋은 조절자 이론(Conant and Ashby, 1970)과 베이지안 뇌 가설(Helmholtz, 1878 (1971); Knill and Pouget, 2004)과 같은 개념이 감각 물리학 측면에서 어떻게 실체화될 수 있는지에 대해 설명합니다. 여기서 주장은 상당히 간단한데, 바로 시스템의 내부 상태가 마르코프 담요에 감각적 인상을 남기는 외부 상태에 대한 확률적 신념을 인코딩하며, 활성 상태의 외부 상태에 대한 영향에 의해 발생한다는 것입니다. 이 섹션에서는 자율적인 것들(예: 세포 또는 뇌)이 활동적으로 샘플링된 감각의 원인을 추론하는 것을 설명하는 정보 기하학과 참석하는 자유 에너지 원리에 대한 형식적 기초를 제공합니다. 여기서 우리는 변분 베이즈(Beal, 2003)가 특정 종류의 입자의 출현적 성질임을 보여주어 베이지안 역학의 형태를 구현하는 변분 주제를 추구합니다. 섹션 9는 제1부의 합성 수프(그리고 바이러스와 같은 거주자)에서 수치 분석을 사용하여 특정 추론을 설명합니다. 섹션 10에서는 적분 변동 정리와 예상 자유 에너지를 기반으로한 자유 에너지 원리의 따르는 것들을 통해 활성 상태와 대리를 고려합니다. 끝에서 두 번째 섹션에서는 이전(열역학적) 처리를 고려한 활동적 추론을 검토합니다. 양자, 확률, 고전 및 베이지안 역학 간의 관계에 대한 간단한 논의로 마무리합니다.

## Part 1: the setup
### Something or nothing

The *“Siphonaptera”* is a nursery rhyme, sometimes referred to as Fleas:
*Big fleas have little fleas, 
Upon their backs to bite 'em, 
And little fleas have lesser fleas, 
and so, ad infinitum.*

'무엇이 사물(thing)인가?'라는 질문에 대한 한 가지 접근법은 무한히 반복되는 과정을 통해 잘 설정됩니다. 이런 반복적 과정에서는 질문 자체가 사라집니다. 이런 타파적 설명은 사물의 상태가 그것의 마르코프 담요에 의해 결정되며, 마르코프 담요는 그 안에 더 작은 마르코프 담요를 가진 더 작은 사물의 상태로 구성된다고 주장합니다. 이렇게 '마르코프 담요가 모든 것을 아래로' 이끈다는 주장은 모든 것에 대한 재귀적인 정의를 제공합니다. 이 정의는 공간적 및 시간적 스케일에서 분리 가능하며, 4장에서는 재정규화 그룹의 개념을 사용하여 해석됩니다. '마르코프 담요가 위아래로 모든 것을 이룬다'는 아이디어는 특정 스케일에 특권이 없음을 나타내며, 다만 질문의 대상이 되는 사물에게 '중요한' 스케일이 존재합니다. 마지막 섹션에서 우리는 '중요한' 것이 특정 스케일에서 정보 기하학이 작용하고 있음을 의미하며, 이는 자율적이고 순회하는 동력학을 제공하지만 충분히 크기 때문에 무작위적인 변동을 억제한다는 것을 알게 될 것입니다.

더 기술적인 설명을 하기전에, 기본적인 이야기는 상식적인 예를 들어서 설명할 수 있습니다. 천체의 위치, 속도, 및 방사 에너지에 의해 충분히 설명되는 태양계를 상상해 보세요. 이런 양들은 각 천체의 표면(즉, 마르코프 담요)의 앙상블 평균을 구성하며, 내부 상태는 그 아래에서 변동합니다. 이제 우리가 스케일을 내려가 특정한 행성(예를 들어, 지구)에 초점을 맞추면, 이 스케일에서는 행성 표면의 기상 흐름과 지형이 적절한 수준의 설명을 구성하며, 많은 (내부) 미세 상태가 그 아래에 있습니다. 이제 우리가 도시로 확대하여 이러한 미세 상태에 접근할 수 있게 되면, 이것이 대도시의 일일 주기 동안 통근자들의 증감을 구성하게 됩니다. 이제 우리는 한 단계 더 내려가서, 이전에 통근자들의 평균 행동에 기여하던 각 요소가 자신만의 마르코프 담요를 가진 개인 또는 개체임을 알게 됩니다. 즉, 실제로 뇌입니다. 이 설명 수준에서, 뇌의 섬세하고 구조적인 내부 작동의 변동은 마르코프 담요 뒤에 숨어 있지만, 우리가 더 확대하면, 이제 통근자 행동을 조정하던 신경 세포 요소와 과정의 마르코프 담요가 됩니다. 여기서 마르코프 담요는 세포 표면에 해당하며, 이것 자체가 내부 또는 내세포 과정, 즉 자신의 마르코프 담요를 가진 내세포 소기관 간의 교환을 둘러싸고 있습니다. 대분자부터 원자 및 아원자 수준까지 계속 내려갈 수 있다고 상상할 수 있습니다. 각 단계에서, 우리는 질문하는 수준의 사물의 마르코프 담요와 소통하고 연결하기 위해 제시되는 앙상블의 상태에 따른 충분한 설명 수준을 발견합니다. 중요한 것은, 각 마르코프 담요 아래(또는 마르코프 담요 뒤에 숨겨진)에는 자체적으로 (담요 상태의 혼합으로 구성된) 내부 또는 고유한 상태들이 있습니다. 다음에서, 우리는 이 이야기를 (바닥에서 위로) 다시 이야기하면서, 이 계층적 설명 수준이 마르코프 담요를 가진 어떤 (약하게 혼합된) 무작위 동적 시스템의 필연적 결과라는 것을 보여주려고 노력할 것입니다. 그러나 먼저, 이후 섹션에서 채택된 다른 관점을 연결하는데 필요한 몇 가지 사전 준비와 배경 자료를 고려하겠습니다.

#### Some preliminaries

이 섹션은 물리학의 기초적인(서론적인) 처리로 읽을 수 있습니다. 이는 엄밀하지는 않지만 기본적인 아이디어를 전달하는데 충분합니다. 일부 주장과 보조정리를 설명하기 위해, 각 섹션은 수치 예제와 그림 설명문에 상세한 설명이 포함되어 있습니다. 수치 분석은 로렌츠 시스템(Lorenz, 1963)에 기반한 확률적 혼돈이나, 활성 물질을 시뮬레이션하기 위해 담요 상태로 꾸민 로렌츠 시스템의 앙상블을 사용하여 다양한 현상을 보여줍니다. 이러한 예제들은 수학이 복잡해 보일 수 있지만, 그것이 이치에 맞는, 긴밀한 현상을 설명한다는 것을 강조하려고 합니다.

수학적 표기법은 대체로 표준적입니다: 양자역학에 관한 절에서는 가끔 디랙 표기법을 사용하고, 통계역학에 관한 절은 (Seifert, 2012)를 따릅니다. 가끔, 텐서를 다룰 때 (아인슈타인) 합산 규약을 사용할 것입니다. 표준 표기법에 대한 예외는 굵은 변수의 사용입니다; 여기서 $x \in X$는 위상 또는 상태 공간에서의 (일반화된) 좌표를 나타내며, $x \in X$는 기대값 또는 가장 가능성이 높은 값을 나타냅니다. $x(a)$는 변수 a에 조건을 달아 기대값을 나타냅니다. 굵은 대문자 $X$는 연산자를 나타냅니다. 명확성을 위해, 함수 미분과 시간을 포함하는 적분은 궤적, 경로 또는 경로 $x[\tau]={x(\tau):\tau\in[0,t]}$의 형태로 표현되며, 여기서 시간 $\tau$에서의 값은 $x(\tau)\equiv x_\tau$로 표시됩니다. 또한 시간에 따라 변하는 확률 밀도 $p(x,\tau)\equiv p_\tau(x_\tau)$를 다룰 것이며, 이것은 $\tau → \infin$ 한계에서의 정적 또는 안정적 - 상태 해결책 $p(x,\infin) \equiv p(x)$를 갖습니다 ; 마찬가지로, 그들의 음의 로그 밀도 또는 놀라움 $\image (x,\tau) \equiv \image _\tau (x _\tau) = −\ln \space p(x,\tau)$에 대해서도 마찬가지입니다. 참조의 편의성을 위해, 용어와 표현의 용어집이 본문의 끝에 제공됩니다. 이어지는 대부분의 내용은 확률 동역학의 세 가지 동등하고 상호 보완적인 설명, 즉 랑주벵 방정식, 경로 적분 형식, 폭커-플랑크 방정식에 의존합니다.
랑주벵 동역학: 이 형식은 시스템 상태 $x(\tau)$ (즉, 어떤 시스템의 상태)의 동역학을 상태 종속적인 흐름과 일부 무작위 플럭튜에이션 $\omega (\tau)$로 표현합니다 :

$$
\begin{equation}
\begin{drcases}
\begin{aligned}
\dot{x} (\tau) & = f(x,\tau) + \omega \\
E[\omega(\tau)] & = 0 \\
E[\omega(\tau) \cdot \omega(\tau-t)] & = 2\Gamma \rho(\tau)
\end{aligned}
\end{drcases} \Rightarrow p(\dot{x}|x,\tau) = \mathscr{N}(f,2\Gamma)
\end{equation}
$$

여기서, 충분히 빠르게 변동하는 상태 그 자체와 관련하여 시간 상관성을 무시할 수 있다는 가정 하에, 무작위 변동은 공분산 $2\Gamma$를 가진 정규 분포를 따릅니다. 이 공식은 이후의 모든 것을 뒷받침합니다. 4장에서는 랑제방 동역학이 어디서 비롯되었는지, 그리고 무작위 변동이 가우시안이며 상관관계가 없는 이유에 대해 좀 더 자세히 살펴볼 것입니다.

**경로 적분 공식:** 이 공식은 위의 랑제방 동역학에 의해 생성된 경로 또는 궤적 $x[\tau]$을, $x(0) \equiv x0$에서 다룹니다:

$$
\begin{equation}
\begin{aligned}
\mathfrak{I}(x[\tau]) & \triangleq - \ln \space p(x[\tau]) = \mathscr{A}(x[\tau]) \\
\mathscr{A}(x[\tau]) & = \int_0^t \mathscr{L}(x,\dot{x}) d\tau \\
\mathscr{L}(x,\.{x}) & = \cfrac{1}{2}[(\.{x}-f) \cdot \cfrac{1}{2\Gamma}() + \nabla \cdot f] \\
&= \cfrac{1}{4\Gamma}\.{x}\cdot\.{x} - \cfrac{1}{2\Gamma}f\cdot\.{x} + \cfrac{1}{h}V(x) \\
V(x) & = \cfrac{h}{4\Gamma}f\cdot f + \cfrac{h}{2} \nabla \cdot f
\end{aligned}
\end{equation}
$$

이 공식은 궤적과 관련된 _행동_ 의 관점에서 경로의 확률을 표현합니다. 이것은 경로의 동작(즉, 행동)의 놀람(즉, 음의 로그 확률)이 상태 공간의 각 점에서 예상되는 흐름과 경로의 동작의 차이에 기반하여 궤적을 따라 축적된 놀람이라는 것을 말합니다. 무작위 변동에 대한 가우스 가정 하에, 각 점에서의 놀람(즉, _라그랑지안_)은 간단한 이차 형태를 가지며, 스트라토노비치 적분의 암시적 사용으로 인해 추가적인 발산 항이 발생합니다(Seifert, 2012). 이 항에 대한 설명은 부록 A를 참조하십시오. 여기서, 우리는 나중에 양자 역학에서 중요한 역할을 할 슈뢰딩거 포텐셜의 관점에서 라그랑지안을 표현했습니다. 이 포텐셜은 흐름에 의존하며, 오직 흐름에만 의존합니다. 비양자 처리에서는 일반적으로 플랑크 상수를 $\hbar=1$로 설정합니다.

사물들이 어떻게 행동하는지의 특성화에 나타날 라그랑지안의 르장드르 변환인 _해밀토니안_ 을 소개하는 것이 유용할 것입니다:

$$
\begin{equation}
\begin{aligned}
\mathscr{H}(x,\.{x}) & =\.{x}\cfrac{\partial \mathscr{L}}{\partial \.{x}}-\mathscr{L}(x.\.{x})=\.{x}\cdot p - \mathscr{L}(x,\.{x}) \\
&= \cfrac{1}{4\Gamma}\.{x}\cdot\.{x} + \cfrac{1}{h}V(x) \\
p & \triangleq \cfrac{\partial \mathscr{L}}{\partial \.{x}} = \cfrac{1}{2 \Gamma}(\.{x}-f)
\end{aligned}
\end{equation}
$$

여기서 마지막 등식은 일반화된 _운동량_ 을 정의합니다. 무작위 변동이 가장 가능성이 높은 값인 0을 취할 때 가장 가능성이 높은 경로가 얻어진다는 점을 주목하십시오:

$$
\begin{equation}
\.{x} = f(x) \rArr \mathscr{H}(x,\.{x}) = \mathscr{L}(x,\.{x}) = - \cfrac{1}{2} \nabla \cdot f(x)
\end{equation}
$$

이는 가장 가능성이 높은 경로에 따른 해밀턴이 흐름의 발산으로 감소한다는 것을 의미합니다. 또한, 발산이 없는 흐름을 가진 보존 시스템(즉, 무시할 만큼 작은 무작위 플럭튜에이션)에서는 해밀턴이 어디에서나 0입니다. 이는 해밀토니언이 보존(즉, 고전) 역학을 특징짓는데 중요하다는 것을 보여줍니다. 마지막으로, 경로 종속적인 위상 측정치 $\Omega (x)$는 주어진 초기 밀도, $p_0(x_0)\equiv p(x,0)$에 대한 다음의 경로 적분에서 평균화될 수 있습니다:
$$
\begin{equation}
E_{p(x[\tau],x_0)}[\Omega(x)] = \int dx_0 \int dx[\tau][\Omega(x[\tau])p(x[\tau]|x_0)p_0(x_0)]
\end{equation}
$$

이것으로 경로 적분 형식에서의 주요 결과를 마칩니다.

**포커-플랑크 방정식:** 이 형식은 상태들에 대한 확률 밀도를 다루며, 이는 시간 $\tau$에 시스템이 상태 $x$에 있을 확률을 설명합니다. 랑제방 방정식 시스템이 주어지면, 다음과 같이 밀도 동력학을 설명할 수 있습니다:

$$
\begin{equation}
\begin{aligned}
\.{p}(x,\tau) &= Lp(x,\tau) = - \nabla \cdot j(x,\tau) \\
L &= \nabla \cdot (\Gamma \nabla - f) \\
j(x,\tau) &= f(x,\tau)p(x, \tau) - \Gamma \nabla p(x,\tau)
\end{aligned}
\end{equation}
$$

여기서 $L$은 포커-플랑크 연산자이며, $j(x,\tau)$는 확률질량의 흐름을 편리하게 요약하는 확률 전류입니다. 이는 흐름에 의존하는 항과 (보통 반대 방향의) 확률 기울기에 따른 무작위 변동에 의해 생성되는 부분을 포함합니다.

#### Nonequilibrium steady states
#### Fluctuations and information length
#### Random dynamical systems and Markov blankets
#### Markov blankets and marginal flows
#### Summary
### Symmetry breaking and self-organsation
#### Self-organisation and self-evidencing
#### Self-organisation, frustration and supersymmetry
#### Self-organisation and information length
#### Summary
### Synthetic soups and active matter
#### An active soup
#### A random dynamical attractor and its Markov blankets
#### The Markov blanket
#### The emergence of order
#### Summary
### States, particles and fluctuations
#### Starting at the end
#### The Markovian partition
#### The adiabatic reduction
#### Elimination and renormalisation
#### Summary

## Part 2: some special cases
## Part 3: a particular case

## Discussion
### Conclusions

## Appendix A: Stratonovich path integrals
## Appendix B: lemmas and proofs
## Appendix C: nonequilibrium steady-static energy functions
## Appendix D: the Fokker-Planck operator
## Appendix E: generalised motion
## Appendix F: discrete state-space models
## References
