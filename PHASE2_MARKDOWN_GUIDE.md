# Phase 2: Pre-Project - Markdown Quick Guide

## 🎯 Overview

This guide shows how to implement **Phase 2 (Pre-Project Data Collection)** using **plain Markdown files**, similar to Obsidian. This approach is:

- ✅ **Simple**: Uses plain text files anyone can edit
- ✅ **Offline**: Works without internet connection
- ✅ **Accessible**: Readable by screen readers and assistive technologies
- ✅ **Data-Light**: Very small file sizes
- ✅ **Portable**: Files can be easily shared and backed up
- ✅ **Open**: Uses open, non-proprietary format

## 📁 Simple File Structure for Phase 2

```
my_project/
├── PROJECT_CONFIG.md          # Phase 1 output
│
├── phase2-data/               # All Phase 2 data
│   ├── notes/                 # Text notes
│   │   ├── 2024-01-15_meeting.md
│   │   ├── 2024-01-16_observation.md
│   │   └── 2024-01-17_chat.md
│   │
│   ├── photos/                # Photo documentation
│   │   ├── 2024-01-15_photo1.md
│   │   └── 2024-01-16_photo2.md
│   │
│   ├── audio/                 # Audio notes (optional)
│   │   └── 2024-01-15_interview.md
│   │
│   └── INDEX.md              # Overview of all Phase 2 data
│
└── assets/                   # Actual media files
    └── photos/
        ├── 2024-01-15_photo1.jpg
        └── 2024-01-16_photo2.jpg
```

---

## 📝 Creating a Note (Simplest Version)

### Basic Note Format

```markdown
# Community Meeting Notes

**Date:** 2024-01-15  
**Time:** 14:00-16:00  
**Location:** Community Center  
**Author:** Jane Doe (Professional)  
**Type:** Note  
**Source:** Discussion  
**Tags:** #community #meeting #education

---

## Participants
- Jane Doe (Professional)
- John Smith (Community Member)
- Maria Garcia (Community Member)

## Key Discussion Points

### Education Challenges
- Limited access to secondary school
- High cost of school supplies
- Distance to school (5km)

### Community Ideas
- Organize transportation sharing
- Create study groups
- Advocate for school bus

## Observations
- Strong community interest in education
- Youth are engaged and articulate
- Parents willing to contribute

## Follow-up Actions
- [ ] Research transportation options
- [ ] Identify study group leaders
- [ ] Schedule next meeting
```

### With Frontmatter (Recommended for Structure)

```markdown
---
title: Community Meeting Notes
date: 2024-01-15
time: 14:00-16:00
location: Community Center
author: Jane Doe
role: professional
type: note
source: discussion
tags:
  - community
  - meeting
  - education
phase: phase2
---

# Community Meeting Notes

## Context
Meeting with community members to discuss education challenges.

## Participants
- Jane Doe (Professional)
- John Smith (Community Member)
- Maria Garcia (Community Member)

## Key Points

### Education Challenges
- Limited access to secondary education
- High cost of school supplies
- Distance to school (5km)

### Community Ideas
- Organize transportation sharing
- Create study groups
- Advocate for school bus

## Observations
- Strong community interest in education
- Youth are engaged and articulate
- Parents willing to contribute

## Follow-up Actions
- [ ] Research transportation options
- [ ] Identify study group leaders
- [ ] Schedule next meeting

---
*Created: 2024-01-15 16:30*
```

---

## 📷 Creating a Photo Entry

### Basic Photo Format

```markdown
# Community Center Photo

**Date:** 2024-01-15  
**Location:** Community Center, Main Hall  
**Photographer:** Jane Doe  
**Type:** Photo  
**Tags:** #infrastructure #community_center

---

![Community Center Main Hall](../assets/photos/2024-01-15_community-center.jpg)

## Description
Photo of the main hall at the community center where meetings are held.

## Observations
- Space can accommodate approximately 50 people
- Good natural lighting
- Needs better ventilation
- Chairs and tables available

## Context
Taken during community meeting on January 15, 2024.
```

