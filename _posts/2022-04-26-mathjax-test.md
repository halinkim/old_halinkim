---
layout: post
title: 주요 벡터 항등식 정리
categories: 수리물리학
tags: [수리물리학]
use_math: true
---

$$
\mathbf{V} \cdot \mathbf{F} = \sum^3_{k=1} V_k F_k \equiv V_k F_k
$$

bacd

$$
\begin{aligned}
\mathbf{V} \cdot \mathbf{F} = \sum^3_{k=1} V_k F_k \equiv V_k F_k
\end{aligned}
$$

abcd

$$
\begin{equation}
\mathbf{V} \cdot \mathbf{F} = \sum^3_{k=1} V_k F_k \equiv V_k F_k
\end{equation}
$$

abdc

$$
\\begin{aligned}
\\mathbf{V} \\cdot \\mathbf{F} = \\sum^3_{k=1} V_k F_k \\equiv V_k F_k
\\end{aligned}
$$

abds

$$
\\begin{equation}
\\mathbf{V} \\cdot \\mathbf{F} = \\sum^3_{k=1} V_k F_k \\equiv V_k F_k
\\end{equation}
$$
dggd

## 아인슈타인 합 규약

직교 좌표계에서의 벡터 $\mathbf{V}$, $\mathbf{F}$에 대하여 다음과 같이 쓸 수 있다.

$\mathbf{V} = \sum^3_{k=1} V_k \mathbf{\widehat{e}}_k \equiv V_k \mathbf{\widehat{e}}_k$

\\begin{aligned}
\mathbf{V} \cdot \mathbf{F} = \sum^3_{k=1} V_k F_k \equiv V_k F_k
\\end{aligned}

\\begin{equation}
\mathbf{V} \cdot \mathbf{F} = \sum^3_{k=1} V_k F_k \equiv V_k F_k
\\end{equation}

\\begin{aligned}
\\mathbf{V} \\cdot \\mathbf{F} = \\sum^3_{k=1} V_k F_k \\equiv V_k F_k
\\end{aligned}

\\begin{equation}
\\mathbf{V} \\cdot \\mathbf{F} = \\sum^3_{k=1} V_k F_k \\equiv V_k F_k
\\end{equation}

스칼라 $$\varphi$$의 기울기와 벡터 $$\mathbf{D}$$의 발산을 다음과 같이 쓸 수 있다.

$$\nabla \varphi =\widehat{\mathbf{e}}_{k}\nabla _{k}\varphi =\widehat{\mathbf{e}}_{k}\partial_{k}\varphi =\widehat{\mathbf{e}}_{k} \dfrac{\partial \varphi }{\partial r_{k}} $$

$$\nabla \cdot \mathbf{D} = \nabla_k D_k = \partial _{k} D_k = \dfrac{\partial D_k }{\partial r_{k}} $$

## 크로네커 델타와 레비-치비타 기호

크로네커 델타를 다음과 같이 정의하자.

$$\delta _{ij}=\begin{cases}1&i=j\\ 0&i\neq j\end{cases}$$

레비-치비타 기호는 다음과 같이 정의한다.

$$\epsilon_{ijk}=\begin{cases}1&ijk=xyz, yzx, zxy\\ -1&ijk=xzy, yxz, zyx\\ 0& \text{otherwise}\end{cases}$$

레비-치비타 기호를 이용하면 다음과 같이 벡터의 외적 성분을 쉽게 나타낼 수 있다.

$$ [\mathbf{V} \times \mathbf{F} ]_i = \epsilon_{ijk}V_j F_k$$

마찬가지로 벡터 $\\mathbf{A}$의 회전 성분 또한 쉽게 나타낼 수 있다.

$$ \[\\nabla \\times \\mathbf{A} \]\_i = \\epsilon\_{ijk} \\partial\_j A\_k$$

아래의 성질은 벡터 항등식을 증명하는 과정에 매우 흔히 쓰인다.

$$ \\epsilon\_{ijk} \\epsilon\_{ist} = \\delta\_{js} \\delta\_{kt} - \\delta\_{jt} \\delta\_{ks}$$

참고로 위의 식의 일반화 식은 다음과 같다.

$$\\epsilon\_{kil} \\epsilon\_{mpq} = \\begin{vmatrix} \\delta \_{km} & \\delta \_{im} & \\delta \_{lm} \\\\ \\delta \_{kp} & \\delta \_{ip} & \\delta \_{lp} \\\\ \\delta \_{kq} & \\delta \_{iq} & \\delta \_{lq} \\end{vmatrix}  $$

