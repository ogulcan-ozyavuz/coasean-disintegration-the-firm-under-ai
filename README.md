# Coasean Disintegration:
## Cooperative Game Theory of the Firm under Autonomous Intelligence

**Ogulcan Ozyavuz**  
*DICE Venture Builder*  
`Working Paper · Mathematical & Organizational Economics`  
September 2026

[![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Status: Working Paper](https://img.shields.io/badge/Status-Working%20Paper-success.svg)](#)
[![JEL Codes](https://img.shields.io/badge/JEL-D21%20%7C%20D23%20%7C%20C71%20%7C%20L22%20%7C%20O33-orange.svg)](#)

---

### Abstract

In *The Nature of the Firm* (1937), Ronald Coase demonstrated that the boundary of the firm is governed by the margin where internal managerial coordination costs equal the cost of transacting across the open market. While Coase qualitatively identified "diminishing returns to management" as the ultimate ceiling on firm scale, organizational economics has rarely formalized the thermodynamic breakdown of internal hierarchy under cognitive automation. 

In this paper, we reformulate the Coasean firm as a **Cooperative Transferable Utility (TU) Game** $(N, \tilde{v})$ subject to super-linear communication friction $\tau(S) = c |S|^\beta$ ($\beta > 1$). We model the arrival of autonomous artificial intelligence as an exogenous, exponential cognitive capital multiplier $A \in [1, \infty)$ that acts asymmetrically across organizational scales: it collapses transaction friction for singletons ($|S|=1$) to zero while leaving the combinatorial communication friction of large hierarchies intact. 

Applying the **Bondareva-Shapley Theorem**, we formally prove the existence of a critical technological threshold $A^*$. For all $A > A^*$, the **Core of the firm becomes completely empty ($\mathcal{C} = \emptyset$)**. In this regime, no compensation schedule can simultaneously satisfy firm solvency and individual rationality. We further demonstrate that internal wage compression (Frank, 1984) drives an expanding wedge between an agent’s rising Shapley value and their corporate wage, triggering an **Adverse Selection Unraveling Spiral**. We conclude that modern corporate white-collar layoffs represent a structural phase transition: the Coasean firm is dissolving into autonomous, high-leverage atomic producers.

**Keywords:** Ronald Coase, The Nature of the Firm, Cooperative Game Theory, The Core, Bondareva-Shapley Theorem, Shapley Value, Artificial Intelligence, Transaction Costs, Organizational Economics.  
**JEL Codes:** D21, D23, C71, L22, O33.

---

## Table of Contents

1. [Introduction: The Coasean Frontier Revisited](#1-introduction-the-coasean-frontier-revisited)
2. [The Model: The Firm as a Cooperative TU Game](#2-the-model-the-firm-as-a-cooperative-tu-game)
   - [2.1 Basic Setup and Agents](#21-basic-setup-and-agents)
   - [2.2 Gross Production and Complementarity](#22-gross-production-and-complementarity)
   - [2.3 Combinatorial Friction and Managerial Overhead](#23-combinatorial-friction-and-managerial-overhead)
   - [2.4 Net Characteristic Function](#24-net-characteristic-function)
   - [2.5 The Pre-AI Industrial Equilibrium: Non-Empty Core](#25-the-pre-ai-industrial-equilibrium-non-empty-core)
3. [The Autonomous Intelligence Shock](#3-the-autonomous-intelligence-shock)
   - [3.1 Asymmetric Scaling: Singleton vs. Grand Coalition](#31-asymmetric-scaling-singleton-vs-grand-coalition)
4. [The Core Emptiness Theorem](#4-the-core-emptiness-theorem)
   - [4.1 Formal Definitions](#41-formal-definitions)
   - [4.2 Application of the Bondareva-Shapley Theorem](#42-application-of-the-bondareva-shapley-theorem)
   - [4.3 The Core Emptiness Threshold (Theorem 1)](#43-the-core-emptiness-threshold-theorem-1)
   - [4.4 The Collapse of the Optimal Coasean Firm Size (Corollary 1.1)](#44-the-collapse-of-the-optimal-coasean-firm-size-corollary-11)
5. [Microeconomic Dynamics: Shapley Value vs. Wage Compression](#5-microeconomic-dynamics-shapley-value-vs-wage-compression)
   - [5.1 The Shapley Value under AI Leverage](#51-the-shapley-value-under-ai-leverage)
   - [5.2 Institutional Wage Compression](#52-institutional-wage-compression)
   - [5.3 The Defection Gap and the Adverse Selection Spiral (Theorem 2)](#53-the-defection-gap-and-the-adverse-selection-spiral-theorem-2)
6. [Macroeconomic Integration: Intensive vs. Extensive Margins](#6-macroeconomic-integration-intensive-vs-extensive-margins)
   - [6.1 The Acemoglu (2024) Intensive Margin Fallacy](#61-the-acemoglu-2024-intensive-margin-fallacy)
   - [6.2 The Aghion (2024) Extensive Margin & Idea Production](#62-the-aghion-2024-extensive-margin--idea-production)
7. [The Entrepreneurial Distribution: The Reality of the Eagle](#7-the-entrepreneurial-distribution-the-reality-of-the-eagle)
8. [Conclusion](#8-conclusion)
9. [References](#references)
10. [Citation](#citation)

---

## 1. Introduction: The Coasean Frontier Revisited

In his seminal 1937 paper *The Nature of the Firm* ([Economica, 4(16), 386–405](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1468-0335.1937.tb00002.x)), Ronald H. Coase posed an essential question to economic theory: *If production is regulated by the price mechanism and markets achieve optimal resource allocation, why does the firm exist at all?*

Coase resolved this paradox by discovering **transaction costs**:

> *"The main reason why it is profitable to establish a firm would seem to be that there is a cost of using the price mechanism. The most obvious cost of 'organising' production through the price mechanism is that of discovering what the relevant prices are... The costs of negotiating and concluding a separate contract for each exchange transaction which takes place on a market must also be taken into account."* (Coase, 1937, pp. 390–391)

Coase demonstrated that a firm will expand until the marginal cost of organizing an additional transaction internally equals the cost of carrying out the transaction across the open market:

$$MC_{\text{internal}}(n) = MC_{\text{market}}$$

Coase famously observed three mechanisms that bound the expansion of the firm:
1. **Decreasing returns to the entrepreneurial function:** As the firm grows, the entrepreneur fails to allocate factors of production to the uses where their value is greatest.
2. **Rising organizational overhead:** The costs of organizing additional transactions within the firm rise as headcount increases.
3. **Loss of factor agility:** The supply price of one or more factors increases because the "other advantages" of small, nimble firms exceed those of a bureaucratic conglomerate.

For nearly a century, the Coasean equilibrium favored large hierarchies because market discovery, contracting, verification, and legal enforcement were prohibitively expensive ($C_{\text{market}} \gg 0$). Even though corporate bureaucracy burned immense capital, physical scale and proprietary distribution networks generated sufficient economic surplus to compensate for managerial friction.

### The Modern Phase Shift

The advent of foundation models, autonomous agentic workflows, and deterministic code synthesis fundamentally destabilizes Coase’s margin through a dual shock:

1. **Market Transaction Cost Collapse ($C_{\text{market}} \to 0$):** Semantic search, automated smart contracting, synthetic code verification, and zero-marginal-cost content synthesis compress the cost of market exchange toward zero.
2. **Cognitive Capital Democratization:** High-order cognitive synthesis (legal auditing, architectural design, software development, data science, financial modeling)—previously gated behind specialized corporate departments—is now executable by single individuals commanding autonomous toolchains.

Yet, legacy economic analysis treats this shock merely as an "efficiency booster" bolted onto existing hierarchies. In this paper, we show that when modeled through cooperative game theory, the Coasean firm does not merely become leaner; **its mathematical Core ceases to exist**.

---

## 2. The Model: The Firm as a Cooperative TU Game

### 2.1 Basic Setup and Agents

Let $N = \{1, 2, \dots, n\}$ denote a finite set of $n$ economic agents ($n \ge 2$) representing the human capital of the enterprise.  
Any non-empty subset $S \subseteq N$ denotes a **coalition** (a department, project team, or spinoff). The universal set $N$ denotes the **Grand Coalition**—the integrated corporation.

We define the enterprise as a **Transferable Utility (TU) Game** characterized by the pair $(N, \tilde{v})$, where $\tilde{v}: 2^N \to \mathbb{R}$ is the net characteristic function with $\tilde{v}(\emptyset) = 0$.

### 2.2 Gross Production and Complementarity

In the traditional economy, human capital exhibits complementarity. The gross production function $v: 2^N \to \mathbb{R}_+$ is superadditive:

$$\forall S, T \subseteq N, \quad S \cap T = \emptyset \implies v(S \cup T) \ge v(S) + v(T)$$

For analytical clarity, we assume agents possess baseline human capital and taste endowments $f_i > 0$. The gross baseline capacity of coalition $S$ is:

$$f(S) = \sum_{i \in S} f_i$$

When agents organize inside the Grand Coalition $N$, they achieve baseline organizational synergy $\gamma \ge 1$:

$$F(N) = \gamma \sum_{i=1}^n f_i = \gamma \cdot f(N)$$

### 2.3 Combinatorial Friction and Managerial Overhead $\tau(S)$

Coase identified internal managerial overhead as the limiting factor of firm size. Organizational and network theory provides the exact mathematical topology for this drag.

In a human hierarchy of size $|S|$, the number of potential pairwise communication channels is given by the complete graph $K_{|S|}$:

$$\binom{|S|}{2} = \frac{|S|(|S|-1)}{2} = \Theta(|S|^2)$$

Under Brooks' Law (1975) and Williamson’s governance friction (1975, 1985), coordination, alignment, meeting overhead, agency monitoring, and rent-seeking scale super-linearly with coalition size:

$$\tau(S) = c \cdot |S|^\beta$$

where:
* $c > 0$ represents the firm's bureaucratic friction coefficient (approval tiers, compliance protocols, political gridlock).
* $\beta > 1$ is the organizational diseconomy elasticity parameter (typically $\beta \approx 2$ due to pairwise link expansion).

For an isolated agent (a singleton coalition $S = \{i\}$), coordination friction is identically zero:

$$\tau(\{i\}) = c \cdot 1^\beta = c \approx 0 \quad (\text{frictionless autonomy})$$

### 2.4 Net Characteristic Function

The net distributable economic surplus of any coalition $S \subseteq N$ is:

$$\tilde{v}(S) = \max \{ 0, \, v(S) - \tau(S) \} = \max \{ 0, \, v(S) - c |S|^\beta \}$$

For the Grand Coalition $N$:

$$\tilde{v}(N) = v(N) - c n^\beta$$

### 2.5 The Pre-AI Industrial Equilibrium: Non-Empty Core

In the pre-AI industrial paradigm, physical capital, regulatory licenses, and enterprise distribution were monopolized by the firm. An isolated agent had virtually zero standalone market output:

$$v(\{i\}) \approx 0 \implies \tilde{v}(\{i\}) = 0, \quad \forall i \in N$$

Although internal bureaucracy was massive ($c n^\beta \gg 0$), the physical economies of scale dominated:

$$\tilde{v}(N) = v(N) - c n^\beta \gg \sum_{i=1}^n \tilde{v}(\{i\}) = 0$$

Under these parameters, the game was balanced, and by the Bondareva-Shapley Theorem, the Core was non-empty ($\mathcal{C} \neq \emptyset$). The corporate manor was coalitionally stable.

---

## 3. The Autonomous Intelligence Shock

We introduce autonomous artificial intelligence as an exogenous, time-dependent **cognitive capital multiplier** $A \in [1, \infty)$ where:

$$A(t) = A_0 e^{\mu t}, \quad \mu > 0$$

The foundational structural asymmetry of cognitive automation is that **$A$ does not scale symmetrically across organizational size**.

### 3.1 Asymmetric Scaling: Singleton vs. Grand Coalition

#### Proposition 1 (Singleton Leverage Explosion)
*For a singleton agent $S = \{i\}$ (or micro-coalition $|S| \le k$ with $k \ll n$), internal managerial friction is absent ($\tau(\{i\}) \approx 0$). Autonomous agent swarms act as a pure, unencumbered multiplier on individual talent $f_i$:*

$$\tilde{v}_A(\{i\}) = A \cdot f_i$$

*Proof:*  
An isolated builder directly commands deterministic execution pipelines (autonomous code generation, synthesis, design, retrieval). Because there are no interpersonal communication channels ($\binom{1}{2} = 0$), there is no managerial agency loss. Hence, $\tau(\{i\}) = 0$, yielding $\tilde{v}_A(\{i\}) = v_A(\{i\}) = A f_i$. $\blacksquare$

#### Proposition 2 (Corporate Absorption Drag)
*For the Grand Coalition $N$, the technology multiplier is attenuated by an institutional absorption discount $\eta < 1$, while the quadratic coordination overhead $c n^\beta$ remains invariant:*

$$\tilde{v}_A(N) = \eta A \cdot F(N) - c n^\beta = \eta A \gamma \sum_{i=1}^n f_i - c n^\beta$$

*Proof:*  
Enterprise deployment of autonomous intelligence requires multi-layered legal compliance, vendor risk reviews, committee alignment, security guardrails, and middle-management consensus. This institutional friction discounts raw model productivity by factor $\eta \in (0, 1)$. Furthermore, because $n$ human agents must still be governed, compensated, and politically reconciled, the pairwise communication graph $K_n$ retains its super-linear friction $c n^\beta$. $\blacksquare$

---

## 4. The Core Emptiness Theorem

### 4.1 Formal Definitions

Let $x = (x_1, x_2, \dots, x_n) \in \mathbb{R}^n$ denote a payoff distribution (imputation) vector representing salaries, bonuses, and equity allocations.

**Definition 1 (Imputation):**  
A payoff vector $x$ is an imputation if it satisfies:
1. **Efficiency (Budget Balance):** $\sum_{i \in N} x_i = \tilde{v}_A(N)$
2. **Individual Rationality:** $x_i \ge \tilde{v}_A(\{i\}), \quad \forall i \in N$

**Definition 2 (The Core):**  
The Core $\mathcal{C}(N, \tilde{v}_A)$ is the set of all imputations against which no sub-coalition $S \subset N$ can successfully defect (block):

$$\mathcal{C}(N, \tilde{v}_A) = \left\{ x \in \mathbb{R}^n : \sum_{i \in N} x_i = \tilde{v}_A(N) \quad \text{and} \quad \sum_{i \in S} x_i \ge \tilde{v}_A(S), \quad \forall S \subseteq N \right\}$$

If $\mathcal{C}(N, \tilde{v}_A) = \emptyset$, the Grand Coalition is fundamentally unstable: for any proposed corporate compensation policy, at least one coalition can achieve higher payoffs by breaking away.

---

### 4.2 Application of the Bondareva-Shapley Theorem

**Definition 3 (Balanced Collection):**  
A collection of non-empty coalitions $\mathcal{B} \subseteq 2^N \setminus \{\emptyset\}$ is balanced if there exist positive weights $(\lambda_S)_{S \in \mathcal{B}}$ such that:

$$\sum_{S \in \mathcal{B} : i \in S} \lambda_S = 1, \quad \forall i \in N$$

**Theorem (Bondareva 1963; Shapley 1967):**  
*A TU cooperative game $(N, v)$ has a non-empty Core ($\mathcal{C} \neq \emptyset$) if and only if for every balanced collection $(\mathcal{B}, \lambda)$:*

$$\sum_{S \in \mathcal{B}} \lambda_S \tilde{v}(S) \le \tilde{v}(N)$$

---

### 4.3 The Core Emptiness Threshold (Theorem 1)

Consider the canonical balanced collection of all singleton coalitions:

$$\mathcal{B}_{\text{single}} = \big\{ \{1\}, \{2\}, \dots, \{n\} \big\}$$

Since each player belongs to exactly one singleton, the balanced weights are uniquely $\lambda_{\{i\}} = 1$ for all $i \in N$.

Under Bondareva-Shapley, a necessary condition for Core non-emptiness is:

$$\sum_{i=1}^n \tilde{v}_A(\{i\}) \le \tilde{v}_A(N)$$

**Theorem 1 (Coasean Disintegration & Core Emptiness):**  
*Assume agents have symmetric baseline talent endowments $f_i = f_0 > 0$.*
1. *If $\eta \gamma \le 1$ (institutional inertia weakly dominates organizational synergy), the Core is empty for all $A \ge 1$:*
   $$\mathcal{C}(N, \tilde{v}_A) = \emptyset, \quad \forall A \ge 1$$
2. *If $\eta \gamma > 1$ (net positive corporate synergy exists), there exists a finite critical technology threshold:*
   $$A^* \equiv \frac{c n^\beta}{n f_0 (\eta \gamma - 1)}$$
   *such that for all $A > A^*$, the Core of the firm is empty:*
   $$\mathcal{C}(N, \tilde{v}_A) = \emptyset$$

*Proof:*  
From the singleton balancedness condition:

$$\sum_{i=1}^n \tilde{v}_A(\{i\}) = \sum_{i=1}^n A f_i = n A f_0$$

The net value of the Grand Coalition is:

$$\tilde{v}_A(N) = \eta A \gamma (n f_0) - c n^\beta$$

Core non-emptiness requires:

$$n A f_0 \le \eta A \gamma n f_0 - c n^\beta$$

Rearranging terms by isolating the cognitive capital multiplier $A$:

$$c n^\beta \le A \cdot n f_0 (\eta \gamma - 1)$$

**Case 1 ($\eta \gamma \le 1$):**  
If $\eta \gamma \le 1$, the term $(\eta \gamma - 1) \le 0$. Consequently:

$$A \cdot n f_0 (\eta \gamma - 1) \le 0 < c n^\beta$$

Because $c > 0$ and $n \ge 2$, the inequality is violated for all $A \ge 1$. The Core is unconditionally empty.

**Case 2 ($\eta \gamma > 1$):**  
If $\eta \gamma > 1$, we divide both sides by $n f_0 (\eta \gamma - 1) > 0$:

$$A \le \frac{c n^\beta}{n f_0 (\eta \gamma - 1)} \equiv A^*$$

Thus, for any technological state $A > A^*$, the inequality is strictly reversed:

$$\sum_{i=1}^n \tilde{v}_A(\{i\}) > \tilde{v}_A(N)$$

Suppose there exists an imputation $x \in \mathcal{C}(N, \tilde{v}_A)$. By Definition 1, $x$ must satisfy individual rationality ($x_i \ge \tilde{v}_A(\{i\}), \forall i$). Summing over all $i \in N$:

$$\sum_{i=1}^n x_i \ge \sum_{i=1}^n \tilde{v}_A(\{i\}) > \tilde{v}_A(N)$$

This directly contradicts budget balance ($\sum_{i \in N} x_i = \tilde{v}_A(N)$). Therefore, no stable imputation exists:

$$\mathcal{C}(N, \tilde{v}_A) = \emptyset$$

$\blacksquare$

---

### 4.4 The Collapse of the Optimal Coasean Firm Size (Corollary 1.1)

Coase defined the optimal firm size $n^*$ as the point maximizing net organizational surplus per capita.

**Corollary 1.1 (Optimal Firm Size Collapse):**  
*Let the firm choose headcount $n$ to maximize average net surplus:*

$$n^*(A) = \arg\max_{n \ge 1} \left[ \frac{\eta A \gamma n f_0 - c n^\beta}{n} \right] = \arg\max_{n \ge 1} \left[ \eta A \gamma f_0 - c n^{\beta - 1} \right]$$

*Since $\beta > 1$ and $c > 0$, the objective function is strictly decreasing in $n$ for all $n \ge 1$. Thus:*

$$n^*(A) = 1, \quad \forall A \ge 1$$

*Proof:*  
The derivative with respect to $n$ is:

$$\frac{\partial}{\partial n} \left( \eta A \gamma f_0 - c n^{\beta - 1} \right) = -c (\beta - 1) n^{\beta - 2} < 0$$

Because the marginal returns to headcount are strictly negative due to super-linear communication overhead, the unconstrained optimal organizational size collapses to the singleton boundary $n^* = 1$. $\blacksquare$

---

## 5. Microeconomic Dynamics: Shapley Value vs. Wage Compression

Why do corporations dissolve through layoffs rather than voluntary wage adjustments? The microeconomic mechanism lies in the tension between the **Shapley Value** and **institutional wage compression**.

### 5.1 The Shapley Value under AI Leverage

The Shapley Value $\phi_i(\tilde{v}_A)$ measures agent $i$'s expected marginal contribution across all coalition formation orders:

$$\phi_i(\tilde{v}_A) = \sum_{S \subseteq N \setminus \{i\}} \frac{|S|!(n - |S| - 1)!}{n!} \Big[ \tilde{v}_A(S \cup \{i\}) - \tilde{v}_A(S) \Big]$$

For an elite producer endowed with high execution capacity $f_i$, adding them to any coalition $S$ increases the coalition's productivity by $\sim O(A)$. Thus, the agent's theoretical equilibrium wage scales linearly with technological progress:

$$\phi_i(\tilde{v}_A) \propto A \cdot f_i$$

### 5.2 Institutional Wage Compression

Empirical personnel economics (Frank, 1984; Lazear & Shaw, 2007; Baker, Jensen & Murphy, 1988) demonstrates that real-world corporate hierarchies systematically compress wages to prevent internal friction, preserve status equity, and satisfy union or regulatory constraints:

$$w_i = \bar{w} + \theta \big( \phi_i - \bar{w} \big), \quad 0 < \theta \ll 1$$

where $\bar{w}$ is the median corporate wage and $\theta$ is the compression elasticity.

### 5.3 The Defection Gap and the Adverse Selection Spiral (Theorem 2)

We define the **Defection Gap** $\Delta_i(A)$ as the spread between an agent’s autonomous outside option and their corporate wage:

$$\Delta_i(A) \equiv \tilde{v}_A(\{i\}) - w_i = A f_i - \Big[ \bar{w} + \theta(\phi_i - \bar{w}) \Big]$$

Differentiating with respect to the technology parameter $A$:

$$\frac{\partial \Delta_i}{\partial A} = f_i - \theta \frac{\partial \phi_i}{\partial A} \approx (1 - \theta) f_i > 0$$

Since $\theta \ll 1$, **technological progress monotonically expands the Defection Gap for high-talent agents**.

```
    PAYOFF
       │                                     / Standalone Outside Option v_A({i}) = A * f_i
       │                                    /
       │                                   / 
       │                                  /  ← DEFECTION ZONE (Core Emptiness)
       │                                 /
       │                                /   
       │───────────────────────────────/────── Corporate Compressed Wage w_i
       │                              /
       │                             /
       │                            /
       └───────────────────────────/──────────────────────→ TECHNOLOGY MULTIPLIER (A)
                                  A* (Critical Tipping Point)
```

**Theorem 2 (The Adverse Selection Unraveling Spiral):**  
*When $A > A^*$, the firm enters an irreversible unraveling cascade:*
1. *The top tier of producers $S_{\text{exit}} = \{i \in N : \Delta_i(A) > 0\}$ departs to operate as autonomous producers.*
2. *The departure of $S_{\text{exit}}$ reduces gross firm output from $v_A(N)$ to $v_A(N \setminus S_{\text{exit}})$.*
3. *Because corporate bureaucracy $\tau(N)$ cannot contract instantaneously (fixed real estate, compliance overhead, middle management), per-capita administrative cost $\frac{c (n - |S_{\text{exit}}|)^\beta}{n - |S_{\text{exit}}|}$ rises.*
4. *To prevent immediate insolvency, the firm implements broad-based layoffs and salary freezes, which lowers $w_j$ for the second tier of talent.*
5. *This triggers $\Delta_j(A) > 0$ for the remaining median producers, accelerating the liquidation of the firm.* $\blacksquare$

---

## 6. Macroeconomic Integration: Intensive vs. Extensive Margins

Our game-theoretic findings resolve a central debate in contemporary AI macroeconomics: the divergence between Daron Acemoglu’s skepticism and Philippe Aghion’s endogenous growth projections.

### 6.1 The Acemoglu (2024) Intensive Margin Fallacy

Acemoglu (2024, NBER WP 32487) uses Hulten’s Theorem to bound total factor productivity (TFP) gains from AI at $\le 0.66\%$ over 10 years, arguing that only $\approx 4.6\%$ of tasks can be profitably automated.

However, Acemoglu's model operates strictly on the **intensive margin** within existing corporate task allocations:

$$\Delta \ln \text{TFP} \approx \sum_{i \in \text{Automated Tasks}} s_i \cdot \pi_i$$

This assumes that the organizational envelope $N$ remains fixed and that AI only acts as a marginal cost reducer inside legacy corporate boundaries.

### 6.2 The Aghion (2024) Extensive Margin & Idea Production

As Aghion, Antonin, and Bunel (2024) demonstrate, general-purpose technologies operate primarily on the **extensive margin** through the **idea production function** (Romer, 1990):

$$\dot{A} = \delta \cdot (\text{AI})^\gamma \cdot L_A^\lambda \cdot A^\phi$$

When autonomous AI empties the Core of the firm, human capital is not destroyed—it is **ejected into the market**. Displaced knowledge workers establish autonomous micro-enterprises, drastically expanding the number of experimental firms.

Administrative data confirms this structural reallocation:
* **U.S. Census Bureau Business Formation Statistics (BFS):** High-Propensity Business Applications (HBA) jumped from an annual baseline of 1.2M (2010–2019) to sustained record plateaus of **1.8M annually** post-2022.
* **Capital Efficiency Decoupling:** Legacy tech conglomerates (Alphabet, Meta) operate at approximately USD 1.5M to USD 2.0M revenue per employee. In contrast, AI-native micro-firms (e.g., Midjourney with ~40 employees generating USD 300M+ ARR) achieve **over USD 7.5M ARR per employee**, operating with near-zero internal communication friction ($\beta \to 1$).

---

## 7. The Entrepreneurial Distribution: The Reality of the Eagle

While the dissolution of the Coasean firm unleashes autonomous productivity, it also exposes agents to the unmitigated, heavy-tailed distribution of the open market.

A corporate wage was fundamentally a **variance-reduction subsidy**: the firm smoothed cash flow volatility and paid a predictable mean $w_i$ in exchange for expropriating the right-tail upside $\phi_i - w_i$.

When the Core empties and workers are ejected into autonomous production:
1. **Survival Attrition (BLS Data):** 20% of new ventures fail within Year 1, 50% fail by Year 5, and 70% fail by Year 10.
2. **The Hamilton (2000) Earnings Penalty:** In a longitudinal analysis of self-employment, Barton Hamilton (*Journal of Political Economy*, 108(3)) proved that the median entrepreneur earns **35% less** over a 10-year horizon than an identically endowed corporate wage worker. Returns to entrepreneurship follow a heavy-tailed Pareto distribution where the mean is pulled entirely by the top 1% to 2% of right-tail outliers (Hall & Woodward, 2010, *AER*).
3. **The Herbert Simon Attention Bottleneck:** As Herbert Simon (1971) established, *"a wealth of information creates a poverty of attention."* When the marginal cost of production approaches zero ($MC_{\text{production}} \to 0$), markets are flooded with synthetic output. Production ceases to be a moat. Economic rent concentrates entirely in **distribution access, proprietary data pipelines, and verified reputational trust**.

---

## 8. Conclusion

Ronald Coase began his 1937 treatise by noting that economists often treat the economic system as an organism that coordinates itself through prices, while ignoring the managerial islands where conscious direction reigns.

We have demonstrated that the boundary of those managerial islands is governed by a cooperative game whose Core depends on the ratio of human communication friction to autonomous cognitive leverage. When cognitive capital $A$ crosses the threshold $A^*$, the Grand Coalition becomes coalitionally unstable.

The ongoing wave of corporate downsizing is not a temporary macroeconomic aberration. It is the mathematical dissolution of the Coasean firm. As autonomous tools continue their exponential ascent, the corporate manor is yielding to the sovereign producer—a decentralized landscape of atomic builders operating at the frontier of the distribution, bearing the full weight of the market's variance, and capturing its uncapped upside.

---

## References

* **Acemoglu, D.** (2024). "The Simple Macroeconomics of AI." *National Bureau of Economic Research*, NBER Working Paper No. 32487.
* **Aghion, P., Antonin, C., & Bunel, L.** (2024). "AI and Growth: Where Do We Stand?" *Federal Reserve Bank of San Francisco Working Paper Series*.
* **Allen, R. C.** (1992). *Enclosure and the Yeoman: The Agricultural Development of the South Midlands, 1450–1850*. Oxford: Oxford University Press.
* **Aoki, M.** (1984). *The Co-operative Game Theory of the Firm*. Oxford: Oxford University Press.
* **Baker, G. P., Jensen, M. C., & Murphy, K. J.** (1988). "Compensation and Incentives: Practice vs. Theory." *The Journal of Finance*, 43(3), 593–616.
* **Bondareva, O. N.** (1963). "Some Applications of Linear Programming Methods to the Theory of Cooperative Games." *Problemy Kibernetiki*, 10, 119–139.
* **Brenner, R.** (1976). "Agrarian Class Structure and Economic Development in Pre-Industrial Europe." *Past & Present*, 70, 30–75.
* **Brooks, F. P.** (1975). *The Mythical Man-Month: Essays on Software Engineering*. Reading, MA: Addison-Wesley.
* **Coase, R. H.** (1937). "The Nature of the Firm." *Economica*, New Series, 4(16), 386–405. [https://doi.org/10.1111/j.1468-0335.1937.tb00002.x](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1468-0335.1937.tb00002.x)
* **David, P. A.** (1990). "The Dynamo and the Computer: An Historical Perspective on the Modern Productivity Paradox." *The American Economic Review Papers and Proceedings*, 80(2), 355–361.
* **Eloundou, T., Manning, S., Mishkin, P., & Rock, D.** (2024). "GPTs are GPTs: An Early Look at the Labor Market Impact Potential of Large Language Models." *Science*, 384(6702).
* **Epstein, S. R.** (2000). *Freedom and Growth: The Rise of States and Markets in Europe, 1300–1750*. London: Routledge.
* **Frank, R. H.** (1984). "Are Workers Paid Their Marginal Products?" *The American Economic Review*, 74(4), 549–571.
* **Gompers, P., & Lerner, J.** (1999). *The Venture Capital Cycle*. Cambridge, MA: MIT Press.
* **Grossman, S. J., & Hart, O. D.** (1986). "The Costs and Benefits of Ownership: A Theory of Vertical and Lateral Integration." *Journal of Political Economy*, 94(4), 691–719.
* **Hall, R. E., & Woodward, S. E.** (2010). "The Burden of the Nondiversifiable Risk of Entrepreneurship for Venture-Backed Startups." *The American Economic Review*, 100(3), 1163–1194.
* **Hamilton, B. H.** (2000). "Does Entrepreneurship Pay? An Empirical Analysis of the Returns to Self-Employment." *Journal of Political Economy*, 108(3), 604–631.
* **Hart, O., & Moore, J.** (1990). "Property Rights and the Nature of the Firm." *Journal of Political Economy*, 98(6), 1119–1158.
* **Jensen, M. C.** (1993). "The Modern Industrial Revolution, Exit, and the Failure of Internal Control Systems." *The Journal of Finance*, 48(3), 831–880.
* **Lazear, E. P., & Shaw, K. L.** (2007). "Personnel Economics: The Economist's View of Human Resources." *Journal of Economic Perspectives*, 21(4), 91–114.
* **Mendels, F. F.** (1972). "Proto-industrialization: The First Phase of the Industrialization Process." *The Journal of Economic History*, 32(1), 241–261.
* **Polanyi, K.** (1944). *The Great Transformation: The Political and Economic Origins of Our Time*. New York: Farrar & Rinehart.
* **Romer, P. M.** (1990). "Endogenous Technological Change." *Journal of Political Economy*, 98(5), S71–S102.
* **Shapley, L. S.** (1953). "A Value for n-Person Games." *Contributions to the Theory of Games*, 2(28), 307–317.
* **Shapley, L. S.** (1967). "On Balanced Sets and Cores." *Naval Research Logistics Quarterly*, 14(4), 453–460.
* **Simon, H. A.** (1971). "Designing Organizations for an Information-Rich World." In M. Greenberger (Ed.), *Computers, Communications, and the Public Interest* (pp. 37–72). Baltimore: Johns Hopkins Press.
* **Williamson, O. E.** (1975). *Markets and Hierarchies: Analysis and Antitrust Implications*. New York: Free Press.
* **Williamson, O. E.** (1985). *The Economic Institutions of Capitalism*. New York: Free Press.

---

## Citation

If you cite this research or mathematical model, please use the following BibTeX entry:

```bibtex
@article{ozyavuz2026coasean,
  title={Coasean Disintegration: Cooperative Game Theory of the Firm under Autonomous Intelligence},
  author={Ozyavuz, Ogulcan},
  journal={Working Paper, DICE Venture Builder},
  year={2026},
  url={https://github.com/ogulcan-ozyavuz/cooperative-game-theory-of-the-firm}
}
```
