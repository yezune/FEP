# 새로운 물리학을 위한 자유 에너지 원리: A Free Energy Principle for A Particular Physics

__Karl Friston__

*The Wellcome Centre for Human Neuroimaging, UCL Queen Square Institute of Neurology, London, UK WC1N 3AR. Email: k.friston@ucl.ac.uk
(This work is under consideration for publication by The MIT Press)*

## Abstract
이 원고는 통계적 의미에서 다른 '것'들과 구별할 수 있는 모든 '것'에 대한 이론을 시도합니다. 그 결과로 나타나는 통계적 독립성은 마르코프 담요를 통해 매개되며, 이는 공간적 및 시간적 규모가 점점 높아지는 앙상블(것들의 집합)의 재귀적 구성을 나타냅니다. 이 분해는 작은 것들의 설명을 제공합니다. 예를 들어, 슈뢰딩거 방정식을 통한 양자역학, 통계역학 및 관련 플럭투에이션 정리를 통한 작은 것들의 앙상블, 고전역학을 통한 큰 것들까지 이어집니다. 이러한 설명은 자율적이거나 활성화된 것들에 대한 베이지안 역학을 보완합니다. 이 작업이 모든 '것'의 공식을 제공하지만, 주요 기여는 마르코프 담요의 자기조직화에 대한 평형이 아닌 정상 상태에 대한 함의를 검토하는 것입니다. 간단히 말해, 우리는 정보 기하학과 함께하는 자유 에너지 원리를 되찾아 어떤 것의 내부 상태를 외부 상태에 대한 추론 또는 표현으로 해석할 수 있게 합니다. 그 결과로 나타나는 베이지안 역학은 양자, 통계, 고전 역학과 호환되며, 생명체와 같은 입자의 형식적인 설명을 제공할 수 있습니다.

**Key words**: *self-organisation; nonequilibrium steady-state; active inference; active particles; free energy; entropy; random dynamical attractor; autopoiesis; Markov blanket; Bayesian; variational.*

## Introduction

이 원고는 어떤 '것'이 다른 것과 구별되고, 아무 '것'도 아닌 것과 구별되는 전제에서 시작하여, 조금 농담스럽게 모든 '것'에 대한 이론을 시도합니다. 이 원고의 목표는 물리학(예: 양자, 통계 및 고전 역학)의 구조물에 호소하여 동적 시스템의 공식을 검증하고, 그 결과로 나오는 공식을 사용하여 동일한 틀 안에서 자기 조직에 대한 설명을 도출하는 것입니다[^note-1]. 우리의 시작점은 불변측도를 가진 시스템의 것들에 대한 정의입니다. 즉, 유인 집합을 가진 약 혼합 시스템입니다. 이러한 시스템의 설명은 일반적으로 무작위 동적 시스템의 형식주의를 사용하여 시작합니다. 예를 들어, 무작위 미분 방정식(예: 랑제뱅 방정식)을 기반으로 한 시스템 상태의 흐름이나 동적입니다. 여기서 현재의 처리가 시작되고, 그 후 멈춥니다. 그것은 몇 가지 분명한 질문을 하며 멈춥니다. 예를 들어, 상태란 무엇이며, 무작위 변동이 어디서 오는가? 이 질문들은 더 간단한 질문들로 이어집니다. 즉, 우리가 어떤 것의 상태를 다루고 있다면, 그 상태를 가진 것은 무엇이고, 어떻게 다른 것과 구별할 수 있는가? 이 질문들에 대한 답변은 글자 그대로 모든 것에 대한 이론으로 이어집니다.

[^note-1]:이 논문은 통계물리학의 보완적인 표현들에 대한 저자의 직관을 확실히 하기 위한 자기교육적인 연습으로 작성되었습니다. 결과적으로 이 논문은 길고, 과도하게 포괄적이며, 저자가 전문가가 아닌 다른 분야의 관례를 채택하려고 노력하면서 공통적인 테마를 강조하려고 합니다.

어떤 것들의 본질을 다루기 위해, 우리는 어떻게 어떤 것이 다른 모든 것과 구별될 수 있는지 묻기 시작합니다. 자기조직의 공식을 추구하면서, 우리는 이러한 분리의 기초로 조건부 독립 개념을 사용합니다. 구체적으로, 어떤 것이 존재하려면 그것을 구성하지 않는 (외부적 또는 외재적) 상태와 통계적으로 분리될 수 있는 (내부적 또는 내재적) 상태를 가져야 한다고 가정합니다. 이러한 분리는 마르코프 담요의 존재를 시사합니다. 즉, 내부 상태와 외부 상태를 조건부로 독립적으로 만드는 상태 집합입니다. 그 것들(즉, 내부 상태와 담요)의 존재는 마르코프 담요를 활성 상태와 감각 상태로 분할해야 함을 시사합니다. 이들은 각각 외부 상태와 내부 상태의 영향을 받지 않습니다. 이것은 약간 임의적으로 들릴 수 있지만, 이것은 상태들에 대한 조건부 독립성의 최소 집합이며, 상태를 가진 것들에 대한 얘기를 허용하는 암시적인 분할입니다. 구체적으로, 이것은 자기조직에서 '자아'를 구성하는 분할을 제공합니다. 이어지는 섹션에서는 다음 분명한 질문을 다룹니다: '것'들이란 무엇인가? 이 시점에서 우리는 무작위 동적 시스템의 랑제뱅 공식을 마르코프 담요의 관점에서 재귀적으로 자기 확인할 수 있는 답안으로 사용합니다. 간단히 말해, 제안된 공식은 것들의 상태(즉, 입자)가 담요 상태의 혼합물로 구성되며, 마르코프 담요가 더 작은 규모에서 것들을 둘러싼다고 말합니다. 효과적으로 이것은 더 작은 것들의 마르코프 담요로부터 것들을 구성함으로써 "것이란 무엇인가?"라는 질문을 회피합니다. 귀납적으로, 우리는 모든 방향으로 마르코프 담요를 가지며, 이는 것들의 본질을 명시할 필요가 없음을 의미합니다.

더 구체적으로, 우리는 주어진 공간적-시간적 규모에서의 랑제뱅 동력학 공식이 마르코프 담요의 앙상블로 분해될 수 있다는 것을 알게 됩니다. 이러한 담요 상태는 더 높은 규모에서 원래 규모의 동력학과 정확히 같은 (랑제뱅) 형태를 가진 동력학을 가집니다. 한 규모에서 다음 규모로 동력학을 올릴 때, 내부 상태는 실질적으로 제거되어 담요 상태의 느린 거시적 동력학만 남깁니다. 이것들은 다음 단계의 것들의 상태가 되며, 그들만의 마르코프 담요를 가지고 있습니다. 이 형식주의의 종착점은 점진적으로 높은 공간적 및 시간적 규모에서의 모든 것에 대한 설명입니다. 암시적인 시간 규모의 분리는 후속 섹션에서 점진적으로 더 큰 것들의 동력학, 물리학 또는 역학의 종류를 검토하는 데 사용됩니다.

이 원고는 기본적인 결과를 확립하는 첫 번째 부분, 이러한 결과를 동적 시스템의 극한 사례에 적용하여 양자, 통계 및 고전 역학을 되찾는 두 번째 부분, 그리고 미립자의 행동에 영향을 주는 내부 상태를 가진 미립자에 대한 베이지안 역학을 통해 활성 또는 자율 시스템의 특수한 경우를 고려하는 세 번째 부분으로 구성된 세 부분에 걸쳐 12개의 섹션으로 구성되어 있습니다.

