# DevSecOps Roadmap — Session Tracker

*Medium → Hero. No timeframes: move on when the current thing is boring, not when a calendar says so.*

> ⭐ = required milestone post. 📣 = optional extra post.

## How to use this tracker

- **One session = one sitting** (one day if you work 6 days a week). Each session groups the boxes that belong together, and a phase spans several sessions.
- **Tick a box only when you've done the task,** not when you've watched a tutorial about it.
- **Finish a session before starting the next.** If one runs long, finish it tomorrow rather than skipping ahead.
- **Phase 11 is pick 2–3 projects,** so you won't do all 14 of its sessions.
- Post when a phase is done, using the template in the appendix.

---

## 🗺️ Overall Progress

- [ ] **Phase 0** — Workbench set up *(Session 1)*
- [ ] **Phase 1** — Linux core *(Sessions 2–7)*
- [ ] **Phase 2** — Secure the box (networking essentials, SSH, firewall, services, packages) *(Sessions 8–13)*
- [ ] **Phase 3** — Automate (Bash, Git, secrets hygiene) *(Sessions 14–26)*
- [ ] **Phase 4** — See the traffic (Wireshark, pcaps, live tooling, local VM lab) *(Sessions 27–34)*
- [ ] **Phase 5** — Defend it (router, sensor, SIEM + auto-response) *(Sessions 35–49)*
- [ ] **Phase 6** — Containers *(Sessions 50–54)*
- [ ] **Phase 7** — Cloud + Terraform *(Sessions 55–66)*
- [ ] **Phase 8** — Kubernetes *(Sessions 67–73)*
- [ ] **Phase 9** — CI/CD + system design *(Sessions 74–75)*
- [ ] **Phase 10** — 🚀 Flagship: self-defending GitOps platform *(Sessions 76–85)*
- [ ] **Phase 11** — Specializations (pick 2–3) *(Sessions 86–99)*

## 📅 Session Index

| Session | Phase | Focus |
|---|---|---|
| 1 | 0 | Finish the workbench |
| 2 | 1 | OverTheWire Bandit |
| 3 | 1 | Own a box: access, users, permissions |
| 4 | 1 | Special permission bits: setuid, setgid, sticky |
| 5 | 1 | Triage tools: top, ps, free, df/du, iostat, ss, dmesg, strace |
| 6 | 1 | Break it: CPU, memory, disk, zombies |
| 7 | 1 | Break it: logs and ports, filesystem literacy, triage runbook |
| 8 | 2 | Networking theory: OSI, TCP/UDP, NAT, DNS, DHCP, TLS |
| 9 | 2 | Subnetting drills |
| 10 | 2 | SSH hardening |
| 11 | 2 | Firewalls: security group and ufw |
| 12 | 2 | Services and systemd |
| 13 | 2 | Packages, time, scheduling |
| 14 | 3 | Bash drills and backup script core |
| 15 | 3 | Backup script: robustness and scheduling |
| 16 | 3 | Backup restore test and log-analysis one-liners |
| 17 | 3 | loganalyze.sh and awk |
| 18 | 3 | Hardening script: structure and idempotency |
| 19 | 3 | Hardening script: content and the 3x run |
| 20 | 3 | Git model and rewriting history |
| 21 | 3 | Merge, rebase, and recovery |
| 22 | 3 | Debugging with git, and repo setup |
| 23 | 3 | PR flow and releases |
| 24 | 3 | Commit signing and workflow strategy |
| 25 | 3 | Secrets leak and scrub |
| 26 | 3 | Secrets prevention |
| 27 | 4 | Wireshark: setup, HTTP, DNS |
| 28 | 4 | Wireshark: TLS and key filters |
| 29 | 4 | Malicious pcap analysis |
| 30 | 4 | Incident report and more pcap exercises |
| 31 | 4 | Live tooling: DNS, routing, path, MTU |
| 32 | 4 | Live tooling: sockets, nc, curl, openssl |
| 33 | 4 | Scanning your own lab, how the web works |
| 34 | 4 | Local virtualization lab |
| 35 | 5 | Architecture, interfaces, forwarding |
| 36 | 5 | Router: NAT and firewall rules |
| 37 | 5 | Router: DHCP, DNS, and verification |
| 38 | 5 | Router level-ups: VLANs, VyOS/OPNsense |
| 39 | 5 | Sensor: tcpdump, Suricata/Zeek setup |
| 40 | 5 | Sensor: real detections on demand |
| 41 | 5 | Target app, nginx, TLS, JSON logs, SIEM choice |
| 42 | 5 | Ship and parse the logs |
| 43 | 5 | Dashboards |
| 44 | 5 | Detections and alert routing |
| 45 | 5 | Automated response |
| 46 | 5 | The attack demo and time-to-block |
| 47 | 5 | Write-up and milestone post |
| 48 | 5 | Cloud router I: VPC and NAT instance |
| 49 | 5 | Cloud router II: flow logs, comparison, destroy |
| 50 | 6 | Container concepts and Docker basics |
| 51 | 6 | Build a real image |
| 52 | 6 | Compose |
| 53 | 6 | Hardening I: multi-stage, minimal base, non-root |
| 54 | 6 | Hardening II: runtime flags, secrets, scanning, size |
| 55 | 7 | Cloud concepts and account hygiene (by hand) |
| 56 | 7 | Terraform concepts and fundamentals |
| 57 | 7 | Terraform remote state and project structure |
| 58 | 7 | Network by hand: VPC, subnets, gateways, security groups |
| 59 | 7 | Network as code: modules, environments, tagging |
| 60 | 7 | Compute and load balancing by hand |
| 61 | 7 | Identity and secrets by hand |
| 62 | 7 | Compute and load balancer as code |
| 63 | 7 | Storage and secrets: by hand, then as code |
| 64 | 7 | Observability and cleanup (by hand) |
| 65 | 7 | IaC scanning and pre-commit |
| 66 | 7 | The proof: destroy, rebuild, drift |
| 67 | 8 | Kubernetes concepts and a local cluster |
| 68 | 8 | Core workloads: Deployments, Services, Ingress, config |
| 69 | 8 | Production readiness: limits, probes, rolling updates |
| 70 | 8 | Autoscaling and stateful data |
| 71 | 8 | Security I: securityContext, NetworkPolicies, RBAC |
| 72 | 8 | Security II: Pod Security Standards, Falco, scanning |
| 73 | 8 | Helm and a managed cluster |
| 74 | 9 | CI/CD pipeline |
| 75 | 9 | System design, threat model, and presenting it |
| 76 | 10 | Foundation: app, repo, Terraform from zero |
| 77 | 10 | Pipeline I: secrets, SAST, tests, deps, IaC and Dockerfile scans |
| 78 | 10 | Pipeline II: image build, scan, SBOM, signing, ECR, OIDC |
| 79 | 10 | GitOps with Argo CD |
| 80 | 10 | Admission control with Kyverno/OPA |
| 81 | 10 | Observability: metrics, logs, traces, dashboards |
| 82 | 10 | Runtime security and alerting |
| 83 | 10 | Attack proofs I: build-time and admission |
| 84 | 10 | Attack proofs II: runtime attack, auto-response, demo |
| 85 | 10 | Ship the story |
| 86 | 11 | Project A — Supply chain I: signing, admission, SBOM, provenance |
| 87 | 11 | Project A — Supply chain II: demo, write-up, post |
| 88 | 11 | Project B — Vault I: deploy, dynamic secrets, rotation, K8s auth |
| 89 | 11 | Project B — Vault II: injector, refactor, audit, demo, post |
| 90 | 11 | Project C — Home SOC I: endpoints, Wazuh, Suricata, ATT&CK |
| 91 | 11 | Project C — Home SOC II: simulate the intrusion, detect each stage |
| 92 | 11 | Project C — Home SOC III: IR playbooks, purple team, post |
| 93 | 11 | Project D — IR automation I: GuardDuty, EventBridge, Lambda |
| 94 | 11 | Project D — IR automation II: Terraform, test, runbook, post |
| 95 | 11 | Project E — Policy as code I: OPA/Conftest, Kyverno, policies |
| 96 | 11 | Project E — Policy as code II: both layers, CIS report, demo, post |
| 97 | 11 | Project F — Offensive practice I: TryHackMe, HackTheBox |
| 98 | 11 | Project F — Offensive practice II: flAWS, Kubernetes Goat |
| 99 | 11 | Project F — Offensive practice III: Juice Shop, write-ups, post |

