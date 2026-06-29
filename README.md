# Application Form

A multi-page HTML/CSS application form that collects user information across four structured steps.

## Pages

| Page | File | Description |
|------|------|-------------|
| 1 | `index.html` | Personal Information |
| 2 | `form1.html` | Medical Information |
| 3 | `form2.html` | Educational Information |
| 4 | `form3.html` | Guidance Information |

## Features

- Multi-step form with a consistent navigation bar across all pages
- Dropdown selects for blood group and genotype
- Required field validation on educational inputs
- Sequential flow with a **Next** button advancing each step

## Form Fields

**Medical Information (`form1.html`)**
- Blood Group (A+, A−, B+, B−, O+, O−, AB+, AB−)
- Genotype (AA, AS, SS, AC, SC, CC)
- Allergies
- Existing Medical Conditions

**Educational Information (`form2.html`)**
- School
- Degree
- Graduation Year (1980–2026)
- Field of Study

## Project Structure

```
├── index.html       # Personal Information (Step 1)
├── form1.html       # Medical Information (Step 2)
├── form2.html       # Educational Information (Step 3)
├── form3.html       # Guidance Information (Step 4)
└── style.css        # Shared stylesheet
```

## Usage

Open `index.html` in a browser and fill out each section. Use the **Next** button at the bottom of each page to advance, or jump between sections using the navigation bar at the top.

## Deployment

Suggested Netlify project name: **`multi-step-application-form`**

## Known Issues

- `form1.html` — `allergies` and `medicalcondition` inputs are missing `name` attributes and will not be included in form submission.
- `form2.html` — The `id` and `name` for "Field of Study" contain spaces, which is invalid HTML. Rename to `field-of-study`.