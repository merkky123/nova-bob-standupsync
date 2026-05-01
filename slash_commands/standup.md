# /standup - Generate Daily Standup Summaries

## Command Purpose
This slash command instructs Bob to read your work notes and generate professional standup summaries in three different formats.

---

## Instructions for Bob

**Task:** Read the contents of `input/my_work_notes.txt` and generate three formatted standup summaries in a single response.

### Format 1: Markdown Standup Summary

Create a professional Markdown document with the following structure:

```markdown
# Daily Standup Summary
**Date:** [Current Date]
**Team Member:** [Name]

---

## 🎯 Yesterday's Accomplishments

[Summarize key accomplishments from the work notes, organized by category:]
- Feature Development
- Bug Fixes
- Code Reviews
- Infrastructure/DevOps
- Documentation
- Meetings

---

## 📋 Today's Plan

[Extract and list planned tasks for today, prioritized]

---

## 🚧 Blockers & Dependencies

[Identify any blockers or dependencies mentioned in the notes]
- List each blocker with context
- Include action items or follow-ups needed

---

## 📊 Metrics

[Include relevant metrics if available:]
- PRs Created/Reviewed
- Issues Resolved
- Commits Made
- Documentation Updates
```

### Format 2: Slack Message Format

Create a concise, emoji-rich format optimized for Slack/Teams:

```
📅 *Daily Standup - [Date]*

---

✅ *YESTERDAY'S WINS*

[Categorized list with emojis:]
🎨 *Feature Development*
• [Key accomplishment 1]
• [Key accomplishment 2]

🐛 *Bug Fixes*
• [Bug fix with issue number]

🔧 *Infrastructure*
• [Infrastructure work]

📝 *Code Quality*
• [Reviews, documentation, etc.]

---

🎯 *TODAY'S FOCUS*

1. [Priority task 1]
2. [Priority task 2]
3. [Priority task 3]

---

⚠️ *BLOCKERS*

🚨 [Blocker title]
[Description and action needed]

---

📊 *Quick Stats*
[Metrics in brief format]
```

### Format 3: Professional Email Format

Create a formal email-ready format:

```
Subject: Daily Standup Update - [Date]

Hi Team,

Here's my standup update for today:

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

YESTERDAY'S ACCOMPLISHMENTS

[Organized by category with detailed descriptions]

Feature Development - [Project Name]
• [Detailed accomplishment with context]
• [Technical details and outcomes]

Bug Resolution
• [Issue description and resolution]
• [Impact and verification]

[Additional categories as needed]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

TODAY'S PRIORITIES

1. [Detailed task description]
   - [Sub-tasks or context]

2. [Next priority]
   - [Additional details]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

BLOCKERS & ASSISTANCE NEEDED

⚠️ [BLOCKER CATEGORY]
[Blocker Title]
• [Detailed description]
• [Impact on work]
• Action: [What's needed to unblock]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

METRICS SUMMARY

[Detailed metrics]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Please let me know if you have any questions or need additional details.

Best regards,
[Name]
```

---

## Processing Guidelines

When generating the summaries, Bob should:

1. **Read the work notes file** - Parse `input/my_work_notes.txt` completely
2. **Extract key information:**
   - Timestamps and activities
   - Completed tasks and accomplishments
   - Bug fixes with issue numbers
   - Code reviews and PRs
   - Meetings and discussions
   - Blockers and dependencies
   - Planned work for today

3. **Categorize work:**
   - Group similar activities together
   - Prioritize by impact and importance
   - Highlight blockers prominently

4. **Format appropriately:**
   - Markdown: Professional, detailed, well-structured
   - Slack: Concise, scannable, emoji-enhanced
   - Email: Formal, comprehensive, stakeholder-friendly

5. **Include metrics:**
   - Count PRs, commits, issues
   - Summarize code review activity
   - Note documentation updates

6. **Maintain consistency:**
   - Use the same date across all formats
   - Keep core information consistent
   - Adjust tone and detail level per format

---

## Usage Example

**User says:** `/standup`

**Bob responds with:** All three formatted summaries in a single response, clearly separated with headers for each format.

---

## Output Structure

```
# Format 1: Markdown Standup Summary
[Full Markdown content]

---

# Format 2: Slack Message Format
[Full Slack content]

---

# Format 3: Professional Email Format
[Full Email content]
```

---

## Notes

- All three formats should be generated in a single response
- Use today's date for all summaries
- Extract information directly from the work notes file
- Maintain professional tone across all formats
- Highlight blockers clearly in all versions
- Include actionable next steps where applicable