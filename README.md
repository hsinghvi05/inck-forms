# INCK Forms

Online form for INCK applicants: fill details, add photo and signature, and share the filled PDF on WhatsApp.

Live: https://hsinghvi05.github.io/inck-forms/

## Files

| File | What it is |
|---|---|
| `index.html` | The whole app (form, PDF builder, WhatsApp share) |
| `images/membership.jpg` | Membership Application Form design |
| `images/declaration.jpg` | Declaration (घोषणा पत्र) design |
| `images/oath.jpg` | Oath Form (शपथ पत्र) design |
| `images/idcard.jpg` | Identity Card design |

## Common changes (all in `index.html`)

- **WhatsApp number** – `const WHATSAPP = '91XXXXXXXXXX'` near the top of the script.
- **Office address / helpline / email** – the `OFFICE` block just below it.
- **Replacing a form design** – overwrite the image in `images/` with one of the same size and layout; the text positions stay correct.
- **Moving a field** – in the `FORMS` block, each entry has `x, y, w, h` in the image's own pixels.
- **Adding a new form type** – add its image to `images/` and a new entry to `FORMS` with its fields and positions.

Note: open it through the live link (or a local web server) to test. Opening `index.html` directly as a file blocks the PDF step in most browsers.
