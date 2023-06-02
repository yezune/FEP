# 어떤 물리학을 위한 자유 에너지 원리

A Free Energy Principle for A Particular Physics

[English](./README-EN.md) | [한국어](./README-KR.md)

#### 참고 자료
[A Free Energy Principle for a Paticular Physics](./ref/A_Free_Energy_Principle_for_a_Particular_Physics.pdf) \
[Acitve Inference](./ref/Active_Inference.pdf) \
[Advanced Theoretical Physics](./ref/Advanced-Theoretical-Physics-Nick_Lucid.pdf) \
[Principles of Physics From Quntum Field Theory to Classical Mechanics](./ref/Principles-of-Physics-From-Quantum-Field-Theory-to-Classical-Mechanics-Jun_Ni.pdf) \


<p style="text-align:center">TABLE 1 <br/>
**Information measures of particular states that characterise self-organisation**
</p>

 Measure                          | Definition                                               | Comments
|---------------------------------|----------------------------------------------------------|-------------------------------------------|
| Self-information                | $\Im(\pi) = -\ln p(x)$                                   | A.k.a. suprise,surprisal or nagative log-evidence, where evidence is also known as the marginal likelihood |
| Self-entropy                    | $H[P]=E_{p(\pi)}[\Im(pi)]$                               | The antropy of particular states |
| Complexity                      | $D[p(\eta\vert\pi)\parallel p(\eta)]$                    | The divergence between the posterior and  prior over external(i.e.,hidden) states|
| Risk (expected complexity)      | $I(E,P)=E_{p(\pi)}[D[p(\eta\vert\pi)\parallel p(\eta)]]$ | The expected complexity or mutual information between external and particular states|
| Accuracy                        | $E_{p(\eta\vert\pi)}[\ln p(\pi\vert\eta)]$               | The expected log likelihood for particular states|
| Ambiguity (expected inaccuracy) | $H(P\vert E)=E_{p(\eta,\pi)}[\Im(\pi\vert\eta)]$         | Negative expected accuracy or log likelihood. This is the conditional entropy of particular states given external states |
| Information                     | $D[p(\eta\vert\pi)\parallel p(\eta\vert\alpha)]$         | A relative entropy, a.k.a. intrinsic value, salience and epistemic value|
| Expected information gain       | $I(E,S\vert A)=E_{p(\pi)}[D[p(\eta\vert\pi)\parallel p(\eta\vert\alpha)]]$| Expected information gain or mutual information between sensory and external states, conditioned on active states |

[TABLE 1](./img/t1.png)
