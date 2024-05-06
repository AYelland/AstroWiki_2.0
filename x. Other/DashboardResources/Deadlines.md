---
first_pass: 2025-04-11
second_pass: 2025-04-17
test_day: 2025-04-24
---

# Days Remaining

| Deadline          |         Date         |                    Days Until...                     |
| ----------------- | :------------------: | :--------------------------------------------------: |
| $1^{\rm st}$ Pass | `= this.first_pass`  | **`= round((this.first_pass - date(today)).days)`**  |
| $2^{\rm nd}$ Pass | `= this.second_pass` | **`= round((this.second_pass - date(today)).days)`** |
| Test Day          |  `= this.test_day`   |  **`= round((this.test_day - date(today)).days)`**   |

# Questions Remaining

```dataviewjs
const completedTasks = dv.pages("#checklist").file.tasks.where(t => t.completed).length
const incompletedTasks = dv.pages("#checklist").file.tasks.where(t => !t.completed).length
const allTasks = dv.pages("#checklist").file.tasks.length

dv.paragraph(dv.header(1, dv.el("b", incompletedTasks)))
```

# Questions Per Day

```dataviewjs
const completedTasks = dv.pages("#checklist").file.tasks.where(t => t.completed).length
const incompletedTasks = dv.pages("#checklist").file.tasks.where(t => !t.completed).length
const allTasks = dv.pages("#checklist").file.tasks.length

const firstPassDeadline = dv.current().first_pass
const daysInbetween = firstPassDeadline.diffNow().as('days')

const questionPerDay = Math.round(incompletedTasks/daysInbetween * 100)/100

dv.paragraph(dv.header(1, dv.el("b", questionPerDay)))
```