제1부: 첫 번째 섹션은 측정 가능한 특성을 가진 마르코프 담요의 동력학에 대한 제약을 도입하는 기초적인 처리입니다. 측정 가능성 제약 – 또는 충분히 긴 시간 동안 불변 척도를 가지고 있는 것 – 은 상태의 흐름을 비평형 정상 상태(Nonequilibrium Steady State - NESS) 밀도의 함수[^note-2]로 표현할 수 있게 합니다. 흐름과 NESS 밀도 간의 관계는 밀도 동력학의 폭커-플랑크 공식과 특히 그 고유 해법에서 직접적으로 따릅니다. 여기서 흥미로운 결과는 비평형 정상 상태에서 마르코프 담요로부터 물려받은 시스템의 운동 방정식에서 암시적인 의존성입니다. 그 결과로 나오는 상대적으로 간단한 보조 정리와 조건부 독립성에 관한 따름정리는 이어지는 섹션에서 긴밀한 행동의 기초를 형성합니다. 두 번째 섹션에서는 대칭성 깨짐 및 자기조직 측면에서 밀도 동력학을 특징 짓는 다양한 방법을 살펴봅니다. 이 섹션에서는 정보 이론과 기하학을 사용하여 비평형 정상 상태로의 다양한 종류의 자기조직을 특징 짓습니다. 세 번째 섹션에서는 특정 시스템(로렌츠 시스템의 앙상블에 기반한 합성 원시 스프)의 수치 분석을 사용하여 자기조직의 예시를 제공합니다. 이 시스템은 원고 전체에서 동일한 동력학에 대해 상호 보완적인 관점을 취하는 방법을 설명하는 데 사용됩니다. 네 번째 섹션에서는 중첩된 규모에서 마르코프 담요의 이 (랑제뱅) 공식의 행동을 고려합니다. 간단히 말해, 우리는 더 높은 규모로 올라감에 따라 무작위 및 본질적인 변동이 점진적으로 억제되어, 무작위 변동에 의해 지배되는 에너지 소산 동력학에서 발산이 없는 흐름에 의해 지배되는 대형 시스템의 보존 동력학으로 이동하는 결과가 나타납니다.

[^note-2]: NESS는 약한 혼합 시스템에서 거의 에르고딕한 안정 상태(Nearly Ergodic Steady-State)의 약자일 수도 있습니다. 제 젊은 동료 Brennan Klein이 지적했듯이, 평형이 아닌 안정 상태는 "것이라는 상태(thingness)"에 "ness"를 제공합니다(중세 영어에서 -nes, -nesse는 "상태의 존재"를 의미하는 명사를 형성하기 위해 형용사에 첨부됩니다). 우리는 나중에 모든 '존재의 상태'가 NESS에 의존한다는 주장을 할 것입니다.

제2부: 섹션 5에서는 양자역학 측면에서 매우 작은 것들을 고려합니다. 이 섹션에서는 첫 번째 섹션에서 확립된 입자의 흐름과 NESS 밀도 간의 관계를 사용하여 슈뢰딩거 파동 방정식을 도출합니다. 여기서의 요령은 NESS 밀도를 파동 함수 역할을 하는 (복소수) 근으로 표현하거나 인수분해하는 것입니다. 섹션 6에서는 앙상블 동력학과 확률 열역학 측면에서 작은 것들의 집단 행동을 고려합니다. 여기서의 초점은 앙상블의 소산 동력학을 통계 역학에서의 확립된 결과와 연결하는 것으로, 즉 열역학 법칙과 Jarzynski 등식과 같은 관련 변동 정리입니다. 그런 다음 작은 진폭의 무작위 변동에 대한 극한에서 큰 것들의 물리학을 살펴봅니다. 이 극한은 고전적 라그랑지안이나 해밀턴을 사용하여 운동 방정식을 작성할 수 있게 하여, 고전 역학, 뉴턴 운동 법칙 및 맥스웰 방정식으로 이어집니다.

제3부: 무생성 입자의 밀도 동역학을 양자, 통계, 고전 역학의 극한 케이스로 설명한 후, 내부 상태를 무시할 수 없는 자율적 행동을 보이는 큰 것들(예: 우리와 같은 큰 활성 입자)의 존재론에 대해 살펴봅니다. 섹션 8은 생물학적 자기조직에 대표적이거나 추론적 능력을 부여할 수 있는 이유를 논합니다. 다시 말해, 좋은 조절자 이론(Conant and Ashby, 1970)과 베이지안 뇌 가설(Helmholtz, 1878 (1971); Knill and Pouget, 2004)과 같은 개념이 감각 물리학 측면에서 어떻게 실체화될 수 있는지에 대해 설명합니다. 여기서 주장은 상당히 간단한데, 바로 시스템의 내부 상태가 마르코프 담요에 감각적 인상을 남기는 외부 상태에 대한 확률적 신념을 인코딩하며, 활성 상태의 외부 상태에 대한 영향에 의해 발생한다는 것입니다. 이 섹션에서는 자율적인 것들(예: 세포 또는 뇌)이 활동적으로 샘플링된 감각의 원인을 추론하는 것을 설명하는 정보 기하학과 참석하는 자유 에너지 원리에 대한 형식적 기초를 제공합니다. 여기서 우리는 변분 베이즈(Beal, 2003)가 특정 종류의 입자의 출현적 성질임을 보여주어 베이지안 역학의 형태를 구현하는 변분 주제를 추구합니다. 섹션 9는 제1부의 합성 수프(그리고 바이러스와 같은 거주자)에서 수치 분석을 사용하여 특정 추론을 설명합니다. 섹션 10에서는 적분 변동 정리와 예상 자유 에너지를 기반으로한 자유 에너지 원리의 따르는 것들을 통해 활성 상태와 대리를 고려합니다. 끝에서 두 번째 섹션에서는 이전(열역학적) 처리를 고려한 활동적 추론을 검토합니다. 양자, 확률, 고전 및 베이지안 역학 간의 관계에 대한 간단한 논의로 마무리합니다.

## Part 1: the setup
### Something or nothing

The *“Siphonaptera”* is a nursery rhyme, sometimes referred to as Fleas:
*Big fleas have little fleas, 
Upon their backs to bite 'em, 
And little fleas have lesser fleas, 
and so, ad infinitum.*

'무엇이 사물(thing)인가?'라는 질문에 대한 한 가지 접근법은 무한히 반복되는 과정을 통해 잘 설정됩니다. 이런 반복적 과정에서는 질문 자체가 사라집니다. 이런 타파적 설명[^note-3]은 사물의 상태가 그것의 마르코프 담요에 의해 결정되며, 마르코프 담요는 그 안에 더 작은 마르코프 담요를 가진 더 작은 사물의 상태로 구성된다고 주장합니다. 이렇게 '마르코프 담요가 모든 것을 아래로' 이끈다는 주장은 모든 것에 대한 재귀적인 정의를 제공합니다. 이 정의는 공간적 및 시간적 스케일에서 분리 가능하며, 4장에서는 재정규화 그룹의 개념을 사용하여 해석됩니다. '마르코프 담요가 위아래로 모든 것을 이룬다'는 아이디어는 특정 스케일에 특권이 없음을 나타내며, 다만 질문의 대상이 되는 사물에게 '중요한' 스케일이 존재합니다. 마지막 섹션에서 우리는 '중요한' 것이 특정 스케일에서 정보 기하학이 작용하고 있음을 의미하며, 이는 자율적이고 순회하는 동력학을 제공하지만 충분히 크기 때문에 무작위적인 변동을 억제한다는 것을 알게 될 것입니다.

[^note-3]: 아리스토텔레스가 우주의 모든 움직임의 주요 원인으로 제시한 최초 움직이는 원인(라틴어: primum movens)을 해소할 수도 있는 설명입니다. 그의 '형이상학'의 12권에서 아리스토텔레스는 최초 움직이는 원인을 완벽한 미, 불가분, 그리고 완벽한 성찰만을 수행하는 것으로 묘사합니다: 그 자체를 성찰하는 것입니다.

