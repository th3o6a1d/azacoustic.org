---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true
contentType: "jam"
eventDate: "" # Required: Date of the jam (format: YYYY-MM-DD) - used for one-off jams
recurrence: "weekly" # Optional: "daily", "weekly", "monthly", or "yearly" for recurring jams
startDate: "" # Required if recurrence is set: Start date for recurring jam (format: YYYY-MM-DD)
endDate: "" # Required if recurrence is set: End date for recurring jam (format: YYYY-MM-DD)
recurrenceDay: "" # Optional: For weekly jams, specify day (0=Sunday, 1=Monday, 2=Tuesday, etc.)
cancelledDates: [] # Optional: List of dates to cancel (format: ["YYYY-MM-DD", "YYYY-MM-DD"])
description: "Description of the jam session"
---

# Jam Session Title

Your jam session content here.