# 삼중곱 벡터 항등식

(1) $\\mathbf{A} \\cdot (\\mathbf{B} \\times \\mathbf{C}) = \\mathbf{B} \\cdot (\\mathbf{C} \\times \\mathbf{A}) = \\mathbf{C} \\cdot (\\mathbf{A} \\times \\mathbf{B}) $

증명)

$$\\begin{aligned}  
    \\mathbf{A} \\cdot (\\mathbf{B} \\times \\mathbf{C}) &= A\_i \[\\mathbf{B} \\times \\mathbf{C}\]\_i\\\\\[5pt\]  
    &= A\_i \\epsilon\_{ijk} B\_j C\_k\\\\\[5pt\]  
    &= A\_i \\epsilon\_{jki} B\_j C\_k\\\\\[5pt\]  
    &= B\_j \\epsilon\_{jki} C\_k A\_i\\\\\[5pt\]  
    &= B\_j \[\\mathbf{C} \\times \\mathbf{A}\]\_j\\\\\[5pt\]  
    &= \\mathbf{B} \\cdot (\\mathbf{C} \\times \\mathbf{A})  
    \\end{aligned}$$

$\\mathbf{C} \\cdot (\\mathbf{A} \\times \\mathbf{B}) $ 또한 같은 방식으로 보일 수 있다.

(2) $\\mathbf{A} \\times (\\mathbf{B} \\times \\mathbf{C}) = \\mathbf{B} (\\mathbf{A} \\cdot \\mathbf{C}) - \\mathbf{C} (\\mathbf{A} \\cdot \\mathbf{B})$

증명)

\* BAC - CAB \[백 캡\] 룰로 외우면 편하다.

$$\\begin{aligned}  
        \\label{eq:1}  
        \\left\[\\mathbf{A}\\times (\\mathbf{B} \\times \\mathbf{C})\\right\]\_{i} &= \\epsilon\_{ijk}A\_j (\\mathbf{B \\times C})\_k \\\\\[5pt\]  
&=\\epsilon\_{ijk}A\_{j}\\epsilon\_{kpq}B\_{p}C\_q\\\\\[5pt\] &= (\\delta\_{ip}\\delta\_{jq}-\\delta\_{iq}\\delta\_{jp})A\_j B\_p C\_q\\\\\[5pt\]  
        &= A\_j B\_i C\_j - A\_j B\_j C\_i\\\\\[5pt\]  
        &= B\_i A\_j C\_j - C\_i A\_j B\_j\\\\\[5pt\]  
        &= B\_i (\\mathbf{A \\cdot C}) - C\_i (\\mathbf{A \\cdot B})  
    \\end{aligned}$$

# 곱셈 규칙 벡터 항등식

(1) $\\nabla (fg) = f(\\nabla g) + g(\\nabla f)$

증명)

\\begin{aligned}  
    \\left\[ \\nabla (fg) \\right\]\_i &= \\partial\_i (fg)\\\\\[5pt\]  
    &= f(\\partial\_i g) + (\\partial\_i f)g\\\\\[5pt\]  
    &= f(\\nabla g)\_i + (\\nabla f)\_i g  
    \\end{aligned}

(2) $\\nabla (\\mathbf{A} \\cdot \\mathbf{B}) = \\mathbf{A} \\times (\\nabla \\times \\mathbf{B}) + \\mathbf{B}\\times (\\nabla \\times \\mathbf{A}) + (\\mathbf{A} \\cdot \\nabla ) \\mathbf{B} + (\\mathbf{B} \\cdot \\nabla)\\mathbf{A}$

증명)