더 기술적인 설명을 하기전에, 기본적인 이야기는 상식적인 예를 들어서 설명할 수 있습니다. 천체의 위치, 속도, 및 방사 에너지에 의해 충분히 설명되는 태양계를 상상해 보세요. 이런 양들은 각 천체의 표면(즉, 마르코프 담요)의 앙상블 평균을 구성하며, 내부 상태는 그 아래에서 변동합니다. 이제 우리가 스케일을 내려가 특정한 행성(예를 들어, 지구)에 초점을 맞추면, 이 스케일에서는 행성 표면의 기상 흐름과 지형이 적절한 수준의 설명을 구성하며, 많은 (내부) 미세 상태가 그 아래에 있습니다. 이제 우리가 도시로 확대하여 이러한 미세 상태에 접근할 수 있게 되면, 이것이 대도시의 일일 주기 동안 통근자들의 증감을 구성하게 됩니다. 이제 우리는 한 단계 더 내려가서, 이전에 통근자들의 평균 행동에 기여하던 각 요소가 자신만의 마르코프 담요를 가진 개인 또는 개체임을 알게 됩니다. 즉, 실제로 뇌입니다. 이 설명 수준에서, 뇌의 섬세하고 구조적인 내부 작동의 변동은 마르코프 담요 뒤에 숨어 있지만, 우리가 더 확대하면, 이제 통근자 행동을 조정하던 신경 세포 요소와 과정의 마르코프 담요가 됩니다. 여기서 마르코프 담요는 세포 표면에 해당하며, 이것 자체가 내부 또는 내세포 과정, 즉 자신의 마르코프 담요를 가진 내세포 소기관 간의 교환을 둘러싸고 있습니다. 대분자부터 원자 및 아원자 수준까지 계속 내려갈 수 있다고 상상할 수 있습니다. 각 단계에서, 우리는 질문하는 수준의 사물의 마르코프 담요와 소통하고 연결하기 위해 제시되는 앙상블의 상태에 따른 충분한 설명 수준을 발견합니다. 중요한 것은, 각 마르코프 담요 아래(또는 마르코프 담요 뒤에 숨겨진)에는 자체적으로 (담요 상태의 혼합으로 구성된) 내부 또는 고유한 상태들이 있습니다. 다음에서, 우리는 이 이야기를 (바닥에서 위로) 다시 이야기하면서, 이 계층적 설명 수준이 마르코프 담요를 가진 어떤 (약하게 혼합된) 무작위 동적 시스템의 필연적 결과라는 것을 보여주려고 노력할 것입니다. 그러나 먼저, 이후 섹션에서 채택된 다른 관점을 연결하는데 필요한 몇 가지 사전 준비와 배경 자료를 고려하겠습니다.

#### Some preliminaries

이 섹션은 물리학의 기초적인(서론적인) 처리로 읽을 수 있습니다. 이는 엄밀하지는 않지만 기본적인 아이디어를 전달하는데 충분합니다. 일부 주장과 보조정리를 설명하기 위해, 각 섹션은 수치 예제와 그림 설명문에 상세한 설명이 포함되어 있습니다[^note-4]. 수치 분석은 로렌츠 시스템(Lorenz, 1963)에 기반한 확률적 혼돈이나, 활성 물질을 시뮬레이션하기 위해 담요 상태로 꾸민 로렌츠 시스템의 앙상블을 사용하여 다양한 현상을 보여줍니다. 이러한 예제들은 수학이 복잡해 보일 수 있지만, 그것이 이치에 맞는, 긴밀한 현상을 설명한다는 것을 강조하려고 합니다.

[^note-4]:이 수치 분석들은 두 가지 목적을 가지고 있습니다. 첫째, 서로 보완적인 관점에서 동일한 시스템을 어떻게 특성화할 수 있는지 보여줍니다. 예를 들어, 우리는 시스템을 작은 입자(예: 전자)로, 양자역학의 관점에서 다룰 수 있습니다; 또는 입자의 집합체(예: 가스)로서 시스템을 다루어 통계 역학을 검토할 수 있습니다; 또는 어떤 활성 매질에서의 덩어리 질량(예: 공)으로 시스템을 다루고, 고전역학의 관점에서 그 반응을 묘사할 수 있습니다. 세 번째 부분에서는 이를 더 발전시켜 자율적인 행동, 즉 시스템의 한 부분이 다른 부분을 어떻게 적극적으로 추론하거나 '측정'하는지를 살펴볼 것입니다. 두 번째 목적은 보다 교육적인 측면(생물학 독자를 위한)을 가지고 있습니다; 즉, 이 시뮬레이션들은 고급 물리학 주변의 모든 신비주의를 해소합니다. 요컨대, 이 모노그래프에서 고려된 모든 역학은 직관적이고 간단한 수치 분석에 적합하며, 한 종류의 역학이 다른 역학과 어떤 관계에서 이해될 수 있게 합니다.

수학적 표기법은 대체로 표준적입니다: 양자역학에 관한 절에서는 가끔 디랙 표기법을 사용하고, 통계역학에 관한 절은 (Seifert, 2012)를 따릅니다. 가끔, 텐서를 다룰 때 (아인슈타인) 합산 규약을 사용할 것입니다. 표준 표기법에 대한 예외는 굵은 변수의 사용입니다; 여기서 $x \in X$는 위상 또는 상태 공간에서의 (일반화된) 좌표를 나타내며, $x \in X$는 기대값 또는 가장 가능성이 높은 값을 나타냅니다. $x(a)$는 변수 a에 조건을 달아 기대값을 나타냅니다. 굵은 대문자 $X$는 연산자를 나타냅니다. 명확성을 위해, 함수 미분과 시간을 포함하는 적분은 궤적, 경로 또는 경로 $x[\tau]={x(\tau):\tau\in[0,t]}$의 형태로 표현되며, 여기서 시간 $\tau$에서의 값은 $x(\tau)\equiv x_\tau$로 표시됩니다. 또한 시간에 따라 변하는 확률 밀도 $p(x,\tau)\equiv p_\tau(x_\tau)$를 다룰 것이며, 이것은 $\tau \to \infty$ 한계에서의 정적 또는 안정적 - 상태 해결책 $p(x,\infty) \equiv p(x)$를 갖습니다 ; 마찬가지로, 그들의 음의 로그 밀도 또는 놀라움 $\Im (x,\tau) \equiv \Im _\tau (x _\tau) = −\ln \space p(x,\tau)$에 대해서도 마찬가지입니다. 참조의 편의성을 위해, 용어와 표현의 용어집이 본문의 끝에 제공됩니다. 이어지는 대부분의 내용은 확률 동역학의 세 가지 동등하고 상호 보완적인 설명, 즉 랑주벵 방정식, 경로 적분 형식, 폭커-플랑크 방정식에 의존합니다.
랑주벵 동역학: 이 형식은 시스템 상태 $x(\tau)$ (즉, 어떤 시스템의 상태)의 동역학을 상태 종속적인 흐름과 일부 무작위 플럭튜에이션 $\omega (\tau)$로 표현합니다 :

$$
\begin{equation}
\begin{drcases}
\begin{aligned}
\dot{x} (\tau) & = f(x,\tau) + \omega \\
E[\omega(\tau)] & = 0 \\
E[\omega(\tau) \cdot \omega(\tau-t)] & = 2\Gamma \rho(\tau)
\end{aligned}
\end{drcases} \Rightarrow p(\dot{x}|x,\tau) = \mathcal{N}(f,2\Gamma)
\end{equation}
$$

