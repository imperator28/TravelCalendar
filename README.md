# Travel Calendar

A single-file, Apple-style calendar for turning a travel plan into a clean image and table you can send to your manager.

**Live:** https://imperator28.github.io/TravelCalendar/

Or open `index.html` in any browser. No build step, no server. First visit shows an example plan built around today's date; use **New calendar** to start blank.

## What it does

- **Statuses as day bands:** Traveling for work, Working from home, Out of office, Public holiday. Travel and WFH carry a location (map pin).
- **Flights** as plane chips with the route (`LAX → PVG · UA857`); the flight number shows in the legend and table.
- **Key dates and key periods** (EVT, PVT, builds, reviews) in any of 8 colors. Overlapping items stack; long labels wrap; every week row shares one height.
- **Holidays:** China public holidays (official 2025–2026 schedules, including make-up workdays; 2027 statutory dates until published) and US federal holidays, each toggleable, tagged CN / US.
- **Fast input:** click a day or drag across days, then pick the category. Drag any item to move it. Click to edit. Undo on move and delete.
- **1, 2 or 3 months** (up to 12 with the steppers). Legend on the right, below, or Auto.
- **Export:** Copy image / Download PNG at 2x, sized to the content.
- **Share:** a table you can copy as plain text (Slack, WeChat), a real table (email, Docs, Notion, Teams, Excel), Markdown, or an image. Dates as `Mon, Nov 16`, `MM/DD` or `MM/DD/YYYY`.
- **Saved calendars:** several calendars kept in the browser, plus Export file / Open file (`.json`) to back up or move them.

## Notes

- Data lives in the browser's local storage for the page's origin. Use **Export file** to keep a copy.
- PNG export uses [html-to-image](https://github.com/bubkoo/html-to-image) from jsDelivr; offline, take a screenshot instead.
- Holiday data is in the `CN` table and `usHolidays()` in the script. Update the `CN` table when the State Council publishes a new year's schedule.
