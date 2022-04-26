---
layout: post
title: 주요 벡터 항등식 정리
categories: 수리물리학
tags: [수리물리학]
use_math: true
---

## 아인슈타인 합 규약
직교 좌표계에서의 벡터 $\mathbf{V}$, $\mathbf{F}$에 대하여 다음과 같이 쓸 수 있다.

$$
\mathbf{V} = \sum^3_{k=1} V_k \mathbf{\widehat{e}}_k \equiv V_k \mathbf{\widehat{e}}_k
$$

$$
\mathbf{V} \cdot \mathbf{F} = \sum^3_{k=1} V_k F_k \equiv V_k F_k
$$

스칼라 $\varphi$의 기울기와 벡터 $\mathbf{D}$의 발산을 다음과 같이 쓸 수 있다.

$$
\nabla \varphi =\widehat{\mathbf{e}}_{k}\nabla _{k}\varphi =\widehat{\mathbf{e}}_{k}\partial _{k}\varphi =\widehat{\mathbf{e}}_{k} \dfrac{\partial \varphi }{\partial r_{k}}
$$

$$\nabla \cdot \mathbf{D} = \nabla_k D_k = \partial _{k} D_k = \dfrac{\partial D_k }{\partial r_{k}} $$

크로네커 델타와 레비-치비타 기호
크로네커 델타를 다음과 같이 정의하자.

$$\delta _{ij}=\begin{cases}1&i=j\\ 0&i\neq j\end{cases}$$

레비-치비타 기호는 다음과 같이 정의한다.

$$\epsilon_{ijk}=\begin{cases}1&ijk=xyz& yzx& zxy\\ -1&ijk=xzy& yxz& zyx\\ 0& \text{otherwise}\end{cases}$$

레비-치비타 기호를 이용하면 다음과 같이 벡터의 외적 성분을 쉽게 나타낼 수 있다.

$$ [\mathbf{V} \times \mathbf{F} ]_i = \epsilon_{ijk}V_j F_k$$

마찬가지로 벡터 $\mathbf{A}$의 회전 성분 또한 쉽게 나타낼 수 있다.

$$ [\nabla \times \mathbf{A} ]_i = \epsilon_{ijk} \partial_j A_k$$



아래의 성질은 벡터 항등식을 증명하는 과정에 매우 흔히 쓰인다.

$$ \epsilon_{ijk} \epsilon_{ist} = \delta_{js} \delta_{kt} - \delta_{jt} \delta_{ks}$$

참고로 위의 식의 일반화 식은 다음과 같다.

$$\epsilon_{kil} \epsilon_{mpq} = \begin{vmatrix} \delta _{km} & \delta _{im} & \delta _{lm} \\ \delta _{kp} & \delta _{ip} & \delta _{lp} \\ \delta _{kq} & \delta _{iq} & \delta _{lq} \end{vmatrix}  $$



## 삼중곱 벡터 항등식

(1) $\mathbf{A} \cdot (\mathbf{B} \times \mathbf{C}) = \mathbf{B} \cdot (\mathbf{C} \times \mathbf{A}) = \mathbf{C} \cdot (\mathbf{A} \times \mathbf{B})$

증명)

$$\begin{aligned}
    \mathbf{A} \cdot (\mathbf{B} \times \mathbf{C}) &= A_i [\mathbf{B} \times \mathbf{C}]_i\\[5pt]
    &= A_i \epsilon_{ijk} B_j C_k\\[5pt]
    &= A_i \epsilon_{jki} B_j C_k\\[5pt]
    &= B_j \epsilon_{jki} C_k A_i\\[5pt]
    &= B_j [\mathbf{C} \times \mathbf{A}]_j\\[5pt]
    &= \mathbf{B} \cdot (\mathbf{C} \times \mathbf{A})
    \end{aligned}$$

$\mathbf{C} \cdot (\mathbf{A} \times \mathbf{B})$ 또한 같은 방식으로 보일 수 있다.


(2) $\mathbf{A} \times (\mathbf{B} \times \mathbf{C}) = \mathbf{B} (\mathbf{A} \cdot \mathbf{C}) - \mathbf{C} (\mathbf{A} \cdot \mathbf{B})$

증명)

* BAC - CAB [백 캡] 룰로 외우면 편하다.

$$\begin{aligned}
        \left[\mathbf{A}\times (\mathbf{B} \times \mathbf{C})\right]_{i} &= \epsilon_{ijk}A_j (\mathbf{B \times C})_k \\[5pt]
