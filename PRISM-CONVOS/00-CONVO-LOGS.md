# PRISM Conversation Logs

**Purpose**: Track all PM coaching conversations to enable context continuity and prevent duplicate conversations.

## Format
- Date: yyyy-mm-dd
- Topic: Keywords from user input
- File: Conversation filename
- Status: active/completed/archived
- Preview: First 100 characters of user input

## Logs

| Date | Topic | File | Status | Preview |
|------|-------|------|--------|---------|

## Search Index
```

```

## Rules for Claude Code

### Before Creating New Conversation
1. **ALWAYS check this file first** (`PRISM-CONVOS/00-CONVO-LOGS.md`) to avoid duplicates
2. Search by topic keywords in user input
3. If matching conversation found:
   - Read the full conversation file in `PRISM-CONVOS/` to understand context
   - Continue the existing conversation instead of creating new one
   - Update `date_modified` in YAML frontmatter
   - Append new messages to the file

### When Creating New Conversation
1. Generate filename: `yyyy-mm-dd-topic-keywords.md`
2. Create in `PRISM-CONVOS/` directory
3. Include YAML frontmatter (see RULES.md for template)
4. Add entry to this index file immediately
5. Update search index

### File Naming Convention
- Format: `yyyy-mm-dd-topic-name.md`
- Topic: 3-5 keywords from user input
- Use hyphens, no spaces
- Keep filename descriptive but concise

### YAML Header Template
```yaml
---
conversation_id: "yyyy-mm-dd-topic-name"
date_created: "yyyy-mm-dd"
date_modified: "yyyy-mm-dd"
topic: "Topic Description"
status: "active"
participants:
  - role: "user"
    name: "User"
  - role: "assistant"
    platform: "platform-name"
tags:
  - "tag1"
  - "tag2"
summary: "Brief summary of conversation"
related_files: []
file_hash: "abc123def"
---
```

---

**Created**: 2025-11-24
**Purpose**: Track all user-AI conversations to avoid duplicates and maintain context
**Maintenance**: Update after each conversation
**AI Compliance**: All AI platforms must follow these rules