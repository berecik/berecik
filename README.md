# **Adam Mańczuk (berecik)**

### **Senior Software Engineer & Systems Architect**

Architecting high-performance concurrent systems in Rust & Python.  
Bridging the gap between robust backends and reactive frontends.

I am a Senior Software Engineer with over **25 years of experience** building scalable infrastructure and application systems. My technical philosophy centers on **Hybrid Architecture**: leveraging Rust's memory safety and raw concurrency for core backend services, while utilizing the ecosystem richness of **Python** and **Flutter** for rapid application logic and cross-platform interfaces.

My work focuses on eliminating architectural entropy through standardization (**dev_skel**) and creating novel bridges between disconnected ecosystems (**flet-django**). I specialize in **Cloud-Native** deployments, orchestrating microservices on **Kubernetes** with a focus on observability and resilience.

---

**🛠 Technology Ecosystem**

| Domain | Core Stack | Proficiency Context |
| :---- | :---- | :---- |
| **Backend Systems** | **Rust** (Actix, Rocket, Tokio) | High-throughput systems, Geospatial processing, Actor-model concurrency. |
| **Application Layer** | **Python** (Django, FastAPI, Celery) | Rapid business logic, AI/LLM orchestration, REST APIs. |
| **Frontend & Mobile** | **Flutter** (Dart), **Flet**, React | Cross-platform native apps (iOS/Android), Internal tooling dashboards. |
| **Infrastructure** | **Kubernetes**, Docker, Helm, Terraform | Infrastructure as Code (IaC), GitOps, CI/CD pipeline automation. |
| **Data & Storage** | PostgreSQL (**PostGIS**), Redis | Spatial indexing, Real-time session state management. |

---

**🚀 Engineering Portfolio**

