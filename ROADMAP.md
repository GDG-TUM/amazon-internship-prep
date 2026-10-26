# 30-Day Study + Build Roadmap

Plan for about 3 hours per checkpoint. Take longer if needed; understanding matters more than speed.

## Week 1 — Linux and networking
1. **Linux CLI:** filesystem, paths, pipes, redirection, permissions. Build an environment inventory. Exit test: explain paths, stdout/stderr, permissions.
2. **Processes and logs:** ps, top, free, df, du, journalctl, systemd. Build `scripts/system-inventory.sh`. Exit test: distinguish stopped, crashed, and unresponsive services.
3. **OSI/TCP/IP, TCP/UDP:** layers, ports, sockets, handshake. Inspect `ss -lntup`. Exit test: explain TCP vs UDP and port vs IP.
4. **IPv4/CIDR:** masks, network/broadcast, usable hosts, private ranges. Write /24, /26, /28 examples. Exit test: calculate a /26 range.
5. **DNS/HTTP/TLS:** DNS records, HTTP methods/status, TLS. Use `curl -v`, `dig`, `getent hosts`. Exit test: trace a browser request.
6. **Routing/DHCP/ARP/NAT:** gateways, routes, leases, switching, SNAT/DNAT. Inspect `ip addr`, `ip route`, `ip neigh`. Exit test: explain why an addressed host may lack internet.
7. **Review + incident:** safely break a local listener/port mapping, diagnose and write Incident 1. Gate: restore connectivity and prove it.

## Week 2 — Databases, storage, data
8. **Relational databases:** tables, keys, constraints, normalization. Draft the event schema.
9. **SQL:** filters, joins, grouping, aggregates. Write five operational queries.
10. **Indexes/transactions:** EXPLAIN, ACID, connection exhaustion. Justify one index.
11. **Storage:** block/file/object, volumes, persistence, S3 concepts. Persist DB data and archive JSONL.
12. **Backup/restore:** backup, retention, RPO/RTO. Restore to a separate test DB and verify records.
13. **Big Data/batch:** ETL, batch vs streaming, aggregation. Generate and process 10,000+ synthetic events.
14. **Data incident:** safely break a disposable service/config, recover and document Incident 2.

## Week 3 — Cloud and AWS
15. **Cloud fundamentals:** IaaS/PaaS/SaaS, regions/AZs, elasticity, shared responsibility. Map local to cloud.
16. **Compute:** EC2, AMIs, SSH, user data, security groups. Write a secure deployment plan; deploy only if affordable.
17. **VPC/CIDR:** draw VPC, public/private subnets, route tables. Explain public vs private routing.
18. **Routes/IGW/NAT/filtering:** document inbound HTTPS and private outbound paths. Check NAT costs before creation.
19. **IAM/security:** roles, policies, least privilege, temporary credentials. Draft required permissions; never hard-code keys.
20. **S3/CloudWatch:** object storage, lifecycle, logs, metrics, alarms. Design archive and monitoring plan.
21. **Deployment/cost:** deploy minimally only if safe and affordable; otherwise rehearse locally and document cloud plan. Explain teardown.

## Week 4 — Troubleshooting and interview readiness
22. **Method:** scope, evidence, hypotheses, controlled tests, verification. Create a health check and incident template.
23. **DNS/HTTP incident:** diagnose resolver, timeout, refused connection, TLS or proxy failure.
24. **Database/storage incident:** diagnose availability, credentials, connection limits, disk, permissions; validate recovery.
25. **Linux resources:** CPU, memory, disk, processes, logs. Build `scripts/health-check.sh`.
26. **Observability:** logs vs metrics, latency, errors, health. Add request outcome/latency evidence.
27. **Tests/reproducibility:** automate API/DB checks and CI basics; recreate from README.
28. **Three timed incidents:** solve without blind fixes; write evidence-based reports.
29. **Interview rehearsal:** answer 15 questions aloud and record a 5–8 minute demo.
30. **Release:** docs, architecture, tests, runbooks, evidence index; tag a release and defend trade-offs.

## Rules
- Never mark a checkpoint complete without evidence and an exit test.
- Split work across sessions when needed; record blockers honestly.
- Prioritize the deliverable over extra reading.
- AWS diagrams and runbooks are acceptable when live deployment is not feasible; never claim a deployment you did not perform.

## Free resources
[Linux Journey](https://linuxjourney.com/) · [Cisco Networking Academy](https://www.netacad.com/) · [MDN HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP) · [PostgreSQL Tutorial](https://www.postgresql.org/docs/current/tutorial.html) · [Docker Get Started](https://docs.docker.com/get-started/) · [AWS Cloud Practitioner Essentials](https://explore.skillbuilder.aws/learn/courses/134/aws-cloud-practitioner-essentials) · [Amazon VPC](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)