---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true
coverImage: "/images/blog/cover.jpg"
description: "A brief description of this blog post"
eventDate: "" # Optional: Use this for calendar events (format: YYYY-MM-DD)
recurrence: "" # Optional: "daily", "weekly", "monthly", or "yearly" for recurring events
recurrenceDay: "" # Optional: For weekly events, specify day (0=Sunday, 1=Monday, 2=Tuesday, etc.)
recurrenceEndDate: "" # Optional: When to stop recurring (format: YYYY-MM-DD)
cancelledDates: [] # Optional: List of dates to cancel (format: ["YYYY-MM-DD", "YYYY-MM-DD"])
---

Your blog post content here.

