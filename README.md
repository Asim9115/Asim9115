# Hi, I'm Asim Khan

I'm a final-year Computer Engineering student interested in **backend engineering, systems, databases, and cloud infrastructure**.

I mostly build with **Go and Python**, and I like working on projects where understanding what happens underneath the abstraction actually matters.

Currently exploring **concurrency, database internals, Linux, containers, and distributed systems**.

---

## What I'm Building

### Containerix — Mini PaaS

**Go · Gin · Docker · Linux cgroup v2 · SQLite · SSE**

A self-hosted PaaS that takes a GitHub repository and turns it into a running application.

The project started from a simple question:

> **What actually happens inside platforms like Render when I deploy a GitHub repository?**

That led me from a basic `clone → build → run` prototype into a deployment system handling:

* asynchronous deployment jobs
* Docker image building and container lifecycle management
* persistent deployment state
* CPU and memory isolation using Linux cgroup v2
* build and runtime log streaming using SSE
* port allocation and container tracking
* startup reconciliation after crashes

**→ [View Containerix](https://github.com/Asim9115/containerix)**

---

### StockGuard — Concurrent Inventory Backend

**Go · PostgreSQL**

A backend built around one problem:

> **What happens when multiple requests try to buy the same inventory at the same time?**

Instead of treating concurrency as an afterthought, the project focuses on database-level correctness:

* optimistic locking to prevent overselling
* deterministic lock ordering to avoid deadlocks
* atomic inventory and order updates using PostgreSQL transactions
* bounded retries with jittered backoff
* layered handler → service → repository architecture
* interface-based dependency injection

The goal is less about building another CRUD API and more about understanding **concurrency and transactional correctness**.

---

### VirtualStox — Stock Market Simulator

**React · Django REST Framework · PostgreSQL · Socket.IO · scikit-learn**

A virtual trading platform built to simulate some of the constraints of a real trading system.

The interesting parts include:

* concurrent BUY/SELL transaction handling
* PostgreSQL row locking with `select_for_update()`
* JWT authentication and portfolio-scoped access
* real-time market updates
* market-hours and slippage validation
* Random Forest predictions using technical indicators
* 210K+ OHLCV records across 42 NSE stocks

---

## Things I Like Working On

```text
Backend systems
      ↓
Databases & transactions
      ↓
Concurrency & synchronization
      ↓
Linux & containers
      ↓
Cloud infrastructure
```

I'm particularly interested in understanding the trade-offs behind systems rather than only using the frameworks that sit on top of them.

---

## Problem Solving

* 340+ LeetCode problems
* Top 100 / 600 — DSA Competition, ACM RAIT Nerul
* 1st Prize — Build vs Break Competition, AIKTC

---

## Currently Learning

* Distributed systems
* Backend system design
* Database internals
* Linux internals
* Containerization
* Cloud infrastructure

---

## Find Me

[LinkedIn](https://linkedin.com/in/asim9115) · [Email](mailto:khanasimali20@gmail.com)