**Total: 99 sessions.**

---

## PHASE 0 — Set Up the Workbench  *(Session 1)*

### Session 1 — Finish the workbench

**EC2 setup**

- [x] AWS account created, MFA on root, billing alarm set first
- [x] Ubuntu Server LTS `t3.micro` launched (free-tier checked)
- [x] Key pair created, `.pem` chmod'd to 400
- [x] Security group: SSH from your IP only
- [x] SSH in successfully
- [x] AWS CLI installed locally; `aws sts get-caller-identity` works
- [x] Stop/start instance from the CLI
- [ ] `labup` / `labdown` alias/script written
- [x] Understand Elastic IP vs changing public IP; release unused EIPs

> 💸 Treat EC2 as metered, not free. Stop the instance when done. Watch for unattached/stopped-but-attached Elastic IPs (~$3.60/mo).

**Accounts**

- [x] GitHub account + SSH key
- [x] AWS (or Azure) account, billing alarm at £5
- [x] AWS Budgets configured
- [ ] Docker Hub account
- [ ] Datadog free trial (or OSS path: Grafana/Wazuh)

**Local tooling**

- [x] Terminal set up (WSL2+Terminal / iTerm2/Ghostty / native Linux)
- [x] `git`, `curl`, `jq`, `ssh` installed
- [x] Editor with terminal (VS Code or vim/neovim motions)
- [x] Password manager + 2FA on GitHub and AWS root

**Notes repo**

- [x] Public `devops-journey` repo created
- [x] Folders added: `01-linux/`, `02-bash/`, `03-networking/`, `04-git/`, `capstone/`, `cloud/`, `projects/`
- [x] `README.md` committed with roadmap, boxes tracked publicly

**DoD:** You can start, stop, and SSH into your cloud box from the CLI, bills are guarded by an alarm, and you have a public repo that will become your portfolio.

---

## PHASE 1 — Linux Core  *(Sessions 2–7)*

> 🧪 Test-out check first: quiz yourself on `find`/`grep`/`xargs`, reading `-rwsr-xr-x`, and owner/group/others.

### Session 2 — OverTheWire Bandit

**Step 1.1 — OverTheWire Bandit**

- [x] Rules page read, SSH into Level 0
- [x] `01-linux/bandit-notes.md` created
- [x] Levels 0–5 cleared
- [x] Levels 6–10 cleared
- [x] Levels 11–15 cleared
- [x] Levels 16–20 cleared
- [x] Levels 21–26 cleared
- [x] Levels 27–34 cleared
- [x] One-line trick noted per level
- [x] Summary written from memory (find, grep, xargs, nc, ssh -i, permissions, cron)
- [x] Can explain the `2>/dev/null` redirect reasoning

### Session 3 — Own a box: access, users, permissions

**Step 1.2 — Access, users, permissions (on EC2)**

- [x] Ubuntu Server launched via AWS CLI (not console)
- [x] SSH in with key pair
- [x] Noted what AWS handled for you (DHCP, DNS, route, firewall)
- [x] Non-root user created, added to `sudo`
- [x] `/etc/passwd`, `/etc/shadow`, `/etc/group` fields explained
- [x] `chmod` octal + symbolic practiced
- [x] `chown` practiced

### Session 4 — Special permission bits: setuid, setgid, sticky

**Step 1.2 — Access, users, permissions (on EC2)**

- [ ] `ls -l /usr/bin/passwd` and `ls -ld /tmp`: `s` and `t` explained
- [ ] `find / -perm -4000 -type f 2>/dev/null` — setuid files listed
- [ ] Sticky bit demo on a shared directory
- [ ] setgid directory demo

### Session 5 — Triage tools: top, ps, free, df/du, iostat, ss, dmesg, strace

**Step 1.3 — Understand the machine**

- [ ] `top`/`htop` — load average explained
- [ ] `ps aux`/`ps -ef` — find & kill by PID
- [ ] `free -h` — free vs available vs buff/cache explained
- [ ] `df -h` vs `du -sh *` — disagreement case explained
- [ ] `iostat`, `vmstat`, `iotop` used
- [ ] `lsof -i` / `ss -tulpn` used
- [ ] `dmesg -T` read, OOM killer messages found
- [ ] `strace -p <pid>` used once

### Session 6 — Break it: CPU, memory, disk, zombies

**Step 1.3 — Understand the machine**

- [ ] CPU stress test diagnosed (`stress-ng`)
- [ ] Memory exhausted, OOM killer evidence found
- [ ] Disk filled (`fallocate`), service failure diagnosed
- [ ] Zombie/orphan process created and understood

### Session 7 — Break it: logs and ports, filesystem literacy, triage runbook

**Step 1.3 — Understand the machine**

- [ ] Logs filled, `logrotate` configured
- [ ] Port conflict diagnosed with `ss -tulpn`
- [ ] `/etc`, `/var`, `/usr`, `/opt`, `/proc`, `/tmp`, `/home` explained
- [ ] `/proc/<pid>/` explored
- [ ] Hard links vs symlinks tested

**DoD:** Can name the bottleneck (CPU/RAM/disk/IO/process/network) and prove it, with a personal `linux-triage.md`.

**PHASE 1 DoD:** All 34 Bandit levels cleared; you can explain users/permissions/special bits; you can name the bottleneck and prove it, with a personal `linux-triage.md`.

- [ ] ⭐ **Milestone post** — broke Linux 6 ways on purpose

---

## PHASE 2 — Secure the Box  *(Sessions 8–13)*

> 🧪 Test-out check first: subnet math for a `/26`, the TCP 3-way handshake, security group vs host firewall.

### Session 8 — Networking theory: OSI, TCP/UDP, NAT, DNS, DHCP, TLS

**Step 2.1 — Networking essentials › Prerequisite theory**

- [ ] OSI vs TCP/IP models
- [ ] L2/L3/L4/L7 mapped
- [ ] TCP vs UDP, handshake, why DNS/video use UDP
- [ ] Public vs private IP ranges
- [ ] NAT explained
- [ ] DNS resolution order
- [ ] DNS record types (A, AAAA, CNAME, MX, TXT, NS, PTR)
- [ ] DHCP DORA sequence
- [ ] TLS handshake overview, cert chain

