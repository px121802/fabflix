# Fabflix — E-Commerce Movie Website

Fabflix is a **full-stack e-commerce web application** that allows users to search movies, view details, and simulate transactions.  
Originally developed as part of **CS122B at UC Irvine**, the project emphasizes **scalable architecture, secure transactions, cloud deployment, and high-performance benchmarking**.

This project was developed collaboratively with a teammate.  
My primary contributions included:  
- **Cloud Deployment (AWS EC2)**: Deployed the application onto AWS EC2 instances, configuring the environment, networking, and database connectivity for production-ready hosting.  
- **Infrastructure & Orchestration**: Set up and configured a Kubernetes cluster with YAML-based deployments, pod auto-scaling, and load balancing across worker nodes.  
- **Backend Development**: Enhanced REST APIs and database integration using prepared statements for secure queries.  
- **Performance Testing**: Designed and executed JMeter load tests, analyzed throughput, and optimized scaling strategies.  

---


## Demo
[Watch the demo on YouTube](https://youtu.be/Om9qPv4aE9A)  

---


## Features
- **Movie Search & Browsing**: AJAX-powered search with filters and responsive results  
- **User Authentication & Security**
  - Session-based login system
  - Google reCAPTCHA integration
  - SQL injection prevention via prepared statements
- **Transaction Simulation**: Add movies to cart, checkout flow, and order persistence  
- **Performance & Scalability**
  - Deployed on a Kubernetes cluster with pod auto-scaling
  - Load balancing across worker nodes
  - Benchmarking with JMeter for throughput and stress testing

---

##  System Architecture
- **Frontend**: HTML, CSS, JavaScript, AJAX  
- **Backend**: Java Servlets, REST APIs  
- **Database**: MySQL with Master–Slave replication  
- **Infrastructure**:
  - Kubernetes cluster (1 control plane, multiple worker nodes)
  - Deployment via YAML configurations
  - Pod auto-scaling with horizontal scaling policies
- **Build Tool**: Maven (WAR packaging, dependency management)

---

## Performance Highlights
| Cluster Setup                                | Throughput (transactions/sec) |
|----------------------------------------------|-------------------------------|
| 1 CP + 3 Workers + 2 Fabflix Pods            | ~219.5 tps                   |
| 1 CP + 4 Workers + 3 Fabflix Pods            | ~223.0 tps                   |

- High concurrency tested with **Apache JMeter**  
- Increased pods/nodes yielded incremental throughput gains  
- Demonstrates scalability of containerized deployment

