---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true
contentType: "event"
eventDate: "" # Required: Date of the event (format: YYYY-MM-DD) - used for one-off events
recurrence: "" # Optional: "daily", "weekly", "monthly", or "yearly" for recurring events
startDate: "" # Required if recurrence is set: Start date for recurring event (format: YYYY-MM-DD)
endDate: "" # Required if recurrence is set: End date for recurring event (format: YYYY-MM-DD)
recurrenceDay: "" # Optional: For weekly events, specify day (0=Sunday, 1=Monday, 2=Tuesday, etc.)
coverImage: "/images/events/cover.jpg"
description: "A brief description of this event"
cancelledDates: [] # Optional: List of dates to cancel (format: ["YYYY-MM-DD", "YYYY-MM-DD"])
---

# Event Title

Your event content here.

