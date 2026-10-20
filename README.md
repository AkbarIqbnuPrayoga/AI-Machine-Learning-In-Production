# Practical AI in Industry

Presentation slides and reference materials bridging academic machine learning and production AI systems.

## Repository Contents

- `presentation.html` - Standalone interactive presentation with built-in presenter notes, navigation controls, and timer (can be opened directly in any modern web browser).
- `presentation.md` - Source slide deck formatted for Marp, containing the slide contents, custom CSS styling, and detailed speaker notes.

## Topics Covered

### Business Objectives of AI
In production, AI is rarely about standalone demos or chasing isolated metric increments; it operates as an automated service making millions of decisions daily to deliver measurable business impact:
- **Cost Reduction**: Automating repetitive operations such as customer support, moderation, and data entry.
- **Revenue Growth**: Driving conversions through personalized search ranking, dynamic pricing, and cross-sell recommenders.
- **Customer Experience**: Delivering fast, contextual, and low-latency interactions that improve user retention.

### Real-World Case Studies (E-Commerce & OTA)
Concrete industry implementations demonstrating how machine learning solves business challenges:
- **Search Autocomplete & Ranking**: Predicting user search queries in real time and ordering flight or hotel results to optimize conversion and relevance.
- **Cross-Sell Recommendations**: Suggesting complementary products (e.g., hotel recommendations alongside flight bookings).
- **Automated Content & Review Processing**: Categorizing sentiment, tagging feedback topics, and filtering low-quality images at scale.
- **Customer Care Automation**: 24/7 intelligent chatbots and personalized, event-triggered communication across channels.

### The Reality of ML Engineering (~80/20 Rule)
A critical mindset shift for students transitioning from academia to industry:
- In coursework and competitions, training the model is the finish line. In industry, a trained model is only the starting line.
- Model architecture and training account for roughly **10–20%** of the work.
- The remaining **80%** is disciplined software engineering: data validation, automated ETL pipelines, containerization, API development, integration testing, and production monitoring.

### Service Deployment Patterns
How AI capabilities are architected and delivered depending on business constraints:
- **Synchronous (Real-time)**: Low-latency endpoints (using FastAPI, Redis, or gRPC) serving predictions immediately upon user requests (e.g., search autocomplete).
- **Asynchronous (Batch)**: High-throughput offline scoring across large datasets (e.g., scoring millions of catalog items overnight using Airflow or Spark).
- **Scheduled & Event-driven**: Recurring background pipelines handling scheduled model retraining, data quality checks, and performance drift monitoring.

### Modern Industry Tech Stack
The standard infrastructure and tools utilized across production systems:
- **Cloud & Orchestration**: AWS, GCP, Azure, Kubernetes, Consul, Vault, and ArgoCD.
- **Databases & Vector Stores**: PostgreSQL, MongoDB, Redis, Milvus, and FalkorDB for semantic search and RAG workflows.
- **Data Pipelines**: Apache Airflow, Kubeflow, dbt, Apache Beam, and Google Dataflow.
- **MLOps & LLMOps**: MLflow for experiment tracking and model registries, AI Gateways for API management and routing, and prompt versioning.
- **Serving & Application**: Python, uv, FastAPI, Pydantic, and Docker.
- **Observability**: Prometheus, Grafana, and Kibana for logging, latency monitoring, and alerting.

### Career Preparation & Practical Advice
Actionable recommendations for students preparing to enter the field:
- **Master Software Engineering Fundamentals**: Solid grasp of data structures, algorithms, and SQL is far more durable than chasing fleeting tool trends.
- **Fluency in Baseline Tooling**: Git, Docker, and the Linux command line are essential requirements from day one.
- **Build End-to-End Projects**: Go beyond Jupyter notebooks. Collect data, train a model, package it into Docker, expose it via a FastAPI endpoint, and deploy it to a live cloud service.
- **Prioritize Real Experience**: Internships provide invaluable exposure to production constraints, code reviews, and cross-functional team dynamics.
- **Communication & Growth Mindset**: Develop the ability to articulate technical trade-offs clearly to non-technical stakeholders.

## Attribution

- **Speaker**: Setia Budi (Machine Learning Engineer at tiket.com)
- **Topic**: A Brief Story of AI Implementation in Industry

## License

This project is licensed under the [GNU General Public License v3.0](LICENSE).