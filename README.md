# Multi-Page Portfolio (HNG Stage 1)

A multi-page portfolio website built with semantic HTML, CSS, and JavaScript. This project extends the Stage 0 profile card into a complete portfolio with navigation, a Contact Us page with form validation, and an About Me page with reflective content. All pages are fully responsive, accessible, and include comprehensive data-testid attributes for automated testing.

## What you get

- `index.html` — The original profile card with navigation (Home page)
- `about.html` — About Me page with reflective content and personal insights
- `contact.html` — Contact Us page with form validation and accessibility features
- `style.css` — Comprehensive styles for all pages with responsive design
- `images/` — Contains the avatar image `slackDisplayPicture(250px by 250px).png`

## File structure

```
hng13-frontend-stage-1/
├─ index.html          # Home page (profile card)
├─ about.html          # About Me page
├─ contact.html        # Contact Us page
├─ style.css           # Styles for all pages
├─ README.md
└─ images/
   └─ slackDisplayPicture(250px by 250px).png
```

## Features

### 🏠 Home Page (index.html)
- Original profile card with user avatar, bio, and social links
- Real-time timestamp updates
- Navigation to other pages

### 📝 About Me Page (about.html)
- **Bio section** — Personal story and background
- **Goals section** — Aspirations and objectives for the program
- **Confidence section** — Areas for growth and improvement
- **Future note** — Reflective message to future self
- **Extra thoughts** — Additional insights and perspectives

### 📧 Contact Us Page (contact.html)
- **Form validation** with real-time feedback
- **Required fields:** Full name, email, subject, message
- **Validation rules:**
  - All fields required
  - Valid email format
  - Message minimum 10 characters
- **Accessibility features:**
  - Proper labels and ARIA attributes
  - Keyboard navigation support
  - Screen reader compatibility

## How to preview

1. **Local server:** Run `python3 -m http.server 8000` and visit `http://localhost:8000`
2. **Direct file:** Open `index.html` directly in your browser

## Technical Implementation

### Accessibility Features
- Semantic HTML5 elements throughout
- Proper heading hierarchy (h1, h2, h3)
- ARIA attributes for form validation
- Keyboard navigation support
- Screen reader compatibility

### Responsive Design
- Mobile-first approach
- Breakpoints for mobile (480px), tablet (768px), and desktop
- Flexible navigation and form layouts
- Optimized typography and spacing

### Form Validation
- Client-side JavaScript validation
- Real-time error feedback
- Email format validation
- Character count validation
- Success message display

## Data Test IDs

### Navigation
- `test-main-navigation` — Main navigation menu

### Contact Form
- `test-contact-name` — Full name input
- `test-contact-email` — Email input
- `test-contact-subject` — Subject input
- `test-contact-message` — Message textarea
- `test-contact-submit` — Submit button
- `test-contact-error-<field>` — Error messages
- `test-contact-success` — Success message

### About Page
- `test-about-page` — Main wrapper
- `test-about-bio` — Bio section
- `test-about-goals` — Goals section
- `test-about-confidence` — Confidence section
- `test-about-future-note` — Future note section
- `test-about-extra` — Extra thoughts section

### Profile Card (Home)
- `test-profile-card` — Article wrapper
- `test-user-avatar` — Avatar image
- `test-user-name` — User name
- `test-user-bio` — Bio paragraph
- `test-user-time` — Timestamp element
- `test-user-social-*` — Social links
- `test-user-hobbies` — Hobbies list
- `test-user-dislikes` — Dislikes list

## Browser Support
- Modern browsers with ES6+ support
- Responsive design works on all screen sizes
- Form validation works without JavaScript (HTML5 validation)
- Enhanced experience with JavaScript enabled
