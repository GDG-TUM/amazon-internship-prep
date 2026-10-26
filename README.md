# Amazon Internship Prep — CloudPulse Lab

> Learn the fundamentals. Build a small system. Break it safely. Diagnose it with evidence.

A 30-day hands-on study and portfolio project for entry-level cloud support / cloud operations roles. Focus areas: Linux, networking, CIDR, DNS, HTTP/TCP/UDP, databases, storage, data processing, AWS fundamentals, and troubleshooting.

## Start here
1. Follow [ROADMAP.md](ROADMAP.md) one checkpoint at a time.
2. Update [TRACKER.md](TRACKER.md) after every session.
3. Record evidence in `logs/daily/` and incidents in `incidents/`.
4. Pass the weekly gates in [CHECKPOINTS.md](CHECKPOINTS.md).
5. Keep planned work separate from verified work in [PROJECT_STATUS.md](PROJECT_STATUS.md).

## Project
CloudPulse will become a small event-ingestion and operations lab: an API, PostgreSQL, synthetic event generation, batch aggregation, persistent storage, health checks, backup/restore, and evidence-based incident reports. AWS deployment is optional; do not incur cloud costs before reviewing pricing and teardown.

## Daily contract
A checkpoint is complete only when you have studied the concepts, built or practised the deliverable, attempted the exit test without copying, saved evidence, updated the tracker, and recorded the next action. If you miss a day, resume the next unfinished checkpoint—never fake progress.

## Suggested daily rhythm (~3 hours)
| Block | Time | Output |
|---|---:|---|
| Study | 45 min | Notes in your own words |
| Build | 90 min | Code, config, diagram, or lab |
| Diagnose | 30 min | Safe experiment and evidence |
| Checkpoint | 15 min | Log, tracker, next action, commit |

## Navigation
- [30-day roadmap](ROADMAP.md)
- [Daily tracker](TRACKER.md)
- [Weekly acceptance gates](CHECKPOINTS.md)
- [Architecture and scope](ARCHITECTURE.md)
- [Current implementation status](PROJECT_STATUS.md)
- [Daily log template](templates/DAILY_LOG.md)
- [Incident report template](templates/INCIDENT_REPORT.md)
- [Weekly review template](templates/WEEKLY_REVIEW.md)
- [Free resources](#free-resources)

## Free resources
- [Linux Journey](https://linuxjourney.com/)
- [Cisco Networking Academy](https://www.netacad.com/)
- [MDN HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP)
- [PostgreSQL Tutorial](https://www.postgresql.org/docs/current/tutorial.html)
- [Docker Get Started](https://docs.docker.com/get-started/)
- [AWS Cloud Practitioner Essentials](https://explore.skillbuilder.aws/learn/courses/134/aws-cloud-practitioner-essentials)
- [Amazon VPC documentation](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)
- [AWS pricing](https://aws.amazon.com/pricing/)

## Safety
Use only systems you own or isolated lab resources. Never commit credentials, private keys, `.env` files, personal data, or sensitive logs. Do not expose PostgreSQL publicly. AWS resources may incur charges; review pricing and teardown first.

**Starting status:** scaffold and learning plan only. No application feature, deployment, or incident is complete until you implement and verify it.