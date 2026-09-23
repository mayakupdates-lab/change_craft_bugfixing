# Newsletter Signup Card

A responsive newsletter signup component built with HTML, CSS, and vanilla JavaScript.

## Part A - Bug Fixes

### 1. Button Contrast
Fixed the subscribe button contrast issue by changing the button text/background combination to provide clear, readable contrast while keeping the existing color scheme.

### 2. Accessible Email Field
Added a proper accessible label using a `label` element associated with the email input through `for` and `id`.

The input also includes:
- `type="email"`
- `autocomplete="email"`
- `aria-describedby` for the validation message

## Part B - Success State

Added a functional success state using vanilla JavaScript.

### Behavior

- A basic email format check runs when the form is submitted.
- Invalid email addresses display an error message.
- The email input receives focus when validation fails.
- A valid-looking email replaces the form with:
  > Thanks, check your inbox to confirm.

## Responsive Design

The component is responsive for desktop and mobile screens.

On narrow screens:
- The form changes from a horizontal layout to a vertical layout.
- The input and button use the available width.
- No content overlaps or gets cut off.

## Accessibility

The component includes:
- Proper label/input association
- Keyboard-accessible form controls
- Visible focus states
- `aria-invalid` for invalid input
- `role="alert"` for validation feedback
- `role="status"` and `aria-live="polite"` for the success message

## Technologies

- HTML5
- CSS3
- Vanilla JavaScript

No external libraries or dependencies are required.

## How to Run

1. Download or clone the repository.
2. Open `index.html` in a modern web browser.

Alternatively, use a local development server such as VS Code Live Server.

## Testing

The following scenarios were tested:

- Empty email submission
- Invalid email submission
- Valid email submission
- Keyboard navigation
- Button keyboard submission
- Mobile/narrow viewport layout
- Visible focus states
- No JavaScript console errors

## What I Would Improve With More Time

With more time, I would connect the form to a real newsletter API and provide more detailed loading, success, and server-error states. I would also run a formal accessibility audit and test the component across additional browsers and screen sizes.
