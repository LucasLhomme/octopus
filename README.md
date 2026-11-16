# Octopus — Infrastructure as Code with Ansible

[![Epitech: Tek2](https://img.shields.io/badge/Epitech-Tek2-005696.svg)](https://www.epitech.eu/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)


A DevOps project centered on **Ansible** and **infrastructure as code**: automatically
deploying a multi-service polling application across **5 machines**, without containers,
purely through automation.

Built as part of the Epitech curriculum (DOP-400 module).

## 🏗️ Deployed application

A distributed voting app made of several services:

- **Poll** (Python / Flask) — front-end collecting the votes
- **Redis** — in-memory queue for incoming votes
- **Worker** (Java) — consumes votes from Redis and writes them to PostgreSQL
- **PostgreSQL** — persistent storage
- **Result** (Node.js) — front-end displaying live results

## ✨ Features

- 🤖 Configuration management with Ansible (playbooks, roles, inventory)
- 🖥️ Deployment across 5 target VMs described declaratively (desired state)
- 📦 One dedicated role per component (Poll, Redis, Worker, Postgres, Result)
- ♻️ Reproducible, scalable, container-free deployment

## 🚀 Usage

```bash
source venv/bin/activate
ansible-playbook -i production playbook.yml
```

## 🛠️ Tech stack

Ansible · Flask · Redis · Java · PostgreSQL · Node.js

## 🧠 What I learned

Automating deployment to eliminate human error — describing *what the machines should be*
rather than configuring them by hand. The essence of DevOps.

---

*Project built as part of the Epitech curriculum (DOP-400 module).*