### Session 9 — Subnetting drills

**Step 2.1 — Networking essentials › Subnetting drills**

- [ ] /24, /16, /8 → dotted-decimal masks
- [ ] 192.168.1.0/26 breakdown
- [ ] 10.0.0.0/16 split into 4 subnets
- [ ] 172.16.34.200/20 network identified
- [ ] /31 and /32 explained
- [ ] 10/10 on random subnet quiz

### Session 10 — SSH hardening

**Step 2.2 — SSH hardening**

- [ ] SSH key pair generated (`ed25519`), copied with `ssh-copy-id`
- [ ] Key-based login confirmed before touching config
- [ ] `sshd_config` hardened (no passwords, no root login, custom port)
- [ ] sshd restarted, password auth verified rejected
- [ ] Second SSH session kept open during config edits
- [ ] One SSH security-group rule per network you use (home, hotspot), each with a description; stale ones deleted

### Session 11 — Firewalls: security group and ufw

**Step 2.3 — Firewalls: security group + `ufw`**

- [ ] `ufw` configured (default deny incoming, allow SSH)
- [ ] Enabled without lockout
- [ ] Underlying `iptables`/`nft` rules inspected
- [ ] Security group vs `ufw` explained (where each drops traffic)
- [ ] Proved the difference: block in `ufw` only vs security group only (refused vs hang)

### Session 12 — Services and systemd

**Step 2.4 — Services and systemd**

- [ ] nginx installed, custom page served
- [ ] `systemctl` status/start/stop/enable/restart fluent
- [ ] Custom systemd unit file written and enabled at boot
- [ ] Logs read via `journalctl`

### Session 13 — Packages, time, scheduling

**Step 2.5 — Packages, time, scheduling**

- [ ] `apt` update/upgrade/search/show/remove practiced
- [ ] `unattended-upgrades` enabled
- [ ] Timezone + NTP sync confirmed
- [ ] Cron job and systemd timer created and compared

**PHASE 2 DoD:** SSH password auth provably disabled, `ufw` + security group configured on purpose, nginx runs under your own systemd unit, box rebuildable by hand in under 30 minutes.

- [ ] ⭐ **Milestone post** (optional) — locked down a cloud server by hand

---

## PHASE 3 — Automate  *(Sessions 14–26)*

> 🧪 Test-out check first: `set -euo pipefail`, quoting, `rebase -i`, why a deleted secret is still in git.

### Session 14 — Bash drills and backup script core

**Step 3.1 — Bash › Prerequisite drills**

- [ ] Variables, quoting rules understood
- [ ] `if`/`case`/`for`/`while`/functions
- [ ] Exit codes, `$?`, `&&`, `||`
- [ ] Command substitution, positional args
- [ ] Redirection incl. here-docs
- [ ] `shellcheck` installed and used going forward
- [ ] `#!/usr/bin/env bash` + `set -euo pipefail` adopted as habit

**Step 3.1 — Bash › Task 1 — Backup script**

- [ ] Takes source + destination args
- [ ] Validates paths exist/are usable
- [ ] Timestamped tar.gz archive
- [ ] Rotation (keep last N)

### Session 15 — Backup script: robustness and scheduling

**Step 3.1 — Bash › Task 1 — Backup script**

- [ ] Logs each run with timestamps
- [ ] Distinct exit codes per failure
- [ ] Handles missing source / unwritable dest / disk full
- [ ] Lockfile prevents overlap
- [ ] `trap` cleans up temp files
- [ ] shellcheck-clean
- [ ] `--help` + argument parsing
- [ ] Scheduled via cron, then rewritten as systemd timer

### Session 16 — Backup restore test and log-analysis one-liners

**Step 3.1 — Bash › Task 1 — Backup script**

- [ ] Verified ran unattended overnight
- [ ] Actually restored from a backup

**Step 3.1 — Bash › Task 2 — Log analysis tool**

- [ ] Top 10 IPs one-liner
- [ ] Top 10 paths one-liner
- [ ] Status code counts
- [ ] 4xx/5xx grouped per hour
- [ ] Total bytes transferred
- [ ] Requests from single IP in time order
- [ ] Unique user-agents sorted
- [ ] Scanner detection (`/admin`, `/wp-login.php`, `/.env`, `/.git/config`)

### Session 17 — loganalyze.sh and awk

**Step 3.1 — Bash › Task 2 — Log analysis tool**

- [ ] Wrapped into `loganalyze.sh`
- [ ] Flags: `--top-ips`, `--status`, `--errors`, `--suspicious`, `--help`
- [ ] Handles gzipped logs
- [ ] Aligned column output
- [ ] shellcheck-clean
- [ ] Every awk field explained
- [ ] awk vs sed vs grep vs cut explained
- [ ] One pipeline rewritten with `sort -k`

### Session 18 — Hardening script: structure and idempotency

**Step 3.1 — Bash › Task 3 — Idempotent hardening script**

- [ ] Functions per concern
- [ ] `main()` at bottom
- [ ] `set -euo pipefail`
- [ ] Refuses to run if not root
- [ ] `--dry-run` flag
- [ ] User only created if missing
- [ ] Config lines only appended if not already present
- [ ] Files backed up before editing
- [ ] Services only restarted if config changed

### Session 19 — Hardening script: content and the 3x run

**Step 3.1 — Bash › Task 3 — Idempotent hardening script**

- [ ] Creates admin user w/ SSH key
- [ ] Hardens sshd
- [ ] Configures ufw
- [ ] Installs & enables fail2ban sshd jail
- [ ] Enables unattended-upgrades
- [ ] Sets login banner
- [ ] Prints summary of changes
- [ ] Ran 3x on fresh VM — idempotency proven

**DoD:** This script becomes the one you run on every new VM going forward.

> **Milestone 1:** one idempotent script builds a hardened nginx box; run it 3 times, nothing changes after the first.

### Session 20 — Git model and rewriting history

**Step 3.2 — Git and secrets hygiene › Task 1 — Beyond add/commit/push**

- [ ] Four areas explained (working dir, staging, local repo, remote)
- [ ] Commit model explained (snapshot + parent + hash)
- [ ] Branches as pointers, HEAD explained
- [ ] `git log --oneline --graph --all` read
- [ ] 5 messy commits squashed via `rebase -i`
- [ ] Commit reworded via rebase
- [ ] Commit dropped via rebase
- [ ] `git commit --amend` used
- [ ] Why never rewrite shared history — can explain

### Session 21 — Merge, rebase, and recovery

**Step 3.2 — Git and secrets hygiene › Task 1 — Beyond add/commit/push**

- [ ] Merge conflict created and resolved by hand
- [ ] Same conflict resolved via rebase
- [ ] Merge vs rebase tradeoff explained with a stance
- [ ] `reset --soft/--mixed/--hard` compared
- [ ] Hard-reset commit recovered via reflog
- [ ] Deleted branch restored from reflog
- [ ] `git stash` / `pop` / `list` used
- [ ] `git cherry-pick` used
- [ ] `git revert` used and compared to reset

### Session 22 — Debugging with git, and repo setup

**Step 3.2 — Git and secrets hygiene › Task 1 — Beyond add/commit/push**

- [ ] Bug planted 10 commits back, found via `git bisect run`
- [ ] `git blame` used
- [ ] `git log -S "string"` used