여기서, 충분히 빠르게 변동하는 상태 그 자체와 관련하여 시간 상관성을 무시할 수 있다는 가정 하에, 무작위 변동은 공분산 $2\Gamma$를 가진 정규 분포를 따릅니다. 이 공식은 이후의 모든 것을 뒷받침합니다. 4장에서는 랑제방 동역학이 어디서 비롯되었는지, 그리고 무작위 변동이 가우시안이며 상관관계가 없는 이유에 대해 좀 더 자세히 살펴볼 것입니다.

**경로 적분 공식:** 이 공식은 위의 랑제방 동역학에 의해 생성된 경로 또는 궤적 $x[\tau]$을, $x(0) \equiv x0$에서 다룹니다:

$$
\begin{equation}
\begin{aligned}
\mathfrak{I}(x[\tau]) & \triangleq - \ln \space p(x[\tau]) = \mathcal{A}(x[\tau]) \\
\mathcal{A}(x[\tau]) & = \int_0^t \mathcal{L}(x,\dot{x}) d\tau \\
\mathcal{L}(x,\.{x}) & = \cfrac{1}{2}[(\.{x}-f) \cdot \cfrac{1}{2\Gamma}() + \nabla \cdot f] \\
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
\mathcal{H}(x,\.{x}) & =\.{x}\cfrac{\partial \mathcal{L}}{\partial \.{x}}-\mathcal{L}(x.\.{x})=\.{x}\cdot p - \mathcal{L}(x,\.{x}) \\
&= \cfrac{1}{4\Gamma}\.{x}\cdot\.{x} + \cfrac{1}{h}V(x) \\
\\
p & \triangleq \cfrac{\partial \mathcal{L}}{\partial \.{x}} = \cfrac{1}{2 \Gamma}(\.{x}-f)
\end{aligned}
\end{equation}
$$

여기서 마지막 등식은 일반화된 _운동량_ 을 정의합니다. 무작위 변동이 가장 가능성이 높은 값인 0을 취할 때 가장 가능성이 높은 경로가 얻어진다는 점을 주목하십시오:

$$
\begin{equation}
\.{x} = f(x) \Rightarrow \mathcal{H}(x,\.{x}) = \mathcal{L}(x,\.{x}) = - \cfrac{1}{2} \nabla \cdot f(x)
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

여기서 $L$은 포커-플랑크 연산자이며, $j(x,\tau)$는 확률질량의 흐름을 편리하게 요약하는 확률흐름입니다. 이는 흐름에 의존하는 항과 (보통 반대 방향의) 확률 기울기에 따른 무작위 변동에 의해 생성되는 부분을 포함합니다.
#### Nonequilibrium steady states


밀도 역학의 포커-플랑크 형식을 갖추고 나면 이제 어떤 무작위 동적 시스템의 비평형 장기 동작을 고려할 수 있습니다. 시스템이 약하게 혼합되어 있기 때문에 충분한 시간이 지난 후에는 pullback 또는 random global attractor라고 하는 불변 상태 집합으로 수렴할 것입니다. attractor는 그 자체가 무작위 집합인 경우(random set) 때문에 무작위로 나타납니다(Crauel, 1999; Crauel and Flandoli, 1994). 관련된 NESS 밀도 p(x)는 포커-플랑크 방정식의 해입니다(Frank, 2004). 식 (6)은 NESS 밀도가 흐름에 의존하며, 이는 항상 회전과 발산이 없는 구성 요소로 표현될 수 있음을 보여줍니다. 이것이 헬름홀츠 분해(Helmholtz decomposition, 벡터 미적분학의 기본 정리라고도 함)이며, 이는 대칭이 아닌 행렬 $Q = -Q^T$와 스칼라 포텐셜 $\Im(x)$의 용어로 구성될 수 있습니다(Ao, 2004)[^note-5].

[^note-5]:간단하게 하기 위해, 우리는 $Q = -QT$가 $x$에 따라 변하지 않는다고 가정하겠습니다, 적어도 지역적으로는 말이죠. 더불어, 무작위 진동의 진폭은 구형이라고 가정되므로, 우리는 $\Gamma$를 스케일링된 항등 행렬 또는 스칼라 양으로 취급할 수 있습니다.

$$
\begin{equation}
f =(Q-\Gamma)\nabla\Im
\end{equation}
$$

이 표준 형식을 사용하면(Yuan 등, 2010), $p(x) = exp(-\Im(x))$가 포커-플랑크 방정식의 해임을 간단하게 보여줄 수 있습니다(Friston and Ao, 2012). 정보 이론에서 스칼라 포텐셜 $\Im(x) = -\ln p(x)$는 자기 정보, _surprisal_ 또는 더 간단하게는 놀람(surprise)으로 알려져 있습니다(Jones, 1979; Tribus, 1961). 이는 우리가 NESS 밀도 또는 놀람에 따라 흐름을 표현할 수 있음을 의미하며, 이는 부록 B의 NESS 정리와 (Friston, 2013)에 따릅니다:

$$
\begin{equation}
\begin{aligned}
f & = (\Gamma - Q)\nabla\ln p(x) \\
 & \Rightarrow \cfrac{p(x)}{j(x)} = -Q\nabla \ln p(x) \Rightarrow \.{p}(x) = 0 \\
 \space \\
\Im(x) & = - \ln \space p(x) \\
f(x) & = (Q-\Gamma)\nabla\Im(x) \\
\nabla \cdot f(x) & = - \Gamma \nabla^{2}\Im(x)
\end{aligned}
\end{equation}
$$

이것이 이 모노그래프의 대부분을 지지하는 핵심 결과입니다. 이것은 무작위 동적 시스템의 흐름이, 비균형 안정 상태에서, 직교하는 구성 요소를 포함한다고 말합니다: 불균형 안정 상태 밀도의 로그 그래디언트를 상승하는 소산 흐름과, 해당 등고선에서 순환하는 보존적인(발산이 없는) 솔레노이드 흐름입니다. 직관적으로, 소산적인(curl이 없는) 흐름은 무작위 플럭튜에이션에 의해 그렇지 않으면 발생할 밀도의 분산을 반대로합니다. 이는 유일하게 남아 있는 확률 흐름이 솔레노이드라는 것을 의미합니다. 나중에 우리는 이 간단한 결과가 상태의 다양한 부분 집합의 흐름을 고려할 때 놀라운 함의를 가지고 있다는 것을 알게 될 것입니다. 이들은 조건부로 독립적입니다. 이 특정 구조는 모든 이후를 지지하는 두 번째 주요 개념인 마코프 블랭킷 개념에 기반을 두고 있습니다.

다음 단계는 포커-플랑크 방정식의 NESS 해를 경로 적분 형식에 대입하여, 놀람(surprisal)의 관점에서 표현된 작용을 통해 어떤 궤적의 확률을 표현하는 것입니다. 식 (2)와 식(8)에서 이것은 다음을 제공합니다:

$$
\begin{equation}
\begin{aligned}
\mathcal{A}(x[\tau]) & = \int_0^t \mathcal{L}(x,\.{x})d\tau \\
\mathcal{L}(x,\.{x}) & = \cfrac{1}{2} [ \cfrac{1}{2\Gamma}( \.{x} - Q \nabla \Im ) \cdot ( \.{x} - Q \nabla \Im) + \.{x} \cdot \nabla \Im + \Gamma(\cfrac{1}{2}\nabla \Im \cdot \nabla \Im - \nabla^{2}\Im)] \\
\mathcal{H}(x,\.{x}) & = \cfrac{1}{2} [ \cfrac{1}{2\Gamma}( \.{x} - Q \nabla \Im ) \cdot ( \.{x} - Q \nabla \Im) - \Gamma(\cfrac{1}{2}\nabla \Im \cdot \nabla \Im - \nabla^{2}\Im)] \\
\end{aligned}
\end{equation}
$$