### With Frontmatter

```markdown
---
title: Community Center Photo
date: 2024-01-15
location: Community Center, Main Hall
photographer: Jane Doe
role: professional
type: photo
source: observation
tags:
  - infrastructure
  - community_center
phase: phase2
file_reference: ../assets/photos/2024-01-15_community-center.jpg
---

# Community Center Photo

![Community Center Main Hall](../assets/photos/2024-01-15_community-center.jpg)

## Description
Photo of the main hall at the community center where meetings are held.

## Observations
- Space can accommodate approximately 50 people
- Good natural lighting
- Needs better ventilation
- Chairs and tables available

## Context
Taken during community meeting on January 15, 2024.

## Accessibility Notes
The photo shows a wheelchair-accessible entrance on the left side.

---
*Created: 2024-01-15 15:45*
```

---

## 🎤 Creating an Audio Note (Optional)

```markdown
---
title: Interview with Community Elder
date: 2024-01-15
time: 10:00-10:30
location: Elder's Home
author: Jane Doe
role: professional
type: audio
source: interview
language: en
tags:
  - interview
  - elder
  - history
phase: phase2
file_reference: ../assets/audio/2024-01-15_interview.mp3
transcript: true
---

# Interview with Community Elder

## Audio File
[Listen to Interview](../assets/audio/2024-01-15_interview.mp3)

## Transcript

**Jane Doe:** Can you tell us about the history of education in this community?

**Elder:** Well, when I was young, we only had a small primary school. Children had to walk 10km to the nearest secondary school. Many couldn't afford it, so they stopped after primary.

**Jane Doe:** How has that changed?

**Elder:** Now we have a secondary school 5km away, but the road is poor and there's no transportation. Still, more children are going to secondary school than before.

## Key Points
- Historical lack of access to secondary education
- Progress with new school, but challenges remain
- Road conditions and distance still barriers

## Observations
- Elder has deep knowledge of community history
- Strong oral tradition in the community
- Willingness to share information

---
*Created: 2024-01-15 11:00*
*Transcribed: 2024-01-15 14:00*
```

---

## 📋 Creating an Index File

The `INDEX.md` file helps you navigate all your Phase 2 data:

```markdown
# Phase 2: Pre-Project Data Collection

## Summary
- **Total Notes:** 5
- **Total Photos:** 3
- **Total Audio:** 1
- **Date Range:** 2024-01-15 to 2024-01-20
- **Contributors:** 3 (2 professionals, 1 community member)

---

## By Date

### January 15, 2024
- [Community Meeting Notes](./notes/2024-01-15_meeting.md)
- [Community Center Photo](./photos/2024-01-15_photo1.md)
- [Interview with Elder](./audio/2024-01-15_interview.md)

### January 16, 2024
- [Observation Walk Notes](./notes/2024-01-16_observation.md)
- [School Photo 1](./photos/2024-01-16_photo1.md)
- [School Photo 2](./photos/2024-01-16_photo2.md)

### January 17, 2024
- [Youth Focus Group](./notes/2024-01-17_youth.md)

---

## By Type

### Notes (5)
- [Community Meeting Notes](./notes/2024-01-15_meeting.md)
- [Observation Walk Notes](./notes/2024-01-16_observation.md)
- [Youth Focus Group](./notes/2024-01-17_youth.md)

### Photos (3)
- [Community Center Photo](./photos/2024-01-15_photo1.md)
- [School Photo 1](./photos/2024-01-16_photo1.md)
- [School Photo 2](./photos/2024-01-16_photo2.md)

### Audio (1)
- [Interview with Elder](./audio/2024-01-15_interview.md)

---

## By Tag

### #education (4)
- [Community Meeting Notes](./notes/2024-01-15_meeting.md)
- [Observation Walk Notes](./notes/2024-01-16_observation.md)
- [School Photo 1](./photos/2024-01-16_photo1.md)
- [School Photo 2](./photos/2024-01-16_photo2.md)

### #infrastructure (3)
- [Community Center Photo](./photos/2024-01-15_photo1.md)
- [School Photo 1](./photos/2024-01-16_photo1.md)
- [School Photo 2](./photos/2024-01-16_photo2.md)

### #community (2)
- [Community Meeting Notes](./notes/2024-01-15_meeting.md)
- [Community Center Photo](./photos/2024-01-15_photo1.md)

---

## Quick Stats
- **Most Active Day:** January 15 (3 entries)
- **Most Common Tag:** #education (4 entries)
- **Most Common Type:** Notes (5 entries)

---

*Last Updated: 2024-01-20 10:00*
```