\\begin{equation}  
    \\begin{aligned}  
    \\left\[\\nabla (\\mathbf{A} \\cdot \\mathbf{B}\\right)\]\_i &= \\partial\_i (A\_p B\_p)\\\\\[5pt\]  
    &= A\_p \\partial\_i B\_p + B\_p \\partial\_i A\_p\\\\\[5pt\]  
    &= \\delta\_{pq}\\delta\_{ij} (A\_p \\partial\_j B\_q + B\_p \\partial\_j A\_q)\\\\\[5pt\]  
    &= (\\epsilon\_{kpi}\\epsilon\_{kqj} + \\delta\_{pj}\\delta{iq}(A\_p \\partial\_j B\_q + B\_p \\partial\_j A\_q)\\\\\[5pt\]  
    &= -\\epsilon\_{kpi}A\_p \[\\nabla \\times \\mathbf{B}\]\_k - \\epsilon\_{kpi} B\_p \[\\nabla \\times \\mathbf{A}\]\_k + A\_p \\partial\_p B\_i + B\_p \\partial\_p A\_i\\\\\[5pt\]  
    &= \\epsilon\_{ipk}A\_p \[\\nabla \\times \\mathbf{B}\]\_k + \\epsilon\_{ipk} B\_p \[\\nabla \\times \\mathbf{A}\]\_k + A\_p \\partial\_p B\_i + B\_p \\partial\_p A\_i\\\\\[5pt\]  
    &= \[\\mathbf{A}\\times (\\nabla \\times \\mathbf{B})\]\_i + \[\\mathbf{B}\\times (\\nabla \\times \\mathbf{A})\]\_i + (\\mathbf{A}\\cdot \\nabla)B\_i + (\\mathbf{B}\\cdot\\nabla)A\_i  
    \\end{aligned}  
\\end{equation}

(3) $\\nabla \\cdot (f \\mathbf{A}) = (\\nabla f)\\cdot \\mathbf{A} + f(\\nabla \\cdot \\mathbf{A})$

증명)

\\begin{equation}  
    \\begin{aligned}  
    \\nabla \\cdot (f \\mathbf{A}) &= \\partial\_i \\left\[ fA\_i \\right\]\\\\\[5pt\]  
    &= f\\partial\_i A\_i + A\_i \\partial\_i f\\\\\[5pt\]  
    &= f(\\nabla \\cdot \\mathbf{A}) + (\\nabla f)\\cdot \\mathbf{A}  
    \\end{aligned}  
\\end{equation}

(4) $\\nabla \\cdot (\\mathbf{A} \\times \\mathbf{B}) = (\\nabla \\times \\mathbf{A})\\cdot \\mathbf{B} - \\mathbf{A}\\cdot (\\nabla \\times \\mathbf{B})$

증명)

\\begin{equation}  
    \\begin{aligned}  
    \\nabla \\cdot (\\mathbf{A} \\times \\mathbf{B}) &= \\partial\_i \\left\[ \\mathbf{A}\\times \\mathbf{B} \\right\]\_i\\\\\[5pt\]  
    &= \\partial\_i ( \\epsilon\_{ijk} A\_j B\_k )\\\\\[5pt\]  
    &= \\epsilon\_{ijk} (A\_j \\partial\_i B\_k + B\_k \\partial\_i A\_j)\\\\\[5pt\]  
    &= - A\_j \[\\nabla \\times \\mathbf{B}\]\_j + B\_k \[\\nabla\\times\\mathbf{A}\]\_k\\\\\[5pt\]  
    &= (\\nabla \\times \\mathbf{A})\\cdot \\mathbf{B} - \\mathbf{A}\\cdot (\\nabla \\times \\mathbf{B})  
    \\end{aligned}  
\\end{equation}

(5) $\\nabla \\times (f \\mathbf{A}) = (\\nabla f)\\times \\mathbf{A} + f(\\nabla \\times \\mathbf{A})$

증명)

\\begin{equation}  
    \\begin{aligned}  
    \\left\[\\nabla \\times (f \\mathbf{A})\\right\]\_i &= \\epsilon\_{ijk} \\partial\_j \[fA\_k\]\\\\\[5pt\]  
    &= \\epsilon\_{ijk} (f\\partial\_j A\_k + A\_k \\partial\_j f)\\\\\[5pt\]  
    &= f\[\\nabla\\times\\mathbf{A}\]\_i + \[(\\nabla f)\\times\\mathbf{A}\]\_i  
    \\end{aligned}  
\\end{equation}

(6) $\\nabla \\times (\\mathbf{A} \\times \\mathbf{B}) = (\\mathbf{B} \\cdot \\nabla)\\mathbf{A} - (\\mathbf{A} \\cdot \\nabla)\\mathbf{B} + \\mathbf{A}(\\nabla \\cdot \\mathbf{B}) - \\mathbf{B}(\\nabla \\cdot \\mathbf{A})$

증명)

