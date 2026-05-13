# Week A/B Timetable Converter

A browser-based timetable converter for schools using `.ics` calendar exports from systems such as iSAMS.

This tool converts a timetable exported as hundreds of separate events into a much cleaner recurring Week A / Week B calendar with holiday exclusions.

No installs. No Python. No terminal. No Google login. Everything runs locally in the browser.

---

## Why this exists

Many timetable systems export calendars like this:

```text
Lesson 1 - Monday
Lesson 1 - Monday
Lesson 1 - Monday
Lesson 1 - Monday
...
```

for the entire academic year.

That creates several problems:

* timetable changes become painful
* deleting terms is messy
* calendars become cluttered
* recurring structures are lost
* importing updated calendars often duplicates everything

This tool converts those exports into proper recurring timetable series instead.

---

## Features

* Upload one or many `.ics` files
* Converts timetables into recurring Week A / Week B events
* Holiday and closure exclusions
* Bulk processing support
* Single-file download for one timetable
* ZIP download for multiple timetables
* Editable academic year settings
* Editable term dates
* Editable closures and public holidays
* Google Calendar compatible output
* Fully browser-based
* No server required

---

## Privacy

This app runs entirely in the browser.

Timetable files are:

* not uploaded
* not stored
* not transmitted anywhere

Everything is processed locally on the user's device.

This makes it suitable for school environments where timetable data should remain private.

---

## How to use

### 1. Open the app

Open:

```text
index.html
```

in a browser.

Or use the hosted version via GitHub Pages.

---

### 2. Upload timetable exports

Upload one or more `.ics` timetable files.

Usually these come from:

* iSAMS
* pupil portal exports
* timetable systems
* calendar exports

---

### 3. Check academic year settings

Adjust if needed:

* term dates
* holidays
* half terms
* public holidays
* closure periods

### Important

Closure dates are inclusive.

For example:

```text
16 Sept → 20 Sept
```

excludes all lessons from the 16th through the 20th.

Term end dates are also inclusive.

---

### 4. Convert calendars

Click:

```text
Convert calendars
```

The app will:

* download a single `.ics` if one file was uploaded
* download a ZIP if multiple files were uploaded

---

### 5. Import into Google Calendar

In Google Calendar:

```text
Settings
→ Import & export
→ Import
```

Import the generated timetable file into:

* a dedicated timetable calendar
* or an existing school calendar

A separate timetable calendar is strongly recommended.

---

## Hosting

This app can be hosted easily using:

* GitHub Pages
* Netlify
* school websites
* embedded Google Sites pages

No backend or database required.

---

## Technical notes

The app:

* detects the first Week A / Week B cycle from the uploaded timetable
* creates recurring fortnightly events
* applies closure exclusions using EXDATE rules
* preserves lesson times and metadata
* outputs standards-compliant `.ics` files

Everything is implemented using static HTML, CSS and JavaScript.

---

## Planned improvements

Potential future features:

* automatic colour coding
* drag-and-drop uploads
* saved academic year templates
* timetable change comparison
* direct Google Calendar integration
* student self-service workflows

---

## Disclaimer

Always test imports using a spare Google Calendar first.

Calendar duplication is one of humanity’s quieter forms of suffering.