### **[DAS-SAR] Distributed Aerial Search and Rescue Swarm**
*Role: Lead Developer* | [**GitHub**](https://github.com/berecik/virtual_drone_crowd)

A paradigm-shifting **Fail-Operational Distributed Lift System (DLS)** designed for heavy-lift aerial evacuation. Instead of a single massive aircraft, it utilizes a swarm of autonomous drones tethered to a common payload, enabling extraction from environments inaccessible to conventional helicopters.

*   **Hybrid Stack:** Orchestrates real-time swarm logic using **Rust** for safety-critical controllers and **Python** for high-level mission planning.
*   **Decentralized Communication:** Leverages **Zenoh** and **ROS 2 (Humble/Jazzy)** for low-latency, resilient data distribution between swarm nodes.
*   **Fail-Operational Design:** Implements redundant lift algorithms where the swarm maintains stability and payload altitude even upon individual drone failure.

### **[Swarm Digital Twin] Drone Swarm Simulation & Testing Framework**
*Role: Creator & Lead Architect* | [**GitHub**](https://github.com/berecik/swarm_digital_twin)

A comprehensive digital twin framework for developing and testing autonomous drone swarm behavior without physical hardware. It provides a complete simulation environment for the [DAS-SAR] project, enabling rapid iteration on safety-critical flight algorithms and AI perception.

*   **Multimodal Simulation:** Features standalone **Python-based rigid-body physics** for rapid testing and full **Docker-orchestrated** environments for multi-drone swarm validation.
*   **Safety-Critical Logic:** Implements real-time swarm coordination and distributed lift controllers in **Rust** via **Zenoh** and **ROS 2**.
*   **End-to-End Validation:** Integrates **AI perception pipelines** (YOLOv8/11) with mocked sensors and 3D localization within a synchronized simulation loop.

### **[claude_on_django] Autonomous Development Framework**
*Role: Architect* | [**GitHub**](https://github.com/berecik/claude_on_django)

An autonomous development framework for the **Django-Bolt** ecosystem. It coordinates teams of AI agents to handle full-stack implementation—from models and APIs to tests and deployment—while maintaining extreme performance through Rust integration.

*   **Django-Bolt Integration:** Leverages **Rust-powered API performance** (60k+ RPS via Actix Web + PyO3) within the Django ecosystem.
*   **Multi-Agent Orchestration:** Deploys specialized AI agents to reason over application data and execute complex, multi-layered development tasks.
*   **Full-Cycle Automation:** Automates the generation of Django ORM models, structured JSON schemas, and Flet-based reactive frontends.

### **[flutterkvm] Flutter PiKVM Client**
*Role: Creator* | [**GitHub**](https://github.com/berecik/flutterkvm)

A specialized mobile and desktop client for **PiKVM**, built with **Flutter**. It allows users to manage and control remote servers via PiKVM with a native, high-performance interface.

*   **Cross-Platform:** Provides a consistent experience across Android, iOS, and Desktop.
*   **Low Latency:** Optimized for remote control scenarios where responsiveness is critical.

### **[CityExplorer] AI-Driven Geospatial Platform**
*Role: Full Stack Architect* | [**Live App**](https://cityexplorer.app)

A production mobile application that acts as an intelligent personal tour guide. The system solves the challenge of delivering real-time, location-aware content by combining high-performance geospatial querying with Generative AI.

*   **Rust Actix Backend:** Leverages the **Actor Model** to handle thousands of concurrent WebSocket connections with sub-millisecond latency.
*   **Geospatial Intelligence:** Utilizes **PostGIS** for advanced spatial indexing (R-Tree), enabling efficient "K-Nearest Neighbors" (KNN) queries.
*   **Generative AI Pipeline:** Orchestrates an asynchronous job queue feeding POI data into LLMs to generate unique, context-aware audio stories.

### **[dev_skel] Microservice Scaffolding Engine**
*Role: Architect & Maintainer* | [**GitHub**](https://github.com/berecik/dev_skel)

**dev_skel** is a comprehensive scaffolding and orchestration engine designed to standardize the lifecycle of modern microservices. Born from the necessity to maintain architectural consistency across polyglot environments (Rust/Python), it serves as the foundational "DNA" for high-performance applications.

*   **Polyglot Bootstrapping:** Instantly scaffolds production-ready directory structures for **FastAPI** (Python) and **Actix** (Rust) services, enforcing **Domain-Driven Design (DDD)** principles.
*   **Container Optimization:** Implements advanced **Docker** patterns, including multi-stage builds and distroless images for Rust (<50MB artifacts).
*   **Kubernetes-Native Config:** Automatically generates production-grade **Helm** charts, including pre-configured Readiness/Liveness probes, HPA rules, and Ingress definitions.

### **[flet-django] The Django-Flutter Bridge**
*Role: Creator & Lead Maintainer* | [**PyPI**](https://pypi.org/project/flet-django/) | [**GitHub**](https://github.com/Marysia-Software-Limited/flet-django)

An innovative open-source framework that bridges the gap between **Django's** mature backend ecosystem and **Flutter's** reactive UI capabilities (via Flet). This project solves the "disconnected frontend" problem, allowing Python developers to build rich, native-feeling desktop and mobile apps without writing a single line of JavaScript or Dart.

*   **Architecture:** Runs the Flet engine directly within the Django process. Utilizes custom **Middleware** to upgrade HTTP requests to **WebSockets**, enabling real-time, bi-directional communication.
*   **The GenericApp Pattern:** Implements abstract base classes (`GenericApp`, `GenericView`) that automate the binding of Django Models to Flutter UI controls.
*   **Zero-Boilerplate CRUD:** Features introspection capabilities that analyze Django Models to auto-generate data tables, forms, and list views.

---

**📂 Other Contributions**

*   **[actix-generic-crud](https://github.com/berecik/actix-generic-crud):** A library demonstrating advanced **Rust** capabilities (Traits/Generics) to solve the "boilerplate problem" in web frameworks.
*   **[fastapi-k8s-microservice-template](https://github.com/berecik/fastapi-k8s-microservice-template):** A reference architecture for deploying Python microservices at scale, serving as the public proof-of-concept for the **dev_skel** philosophy.
*   **[tree-sitter-macro](https://github.com/berecik/tree-sitter-macro):** Rust macros for tree-sitter integration, showcasing deep language parsing and manipulation techniques.

---

**📬 Contact**

*   **Email:** beret@hipisi.org.pl  
*   **GitHub:** [github.com/berecik](https://github.com/berecik)
