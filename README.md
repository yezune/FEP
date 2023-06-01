# 어떤 물리학을 위한 자유 에너지 원리

A Free Energy Principle for A Particular Physics

[English](./README-EN.md) | [한국어](./README-KR.md)

#### 참고 자료
[A Free Energy Principle for a Paticular Physics](./ref/A_Free_Energy_Principle_for_a_Particular_Physics.pdf) \
[Acitve Inference](./ref/Active_Inference.pdf) \
[Advanced Theoretical Physics](./ref/Advanced-Theoretical-Physics-Nick_Lucid.pdf) \
[Principles of Physics From Quntum Field Theory to Classical Mechanics](./ref/Principles-of-Physics-From-Quantum-Field-Theory-to-Classical-Mechanics-Jun_Ni.pdf) \

### Equation test

$$
\begin{equation}\tag{1.9}
\begin{aligned}
\mathcal{A}(x[\tau]) 
  &= \int_0^t \mathcal{L}(x,\dot{x})d\tau \\
\mathcal{L}(x,\dot{x})
  &= \tfrac{1}{2}[\tfrac{1}{2\Gamma}(\dot{x} - Q\nabla\Im)\cdot(\dot{x}-Q\nabla\Im) + \dot{x}\cdot\nabla\Im + \Gamma(\tfrac{1}{2}\nabla\Im\cdot\nabla\Im - \nabla^{2}\Im)] \\
\mathcal{H}(x,\dot{x})
  &= \tfrac{1}{2}[\tfrac{1}{2\Gamma}(\dot{x} - Q\nabla\Im)\cdot(\dot{x}-Q\nabla\Im) - \Gamma(\tfrac{1}{2}\nabla\Im\cdot\nabla\Im - \nabla^{2}\Im)] \\
\end{aligned}
\end{equation}
$$

$$
\begin{equation}\tag{1.10}
\begin{aligned}
\mathcal{A}(x[\tau])
  &= \underbrace{
    \tfrac{1}{2}\int_0^t\tfrac{1}{2\Gamma}\dot{x}^2 d \tau
    }_{\text{kinetic}}+
    \underbrace{
      \tfrac{1}{2} \int_0^t \dot{\Im} d \tau
    }_{\text{path-independent}}+
    \underbrace{
      \tfrac{1}{h}\int_0^t V(x) d \tau
    }_{\text{path-dependent}} \\
\int_0^t \dot{\Im} d \tau
  &= \Im\left(x_t\right)-\Im\left(x_0\right) \\
V(x)
  &=\tfrac{h}{2} \Gamma\left(\tfrac{1}{2} \nabla \Im \cdot \nabla \Im-\nabla^2 \Im\right)
\end{aligned}
\end{equation}
$$