이 결과는 솔레노이달 흐름과 그래디언트 흐름이 직교한다는 사실을 사용합니다, 즉 $ Q \nabla \Im \cdot \Gamma \nabla \Im $. 식 (9)는 기본적으로 평형상태가 아닌 동력학의 경로적분 표현입니다. 이는 어떤 궤적의 확률을 상태 공간을 통한 경로적분의 라그랑지안으로 표현하며, 여기서 라그랑지안은 운동과 놀람 (즉, NESS potential)을 통해 표현될 수 있습니다.
중요한 점은, 식 (9)의 세 항이 무작위 변동의 진폭에 대해 다르게 의존한다는 것입니다. 이 의존성은 우리가 솔레노이달 흐름이 없는 1차원 시스템의 표현을 고려하면 더욱 명확하게 볼 수 있습니다:

$$
\begin{equation}
\begin{aligned}
\mathcal{A}(x[\tau]) & =\underbrace{\frac{1}{2} \int_0^t \frac{1}{2 \Gamma} \dot{x}^2 d \tau}_{\text {kinetic }}+\underbrace{\frac{1}{2} \int_0^t \dot{\mathfrak{I}} d \tau}_{\text {path-independent }}+\underbrace{\frac{1}{h} \int_0^t V(x) d \tau}_{\text {path-dependent }} \\
\int_0^t \dot{\mathfrak{I}} d \tau & =\mathfrak{I}\left(x_t\right)-\mathfrak{I}\left(x_0\right) \\
V(x) & =\frac{h}{2} \Gamma\left(\frac{1}{2} \nabla \mathfrak{I} \cdot \nabla \mathfrak{I}-\nabla^2 \mathfrak{I}\right)
\end{aligned}
\end{equation}
$$

이것은 어떤 경로의 행동을 운동에 의존하는 (운동에너지) 항, 변화하는 놀람에 의존하는 (경로에 독립적인) 항, 그리고 무작위 진동의 진폭에 비례하는 (경로에 종속적인) 항의 형태로 표현될 수 있다는 것을 의미합니다. 부록 C에서는 기대 라그랑지안과 관련된 해밀턴이 간단하게 다루어져 있습니다

여기서 중요하게 주목해야 할 것은 식(10)의 첫 번째 항이 운동 에너지의 형태를 가지며, 여기서 무작위 진동의 진폭은 역질량의 역할을 합니다. 두 번째 항은 단순히 (NESS) 잠재력 차이이며, 세 번째 (슈뢰딩거 포텐셜) 항은 무작위 진동의 진폭에 비례하여 증가합니다. 이는 무작위 진동이 크면 상태가 무시할 만한 질량을 가진 것처럼 행동하고 슈뢰딩거 포텐셜이 지배적이라는 것을 의미합니다. 반대로,작위 진동의 진폭이 무시할 만큼 작으면 첫 번째와 두 번째 항이 우세하게 되어 행동을 운동에너지와 잠재력 항으로 분해할 수 있습니다. 이 양대 주장은 나중에 양자와 고전 역학 사이의 구별로 나타날 것입니다. 식(10)은 $\hbar = 0$이면 슈뢰딩거 포텐셜의 기여가 사라진다는 것을 제안합니다 (파인먼, 1948). 그러나 이 논문에서는 플랑크 상수를 비례 상수로 취급합니다(이것은 무작위 진동의 진폭에 특정 단위를 부여합니다), 따라서 그들의 진폭이 0으로 수렴할 때 고전적인 한계가 도달됩니다; 즉, $\Gamma = 0$.

이 한계에서, 고전적인 경로는 최소 행동의 변분 원칙으로 설명할 수 있는 가장 가능성이 높은 경로입니다:

$$
\begin{equation}
\begin{aligned}
\delta_x\mathcal{A}(Xx[\tau]) &= 0 \\ 
&\Rightarrow \.{x}(\tau) = f(x(\tau)) \\
&\Rightarrow x[\tau] = argmin_{x[\tau]} \mathcal{A}(x[\tau])
\end{aligned}
\end{equation}
$$

이것은 가장 가능성이 높은 경로가 행동을 최소화하여 경로에 대한 그것의 변화를 0으로 만든다는 것을 의미합니다. 중요한 것은, 비균형 정상 상태에서, 행동에 대한 경로에 의존적이고 독립적인 기여는 놀람(surprisal)과 그 기울기의 형태로 표현될 수 있다는 것입니다. 우리는 이 비균형 정상 상태 동력학의 결과를 여러 다른 설정에서 활용할 것입니다. 시너제틱스와 패턴 형성의 처리에서, 이 최소 행동 원칙은 때때로 에너지 기울기의 파괴로 표현됩니다 (Tschacher와 Haken, 2007).

#### Fluctuations and information length

_“Time is designed in such a way that given the present, the future is independent of the past”_ (Caticha, 2015b) p6116

우리는 확률 측정과 미분 기하학에서 상속된 측정 척도라는 측면에서 '것들의 측정'에 관심이 있을 것입니다. 이 섹션은 확률 이론에 미분 기하학을 적용할 때 발생하는 길이와 정보 기하학에 대한 간단한 배경을 제공합니다. 여기서의 주요 메시지는 이 모든 측정이 시간에 깊이 있게 의존한다는 것입니다. 이 서문의 일환으로, 무작위 변동의 본질을 고려하는 것이 유용합니다. 나중에 우리는 이러한 변동이 집합 당 상태에 대해 충분히 빠르게 변동하는 상태의 혼합물이라는 것을 알게 될 것입니다. 이런 의미에서 무작위 변동은 (정의상) 느린 상태와 상관없는 빠른 상태입니다. 빠른 상태와 느린 상태의 암시적인 통계적 독립성은 우리가 '무작위' 변동에 대해 이야기할 수 있게 합니다. 식(1)의 랑게빈 동력학의 형태는 이 시간 척도의 분리를 보여줍니다. 예를 들어, $\Gamma$의 단위(초당)는 그것이 비율 상수의 역할을 하는 것을 제안합니다. 실제로, 한 가지 시각에서는, 변동의 진폭은 변동에 의한 상태의 분산 또는 분산이 시간에 걸쳐 얼마나 빠르게 축적되는지에 대응합니다(Cox and Miller, 1965). 또한, 정상 상태에서, 진폭은 흐름을 놀람의 기울기에 결합하는 효과적인 비율 상수입니다 -식(7). 다시 말해, 주어진 NESS 밀도에 대해, 흐름은 변동의 진폭에 비례하여 증가합니다. 길이라는 개념을 도입하여 이를 공식화할 수 있습니다:

$$
\begin{equation}
\begin{aligned}
\ell = \int_0^T \sqrt{ \dot{x}(\tau)^{i} g_{ij} \.{x}(\tau)^j } dt
\end{aligned}
\end{equation}
$$

여기서 우리는 (아인슈타인) 합산 규칙을 사용했으며, 반복된 첨자와 아래 첨자에 대한 암시적인 합산이 있습니다. 식 (12)는 메트릭 텐서 $g_{ij}$가 제공하는 리만 메트릭을 사용하여 경로의 길이를 표현합니다. 지역적으로 최소 거리의 경로는 적위선(_geodesics_)이라고 불리며, 유클리드 공간에서의 직선의 아날로그입니다. 식 (10)에서, 낮은 진폭의 변동의 클래식한 한계에서 경로의 행동은 경로 길이의 상한선으로 해석될 수 있습니다 (코시-슈바르츠 부등식에 의해):

