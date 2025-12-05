# **Adam Mańczuk (berecik)**

### **Senior Software Engineer & Systems Architect**

Architecting high-performance concurrent systems in Rust & Python.  
Bridging the gap between robust backends and reactive frontends.

I am a Senior Software Engineer with over **25 years of experience** building scalable infrastructure and application systems. My technical philosophy centres on **Hybrid Architecture**: leveraging Rust's memory safety and raw concurrency for core backend services, while utilising the ecosystem richness of **Python** and **Flutter** for rapid application logic and cross-platform interfaces.

My work focuses on eliminating architectural entropy through standardisation (dev\_skel) and creating novel bridges between disconnected ecosystems (flet-django). I specialise in **Cloud-Native** deployments, orchestrating microservices on **Kubernetes** with a focus on observability and resilience.

## ---

**🛠 Technology Ecosystem**

| Domain | Core Stack | Proficiency Context |
| :---- | :---- | :---- |
| **Backend Systems** | **Rust** (Actix, Rocket, Tokio) | High-throughput systems, Geospatial processing, Actor-model concurrency. |
| **Application Layer** | **Python** (Django, FastAPI, Celery) | Rapid business logic, AI/LLM orchestration, REST APIs. |
| **Frontend & Mobile** | **Flutter** (Dart), **Flet**, React | Cross-platform native apps (iOS/Android), Internal tooling dashboards. |
| **Infrastructure** | **Kubernetes**, Docker, Helm, Terraform | Infrastructure as Code (IaC), GitOps, CI/CD pipeline automation. |
| **Data & Storage** | PostgreSQL (**PostGIS**), Redis | Spatial indexing, Real-time session state management. |

## ---

**🚀 Engineering Portfolio**

### **\[dev\_skel\] Microservice Scaffolding Engine**

*Role: Architect & Maintainer* | *Status: Internal / Tooling*

**dev\_skel** is a comprehensive scaffolding and orchestration engine designed to standardise the lifecycle of modern microservices. Born from the necessity to maintain architectural consistency across polyglot environments (Rust/Python), it serves as the foundational "DNA" for high-performance applications. It represents a shift from manual configuration to "Platform as Code."

**Core Architectural Features:**

* **Polyglot Bootstrapping:** Instantly scaffolds production-ready directory structures for **FastAPI** (Python) and **Actix** (Rust) services. It enforces **Domain-Driven Design (DDD)** principles, separating domain logic from transport layers (HTTP/gRPC) from day one.  
* **Container Optimisation:** Implements advanced **Docker** patterns, including multi-stage builds that utilise distroless images for Rust (resulting in \<50MB artefacts) and optimised slim images for Python, minimising the security attack surface.  
* **Kubernetes-Native Config:** Automatically generates production-grade **Helm** charts and raw manifests, including pre-configured Readiness/Liveness probes, **HPA** (Horizontal Pod Autoscaling) rules, and Ingress definitions tailored for NGINX controllers.  
* **CI/CD Pipeline Generation:** Injects battle-tested workflow configurations (GitHub Actions/GitLab CI) covering:  
  * **Linting/Formatting:** clippy, rustfmt, black, isort.  
  * **Security Scanning:** Container vulnerability scans and dependency auditing (cargo audit, bandit).  
  * **Automated Deployment:** GitOps-ready manifest updates.

### ---

**\[flet-django\] The Django-Flutter Bridge**

*Role: Creator & Lead Maintainer* | [**PyPI**](https://pypi.org/project/flet-django/) | [**GitHub**](https://github.com/Marysia-Software-Limited/flet-django)

An innovative open-source framework that bridges the gap between **Django's** mature backend ecosystem and **Flutter's** reactive UI capabilities (via Flet). This project solves the "disconnected frontend" problem, allowing Python developers to build rich, native-feeling desktop and mobile apps without writing a single line of JavaScript or Dart.

**Technical Deep Dive:**

* **Architecture:** The framework runs the Flet engine directly within the Django process. It utilises a custom **Middleware** (UrlsMiddleware) to intercept HTTP requests and upgrade them to **WebSocket** connections, enabling real-time, bi-directional communication between the Python backend and the Flutter UI shell.  
* **The GenericApp Pattern:** Implements a set of abstract base classes (GenericApp, GenericView) that automate the binding of Django Models to Flutter UI controls.  
* **Zero-Boilerplate CRUD:** Features introspection capabilities that analyse Django Models to auto-generate data tables, forms, and list views, reducing the development time for internal tools by an order of magnitude.  
* **Roadmap:** Includes plans for AuthMiddleware to map Django's permission system to UI visibility states seamlessly.

### ---

**\[CityExplorer\] AI-Driven Geospatial Platform**

*Role: Full Stack Architect* | (https://cityexplorer.app)

A production mobile application that acts as an intelligent personal tour guide. The system solves the challenge of delivering real-time, location-aware content to users moving through physical space by combining high-performance geospatial querying with Generative AI.

**System Architecture:**

* **Rust Actix Backend:** The core is built on **Rust** using the **Actix** framework. It leverages the **Actor Model** to handle thousands of concurrent WebSocket connections, allowing the server to process location updates from moving users with sub-millisecond latency and zero Garbage Collection pauses.  
* **Geospatial Intelligence:** Utilises **PostGIS** for advanced spatial indexing (R-Tree), enabling efficient "K-Nearest Neighbours" (KNN) queries to identify points of interest within a dynamic walkable radius.  
* **Generative AI Pipeline:** Orchestrates an asynchronous job queue that aggregates POI data and feeds it into Large Language Models (LLMs) to generate unique, context-aware audio stories.  
* **UX Engineering:** Implements optimistic UI patterns and "loading states" (the 'writing girl' metaphor) to mask the inherent latency of AI generation, ensuring a fluid user experience.

### ---

**\[actix-generic-crud\] Rust Abstract Controller**

*Role: Creator* | [**GitHub**](https://github.com/berecik/actix-generic-crud)

A library demonstrating advanced **Rust** capabilities, specifically focusing on **Traits** and **Generics** to solve the "boilerplate problem" in statically typed web frameworks.

* **Data-Agnostic Design:** Provides a generic CrudController that can interface with any storage backend (SQL, NoSQL, In-Memory) that implements the defined Repository traits.  
* **Type System Mastery:** Demonstrates how to leverage Rust's zero-cost abstractions to create reusable web components that do not sacrifice runtime performance.

### ---

**\[fastapi-k8s-microservice-template\]**

*Role: Architect* | [**GitHub**](https://github.com/berecik/fastapi-k8s-microservice-template)

A reference architecture for deploying Python microservices at scale, serving as the public proof-of-concept for the dev\_skel philosophy.

* **Features:** Full **Kubernetes** integration, asynchronous database drivers (Motor/AsyncPG), structured JSON logging for ELK stack integration, and OpenTelemetry instrumentation.

## ---

**📬 Contact**

* **Email:** beret@hipisi.org.pl  
* **GitHub:** [github.com/berecik](https://github.com/berecik)