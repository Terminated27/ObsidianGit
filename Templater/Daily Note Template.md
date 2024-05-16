---
tags: journal
---
#daily_note
### Yesterday
[[ <% tp.date.yesterday() %> ]]
# To-do today

 ```tasks
 not done
 due on <% tp.date.now() %>
 ```

 ```tasks
 done on <% tp.date.now() %>
 ```

# What I did

- 

# What I ate

### breakfast
- 

### lunch
- 

### dinner
- 

# How I felt

- 

# To-do later

### Tomorrow 
[[<% tp.date.tomorrow() %>]]
 ```tasks
 due on <% tp.date.tomorrow() %>
 sort by urgency
 sort by priority
 ```

### Later

 ```tasks
 due after <% tp.date.tomorrow() %>
 not done
 sort by due
 ```

### No due date

 ```tasks
 path does not include Templates
 not done
 no due date
 sort by urgency
 sort by priority
 ```

<% await tp.file.rename(tp.date.now()) %>
