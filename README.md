<h1 align="center">Hi, I'm Akshay 👋</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1000&center=true&vCenter=true&width=600&lines=Computer+Engineering+%40+HKU;Quant+%2B+Machine+Learning+%2B+Hardware;Building+a+computer+from+scratch%2C+eventually." alt="Typing SVG" />
</p>

---

> Computer Engineering @ The University of Hong Kong · quant, ML, and hardware, in roughly that order on a good day

Indian by passport, raised across Dubai and Oman, now building things in Hong Kong. I am a Computer Engineering undergraduate at HKU on a full-tuition scholarship, working where **quantitative finance, machine learning, and hardware** overlap. I am drawn to problems that refuse to stay in one discipline, and I am slowly building toward the one project that ties all three together: a computer from scratch, from a Verilog CPU up to an ML accelerator.

Research assistant by day, aspiring quant by night, reformed distro-hopper at all hours.

<br />

<table>
<tr>
<td width="33%" valign="top">

**Hardware**

```verilog
module akshay (
  input  clk,
  output reg silicon
);
  // Altium PCBs, VESC
  // shields, FPGAs, and a
  // plan to build a CPU
  // from the gates up.
  always @(posedge clk)
    silicon <= 1'b1;
endmodule
```

</td>
<td width="33%" valign="top">

**Quant**

```python
def edge(signals):
    # 6 alphas, HMM regimes,
    # Black-Litterman + HRP,
    # VaR/CVaR. Built right,
    # whatever the PnL did.
    return optimise(
        blend(signals)
    )
```

</td>
<td width="33%" valign="top">

**ML / AI**

```python
def answer(query):
    # hybrid retrieval, LLM
    # rerank, generate; under
    # a hard latency budget.
    hits = semantic(query) \
         + keyword(query)
    ctx = rerank(hits)[:k]
    return generate(query,
                    ctx)
```

</td>
</tr>
</table>

---

### 🛠️ What I actually work on

**Quantitative & computational finance**
Multi-signal alpha engines with three-state HMM regime detection, Black-Litterman and Hierarchical Risk Parity portfolio optimisation, and VaR/CVaR risk management; plus discounted-cash-flow and probability-weighted valuation work. Mostly crypto, often over windows short enough that the results are noise more than signal, all of it engineered properly regardless of what the PnL did. Incoming Summer Analyst at **Caerus Global Management** via the Asia Quant Academy programme.

Portfolios in that work are scored against a single composite objective, weighting downside-adjusted, total, and drawdown-adjusted return:

$$\text{Score} = 0.4 \cdot \text{Sortino} + 0.3 \cdot \text{Sharpe} + 0.3 \cdot \text{Calmar}$$

where each ratio compares excess return $(R_p - R_f)$ against a different notion of risk:

$$\text{Sharpe} = \frac{R_p - R_f}{\sigma_p} \qquad \text{Sortino} = \frac{R_p - R_f}{\sigma_d} \qquad \text{Calmar} = \frac{R_p - R_f}{\lvert \text{MDD} \rvert}$$

with $\sigma_p$ the total volatility, $\sigma_d$ the downside deviation, and $\text{MDD}$ the maximum drawdown.

**Machine learning & AI systems**
Retrieval-augmented generation done with intent: LLM reranking, query decomposition, hybrid keyword-and-semantic retrieval, and latency budgets that actually hold under load. Multi-agent systems, computer vision with YOLO, and an old soft spot for computational chemistry (I once solved the hydrogen atom from first principles and rendered the orbitals in Blender).

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/rag-pipeline-dark.svg" />
    <img src="assets/rag-pipeline-light.svg" alt="RAG pipeline: a query is decomposed, retrieved over semantic and keyword channels, fused and reranked into a top-k context, then passed to an LLM to generate a grounded answer, under a sub-25s latency budget." width="100%" />
  </picture>
</p>

**Hardware & electronics**
Buck and boost converters, VESC shields, and PCB design in Altium; the FPGA and computer-architecture half of the degree; soldering, with the small burn hole in one finger to show for it. The long game is the build-it-all-from-silicon project that makes the other two tracks honest:

```text
   ┌─────────────────────────────────────────────┐
   │  ML accelerator         (GPU / systolic array)│
   ├─────────────────────────────────────────────┤
   │  OS  ·  scheduler  ·  memory management       │
   ├─────────────────────────────────────────────┤
   │  ISA  ·  assembler  ·  toolchain              │
   ├─────────────────────────────────────────────┤
   │  CPU  ·  ALU  ·  registers     (Verilog/VHDL) │
   ├─────────────────────────────────────────────┤
   │  logic gates  ·  silicon       (first floor)  │
   └─────────────────────────────────────────────┘
            building upward, one layer at a time
```

---

### ⚡ Currently

- **Research Assistant @ HKU InnoWing**: an advanced RAG system over the InnoWings knowledge base, and a multi-agent moot-court simulator for law students (now growing a voice interface)
- Co-authoring a paper on **AI in urban planning**, grown out of a coursework methodology that turned out to be thorough enough to publish
- Four active research assistantships across LLMs, DFT simulation, and more, with publications as the goal
- Getting genuinely, properly good at C++, the one language I dodged for too long

### 🏅 A few things along the way

- One of 36 nationally selected for the **Research Science Initiative** at IIT Madras; one of 50 internationally for **Columbia's Roaring Cubs Collective** (published there on AI road-damage detection)
- **Top 10 / 105+ teams** at the HKU Web3 Quant Trading Hackathon · semi-finalist at Venture Capital On Campus and Alibaba JumpStarter ZPIRE
- International Research Olympiad 2025, Global Rank 191
- AI Trainee at **RAICOM** and Electronics Team at **ROBOCON** at HKU, because someone has to keep both halves of "Computer Engineering" busy

---

### 🧰 Toolbox

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![MATLAB](https://img.shields.io/badge/MATLAB-0076A8?style=for-the-badge&logo=mathworks&logoColor=white)


---

<p align="center"><i>"Your right is to action alone, never to its fruits; let not the fruits of action be your motive."</i><br/>Bhagavad Gita, 2.47</p>

---

### 🔗 Find me

<p align="left">
  <a href="https://www.linkedin.com/in/akshaytp-b8a50a243/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:akshaytp@connect.hku.hk">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>

> Repos to be pinned and linked soon. A fair amount of the work above currently lives in collaborators' repositories.