&=\epsilon_{ijk}A_{j}\epsilon_{kpq}B_{p}C_q\\[5pt] &= (\delta_{ip}\delta_{jq}-\delta_{iq}\delta_{jp})A_j B_p C_q\\[5pt]
        &= A_j B_i C_j - A_j B_j C_i\\[5pt]
        &= B_i A_j C_j - C_i A_j B_j\\[5pt]
        &= B_i (\mathbf{A \cdot C}) - C_i (\mathbf{A \cdot B})
    \end{aligned}$$



## 곱셈 규칙 벡터 항등식
(1) $\nabla (fg) = f(\nabla g) + g(\nabla f)$

증명)

$$\begin{aligned}
    \left[ \nabla (fg) \right]_i &= \partial_i (fg)\\
    &= f(\partial_i g) + (\partial_i f)g\\
    &= f(\nabla g)_i + (\nabla f)_i g
\end{aligned}$$


(2) $\nabla (\mathbf{A} \cdot \mathbf{B}) = \mathbf{A} \times (\nabla \times \mathbf{B}) + \mathbf{B}\times (\nabla \times \mathbf{A}) + (\mathbf{A} \cdot \nabla ) \mathbf{B} + (\mathbf{B} \cdot \nabla)\mathbf{A}$

증명)

$$\begin{aligned}
    \left[\nabla (\mathbf{A} \cdot \mathbf{B}\right)]_i &= \partial_i (A_p B_p)\\[5pt]
    &= A_p \partial_i B_p + B_p \partial_i A_p\\[5pt]
    &= \delta_{pq}\delta_{ij} (A_p \partial_j B_q + B_p \partial_j A_q)\\[5pt]
    &= (\epsilon_{kpi}\epsilon_{kqj} + \delta_{pj}\delta{iq}(A_p \partial_j B_q + B_p \partial_j A_q)\\[5pt]
    &= -\epsilon_{kpi}A_p [\nabla \times \mathbf{B}]_k - \epsilon_{kpi} B_p [\nabla \times \mathbf{A}]_k + A_p \partial_p B_i + B_p \partial_p A_i\\[5pt]
    &= \epsilon_{ipk}A_p [\nabla \times \mathbf{B}]_k + \epsilon_{ipk} B_p [\nabla \times \mathbf{A}]_k + A_p \partial_p B_i + B_p \partial_p A_i\\[5pt]
    &= [\mathbf{A}\times (\nabla \times \mathbf{B})]_i + [\mathbf{B}\times (\nabla \times \mathbf{A})]_i + (\mathbf{A}\cdot \nabla)B_i + (\mathbf{B}\cdot\nabla)A_i
    \end{aligned}$$


(3) $\nabla \cdot (f \mathbf{A}) = (\nabla f)\cdot \mathbf{A} + f(\nabla \cdot \mathbf{A})$

증명)

$$\begin{aligned}
    \nabla \cdot (f \mathbf{A}) &= \partial_i \left[ fA_i \right]\\[5pt]
    &= f\partial_i A_i + A_i \partial_i f\\[5pt]
    &= f(\nabla \cdot \mathbf{A}) + (\nabla f)\cdot \mathbf{A}
    \end{aligned}$$


(4) $\nabla \cdot (\mathbf{A} \times \mathbf{B}) = (\nabla \times \mathbf{A})\cdot \mathbf{B} - \mathbf{A}\cdot (\nabla \times \mathbf{B})$

증명)

$$\begin{aligned}
    \nabla \cdot (\mathbf{A} \times \mathbf{B}) &= \partial_i \left[ \mathbf{A}\times \mathbf{B} \right]_i\\[5pt]
    &= \partial_i ( \epsilon_{ijk} A_j B_k )\\[5pt]
    &= \epsilon_{ijk} (A_j \partial_i B_k + B_k \partial_i A_j)\\[5pt]
    &= - A_j [\nabla \times \mathbf{B}]_j + B_k [\nabla\times\mathbf{A}]_k\\[5pt]
    &= (\nabla \times \mathbf{A})\cdot \mathbf{B} - \mathbf{A}\cdot (\nabla \times \mathbf{B})
    \end{aligned}$$


(5) $\nabla \times (f \mathbf{A}) = (\nabla f)\times \mathbf{A} + f(\nabla \times \mathbf{A})$

증명)

