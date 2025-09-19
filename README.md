# SRE / Infra Simulation Lab / Platform Engineer

This repository is a **hands-on infrastructure simulation lab** designed to practice and showcase advanced skills in **Linux, automation, monitoring, networking, high availability, and security**.

---

## 📦 Installation

Clone the repo:

```bash
git clone https://github.com/diegorlopezm/sre-infra-simulation.git
cd sre-infra-simulation/
```
If you are using Docker + Compose:
```bash
cd docker-lab
docker-compose up -d
```
If you want to run Ansible playbooks:
```bash
cd ansible
ansible-playbook -i inventories/dev playbooks/hardening.yml
```

## 🚀 Usage

Use the Docker lab to simulate databases, HAProxy load balancing, stress tests, and failover.

Use Ansible playbooks to practice automation, patching, and security hardening.

Use the Monitoring stack to visualize metrics and set up alerts.

Review security configs to apply TLS, ModSecurity (WAF), and best HTTP headers.

## 📂 Repository Structure
```bash
<repo-name>/
├── README.md
├── docs/
│   ├── questions.md              # Interview-style Q&A
│   ├── architecture-diagram.png  # High-level diagrams (HA, DR, LB)
│   ├── linux-tuning.md           # Performance tuning notes
│   ├── networking-ha.md          # HAProxy + TCP/UDP configs
│   ├── security-ir.md            # Incident response & hardening
│   └── ansible-strategy.md       # How roles/playbooks are structured
├── ansible/
│   ├── inventories/
│   │   ├── dev
│   │   └── prod
│   ├── playbooks/
│   │   ├── hardening.yml
│   │   ├── monitoring.yml
│   │   └── patching.yml
│   └── roles/
│       ├── ssh-hardening/
│       ├── monitoring-agent/
│       └── haproxy/
├── monitoring/
│   ├── prometheus.yml
│   ├── grafana-dashboard.json
│   └── alert-rules.yml
├── docker-lab/
│   ├── docker-compose.yml        # Full infra lab (DB, web, HAProxy, monitoring, stress)
│   ├── haproxy.cfg
│   ├── nginx.conf
│   └── stress-scenarios.md
└── security/
    ├── modsecurity-rules.conf
    ├── tls-config.md
    └── headers-best-practices.md
```
## 🎯 Goal

💡 The goal is to reproduce real-world enterprise challenges (failover, DR, performance bottlenecks, automation at scale) in a controlled environment, while building a portfolio of solutions that reflect how a senior IT Engineer / SRE / DevOps would approach them.

## 🛠️ Next Steps

- [ ] Add more stress scenarios (CPU, RAM, I/O).

- [ ] Expand Ansible roles for PostgreSQL replication & failover.

- [ ] Document incident response runbooks.

- [ ] Add CI/CD pipeline with GitHub Actions for linting + testing.
