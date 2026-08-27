# 🤝 Contributing to Kubernetes & Containers Interactive Simulator

Thank you for your interest in contributing! This project is an open-source, community-driven educational platform designed to make Kubernetes, container runtimes, and cloud-native architecture intuitive and accessible to everyone.

---

## 🚀 How Can You Help?

We welcome all kinds of contributions:
- 💡 **New Simulators & Visualizers**: Build new interactive models (e.g. Istio Service Mesh, CSI Storage Drivers, Helm Rollouts, HPA Scaling).
- 🎨 **UI/UX & Accessibility Enhancements**: Improve animations, color contrast, responsive layouts, and tactile keyboard controls.
- 📖 **Pedagogical Content & Deep Dives**: Expand explanation cards, add real-world troubleshooting scenarios, or refine mental models.
- 🧪 **Bug Fixes & Performance**: Optimize CSS/SVG rendering, resolve edge cases in state machines, or enhance browser compatibility.
- 🌐 **Translations**: Help translate the textbook and quiz questions into different languages.

---

## 🛠️ Getting Started (Local Development)

This project has **Zero Build Steps**! You do not need Node.js, npm, or compilers:

1. **Fork the repository** on GitHub by clicking the **Fork** button at the top right.
2. **Clone your fork** to your local machine:
   ```bash
   git clone https://github.com/<your-username>/Kubernetes_Containers_Simulator.git
   cd Kubernetes_Containers_Simulator
   ```
3. **Create a new feature branch**:
   ```bash
   git checkout -b feature/awesome-new-simulator
   ```
4. **Make your changes** directly in `index.html`.
5. **Test in your browser**: Simply double-click `index.html` or open it in Chrome / Firefox / Edge / Safari. Verify all simulators and animations run smoothly at 60fps.

---

## 📥 Submitting a Pull Request (PR)

1. **Commit your changes**:
   ```bash
   git add .
   git commit -m "feat(simulator): add Istio Envoy sidecar proxy flow"
   ```
2. **Push to your fork**:
   ```bash
   git push origin feature/awesome-new-simulator
   ```
3. **Open a Pull Request**:
   - Go to `https://github.com/akshaycolombus/Kubernetes_Containers_Simulator`
   - Click **Compare & pull request**.
   - Describe what your change does, why it helps learners, and include screenshots if relevant.

---

## 📜 Code & Design Guidelines
- **Single-File Principle**: Keep the textbook 100% self-contained in `index.html` using CDN resources.
- **Semantic Colors**: Follow the Kubernetes architecture color palette (Control Plane: Indigo, Worker Nodes: Emerald, Workloads: Blue, Pods: Amber, Services: Cyan, Errors: Rose).
- **Smooth Animations**: Use hardware-accelerated CSS transforms (`transform`, `opacity`) and standard cubic bezier easing.

Thank you for helping build the future of visual cloud-native education!
