```dataviewjs
const completedTasks = dv.pages("#checklist").file.tasks.where(t => t.completed).length
const incompletedTasks = dv.pages("#checklist").file.tasks.where(t => !t.completed).length
const allTasks = dv.pages("#checklist").file.tasks.length

dv.paragraph(dv.header(1, dv.el("b", incompletedTasks)))
```