$$\begin{aligned}
    \left[\nabla \times (f \mathbf{A})\right]_i &= \epsilon_{ijk} \partial_j [fA_k]\\[5pt]
    &= \epsilon_{ijk} (f\partial_j A_k + A_k \partial_j f)\\[5pt]
    &= f[\nabla\times\mathbf{A}]_i + [(\nabla f)\times\mathbf{A}]_i
    \end{aligned}$$


(6) $\nabla \times (\mathbf{A} \times \mathbf{B}) = (\mathbf{B} \cdot \nabla)\mathbf{A} - (\mathbf{A} \cdot \nabla)\mathbf{B} + \mathbf{A}(\nabla \cdot \mathbf{B}) - \mathbf{B}(\nabla \cdot \mathbf{A})$

증명)

$$\begin{aligned}
    \left[\nabla \times (\mathbf{A} \times \mathbf{B})\right]_i &= \epsilon_{ijk}\partial_j [\mathbf{A}\times\mathbf{B}]_k\\[5pt]
    &= \epsilon_{ijk}\partial_j ( \epsilon_{kpq} A_p B_q)\\[5pt]
    &= \epsilon_{ijk}\epsilon_{kpq}(A_p \partial_j B_q + B_q \partial_j A_p)\\[5pt]
    &= (\delta_{ip}\delta_{jq} - \delta_{iq}\delta_{jp})(A_p \partial_j B_q + B_q \partial_j A_p)\\[5pt]
    &= A_i \partial_j B_j + B_j \partial_j A_i - A_j \partial_j B_i - B_i \partial_j A_j\\[5pt]
    &= A_i (\nabla \cdot \mathbf{B}) + (\mathbf{B}\cdot\nabla)A_i - (\mathbf{A}\cdot\nabla)B_i - B_i (\nabla \cdot \mathbf{A})
    \end{aligned}$$

## 2계 도함수 벡터 항등식
(1) $\nabla \cdot (\nabla \times \mathbf{A}) = 0$

증명)

$$\begin{aligned}
    \nabla \cdot (\nabla \times \mathbf{A}) &= \partial_i [\nabla \times \mathbf{A}]_i\\[5pt]
    &= \partial_i \epsilon_{ijk} \partial_j A_k\\[5pt]
    &= \dfrac{1}{2} \partial_i \partial_j A_k \epsilon_{ijk} + \dfrac{1}{2} \partial_i \partial_j A_k \epsilon_{ijk}\\[5pt]
    &= \dfrac{1}{2} \partial_i \partial_j A_k \epsilon_{ijk} + \dfrac{1}{2} \partial_j \partial_i A_k \epsilon_{jik}\\[5pt]
    &= \dfrac{1}{2} (\epsilon_{ijk} + \epsilon_{jik}) \partial_i \partial_j A_k\\[5pt]
    &= 0
    \end{aligned}$$


(2) $\nabla \times (\nabla f) = 0$

증명)

$$\begin{aligned}
    \left[ \nabla \times (\nabla f) \right]_i &= \epsilon_{ijk} \partial_j [\nabla f]_k\\
    &= \epsilon_{ijk} \partial_j \partial_k f\\
    &= \dfrac{1}{2} \partial_j \partial_k f \epsilon_{ijk} + \dfrac{1}{2} \partial_j \partial_k f \epsilon_{ijk}\\
    &= \dfrac{1}{2} \partial_j \partial_k f \epsilon_{ijk} + \dfrac{1}{2} \partial_k \partial_j f \epsilon_{ikj}\\
    &= \dfrac{1}{2} (\epsilon_{ijk} + \epsilon_{ikj}) \partial_j \partial_k f\\
    &= 0
\end{aligned}$$


(3) $\nabla \times (\nabla \times \mathbf{A}) = \nabla(\nabla \cdot \mathbf{A}) - \nabla ^2 \mathbf{A}$

증명)

$$\begin{aligned}
    \left[\nabla \times (\nabla \times \mathbf{A})\right]_i &= \epsilon_{ijk} \partial_j [\nabla\times \mathbf{A}]_k \\[5pt]
    &= \epsilon_{ijk} \partial_j \epsilon_{kpq}\partial_p A_q\\[5pt]
    &= \epsilon_{kij} \epsilon_{kpq} \partial_j \partial_p A_q\\[5pt]
    &= (\delta_{ip} \delta_{jq} - \delta_{iq} \delta_{jp})\partial_j \partial_p A_q\\[5pt]
    &= \partial_j \partial_i A_j - \partial_j \partial_j A_i\\[5pt]
    &= \nabla_i (\nabla \cdot \mathbf{A}) - \nabla^2 A_i
    \end{aligned}$$