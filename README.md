# ☸️ Kubernetes & Containers Interactive Digital Textbook & Simulator

A 100% self-contained, highly visual, explorable digital textbook and interactive simulator designed to demystify Kubernetes architecture, container networking, scheduling algorithms, and cluster resiliency for beginners and certification candidates.

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Kubernetes](https://img.shields.io/badge/Kubernetes-1.30+-326CE5?logo=kubernetes&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-v3.0+-38BDF8?logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla%20ES6+-F7DF1E?logo=javascript&logoColor=black)\n![Visitors](https://api.visitorbadge.io/api/visitors?path=akshaycolombus%2FKubernetes_Containers_Simulator&label=VISITORS&countColor=%2322d3ee)

---

## 🌟 Interactive Simulators Included

### 1. 🌐 Multi-Tier Request Lifecycle & Wireshark Dissector
- **3 Dynamic Traffic Scenarios**:
  - `Cloud LoadBalancer & NodePort (:31456)`
  - `L7 Ingress Controller (Host/Path Routing)`
  - `East-West Microservice (Intra-cluster Pod-to-Pod VIP via CoreDNS)`
- **Live Wireshark-Style Packet Dissector**: Layer 3 (IP), Layer 4 (TCP), Layer 7 (HTTP URI & Headers), and NAT state.
- **Kernel iptables / IPVS Translation Table**: Real-time PREROUTING and DNAT rule matching with chosen pod IPs.
- **Pod Fault Modifiers**: Readiness probe fail toggle (pulled from EndpointSlice) and HTTP 500 error injection.
- **10-Orb Burst Stream & Speed Controls**: Slow-Mo (0.5x), Normal (1.0x), and Fast (2.0x).

### 2. 🗂️ Dual-View Topology & Reactive Cluster Scaling Sandbox
- **Replica Stepper (1 to 6 Pods)**: Dynamically scales workloads and places them on physical worker nodes.
- **Anti-Affinity Constraint Enforcement**: Spreads 1 pod per physical VM; marks surplus pods as `Pending`.
- **Hardware Capacity Gauges**: Real-time CPU and RAM allocation meters per worker node.
- **Twin Pod Cross-Link Highlighting**: Hovering over any logical pod highlights its physical VM host.

### 3. ⚙️ Scheduler Decision Engine (Filter & Score Playground)
- **Configurable Pod Specifications**: CPU requests, RAM requests, NodeSelectors (`disk=ssd`, `region=us-east`), and GPU Tolerations.
- **Stage 1 (Predicates / Filtering)**: Evaluates candidate nodes with stamped disqualification rationale.
- **Stage 2 (Priorities / Scoring)**: Ranks surviving nodes with resource balance and Image Locality bonuses.
- **Binding & CRI Stream**: Winner trophy assignment and simulated containerd gRPC socket calls.

### 4. 💥 Cluster Failure & Chaos Engineering Sandbox
- **8 Outage Scenarios**:
  - `CrashLoopBackOff` (Exponential backoff 10s -> 20s)
  - `OOMKilled` (Memory cgroup limit exceeded, Exit 137)
  - `Readiness Failure` (Endpoints exclusion)
  - `Liveness Failure` (Forced container kill & restart)
  - `Worker Node Power Loss` (Heartbeat timeout & pod eviction)
  - `Node Drain` (`kubectl drain`)
  - `Control Plane Outage` (Proves data plane survivability)
- **Automated Chaos Monkey**: Fault injection loop with live SLA uptime percentage.
- **Dual-Tab CLI Output**: `$ kubectl get pods -o wide` and `$ kubectl describe & events`.

### 5. 🧠 10-Card Spaced Repetition Misconception Buster Deck
- 10 exam-grade Kubernetes misconceptions covering Services, Deployments, NodePorts, Pause container namespaces, ephemeral IPs, and resource limits.
- Spaced repetition self-rating (`Needs Review` vs `Mastered ✓`) with `localStorage` persistence.
- Category filters: All, Networking, Architecture, and Workloads.

### 6. 📝 Diagnostic Knowledge Check & 30-Term CLI Reference
- Diagnostic scenario-based quiz with instant feedback and chapter remediation links.
- 30-term searchable glossary with 1-click copyable `kubectl` cheat-sheet commands.

---

## 🚀 Quick Start (Zero Build Steps)

No Node.js, npm, or build tools are required. Simply open `index.html` in any modern web browser:

```bash
# Clone the repository
git clone https://github.com/akshaycolombus/Kubernetes_Containers_Simulator.git

# Navigate into the project
cd Kubernetes_Containers_Simulator

# Open in default browser (Windows)
start index.html

# Open in default browser (macOS)
open index.html

# Open in default browser (Linux)
xdg-open index.html
```

---

## 🎨 Design System & Technologies

- **Design Framework**: Tailwind CSS (via CDN).
- **Typography**: Inter (UI) & JetBrains Mono (Code/CLI) via Google Fonts.
- **Iconography**: FontAwesome 6.4.
- **Vector Graphics**: Dynamic SVG cubic bezier network cables.
- **Physics Engine**: Vanilla JavaScript hardware-accelerated transforms.
- **Storage**: Browser `localStorage` for quiz scores and flashcard mastery.

---

## 📄 License
MIT License. Open source for educators, students, and engineers.