**Step 3.2 — Git and secrets hygiene › Task 2 — Real collaboration flow**

- [ ] Repo created, `main` default
- [ ] Branch protection enabled (PR required, status check, no force-push)
- [ ] `PULL_REQUEST_TEMPLATE.md` added
- [ ] `CODEOWNERS` added
- [ ] `CONTRIBUTING.md` + real `README.md` added

### Session 23 — PR flow and releases

**Step 3.2 — Git and secrets hygiene › Task 2 — Real collaboration flow**

- [ ] Feature branch naming convention used
- [ ] Conventional Commits used
- [ ] PR explaining *why* opened
- [ ] Review obtained
- [ ] Merge strategy compared and chosen with reason
- [ ] Release tagged with semver + notes

### Session 24 — Commit signing and workflow strategy

**Step 3.2 — Git and secrets hygiene › Task 2 — Real collaboration flow**

- [ ] GPG/SSH signing key generated
- [ ] `commit.gpgsign true` configured
- [ ] Public key added to GitHub
- [ ] Commits show Verified
- [ ] Supply-chain attack that signing prevents explained
- [ ] Trunk-based vs GitFlow vs GitHub Flow explained, one chosen and defended

### Session 25 — Secrets leak and scrub

**Step 3.2 — Git and secrets hygiene › Task 3 — Secrets hygiene**

- [ ] Fake secret committed, 5 more commits on top
- [ ] Secret deleted in new commit, pushed
- [ ] Proven still recoverable via `git log -p | grep`
- [ ] `git-filter-repo` or BFG installed
- [ ] Secret removed from all history
- [ ] Rewritten history force-pushed
- [ ] Verified gone from history
- [ ] Noted: credential must still be rotated even after scrubbing

### Session 26 — Secrets prevention

**Step 3.2 — Git and secrets hygiene › Task 3 — Secrets hygiene**

- [ ] `gitleaks` installed
- [ ] Pre-commit hook blocks secrets
- [ ] Tested — fake key rejected
- [ ] Comprehensive `.gitignore` written
- [ ] `.env.example` added
- [ ] GitHub secret scanning + push protection enabled

**DoD:** Can explain full incident-response sequence: rotate → scrub → investigate.

- [ ] ⭐ **Milestone post** — *I stopped configuring servers by hand* (hardening script, 3 runs) + the leaked-secret lesson

---

## PHASE 4 — See the Traffic  *(Sessions 27–34)*

> 🧪 Test-out check first: SYN/SYN-ACK/ACK, what HTTPS hides and doesn't, what `dig +trace` shows.

### Session 27 — Wireshark: setup, HTTP, DNS

**Step 4.1 — Wireshark: own traffic**

- [ ] Wireshark installed; capture vs display filters understood
- [ ] Plain HTTP capture: 3-way handshake identified
- [ ] GET request + raw headers found
- [ ] Follow TCP Stream used
- [ ] Connection teardown found
- [ ] TTL noted
- [ ] DNS capture: query/response matched by transaction ID
- [ ] Answer section, record type, TTL read
- [ ] NXDOMAIN capture

### Session 28 — Wireshark: TLS and key filters

**Step 4.1 — Wireshark: own traffic**

- [ ] TLS capture: ClientHello + SNI found
- [ ] ServerHello + cert found
- [ ] Application Data (opaque) point found
- [ ] Wrote down what an observer can/can't see over HTTPS
- [ ] Fluent in key filters (ip.addr, tcp.port, http.request.method, dns, syn scan, retransmission)

### Session 29 — Malicious pcap analysis

**Step 4.2 — Malicious pcap analysis**

- [ ] Infected host identified (IP/MAC/hostname)
- [ ] Timeline built
- [ ] Initial delivery found
- [ ] C2 server identified
- [ ] Beaconing characterized
- [ ] Suspicious HTTP objects exported
- [ ] User-Agent strings noted
- [ ] Exfiltration signs checked

### Session 30 — Incident report and more pcap exercises

**Step 4.2 — Malicious pcap analysis**

- [ ] Incident report written (summary, timeline, IOCs, impact, recommendations)
- [ ] 3 different pcap exercises completed
- [ ] Answers checked against solutions

### Session 31 — Live tooling: DNS, routing, path, MTU

**Step 4.3 — Live tooling proof**

- [ ] `dig` sections read; `+trace` walked
- [ ] MX/TXT/NS/reverse lookups done
- [ ] Resolvers compared (8.8.8.8 vs 1.1.1.1 vs ISP)
- [ ] `/etc/resolv.conf` / systemd-resolved understood
- [ ] `ip a`, `ip r`, `ip neigh` reviewed
- [ ] `traceroute`/`mtr` run and explained
- [ ] Default gateway explained
- [ ] MTU/fragmentation discovered via ping sizes

### Session 32 — Live tooling: sockets, nc, curl, openssl

**Step 4.3 — Live tooling proof**

- [ ] `ss -tulpn` reviewed
- [ ] `nc` chat + file transfer done
- [ ] `curl -v` full request/response read
- [ ] `openssl s_client` cert inspection

### Session 33 — Scanning your own lab, how the web works

**Step 4.3 — Live tooling proof**

- [ ] `nmap -sn` host discovery (own lab only)
- [ ] `nmap -sV` service detection
- [ ] SYN vs full-connect scan explained
- [ ] Scan captured live in Wireshark
- [ ] "URL to Enter key" lifecycle explained in 2 min
- [ ] Status codes known (200/301/302/400/401/403/404/429/500/502/503/504)
- [ ] Reverse proxy vs forward proxy vs load balancer explained

### Session 34 — Local virtualization lab

**Step 4.4 — Local virtualization**

- [ ] Hypervisor installed (VirtualBox / Proxmox / VMware / UTM)
- [ ] Snapshot workflow practiced
- [ ] Fresh Ubuntu Server VM spun up from ISO in under 10 min
- [ ] Optional: mini-PC homelab box acquired

> Local stays because EC2 can't do: (1) the router capstone — no L2 broadcast domain, (2) promiscuous packet sniffing, (3) nested virtualization.

- [ ] Ubuntu Server installed from ISO (minimal), static IP set at console, SSH in from host
- [ ] Compared: what you configured here that EC2 handled silently

**PHASE 4 DoD:** You can narrate a capture, produce an IOC list and incident writeup from an unknown pcap, and have a snapshot-ready local VM lab. Personal `networking-cheatsheet.md` written.

- [ ] ⭐ **Milestone post** — nmap scan captured in Wireshark

---

## PHASE 5 — Defend It: Router, Sensor, SIEM  *(Sessions 35–49)*

> Three milestones: **Router → Sensor → SIEM + auto-response.**

### Session 35 — Architecture, interfaces, forwarding

**Architecture**

- [ ] Diagram drawn before building (WAN → router → LAN switch → hosts, sensor + SIEM marked)
- [ ] IP scheme planned
- [ ] Hardware decided (mini-PC or VM w/ 2 NICs)

**Part 1 — Router**

- [ ] Two NICs present and named
- [ ] Static IP on LAN interface
- [ ] WAN gets address from home router
- [ ] Config persisted across reboot
- [ ] IP forwarding enabled and persisted
- [ ] IP forwarding kernel effect explained

### Session 36 — Router: NAT and firewall rules

**Part 1 — Router**

