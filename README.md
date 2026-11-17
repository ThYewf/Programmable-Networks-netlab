# Programmable Networks — Lab Portfolio

This repository contains my practical lab work and assignments for the Programmable Networks course.

The repository follows my Linux lab working directory (`~/netlab`), so files from different weeks may share the same root directory. Generated webpages are organized under `docs/`, while experiment outputs and supporting evidence are stored in their respective evidence directories.

## Lab Portfolio

| Week | Topic | Contents |
|------|-------|----------|
| Week 2 | Network topology and configuration | Topology files, configuration scripts and lab documentation |
| Week 3 | Routing and network troubleshooting | Routing scripts, scenarios, validation and evidence |
| Week 5 | P4 programming | P4 programming work is maintained separately |
| Week 6 | Multi-tenant VXLAN overlay | Hypervisors, tenant isolation, flood-and-learn, MTU validation and performance tests |
| Week 7 | Upcoming coursework | To be added when completed |

## Week 6 — Overlay Your Own Data Centre

The Week 6 assignment implements a multi-tenant data centre using Linux bridges, VXLAN and Mininet.

- Four hypervisors connected through a shared IP underlay.
- Two isolated tenants using VNIs 310 and 420.
- Overlapping tenant IP subnet `10.79.60.0/24`.
- VXLAN flood-and-learn forwarding.
- MTU black-hole detection and two recovery approaches.
- Experimental evidence collected from ping, tcpdump, bridge FDB and iperf3.

### Week 6 Files

| File or directory | Description |
|-------------------|-------------|
| `build_overlay.py` | Network builder and VXLAN configuration |
| `overlay.yaml` | Final working design |
| `blackhole.yaml` | Deliberately unsafe MTU design |
| `mtu_a.yaml` | Fix A: tenant MTU 1450 |
| `mtu_b.yaml` | Fix B: jumbo underlay MTU 9000 |
| `page6.yaml` | Written assignment answers |
| `make_page6.py` | HTML page generator |
| `evidence6/` | Experiment results |
| `docs/week6/` | Generated assignment webpage |

[View Week 6 assignment page](https://thyewf.github.io/Programmable-Networks-netlab/week6/)

## AI Usage Declaration

**AI Use Level: 3 — Open**

I used ChatGPT (OpenAI) as a learning and development assistant during the coursework.

AI assistance included explaining networking concepts, discussing implementation approaches, reviewing Python and YAML configurations, suggesting test commands, interpreting experimental results, and helping draft and improve written explanations.

The network design decisions, lab execution, testing, verification and experimental evidence were carried out by me. I reviewed the AI-assisted code and written material and remain responsible for understanding, explaining and defending the submitted work.

AI-generated suggestions were checked against the actual lab environment and measured results before being included in the assignment.
