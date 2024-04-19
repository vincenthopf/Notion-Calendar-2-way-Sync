# Two-Way Notion-Google Calendar Sync Script 

Yet another script to synchronize events between Google Calendar and a Notion database.

Based on [hk21702's Yet another Google calender notion 2 way snc](https://github.com/hk21702).
Ehanced intructions and code for better stability.

Currently supports two-way event creation, deletion, and updating.
| Property | Synchronization | Info |
| ---- | ---- | ---- |
| Name | 🔀 Yes| Title |
| Date | 🔀 Yes| Date & Time (Start and End) |
| Tags | ⚠️ Notion Database Only | Multi-select - Personal organization and script interaction |
| Location | 🔀 Yes| Text |
| Description | 🔀 Yes| Text |

## For [setup instructions 🔰](https://github.com/hk21702/YA-GCal-Notion-Sync-Script/wiki/Setup-Instructions%F0%9F%94%B0) and FAQ, please go to the [wiki!](https://github.com/hk21702/YA-GCal-Notion-Sync-Script/wiki)

## Additional Info/Features


- Nothing to download or install
- Automatic Script Trigger
- Time Intervals
- Google Calendar Updates
- Logs that are saved and can be looked at later
- Sync both from GCal, and from Notion
  - Creation
  - Updates
    - Changing calendars from Notion
  - Deletions
- Multi-calendar support
- Support for recurring Events (Only available by setting through GCal)
- No Notion formulas
- Flexible property names
- Support for all day events, multi day events and scheduled events

## Known limitations/Bugs

- Sync from Notion sometimes doesn't register when the page was recently updated by GCal
  - Caused by lack of precision in Notion's last edited timestamp
- Will only check 100 most recently edited pages in database (Caused by Notion API limit)
- Rich text (bolding, italics, etc.) used in the description will be overwritten to plain text after syncing.
- Doesn't work with auto-generated calendars such as Birthdays. Might be a limitation of GCal API.
- Descriptions can only have MAX 2,000 characters. This is a limit imposed by Notion.
