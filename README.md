# EVENT UI

*Prompt to tell AI to generate a wireframe with a placeholder appearance:*  
I used ChatGPT client to generate this image. Choose what you want to use.

```text
You are a senior UI/UX designer.
Generate an image of a low-fidelity grayscale wireframe for a modern event management landing page.

Figma wireframe style, minimal, grid-based layout, no UI styling.

Page sections from top to bottom:
- Fixed dark header/navbar
- Large centered hero section
- Featured events card grid
- Multi-column footer

Header:
- Left: small calendar-style logo + “Event App”
- Right: navigation links: Home, About, Features, Contact
- Far right: pill-shaped CTA button “Get Started”

Hero section:
- Centered layout
- Small top badge / status label
- Very large main headline: “Welcome to Event App”
- Supporting paragraph under headline
- Two side-by-side CTA buttons:
  - Create Event
  - Browse Events

Featured events section:
- Small label above section title
- Title: “Featured Events”
- Right-aligned “View All Events” control
- 6 event cards arranged in 3 columns and 2 rows

Each event card includes:
- image placeholder
- category chip
- date and time row
- event title
- location line
- attendee count line
- CTA button

Footer:
- Dark footer block
- Left: logo, description, social icons
- Middle/right: 2 columns of links
- Bottom row: copyright, legal, email

Style:
- grayscale only
- no real images
- placeholder shapes only
- rounded corners
- strong spacing
- clean hierarchy
- desktop full-page wireframe
```


> Now we will ask AI to help us build this page step by step.
I set up an AGENTS.md file with these guidelines. It can be expanded or done differently.

Set AI Rules (Important)
```text
You are a senior professional UI designer & frontend developer.

Generate a HTML page layout using Tailwind CSS utilities only based on the wireframe provided.
Rules:
- User placeholder blocks and nice svg icons for each section instead of real content
- Use Tailwind via CDN
- Do NOT create a CSS file
- Do NOT use <style>
- Use semantic HTML (header, main, aside, section, footer)
- Make code clean and readable
- Output only HTML

This is the wireframe to reference.

```

> This tells AI how to behave as our developer assistant.

*Header Prompt*
```text
Create ONLY the header (navbar) section of a modern SaaS event management website using Tailwind CSS.

Requirements:
- Fixed top navigation bar
- Dark background (slate-900)
- Left: logo with calendar-style icon + “Event App”
- Center/right: navigation links (Home, About, Features, Contact)
- Far right: primary CTA button “Get Started”
- Optional secondary link: “Sign In”

Design system:
- Use red-600 for primary button
- Hover states: red-700
- Text: white / slate-300
- Clean spacing, rounded elements, subtle shadows
- Smooth hover transitions
```

*Hero Section Prompt*
```text
Create ONLY the hero section of a modern SaaS event management landing page.

Layout:
- Centered content
- Small badge at top
- Large headline: “Welcome to Event App”
- Supporting paragraph
- Two CTA buttons side-by-side:
  - Primary: Create Event
  - Secondary: Browse Events

Design system:
- Background: white / slate-50 gradient feel
- Primary button: red-600 → hover red-700
- Secondary button: outline (slate-200 border)
- Headline: slate-900
- Paragraph: slate-600
- Badge: red-50 + red-600 text

Style:
- Clean spacing
- Rounded buttons (xl)
- Subtle shadows
- Smooth hover (scale + shadow)
```

*Featured Events Section Prompt*
```text
Create ONLY the “Featured Events” section for a SaaS event platform.

Layout:
- Top row:
  - Left: small label + section title “Featured Events”
  - Right: “View All Events” link
- Below: grid of 6 cards (3 columns, 2 rows)

Each card must include:
- Image placeholder (gray block or icon)
- Category badge
- Date & time row
- Event title
- Location row (icon)
- Attendee count row (icon)
- CTA button

Design system:
- Cards: white, border slate-200, shadow-slate
- Hover: slight scale + elevation
- Badge: red-50 background, red-600 text
- Buttons: red-600 → hover red-700
- Text hierarchy:
  - Title: slate-900
  - Meta: slate-500/600
```

*Enhance the existing event card UI by replacing image placeholders with real images from Unsplash.*
```text
Enhance the existing event card UI by replacing image placeholders with real images from Unsplash.

Use curated Unsplash image URLs (images.unsplash.com/photo-xxxx) instead of random ones.

Example:
Map categories to images:
- Music → concert crowd
- Tech → coding / laptop
- Business → meeting / office
- Fitness → gym / running
- Networking → people talking

Ensure each card has a different image and feels realistic.
```

*Footer Prompt*
```text
Create ONLY the footer for a SaaS event platform.

Layout:
- Dark background (slate-900)
- 3–4 columns:
  - Left: logo + description + social icons
  - Right: two columns of links (Quick Links, Resources)
- Bottom row:
  - Copyright
  - Legal links
  - Email/contact

Design system:
- Text: slate-300 / slate-400
- Headings: white
- Links: hover → red-500/600
- Icons: subtle + hover highlight
- Divider: slate-800

Style:
- Clean spacing
- Rounded icon buttons
- Modern SaaS footer feel
```