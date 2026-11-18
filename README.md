# HR CLI Lab — TUKE KPI FEI, 26.11.2026

Two short hands-on exercises from real HR SaaS engineering.

- Work in pairs.
- Use any language and any tools you normally use, AI assistants included.
- Copy the prompt into your tool, or read it as a ticket and build it by hand.
- All data is synthetic. No real people.
- Start each exercise only when the instructor says so.

---

## Exercise 1 — HR-101: Employee Directory CLI (15 min)

```text
Build a console app "hr" in any language.
Our HR SaaS serves several customer companies (tenants) from one data store.
Create the data yourself:
- users.json: anna works for Acme, boris works for Globex.
- employees.json: 30 employees with ids 1001-1030. Odd ids belong to Acme,
  even ids to Globex. Each has name, city, job title, department and company.
Print each employee on one line: id, name, company.
Commands:
  hr --user <username> list
  hr --user <username> show <employeeId>
  hr --user <username> search <text>
  hr --user <username> stats          # headcount per department
  hr --user <username> export <file.csv>
```

---

## Exercise 2 — HR-201: Contract History CLI (15 min)

```text
Build a console app "hr" that shows how an employee's contract changes over time.
Save these changes, exported from our HR system, as changes.json:
- E-1001 hours 40, effective 2026-01-01, entered 2026-01-02
- E-1001 department Sales, effective 2026-01-01, entered 2026-01-02
- E-1001 department Marketing, effective 2026-03-01, entered 2026-03-03
- E-1001 hours 32, effective 2026-03-01, entered 2026-04-10
- E-1001 department Marketing, effective 2026-02-15, entered 2026-04-15
Commands:
  hr show <employeeId> --on <date>   # contract (hours, department) on a date
  hr history <employeeId>            # all changes
```

No AI tool? The same data is ready in [`changes.json`](changes.json).