- [ ] nftables masquerade rule written
- [ ] Default-deny INPUT, allow established/related
- [ ] FORWARD LAN→WAN allowed
- [ ] FORWARD WAN→LAN blocked except established
- [ ] Ruleset persisted across reboot
- [ ] INPUT/FORWARD/OUTPUT chains explained

### Session 37 — Router: DHCP, DNS, and verification

**Part 1 — Router**

- [ ] dnsmasq installed and configured on LAN interface
- [ ] DHCP range/lease/gateway/DNS set
- [ ] Static lease for one host by MAC
- [ ] Local DNS entry added
- [ ] DORA sequence observed in dnsmasq log
- [ ] Second device gets IP from your router
- [ ] Internet reachable through your NAT
- [ ] Traceroute shows your router as hop 1
- [ ] Firewall rule blocking a site tested then removed
- [ ] Reboot survives, everything comes back

### Session 38 — Router level-ups: VLANs, VyOS/OPNsense

**Part 1 — Router**

- [ ] Level-up: VLANs added (trusted/untrusted)
- [ ] Level-up: rebuilt with VyOS/OPNsense + comparison writeup

### Session 39 — Sensor: tcpdump, Suricata/Zeek setup

**Part 2 — Sensor**

- [ ] Manual `tcpdump` capture done and opened in Wireshark
- [ ] tcpdump filters practiced (host/port/protocol)
- [ ] Promiscuous mode understood
- [ ] Suricata and/or Zeek installed, pointed at LAN interface
- [ ] Emerging Threats ruleset pulled and updated
- [ ] `eve.json` / Zeek logs confirmed writing

### Session 40 — Sensor: real detections on demand

**Part 2 — Sensor**

- [ ] False positives tuned out
- [ ] EICAR test file triggers alert
- [ ] nmap from one host triggers port-scan alert
- [ ] Bad-domain DNS request logged
- [ ] Custom Suricata rule written and fired

**DoD:** Sensor produces real timestamped events, triggerable on demand.

### Session 41 — Target app, nginx, TLS, JSON logs, SIEM choice

**Part 3 — nginx → SIEM → analytics → automated response**