---

## 🔍 Using Tags for Organization

### Tagging Strategy

Use **consistent tags** to categorize your data:

| Category | Example Tags |
|----------|--------------|
| **Topic** | #education, #water, #health, #employment |
| **Source** | #meeting, #observation, #interview, #chat |
| **Location** | #community_center, #school, #market, #home |
| **Group** | #youth, #elders, #women, #parents |
| **Type** | #note, #photo, #audio, #urgent |
| **Status** | #draft, #reviewed, #final |

### Tagging Tips

1. **Be consistent**: Use the same tag for the same concept
2. **Be specific**: Use `#secondary_education` not just `#education` when appropriate
3. **Limit tags**: 3-5 tags per entry is usually enough
4. **Use hierarchy**: `#education/access` for sub-categories (if your tool supports it)
5. **Avoid spaces**: Use `#youth_employment` not `#youth employment`

---

## 🔄 Moving to Phase 3

When you're ready to move to Phase 3 (Topic Selection), you can:

### Option 1: Manual Clustering
1. Review all data in your `phase2-data/` folder
2. Create a `clusters/` folder
3. Create Markdown files for each cluster
4. Link related data entries in each cluster file

### Option 2: Tag-Based Clustering
1. Look at your INDEX.md file
2. Identify common tags
3. Group entries by tag
4. Create clusters based on tag groups

### Option 3: Using Obsidian (Recommended)
1. Open your vault in Obsidian
2. Use the **Graph View** to see connections
3. Use **Backlinks** to see related notes
4. Create cluster notes and link to them

---

## 📱 Tools You Can Use

### No Installation Required
- **Notepad** (Windows) / **TextEdit** (Mac) / **Gedit** (Linux)
  - Basic Markdown support
  - No preview, but works

- **Any web browser**
  - Use online Markdown editors
  - Or just use a text editor

### Recommended Tools

#### Desktop
1. **Obsidian** (Best for connected notes)
   - Free for personal use
   - Graph view for seeing connections
   - Backlinks for navigation
   - Plugins for extra features
   - Mobile apps available

2. **VS Code** (Best for developers)
   - Free and open source
   - Markdown preview built-in
   - Extensions for enhanced Markdown
   - Git integration

3. **Typora** (Best for beautiful writing)
   - Clean, distraction-free interface
   - Live preview
   - Simple and intuitive

#### Mobile
1. **Obsidian Mobile**
   - Syncs with desktop
   - Offline capability
   - Photo capture integration

2. **Markor** (Android)
   - Open source
   - Simple Markdown editor
   - Offline-first

3. **iSH + Vim** (iOS)
   - For advanced users
   - Full terminal experience

---

## 💡 Tips for Effective Data Collection

### 1. Be Consistent
- Use the same format for similar entries
- Use consistent naming conventions
- Use consistent tagging

### 2. Add Context
- Always include date, time, location
- Note who was present
- Explain the context of the data

### 3. Use Clear Titles
- Make titles descriptive
- Include date in title
- Keep titles concise

### 4. Link Related Entries
- Link to other notes when relevant
- Use `[[Wiki Links]]` (Obsidian) or `[text](path.md)` (standard Markdown)
- Create connections between related data