$$
\begin{equation}
\begin{aligned}
 \lim_{Q,\Gamma \rightarrow 0}\mathcal{A}(x[\tau]) &= \int_0^T \dot{x}(\tau)^{i} g_{ij} \.{x}(\tau)^j dt \geq \ell^2 \\
g &= \cfrac{1}{4\Gamma}
\end{aligned}
\end{equation}
$$

간단히하기 위해, 우리는 회전형 흐름을 무시했습니다. 이것은 만약 길이가 무작위 플럭튜에이션의 정밀도(즉, 공분산의 역수)의 용어로 측정된다면, 가장 가능성이 높은 (클래식한) 경로는 가장 짧을 것이라는 것을 제안합니다. 동일하게, 정밀도는 상태 공간에 대한 기하학을 제공하는 리만 메트릭을 제공하며, 이는 플럭튜에이션이 큰 진폭을 가질 때 점들이 서로 가깝습니다. 무작위 플럭튜에이션의 진폭과 메트릭 텐서 간의 동등성은 우리의 단순화 가정인 무작위 플럭튜에이션의 진폭이 구형(즉, 모든 방향에서 똑같이 보이는)이라는 것을 근거로 합니다. 이는 좌표 선택에 불변인 리만 메트릭을 가진 대칭 상태 공간에서 작업하는 것과 동일합니다.

이 메트릭 처리를 더 나아가서, 밀도의 충분한 통계량(즉, 매개변수)의 공간을 정보 기하학으로 갖추게 할 수 있습니다. 간단히 말해서, 정보 기하학은 통계적 다양체에서 거리를 측정하는 데 사용될 수 있는 리만 메트릭에 근거합니다(Amari, 1998; Ay, 2015). 통계적 다양체란 각 점이 확률 밀도를 나타내는 메트릭 공간입니다. 즉, 매개변수 공간의 점들은 확률 밀도의 충분한 통계량에 해당하며, 통계적 다양체의 가까운 점들은 유사한 밀도에 해당합니다. 예를 들어, 가우시안 밀도의 통계적 순간(즉, 평균과 정밀도)에 의해 생성된 이차원 공간은 일반적인 통계적 다양체를 구성합니다. 통계적 다양체의 특별한 점은 항상 메트릭 텐서를 갖추고 있으며, 이는 피셔 정보 메트릭의 형태로 제공됩니다.

현재의 상황에서는 (Crooks, 2007)에 따라, 피셔 정보를 메트릭으로 사용하는 정보 길이를 통해 체계적인 밀도 동역학을 특성화할 수 있습니다. 밀도를 시간에 독립적인 집합 변수 또는 모드 $\zeta_i(x)$와 시간에 종속적인 충분한 통계적 역할을 하는 공액 변수 $\lambda(\tau)$로 분해하는 것을 고려해보세요 [^note-6] :

[^note-6]: 우리는 Z를 분할 함수 또는 정규화 상수를 나타내는 데 사용할 것입니다. 

$$
\begin{equation}
\begin{aligned}
\mathfrak{I}(x,\tau) = \lambda^i (\tau)\zeta_i (x) + \ln Z
\end{aligned}
\end{equation}
$$

이 매개변수화 하에, 피셔 정보 메트릭 $I(\lambda)$는 다음과 같습니다:

$$
\begin{equation}
\begin{aligned}
\ell & = \int_0^t \sqrt{g_{ij}\.{\lambda}^{i}\.{\lambda}^{j}} d\tau \\
g &= I(\lambda) \Leftrightarrow g_{ij} = cov(\zeta_i(x),\zeta_j(x)) = E\Bigg[\cfrac{\partial\Im}{\partial\lambda^{i}} \cfrac{\partial\Im}{\partial\lambda^{j}} \Bigg] = \cfrac{\partial D[p_{\lambda^{'}}(x)||p_{\lambda}(x)]}{\partial\lambda^{'i}\partial\lambda^{'j}}\Biggm\vert_{\lambda^{'} = \lambda}
\end{aligned}
\end{equation}
$$


주목할 점은 정보 기하학이 상태 공간 그 자체가 아니라 상태에 대한 밀도를 매개변수화하는 공액 변수 공간에 있다는 것입니다. 이 공간은 통계적 다양체이며, 그 기하학은 나중에 베이지안 역학의 중심적인 측면이 될 것입니다. 현재로서는 정보, 기하학, 통계 역학 간의 깊은 관계를 예고하고 있습니다 (Crooks, 2007; Kleeman, 2014).

(15)의 마지막 등식은 두 확률 분포 사이의 발산의 두 번째 도함수를 단순하게 계산함으로써 확인할 수 있습니다. 이 확률 분포들은 무한히 가까이 있으며, 여기서 $\lambda^{'} = \lambda + d\lambda$입니다. 이는 통계적 다양체 위에서 정보 길이가 매개변수화된 밀도가 빨리 변할 때 더 빨리 축적된다는 것을 의미합니다. 이 해석은 또한 통계적 다양체에서 작은 이동 $d\lambda \rightarrow 0$에 대한 연속적인 밀도 간의 발산(제곱근)의 축적으로 정보 길이를 설명하는 것을 허용합니다.

$$
\begin{equation}
\begin{aligned}
\ell & = \int d \ell \\
d\ell^2 & = g_{ij}d\lambda^j d\lambda^i \\
\cfrac{1}{2}d\ell^2 &= D[p_{\lambda^{'}}(x)||p_{\lambda}(x)] = \cfrac{1}{2} \cfrac{\partial D[p_{\lambda^{'}}(x)||p_{\lambda}(x)]}{\partial\lambda^{'i} \partial\lambda^{'j}}\Biggm\vert_{\lambda^{'}=\lambda} d\lambda^j \lambda^i \\
\end{aligned}
\end{equation}
$$


마지막 등식은 발산의 테일러 전개로부터 따르며, 첫 번째로 사라지지 않는 항은 (15)의 두 번째 도함수입니다. 이는 $\lambda^{'}=\lambda$일 때 발산과 그 첫 번째 도함수가 0이기 때문입니다. 방정식 (16)은 정보 길이를 매개변수 공간을 통해 이동하는 밀도가 지나가는 고유한 구성의 수로 이해할 수 있다는 것을 의미합니다. 이 결과는 확률 분포의 매개변수로 시스템의 다양한 구성을 처리함으로써 열역학 변수를 시스템의 다양한 구성과 우아하게 연결하는 방법을 제공합니다 (Crooks, 2007; Kleeman, 2014). 그러나, 우리의 초점은 밀도 동역학에 정보 기하학을 부여하는 특별한 매개변수인 시간에 있을 것입니다.

중요한 정보 길이는 시간 자체가 진화하는 밀도를 매개변수화하고, $\lambda(\tau) = \tau \Rightarrow .{\lambda} = 1$ 그리고 따라서 시간은 정보 기하학을 가지고 있다. 어떤 초기 상태에서 준비된 시스템을 고려하십시오. 밀도 $p_0 \equiv p(x,0)$는 다음과 같습니다.

$$
\begin{equation}
\begin{aligned}
\ell & = \int d \ell \\
d\ell^2 & = g_{ij}d\lambda^j d\lambda^i \\
\cfrac{1}{2}d\ell^2 &= D[p_{\lambda^{'}}(x)||p_{\lambda}(x)] = \cfrac{1}{2} \cfrac{\partial D[p_{\lambda^{'}}(x)||p_{\lambda}(x)]}{\partial\lambda^{'i} \partial\lambda^{'j}}\Biggm\vert_{\lambda^{'}=\lambda} d\lambda^j \lambda^i \\
\end{aligned}
\end{equation}
$$

이 문맥에서, 피셔 정보 메트릭은 밀도가 진화하는 속도를 반영하는 시간적 스케일링을 제공합니다. (16)에서:

$$
\begin{equation}
\begin{aligned}
d\ell(\tau)^2 &= g(\tau)d\tau^2 \\
\cfrac{1}{2}d\ell(\tau)^2 &= D[p(x,\tau + d\tau)||p(x,\tau)] \\
\end{aligned}
\end{equation}
$$

다시 말해, 시간에 대한 메트릭은 (제곱된) 속도 상수의 역할을 하며, 단위는 초당 (제곱)입니다. 직관적으로, 시간이 경과함에 따라 정보 길이는 (17)의 폭커-플랑크 연산자를 통한 무작위 플럭튜에이션의 진폭과 (흐름의) 발산에 따라 달라집니다. 이는 상태 공간의 한 부분에서 메트릭 시간이 느리게 진행되고 다른 곳에서는 빠르게 진행될 수 있음을 의미합니다. 방정식 (18)은 또한 정보 길이를 무한히 짧은 시간 간격 동안 (제곱된) 발산의 누적으로 간주할 수 있음을 제안합니다. 이 누적은 (사전 메트릭) 발산으로부터 메트릭을 구성할 수 있게 합니다. 이는 초기 밀도와 나중의 시점에서의 밀도 간의 발산과 대조되어야 합니다. 다음 섹션에서 이에 대한 예를 볼 수 있을 것입니다.

(18)의 정보 길이는 균형 상태 또는 비균형 정상 상태로의 수렴을 유용하게 특성화합니다 (Kim, 2018). 시간이 지나면서 모든 초기 상태에서의 미래 밀도는 NESS 밀도로 수렴하고 정보 길이는 점근적 한계로 수렴합니다. 이 한계는 초기 밀도에서 NESS 밀도까지의 거리를 측정합니다. 수렴 시, (18)의 발산은 사라지고 정보 길이의 추가 증가는 없습니다.

$$
\begin{equation}
\begin{aligned}
\lim_{\tau \to \infty}D[p(x,\tau)||p(x)] = 0 \Rightarrow d\ell(\tau) = 0 \\
\end{aligned}
\end{equation}
$$

실질적으로, 정보 길이의 관점에서 보면, 미래에서 시간은 느려집니다. 직관적으로, 한 시간 뒤에 무엇을 하고 있을지, 그것이 현재 당신이 하는 것과 어떻게 다른지 상상해보십시오. 이제, 이 연습을 반복하지만 10년 뒤의 당신과 10년 후 한 시간을 상상해보십시오. 멀리 떨어져 있는 미래에서 당신 자신의 진화하는 버전을 구별하기 어렵다는 점에서, 시간은 실질적으로 멈추었습니다.

요약하면, 시간에 의해 매개변되는 시간 종속적인 밀도의 정보 길이는 초기 밀도와 최종 밀도 사이의 발산을 사용하는 것을 보완하는 척도를 제공합니다. 이는 밀도의 경로나 초기 상태에서의 밀도의 진화에 의존하지 않습니다. 두 가지 모두 비균형 정상 상태로의 수렴을 특성화하는 데 중요한 역할을 합니다. 나중에, (19)의 발산이 확률론적이고 베이지안 역학에서 모두 자유 에너지의 형태로 나타나는 것을 볼 것입니다. 또한 정보 길이가 열역학 형식에서의 확률론적 엔트로피 생성과 밀접하게 관련되어 있음을 볼 것입니다. 지금까지, 우리가 미리 보여준 모든 것은 어떤 무작위 동적 시스템에도 적용됩니다. 다음 섹션에서는, 시스템이 마르코프 담요를 가지고 있을 때 이러한 특성들을 다시 살펴보겠습니다.

#### Random dynamical systems and Markov blankets

A Markov blanket is a set of states that separates two other sets in a statistical sense. The term Markov blanket was introduced in the context of Bayesian networks or graphs (Pearl, 1988) and refers to the children of a set (the set of states that are influenced), its parents (the set of states that influence it) and the parents of its children. The existence of a Markov blanket induces a partition of states into internal and external states, where external states are hidden (insulated) from the internal (insular) states by the Markov blanket. In other words, external states can only be seen vicariously by internal states, through blanket states. Furthermore, the Markov blanket can itself be partitioned into two sets that are, and are not, children of external states. We will refer to these as sensory states and active states respectively: $b = \lbrace s,a \rbrace \in B$ . Put simply, the existence of a Markov blanket implies a partition of states into external, sensory, active and internal states: $x = \lbrace \eta,s,a,\mu \rbrace \in X$. External states cause sensory states that influence – but are not influenced by – internal states, while internal states cause active states that influence – but are not influenced by – external states. Crucially, the dependencies induced by Markov blankets create a circular causality that is reminiscent of the action-perception cycle: see Figure 1 and (Fuster, 2004). Circular causality here means that external states cause changes in internal states, via sensory states, while the internal states couple back to the external states through active states, such that internal and external states influence each other in a vicarious and reciprocal fashion.

#### Markov blankets and marginal flows

In the next section, we will unpack the implications of Markov blankets for self-organisation in terms of information theory. This treatment rests upon the conditional independencies among the partition of states that result from precluding an influence of external states on active and internal states – and an influence of internal states on sensory and external states. This dynamical architecture is summarised in terms of a marginal flow lemma and its corollaries below. In brief, these results express the flow at nonequilibrium steady-state under the conditional independencies implied by a Markov blanket and vice versa. In other words, they connect the sparse influences mediated by Langevin flow to conditional independencies among subsets of states. Effectively, this
generalises the standard form for flow in (1.8) to a partition of states that contains a Markov Blanket. Appendix B contains the accompanying proofs and considers the complementary perspectives on how sparse influences underwrite conditional independence and vice versa.

The generalisation of the NESS density laminar to Markov blankets rests on the notion of marginal flow; namely, the flow of certain states averaged (i.e., marginalised) over other states. We will use the ~ notation to denote the complement of a subset of states; for example, $x = (\mu, \dot{\mu})$.

**Lemma** (marginal flow): for any weakly mixing random dynamical system at nonequilibrium steady-state, the marginal flow $f_{\eta}(\mu)$ of any subset of states $\eta \in X$, averaged under the complement of another $\mu \in X$ can be expressed in terms of the gradients of the logarithm of the corresponding marginal density:

$$
\begin{equation}
\begin{aligned}
f_{\eta(\mu)} \triangleq E_{p(\tilde{\mu}|\mu)}[f_{\eta}(\mu,\tilde{\mu})] = (Q_{\eta\eta}-\Gamma_{\eta\eta})\nabla_{\eta} \Im(\mu) + Q_{\eta\tilde{\eta}}\nabla_{\tilde{\eta}}\Im(\mu) \\
\end{aligned}
\end{equation}
$$

**Corollary** (conditional independence): if the flow of one subset of states does not depend on another, then it becomes the flow expected under the second subset. For example, in terms of the Markov blanket:

$$
\begin{equation}
\begin{aligned}

\begin{bmatrix}
  f_{\eta}(x) \\
  f_{s}(x)  \\
  f_{\mu}(x) \\
  f_{a}(x)  \\
\end{bmatrix}
= 
\begin{bmatrix}
  f_{\eta}(\eta,x) \\
  f_{s}(\eta,x)  \\
  f_{\mu}(\mu,x) \\
  f_{a}(\mu,x)  \\
\end{bmatrix}
=
\begin{bmatrix}
  (Q_{\eta\eta}-\Gamma_{\eta\eta})\nabla_{\eta}\Im(\eta,b) \\
  (Q_{ss}-\Gamma_{ss})\nabla_{s}\Im(\eta,b) + Q_{sa}\nabla_{a}\Im(\eta,b) \\
  (Q_{\mu\mu}-\Gamma_{\mu\mu\eta})\nabla_{\mu}\Im(\mu,b) \\
  (Q_{aa}-\Gamma_{aa})\nabla_{a}\Im(\eta,b) + Q_{as}\nabla_{s}\Im(\mu,b) \\
\end{bmatrix}

\end{aligned}
\end{equation}
$$

In short, the conditional independencies induced by the Markov blanket mean that the flow of external states is the same for every internal state, which is just its average over the internal states (similarly for other partitions).

**Corollary** (expected flow): the marginal flow of any subset $\eta \subset \subset x$ averaged over all other states depends only on the gradients of its marginal density, provided there is no solenoidal coupling with its complement:

$$
\begin{equation}
\begin{aligned}
f_{\eta}(\eta) = (\Gamma_{\eta\eta} - Q_{\eta\eta})\nabla_{\eta}\ln p(\eta) = (Q_{\eta\eta} - \Gamma_{\eta\eta})\nabla_{\eta}\Im(\eta) \\
\end{aligned}
\end{equation}
$$

This is a special case of the marginal flow lemma, when $\eta = \mu$ and $Q_{\eta\eta}=0$ . It implies that the expected flow of any state or subset of states, averaged over all other states, will behave in exactly the same way as all states considered together. In other words, it will ascend the gradients of its (marginal) density.

The marginal flow lemma allows us to express the conditional independencies implicit in the structural or probabilistic graphical model of Figure 1 in terms of the flows in (21). In other words, if a system maintains a Markov blanket at nonequilibrium steady-state, then it must possess flows that depend only upon certain states. This structured dynamics underwrites everything that follows.

#### Summary

This section has introduced the technical foundations that we will call upon later to characterise dynamics in various settings. Its focus was on self-organisation to nonequilibrium steady-state, which can be characterised as the solution to the Fokker Planck formulation of density dynamics. Crucially, this enables one to express the flow of states in terms of a nonequilibrium steady-state density, surprisal or potential. We have looked briefly at the geometry of density dynamics in terms of information length. Finally, the conditional independencies implied by a Markov blanket have been expressed in terms of how the (marginal) flow of certain states depends on other states. The marginal flows induced by a Markov blanket will become important later, when we interpret gradient flows in relation to information geometry – in Part Three.

![Figure 1](./img/01.png)
<p style="text-align: center;">Figure 1</p>

_Markov blankets_. This probabilistic graphical model illustrates the partition of states into internal states (blue) and hidden or external states (cyan) that are separated by a Markov blanket – comprising sensory (magenta) and active states (red). The upper panel shows this partition as it would be applied to action and perception in a brain. In this setting, self-organisation of internal states then corresponds to perception, while active states couple brain states back to external states. The lower panel shows the same dependencies but rearranged so that the internal states are associated with the intracellular states of a Bacillus, where the sensory states become the surface states or cell membrane overlying active states (e.g., the actin filaments of the cytoskeleton). Note that the only missing influences are between internal and external states – and directed influences from external (respectively internal) to active (respectively sensory) states. The surviving directed influences are highlighted with dotted connectors. Autonomous states are those states that are not influenced by external states, while particular states constitute a particle; namely, autonomous and sensory states – or blanket and internal states. The equations of motion in the upper panel follow from the marginal flow lemma.

### Symmetry breaking and self-organsation

_"How can the events in space and time which take place within the spatial boundary of a living organism be accounted for by physics and chemistry?"_(Schrödinger, 1944)

The introduction of Markov blankets – and the distinction between the external and internal states of a particle – changes the game somewhat, in terms of ensemble densities. In the absence of a partition, we can only talk about the entropy of a density and how it changes with time. However, in the setting of a partition, we can consider the entropy of particular states in relation to hidden states (or vice versa). This relative entropy is known as mutual information. So, are we interested in systems with a high or a low mutual information? It transpires that the answer is both, in the sense that we are interested in particles that explore their state-space but have a well-defined attracting manifold with low measure (i.e., low entropy). This speaks to a dialectic between opposing constraints. In brief, if the NESS entropy of particular states is small, then the average uncertainty about particular states, given external states must be small. In other words, knowing the external state resolves ambiguity about particular states. However, at the same time, the mutual information or coupling between external and particular states must also be small; otherwise, there will be a risk of being unable to disambiguate external from particular states; i.e., the particle will dissipate or dissolve. Heuristically, this allows for the fact that we can identify Markov blankets that are distinct from their external milieu (e.g., disambiguating a fish from the water in which it is swimming), while – at the same time – observing an intricate and self-organised coupling between particular dynamics and external states (e.g., a particular fish swimming in water). Even more simply, a fish remains a fish, despite the myriad of delicate, context-sensitive behaviours that preserve its integrity (Clarke et al., 2015). In what follows, we consider how this dialectic emerges from a straightforward statistical treatment using information theory.

Having established a partition of systemic states, we are now in a position to define the sort of self-organising systems we want to characterise. In brief, these are systems with space-filling random dynamical attractors with low measure. In other words, their probability mass is concentrated in small volumes that are connected in a way that permits itinerant (i.e. wandering) percolation of trajectories through state-space, from one manifold of the attractor to another: c.f., the percolation produced by phase transitions in deterministic systems (Vespignani and Zapperi, 1998). The implicit symmetry breaking (i.e., divergence of nearby trajectories to different regimes of phase-space) is a hallmark of nonequilibrium dynamics (Evans and Searles, 2002) and is intimately related to phenomena like self-organised criticality in dynamical systems (Bak et al., 1988; Vespignani and Zapperi, 1998). Indeed, much of complexity science addresses the problem of how to formalise multiscale, itinerant and chaotic dynamics. This is a vast field, encompassing renormalisation group theory, scale-invariance, criticality and universality (Kwapien and Drozdz, 2012; Nicolis and Prigogine, 1977; Schwabl, 2002). In this monograph, we will elude many of the finer details (and phenomena such as bifurcations, frustration and phase transitions) and suppose that the interesting behaviour of self-organising systems can be captured by nonequilibrium steady-state densities with the right sort of shape.

So, what is the right sort of shape? We start by considering the marginal (NESS) density over particular states. Given a partition into external and particular states, it is straightforward to characterise a simple form of self-organisation in terms of entropy production. This follows because there is a separation between autonomous $\alpha =\lbrace a,\mu\rbrace \in A$ and sensory states $s \in S$. Crucially, by definition, the flow of autonomous states does not depend on external states $\eta \in E$. This means that autonomous states will appear to suppress the self-information or surprisal of particular states $\pi\in P$ and its long-term average; namely, their entropy. From the marginal flow lemma (1.21), we have (ignoring solenoidal coupling between active and sensory states):


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

[Figure 1](./img/01.png)
[Figure 2](./img/02.png)
[Figure 3](./img/03.png)
[Figure 4](./img/04.png)
[Figure 5](./img/05.png)
[Figure 6](./img/06.png)
[Figure 7](./img/07.png)
[Figure 8](./img/08.png)
[Figure 9](./img/09.png)
[Figure 10](./img/10.png)
[Figure 11](./img/11.png)
[Figure 12](./img/12.png)
[Figure 13](./img/13.png)
[Figure 14](./img/14.png)
[Figure 15](./img/15.png)
[Figure 16](./img/16.png)
[Figure 17](./img/17.png)
[Figure 18](./img/18.png)
[Figure 19](./img/19.png)
[Figure 20](./img/20.png)
[Figure 21](./img/21.png)
[Figure 22](./img/22.png)
[Figure 23](./img/23.png)