- [ ] App deployed on lab host
- [ ] nginx reverse proxy in front
- [ ] TLS enabled (self-signed or Let's Encrypt)
- [ ] JSON access/error logging enabled
- [ ] Rate limiting + security headers added
- [ ] SIEM chosen (Datadog / Wazuh / Grafana+Loki+Promtail / ELK)

### Session 42 — Ship and parse the logs

**Part 3 — nginx → SIEM → analytics → automated response**

- [ ] Agent/shipper installed on router + nginx host
- [ ] nginx logs shipped
- [ ] Suricata/Zeek logs shipped
- [ ] System logs shipped (auth.log)
- [ ] Logs confirmed parsed into fields

### Session 43 — Dashboards

**Part 3 — nginx → SIEM → analytics → automated response**

- [ ] Dashboard: requests/sec over time
- [ ] Dashboard: status code breakdown
- [ ] Dashboard: top source IPs
- [ ] Dashboard: top requested paths
- [ ] Dashboard: geo map of source IPs
- [ ] Dashboard: IDS alert volume by severity
- [ ] Dashboard: failed SSH logins over time
- [ ] Dashboard: p95/p99 latency

### Session 44 — Detections and alert routing

**Part 3 — nginx → SIEM → analytics → automated response**

- [ ] Detection: scanner/credential stuffing (>50 4xx/min)
- [ ] Detection: brute force (>10 failed SSH/5min)
- [ ] Detection: 5xx rate threshold
- [ ] Detection: high-severity IDS alert
- [ ] Detection: sensitive path probing
- [ ] Alerts routed to Slack/Discord

### Session 45 — Automated response

**Part 3 — nginx → SIEM → analytics → automated response**

- [ ] Responder script blocks an IP
- [ ] Webhook listener exposed safely, authenticated
- [ ] SIEM monitor → webhook → responder wired
- [ ] Allowlist protects your own management IP
- [ ] Blocks auto-expire after N minutes
- [ ] Every automated action logged with reason + alert ID
- [ ] Slack/Discord notification on block

### Session 46 — The attack demo and time-to-block

**Part 3 — nginx → SIEM → analytics → automated response**

- [ ] Attack script written (path enum + SSH brute force)
- [ ] Full loop run and confirmed: traffic → log → SIEM → alert → webhook → block → notify
- [ ] Attacking host confirmed blocked
- [ ] Loop screenshotted/recorded
- [ ] Time-to-block measured

### Session 47 — Write-up and milestone post

**Write-up**

- [ ] Architecture diagram
- [ ] Detection→response sequence diagram
- [ ] Config committed (secrets excluded)
- [ ] README a stranger could follow
- [ ] Blog post written

**PHASE 5 DoD:** Scripted attack against your own infra gets auto-blocked with a chat alert, demoable live.

- [ ] ⭐ **Milestone post** — the big LinkedIn post (demo GIF, hook, diagram, repo link, cross-post to r/homelab + r/devops)

### Session 48 — Cloud router I: VPC and NAT instance

**Part 4 (bonus) — Cloud version of the router**

- [ ] VPC with public + private subnet in Terraform
- [ ] NAT instance (not NAT Gateway) launched in public subnet
- [ ] Source/dest check disabled on ENI, explained
- [ ] IP forwarding + masquerade rules replicated
- [ ] Private subnet route table points at NAT instance ENI
- [ ] Private host reaches internet through your NAT instance

### Session 49 — Cloud router II: flow logs, comparison, destroy

**Part 4 (bonus) — Cloud version of the router**

- [ ] VPC Flow Logs enabled, shipped to SIEM
- [ ] Comparison written: hand-rolled vs VPC routing vs NAT Gateway
- [ ] Destroyed when done
- [ ] **📣 Post on LinkedIn** — router built twice comparison

---

## PHASE 6 — Containers  *(Sessions 50–54)*

### Session 50 — Container concepts and Docker basics

**Prerequisite concepts**

- [ ] Container = namespaces + cgroups + layered FS — explained
- [ ] Container vs VM explained
- [ ] Images vs containers vs registries explained
- [ ] Layers + build cache explained

**Basics**

- [ ] `run/ps/logs/exec -it/stop/rm/images/rmi` fluent
- [ ] Ran interactively, poked around inside
- [ ] Port mapping order understood
- [ ] Volumes vs bind mounts understood
- [ ] `docker inspect` / `docker stats` used

### Session 51 — Build a real image

**Build a real image**

- [ ] Dockerfile written for an app
- [ ] FROM/RUN/COPY/WORKDIR/ENV/EXPOSE/CMD vs ENTRYPOINT understood
- [ ] `.dockerignore` added
- [ ] Layers ordered for cache efficiency
- [ ] Built, tagged properly, pushed to registry

### Session 52 — Compose

**Compose**

- [ ] `docker-compose.yml` with frontend+backend+db
- [ ] Named volumes persist DB data
- [ ] Custom network for name resolution
- [ ] `depends_on` + healthchecks correct
- [ ] `.env` file used (gitignored)
- [ ] `up -d`, `logs -f`, `down -v` fluent

### Session 53 — Hardening I: multi-stage, minimal base, non-root

**Hardening**

- [ ] Multi-stage build
- [ ] Minimal base (alpine/slim/distroless)
- [ ] Base image pinned by digest
- [ ] Non-root user created and verified
- [ ] `HEALTHCHECK` added

### Session 54 — Hardening II: runtime flags, secrets, scanning, size

**Hardening**

- [ ] `--read-only` + `--cap-drop=ALL` where possible
- [ ] No secrets baked in — verified via `docker history`
- [ ] Trivy scan clean or consciously accepted
- [ ] hadolint findings fixed
- [ ] Image size before/after recorded

**DoD:** Non-root, Trivy-clean, minimal image size, namespaces/cgroups explainable.

- [ ] ⭐ **Milestone post**: image size before/after

---

## PHASE 7 — Cloud + Terraform (fused)  *(Sessions 55–66)*

> 💸 Billing alarm at £5. Free-tier types only. `terraform destroy` every session. Never leave NAT Gateway/ALB/EKS running overnight.

> Build each slice by hand (7a), then immediately codify it (7b): account security → network → compute/LB → identity/secrets → data → observability/proof.

### Session 55 — Cloud concepts and account hygiene (by hand)

**7a — Cloud (AWS or Azure) › Prerequisite concepts**

- [ ] Shared responsibility model explained
- [ ] Regions vs AZs, multi-AZ importance
- [ ] IAM mental model (users/groups/roles/policies), roles > keys
- [ ] Least privilege explained

**7a — Cloud (AWS or Azure) › Account hygiene**

- [ ] MFA on root, root never used again
- [ ] Admin IAM user created w/ MFA
- [ ] Billing alarm at £5
- [ ] CloudTrail enabled
- [ ] GuardDuty enabled
- [ ] AWS Config / Security Hub baseline checked

### Session 56 — Terraform concepts and fundamentals

**7b — Terraform › Prerequisite concepts**

- [ ] Declarative vs imperative explained
- [ ] State file purpose, why it's never in git
- [ ] plan → apply → destroy cycle
- [ ] Providers/resources/data sources/variables/outputs/locals

**7b — Terraform › Fundamentals**

- [ ] Terraform installed; init/plan/apply/destroy on trivial resource
- [ ] Plan output read carefully (+/-/~/-/+)
- [ ] `fmt` + `validate` in workflow
- [ ] Typed variables w/ descriptions and defaults
- [ ] Outputs surface ALB DNS name
- [ ] Data source used (e.g. latest AMI lookup)

### Session 57 — Terraform remote state and project structure

**7b — Terraform › Remote state**

- [ ] S3 bucket for state, versioned + encrypted
- [ ] DynamoDB table for locking
- [ ] Backend configured, local state migrated
- [ ] `*.tfstate*` and `.terraform/` gitignored

**7b — Terraform › Professional structure**

- [ ] Split into main/variables/outputs/providers/versions.tf
- [ ] Provider + Terraform version pinned

### Session 58 — Network by hand: VPC, subnets, gateways, security groups

**7a — Cloud (AWS or Azure) › Networking**

- [ ] VPC with sensible CIDR
- [ ] 2 public subnets across AZs
- [ ] 2 private subnets across AZs
- [ ] IGW + public route table
- [ ] NAT Gateway + private route table (destroy after)
- [ ] Security groups scoped to minimum needed
- [ ] SGs vs NACLs explained

### Session 59 — Network as code: modules, environments, tagging

**7b — Terraform › Professional structure**

- [ ] Own module written (e.g. modules/vpc)
- [ ] Module reused twice with different vars
- [ ] Environments separated (envs/dev, envs/prod)
- [ ] Resources tagged consistently via default_tags

**7b — Terraform › Recreate 7a in code**

- [ ] VPC, subnets, IGW, NAT, route tables
- [ ] Security groups

### Session 60 — Compute and load balancing by hand

**7a — Cloud (AWS or Azure) › Compute + LB**

- [ ] EC2 in private subnet
- [ ] Dockerized app deployed (or ECS Fargate)
- [ ] ALB in public subnets
- [ ] Target group + passing health checks
- [ ] HTTPS listener w/ ACM cert, HTTP→HTTPS redirect
- [ ] App reachable over HTTPS; instance not directly internet-reachable

### Session 61 — Identity and secrets by hand

**7a — Cloud (AWS or Azure) › Identity & secrets**

- [ ] IAM role for EC2/ECS task, least privilege
- [ ] Attached via instance profile, no access keys on box
- [ ] DB credentials in Secrets Manager/Parameter Store
- [ ] App fetches secrets at runtime via role
- [ ] Repo grepped for credentials — zero hits

### Session 62 — Compute and load balancer as code

**7b — Terraform › Recreate 7a in code**

- [ ] ALB, target group, listeners, ACM cert
- [ ] EC2/ECS w/ IAM role

### Session 63 — Storage and secrets: by hand, then as code

**7a — Cloud (AWS or Azure) › Storage & data**

- [ ] S3 bucket: block public access, versioning, encryption
- [ ] Bucket policy scoped to your role
- [ ] RDS in private subnet, encrypted, not public
- [ ] Automated backups enabled

**7b — Terraform › Recreate 7a in code**

- [ ] S3 and RDS
- [ ] Secrets Manager entries (values injected, not committed)

### Session 64 — Observability and cleanup (by hand)

**7a — Cloud (AWS or Azure) › Observability**

- [ ] Logs shipping to CloudWatch
- [ ] CloudWatch alarm on CPU/error rate
- [ ] Own activity found in CloudTrail
- [ ] GuardDuty sample finding triggered and read

**7a — Cloud (AWS or Azure) › Clean up**

- [ ] NAT Gateway, ALB, RDS, EC2 deleted
- [ ] Bill confirmed back to ~£0

**DoD:** HTTPS-reachable app, private compute/DB, zero hardcoded credentials.

- [ ] 📣 Optional post: VPC diagram + no-credentials-in-code note

### Session 65 — IaC scanning and pre-commit

**7b — Terraform › IaC scanning**

- [ ] tfsec (or Trivy config) run, findings fixed
- [ ] Checkov run, findings fixed or documented
- [ ] terraform-docs added
- [ ] pre-commit config running fmt/validate/tfsec

### Session 66 — The proof: destroy, rebuild, drift

**7b — Terraform › The proof**

- [ ] `terraform destroy` — everything gone
- [ ] `terraform apply` — everything back from nothing
- [ ] Done twice
- [ ] Manual console drift detected via `plan`

**DoD:** Entire environment rebuilds from zero with one command.

- [ ] ⭐ **Milestone post**: destroy → rebuild GIF

---

## PHASE 8 — Kubernetes  *(Sessions 67–73)*

### Session 67 — Kubernetes concepts and a local cluster

**Prerequisite concepts**

- [ ] Control plane: API server, etcd, scheduler, controller manager
- [ ] Node components: kubelet, kube-proxy, container runtime
- [ ] Reconciliation loop explained
- [ ] Pods vs ReplicaSets vs Deployments vs Services
- [ ] Why bare Pods are avoided

**Local cluster**

- [ ] kind/minikube cluster running
- [ ] `get/describe/logs/exec/apply/delete` fluent
- [ ] `kubectl explain` used
- [ ] Bare Pod deployed, deleted, nothing self-heals
- [ ] Deployment self-heals a deleted Pod

### Session 68 — Core workloads: Deployments, Services, Ingress, config

**Core workloads**

- [ ] Deployment w/ 3 replicas
- [ ] ClusterIP Service + internal DNS
- [ ] NodePort/LoadBalancer difference understood
- [ ] Ingress + controller w/ host-based routing
- [ ] ConfigMap (env vars + file mount)
- [ ] Secret used, base64-is-not-encryption understood
- [ ] Namespaces separating environments

### Session 69 — Production readiness: limits, probes, rolling updates

**Production-readiness**

- [ ] Resource requests/limits on every container
- [ ] Liveness vs readiness probes
- [ ] Rolling update strategy (maxSurge/maxUnavailable)
- [ ] Zero-downtime rolling update proven under load
- [ ] `kubectl rollout undo` used

### Session 70 — Autoscaling and stateful data

**Production-readiness**

- [ ] HorizontalPodAutoscaler scaling out/in
- [ ] PersistentVolumeClaim for stateful data
- [ ] StatefulSet for DB, reasoning explained

### Session 71 — Security I: securityContext, NetworkPolicies, RBAC

**Security hardening**

- [ ] securityContext hardened (non-root, read-only FS, no priv escalation, drop caps)
- [ ] NetworkPolicies default-deny + explicit allow, proven
- [ ] RBAC: ServiceAccount + Role + RoleBinding scoped

### Session 72 — Security II: Pod Security Standards, Falco, scanning

**Security hardening**

- [ ] Pod Security Standards (restricted) enforced
- [ ] Falco installed
- [ ] Falco alert triggered on purpose
- [ ] Manifests scanned w/ kubesec/Checkov

### Session 73 — Helm and a managed cluster

**Packaging & managed cluster**

- [ ] Helm chart w/ templated values
- [ ] Install/upgrade/rollback via Helm
- [ ] Deployed to EKS/AKS via Terraform
- [ ] Managed cluster destroyed when idle

**DoD:** Self-heals, scales, zero-downtime updates, NetworkPolicies proven, Falco catches misbehavior.

- [ ] ⭐ **Milestone post**: pod-kill loop + zero failed requests, then NetworkPolicy post

---

## PHASE 9 — CI/CD and System Design  *(Sessions 74–75)*

### Session 74 — CI/CD pipeline

**CI/CD pipeline**

- [ ] CI vs CD (delivery) vs CD (deployment) explained
- [ ] GitHub Actions workflow on PR trigger
- [ ] Steps: checkout→lint→test→build→scan→push
- [ ] Dependency caching
- [ ] Matrix build across versions
- [ ] OIDC federation to AWS (no long-lived keys)
- [ ] PR check made required
- [ ] Manual approval gate before prod
- [ ] Blue/green vs canary vs rolling explained

### Session 75 — System design, threat model, and presenting it

**System design**

- [ ] Design doc: LB, horizontal scaling, statelessness, caching, DB replicas, queues
- [ ] Failure modes covered (AZ death, DB failover, dependency timeout, circuit breakers)
- [ ] SLIs/SLOs/error budget defined
- [ ] Threat model added (trust boundaries, entry points, blast radius)
- [ ] Architecture diagram drawn
- [ ] Presented out loud in 10 minutes

**DoD:** Doc + diagram defensible in a senior interview.

- [ ] ⭐ **Milestone post**: architecture diagram + threat model

---

## PHASE 10 — 🚀 Flagship: The Self-Defending GitOps Platform  *(Sessions 76–85)*

### Session 76 — Foundation: app, repo, Terraform from zero

**Step 10.1 — Foundation**

- [ ] App picked (real auth + DB + API, not a to-do list)
- [ ] Repo structure: app/, infra/, k8s/, .github/workflows/, docs/
- [ ] README with architecture diagram at top
- [ ] Terraform provisions VPC+EKS+ECR+RDS+IAM, remote state, modular
- [ ] `terraform apply` from zero works

### Session 77 — Pipeline I: secrets, SAST, tests, deps, IaC and Dockerfile scans

**Step 10.2 — Secure pipeline (every PR passes, in order)**

- [ ] gitleaks
- [ ] Semgrep (SAST)
- [ ] Unit + integration tests w/ coverage gate
- [ ] Dependency scan (npm audit/pip-audit/Dependabot/Renovate)
- [ ] tfsec + Checkov
- [ ] hadolint

### Session 78 — Pipeline II: image build, scan, SBOM, signing, ECR, OIDC

**Step 10.2 — Secure pipeline (every PR passes, in order)**

- [ ] Multi-stage, non-root, distroless image build
- [ ] Trivy scan, fail build on HIGH/CRITICAL
- [ ] SBOM generated (Syft), attached as artifact
- [ ] Image signed w/ cosign/sigstore (keyless OIDC)
- [ ] Pushed to ECR w/ immutable git-SHA tag
- [ ] All AWS auth via OIDC, zero long-lived creds

### Session 79 — GitOps with Argo CD

**Step 10.3 — GitOps deployment**

- [ ] Argo CD (or Flux) installed
- [ ] Config repo/dir as single source of truth
- [ ] Pipeline updates image tag, Argo syncs
- [ ] Drift + self-heal proven (manual delete → comes back)

### Session 80 — Admission control with Kyverno/OPA

**Step 10.3 — GitOps deployment**

- [ ] Kyverno/OPA Gatekeeper admission policies (unsigned images, privileged pods, root, no limits — all rejected)
- [ ] Unsigned image deploy rejected + screenshotted

### Session 81 — Observability: metrics, logs, traces, dashboards

**Step 10.4 — Observability & runtime security**

- [ ] Prometheus + Grafana (or Datadog) — RED metrics
- [ ] Logs to Loki or Phase 5 SIEM
- [ ] OpenTelemetry tracing
- [ ] Dashboards: health, deploy markers, errors, latency percentiles

### Session 82 — Runtime security and alerting

**Step 10.4 — Observability & runtime security**

- [ ] Falco alerts routed to Slack
- [ ] Alerting thresholds tuned (no fatigue)
- [ ] K8s audit logs to SIEM

### Session 83 — Attack proofs I: build-time and admission

**Step 10.5 — Attack it**

- [ ] Build-time proof: vulnerable dep + hardcoded secret PR blocked, screenshotted
- [ ] Admission proof: unsigned image + root pod rejected, screenshotted

### Session 84 — Attack proofs II: runtime attack, auto-response, demo

**Step 10.5 — Attack it**

- [ ] Runtime proof: scripted attack (path enum, brute force, unexpected shell)
- [ ] Falco + SIEM detect it, Slack alerts fire
- [ ] Automated response: IP blocked and/or compromised pod killed+replaced
- [ ] Optional: auto-rollback on error-rate spike
- [ ] Whole thing recorded as demo GIF

### Session 85 — Ship the story

**Step 10.6 — Ship the story**

- [ ] Architecture, pipeline, and detection→response diagrams
- [ ] README opens with what/why, then how to run
- [ ] `docs/SECURITY.md` listing every control + threat addressed
- [ ] Blog post on the build
- [ ] Demo video/GIF in README
- [ ] **📣 THE LinkedIn post** — demo GIF, diagram, hook, every tool named, honest "what broke," repo link, cross-post to r/devops + r/kubernetes, follow-up comment a week later

**FLAGSHIP DoD:** A stranger reads the README, understands the system in 2 minutes, sees proof both layers work.

---

## PHASE 11 — Specializations (pick 2–3)  *(Sessions 86–99)*

### Session 86 — Project A — Supply chain I: signing, admission, SBOM, provenance

**Project A — Supply-chain security lab**

- [ ] Cosign keyless signing in pipeline
- [ ] Kyverno rejects unsigned images
- [ ] SBOM (Syft) + scan (Grype) every build
- [ ] SLSA provenance attestation attached

### Session 87 — Project A — Supply chain II: demo, write-up, post

**Project A — Supply-chain security lab**

- [ ] Demo: unsigned image rejected at admission
- [ ] Writeup: SolarWinds/xz-utils style attack defended against
- [ ] **📣 Post on LinkedIn**

### Session 88 — Project B — Vault I: deploy, dynamic secrets, rotation, K8s auth

**Project B — Secrets management with Vault**

- [ ] Vault deployed (dev mode → real config w/ unsealing)
- [ ] Database secrets engine — dynamic short-lived creds
- [ ] Automatic rotation configured
- [ ] Kubernetes auth method (ServiceAccount-based)

### Session 89 — Project B — Vault II: injector, refactor, audit, demo, post

**Project B — Secrets management with Vault**

- [ ] Vault Agent Injector delivers secrets to pods
- [ ] Flagship app refactored — zero static secrets
- [ ] Audit log on every secret access
- [ ] Demo: credential expiring + reissued automatically
- [ ] **📣 Post on LinkedIn**

### Session 90 — Project C — Home SOC I: endpoints, Wazuh, Suricata, ATT&CK

**Project C — Full home SOC**

- [ ] Phase 5 capstone extended across Linux + Windows endpoints
- [ ] Wazuh agents everywhere (FIM, rootkit checks, vuln detection)
- [ ] Suricata IDS on router
- [ ] Detections mapped to MITRE ATT&CK

### Session 91 — Project C — Home SOC II: simulate the intrusion, detect each stage

**Project C — Full home SOC**

- [ ] Full intrusion simulated (access→persistence→privesc→exfil)
- [ ] Each stage detected + documented

### Session 92 — Project C — Home SOC III: IR playbooks, purple team, post

**Project C — Full home SOC**

- [ ] IR playbooks written (detect→triage→contain→eradicate→recover→lessons)
- [ ] Purple-team exercise run (attack, detect, improve, repeat)
- [ ] **📣 Post on LinkedIn**

### Session 93 — Project D — IR automation I: GuardDuty, EventBridge, Lambda

**Project D — Cloud incident-response automation**

- [ ] GuardDuty enabled, sample findings generated
- [ ] EventBridge rule on high-severity findings
- [ ] Lambda: quarantine SG, snapshot EBS, tag compromised, notify

### Session 94 — Project D — IR automation II: Terraform, test, runbook, post

**Project D — Cloud incident-response automation**

- [ ] All in Terraform
- [ ] Tested with real sample finding, containment screenshotted
- [ ] Human runbook documented
- [ ] **📣 Post on LinkedIn**

### Session 95 — Project E — Policy as code I: OPA/Conftest, Kyverno, policies

**Project E — Policy as code / compliance**

- [ ] OPA/Conftest validating Terraform plans in CI
- [ ] Kyverno enforcing at K8s admission
- [ ] Policies: no public S3, encryption required, mandatory tags, no privileged pods, no `latest`, resource limits

### Session 96 — Project E — Policy as code II: both layers, CIS report, demo, post

**Project E — Policy as code / compliance**

- [ ] Same policies enforced in both CI and admission
- [ ] Compliance report mapped to CIS Benchmark
- [ ] Demo: bad config rejected at both layers
- [ ] **📣 Post on LinkedIn**

### Session 97 — Project F — Offensive practice I: TryHackMe, HackTheBox

**Project F — Offensive practice**

- [ ] TryHackMe DevSecOps + SOC Level 1 paths
- [ ] HackTheBox cloud/container challenges

### Session 98 — Project F — Offensive practice II: flAWS, Kubernetes Goat

**Project F — Offensive practice**

- [ ] flAWS.cloud + flaws2.cloud
- [ ] Kubernetes Goat — exploited, then every finding fixed

### Session 99 — Project F — Offensive practice III: Juice Shop, write-ups, post

**Project F — Offensive practice**

- [ ] OWASP Juice Shop — Top 10 worked hands-on
- [ ] Writeup per challenge: exploit + prevention
- [ ] **📣 Post on LinkedIn**

---

## 🧭 Ongoing track (runs alongside the sessions, not scheduled)

## The Meta-Game — Standing Out

### Portfolio
- [ ] Every project README has diagram + demo GIF + clear "why"
- [ ] Pinned repos ordered by impressiveness
- [ ] Green contribution graph reflects real work
- [ ] One blog post per capstone

### Certifications
- [ ] AWS Solutions Architect Associate (after Phase 7)
- [ ] CKA (after Phase 8)
- [ ] CompTIA Security+ (after Phase 11)
- [ ] Optional: CKS, AWS Security Specialty, Terraform Associate

### Community & visibility
- [ ] OSS contribution (even a docs PR)
- [ ] Active in CNCF / r/devops / K8s Slack
- [ ] Flagship posted to LinkedIn + r/devops
- [ ] One meetup or conference attended

### Interview readiness
- [ ] Can explain every project in depth, incl. what went wrong
- [ ] Can whiteboard a scalable architecture live
- [ ] Can do "URL to Enter key" in 2 minutes
- [ ] Can debug a broken deployment out loud
- [ ] Has stories: production incident, tough tradeoff, being wrong
- [ ] Can always answer "why," including the option rejected

---

## Final Checkpoint — Is He a Hero Yet?

- [ ] Can rebuild any environment from code, one command
- [ ] Can diagnose a broken system by reasoning, not googling verbatim
- [ ] Has automated something from an hour down to zero
- [ ] Has caught and auto-responded to an attack in his own logs
- [ ] Has a public portfolio demonstrating all of the above
- [ ] Can teach any section of this roadmap to someone else

> **North star:** Traffic → observe → detect → respond → automate. First in a homelab, then in the cloud, with security in the pipeline instead of bolted on after.

---

## 📣 Appendix — LinkedIn Post Template

**Structure:**
1. **Hook** (line 1 — lead with result/surprise, never "excited to share")
2. **What was built** — 2–3 plain-English sentences
3. **What broke** — the most valuable paragraph, makes it read as real
4. **What was learned** — the transferable insight
5. **Tools used** — named explicitly
6. **Link** — repo/blog

**Rules:**

- [ ] Always include a visual (diagram, GIF, screenshot)
- [ ] Link in first comment if reach matters
- [ ] 3–5 hashtags, not fifteen
- [ ] Short paragraphs, whitespace
- [ ] No emoji spam / no "thrilled to announce"
- [ ] Reply to every comment
- [ ] Post consistently, ~one per project

**Skeleton:**
```
[Surprising result or concrete number, one sentence.]

I built [what it is] using [3–4 headline tools].

The part that took longest: [what broke, why].
[What it turned out to be. What he'd do differently.]

What I actually took away from it: [the transferable insight].

Full writeup and code: [link in comments]

#DevOps #[Tool] #CloudSecurity
```

**Also worth doing:**

- [ ] Update LinkedIn headline as he progresses
- [ ] Add each project to the Projects section of the profile
- [ ] Pin the flagship post
- [ ] Turn best 2–3 posts into full blog articles later