### 5. Review Regularly
- Review your data regularly
- Update the INDEX.md file
- Look for patterns and themes

---

## 📊 Example: Complete Phase 2 Workflow

### Day 1: Community Meeting

1. **Create note file**:
   ```bash
   # In your phase2-data/notes/ folder
   touch 2024-01-15_community-meeting.md
   ```

2. **Add content** using the note template

3. **Save the file**

4. **Update INDEX.md** to include the new note

### Day 2: Observation Walk

1. **Create note file**:
   ```bash
   touch 2024-01-16_observation-walk.md
   ```

2. **Add content**

3. **Take photos** and save to `assets/photos/`

4. **Create photo entries** in `phase2-data/photos/`

5. **Update INDEX.md**

### Day 3: Review and Organize

1. **Review all data** in INDEX.md
2. **Identify patterns** and common themes
3. **Add tags** to entries for better organization
4. **Create connections** between related entries
5. **Prepare for Phase 3** (clustering)

---

## 🎯 Quick Reference: Markdown Syntax

### Headings
```markdown
# Heading 1 (Main title)
## Heading 2 (Section)
### Heading 3 (Subsection)
```

### Text Formatting
```markdown
*Italic* or _Italic_
**Bold** or __Bold__
~~Strikethrough~~
`Inline Code`
```

### Lists
```markdown
- Unordered item
- Another item
  - Nested item

1. Ordered item
2. Another item

- [ ] Task (unchecked)
- [x] Task (checked)
```

### Links
```markdown
[Link Text](path/to/file.md)
![Image Alt Text](path/to/image.jpg)
```

### Tables
```markdown
| Column 1 | Column 2 |
|---------|---------|
| Row 1   | Data    |
| Row 2   | Data    |
```

### Blockquotes
```markdown
> This is a quote
> It can span multiple lines
```

### Horizontal Rule
```markdown
---
***
___
```

---

## 📁 Backup and Sync

### Manual Backup
1. **Copy to USB drive**: Regularly copy your entire project folder
2. **Cloud backup**: Use Dropbox, Google Drive, or Nextcloud (optional)
3. **Zip archive**: Create periodic zip files

### Git Backup (Advanced)
```bash
# Initialize Git repository
git init

# Add all files
git add .

# Commit changes
git commit -m "Add Phase 2 data collection"

# Create backup branch
git branch backup-2024-01-20

# Push to remote (optional)
git remote add origin https://github.com/your-repo.git
git push -u origin main
```

---

## ✅ Checklist for Phase 2 Completion

- [ ] Created project folder structure
- [ ] Created at least 5-10 data entries (notes, photos, audio)
- [ ] Used consistent formatting for all entries
- [ ] Added metadata (date, author, type, tags) to all entries
- [ ] Created INDEX.md file
- [ ] Organized data by date, type, and tags
- [ ] Identified patterns and themes in the data
- [ ] Reviewed all entries for completeness
- [ ] Backed up data (USB, cloud, or Git)
- [ ] Ready to move to Phase 3 (Topic Selection)

---

## 🚀 Next Steps

After completing Phase 2:

1. **Move to Phase 3**: Start clustering your data
2. **Create clusters**: Group related entries together
3. **Select topic**: Choose the primary focus for your project
4. **Finalize configuration**: Update project configuration based on selected topic

---

## 📚 Additional Resources

- [Markdown Guide](https://www.markdownguide.org/) - Complete Markdown reference
- [Obsidian Help](https://help.obsidian.md/) - Obsidian documentation
- [VS Code Markdown](https://code.visualstudio.com/docs/languages/markdown) - VS Code Markdown features

---

*This guide shows how Phase 2 can work entirely with Markdown files, similar to Obsidian. The entire environment could use this approach for maximum simplicity and accessibility.*

*Document Version: 1.0*
*Last Updated: 2024*
