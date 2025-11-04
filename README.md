# AZ Acoustic Collective Website

A website for a musician collective in Phoenix, AZ, specializing in bluegrass, folk, and old time music.

## Features

- **Blog**: Posts with cover images and descriptions, organized by date (supports future-dated posts)
- **Calendar**: View of upcoming events and jams pulled from blog posts with `eventDate` parameter
- **Pages**: About, Jams, and Hiring pages
- **Contact Form**: Netlify-enabled form for collecting addresses and contact information
- **Design**: Desert-themed color palette with old-timey typography

## Content Structure

### Creating Blog Posts

Create blog posts in `content/blog/`:

```bash
hugo new blog/my-post.md
```

Blog posts support:
- `coverImage`: Path to cover image (e.g., `/images/blog/cover.jpg`)
- `description`: Short description for listings
- `eventDate`: Optional date for calendar events (format: `YYYY-MM-DD`)

### Adding Calendar Events

Create pages in `content/events/` or `content/jams/` with the following metadata:

**Required:**
- `eventDate`: Event date in `YYYY-MM-DD` format (e.g., `"2024-03-20"`)

**Optional:**
- `recurrence`: Recurrence pattern - `"daily"`, `"weekly"`, `"monthly"`, or `"yearly"`
- `recurrenceDay`: Day of week for weekly events (0=Sunday, 1=Monday, 2=Tuesday, etc.)
- `recurrenceEndDate`: End date for recurring events (defaults to 2 years from start)
- `cancelledDates`: Array of cancelled dates (e.g., `["2024-03-05", "2024-04-02"]`)

**Example - One-off event:**
```yaml
---
title: "Sample Event"
date: 2024-01-15
eventDate: "2024-03-20"
description: "Event description"
---
```

**Example - Recurring weekly jam:**
```yaml
---
title: "Weekly Jam Session"
eventDate: "2024-02-06"
recurrence: "weekly"
recurrenceDay: "2"  # Tuesday
description: "Weekly bluegrass jam"
---
```

### Images

Place blog cover images in `static/images/blog/` and reference them as `/images/blog/filename.jpg` in your front matter.

## Development

This site uses Hugo. To run locally:

```bash
hugo server
```

Then visit `http://localhost:1313`

## Deployment

This site is configured for Netlify deployment. The contact form will automatically work once deployed to Netlify.

## Design

The site uses a desert color palette with old-timey typography:
- **Fonts**: IM Fell English SC (headings), Crimson Text (body)
- **Colors**: Desert sand, clay, sage, terracotta tones
- **Style**: Vintage, warm, inviting