\\begin{equation}  
    \\begin{aligned}  
    \\left\[\\nabla \\times (\\mathbf{A} \\times \\mathbf{B})\\right\]\_i &= \\epsilon\_{ijk}\\partial\_j \[\\mathbf{A}\\times\\mathbf{B}\]\_k\\\\\[5pt\]  
    &= \\epsilon\_{ijk}\\partial\_j ( \\epsilon\_{kpq} A\_p B\_q)\\\\\[5pt\]  
    &= \\epsilon\_{ijk}\\epsilon\_{kpq}(A\_p \\partial\_j B\_q + B\_q \\partial\_j A\_p)\\\\\[5pt\]  
    &= (\\delta\_{ip}\\delta\_{jq} - \\delta\_{iq}\\delta\_{jp})(A\_p \\partial\_j B\_q + B\_q \\partial\_j A\_p)\\\\\[5pt\]  
    &= A\_i \\partial\_j B\_j + B\_j \\partial\_j A\_i - A\_j \\partial\_j B\_i - B\_i \\partial\_j A\_j\\\\\[5pt\]  
    &= A\_i (\\nabla \\cdot \\mathbf{B}) + (\\mathbf{B}\\cdot\\nabla)A\_i - (\\mathbf{A}\\cdot\\nabla)B\_i - B\_i (\\nabla \\cdot \\mathbf{A})  
    \\end{aligned}  
\\end{equation}

# 2계 도함수 벡터 항등식

(1) $\\nabla \\cdot (\\nabla \\times \\mathbf{A}) = 0$

증명)

\\begin{aligned}  
    \\nabla \\cdot (\\nabla \\times \\mathbf{A}) &= \\partial\_i \[\\nabla \\times \\mathbf{A}\]\_i\\\\\[5pt\]  
    &= \\partial\_i \\epsilon\_{ijk} \\partial\_j A\_k\\\\\[5pt\]  
    &= \\dfrac{1}{2} \\partial\_i \\partial\_j A\_k \\epsilon\_{ijk} + \\dfrac{1}{2} \\partial\_i \\partial\_j A\_k \\epsilon\_{ijk}\\\\\[5pt\]  
    &= \\dfrac{1}{2} \\partial\_i \\partial\_j A\_k \\epsilon\_{ijk} + \\dfrac{1}{2} \\partial\_j \\partial\_i A\_k \\epsilon\_{jik}\\\\\[5pt\]  
    &= \\dfrac{1}{2} (\\epsilon\_{ijk} + \\epsilon\_{jik}) \\partial\_i \\partial\_j A\_k\\\\\[5pt\]  
    &= 0  
    \\end{aligned}

(2) $\\nabla \\times (\\nabla f) = 0$

증명)

\\begin{aligned}  
    \\left\[ \\nabla \\times (\\nabla f) \\right\]\_i &= \\epsilon\_{ijk} \\partial\_j \[\\nabla f\]\_k\\\\\[5pt\]  
    &= \\epsilon\_{ijk} \\partial\_j \\partial\_k f\\\\\[5pt\]  
    &= \\dfrac{1}{2} \\partial\_j \\partial\_k f \\epsilon\_{ijk} + \\dfrac{1}{2} \\partial\_j \\partial\_k f \\epsilon\_{ijk}\\\\\[5pt\]  
    &= \\dfrac{1}{2} \\partial\_j \\partial\_k f \\epsilon\_{ijk} + \\dfrac{1}{2} \\partial\_k \\partial\_j f \\epsilon\_{ikj}\\\\\[5pt\]  
    &= \\dfrac{1}{2} (\\epsilon\_{ijk} + \\epsilon\_{ikj}) \\partial\_j \\partial\_k f\\\\\[5pt\]  
    &= 0  
    \\end{aligned}

(3) $\\nabla \\times (\\nabla \\times \\mathbf{A}) = \\nabla(\\nabla \\cdot \\mathbf{A}) - \\nabla ^2 \\mathbf{A}$

증명)

\\begin{aligned}  
    \\left\[\\nabla \\times (\\nabla \\times \\mathbf{A})\\right\]\_i &= \\epsilon\_{ijk} \\partial\_j \[\\nabla\\times \\mathbf{A}\]\_k \\\\\[5pt\]  
    &= \\epsilon\_{ijk} \\partial\_j \\epsilon\_{kpq}\\partial\_p A\_q\\\\\[5pt\]  
    &= \\epsilon\_{kij} \\epsilon\_{kpq} \\partial\_j \\partial\_p A\_q\\\\\[5pt\]  
    &= (\\delta\_{ip} \\delta\_{jq} - \\delta\_{iq} \\delta\_{jp})\\partial\_j \\partial\_p A\_q\\\\\[5pt\]  
    &= \\partial\_j \\partial\_i A\_j - \\partial\_j \\partial\_j A\_i\\\\\[5pt\]  
    &= \\nabla\_i (\\nabla \\cdot \\mathbf{A}) - \\nabla^2 A\_i  
    \\end{aligned}