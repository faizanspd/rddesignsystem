# rddesignsystem
-
# Color Guidelines 🎨 

This document explains how each color token is used across the product to ensure visual consistency, accessibility, and predictable UI behavior.

---

## Background & Surfaces

### `background` — `#F3F4F6`
Used as the **default page background** across the app.  
This is the base gray layer (Gray-100) that all UI surfaces sit on.

Common use cases:
- App shell background
- Dashboard pages
- Settings pages
- Empty page layouts

### `card` — `#FFFFFF`
Used for **elevated surfaces** that sit on top of the background.

Common use cases:
- Dropdown menus
- Cards
- Tables
- Empty states
- Filter panels
- Modals

This creates a clear visual hierarchy between the page background and content.

---

## Brand Colors

### `brand.primary` — `#0D9488`
The main brand action color.

Used for:
- Primary buttons
- Input focus borders
- Checkbox & radio button active/hover states
- Highlighted icons
- Success actions

Represents **primary interaction and confirmation**.

### `brand.highlight` / `text.brand` — `#0F766E`
Used for **emphasized text and secondary highlights**.

Used for:
- Highlighted text across the app
- Secondary button hover text
- Headings when emphasis is required
- Editable table fields (with dotted underline)

Draws attention without overpowering the primary brand color.

### `brand.light` — `#F0FDFA`
A soft background highlight color.

Used for:
- Hover backgrounds
- Selected row highlights
- Light emphasis states
- Subtle UI feedback

Helps show interaction without heavy visual weight.

---

## Text Colors

### `text.primary` — `#303133`
The main text color for core content.

Used for:
- Page titles
- Main content
- Table values
- Input field text
- Input labels
- Secondary button text
- Ghost button text
- Radio & checkbox labels

Ensures strong readability and contrast.

### `text.secondary` — `#606266`
Used for supporting or less important text.

Used for:
- Helper text
- Metadata
- Less important table columns
- Descriptions

Reduces visual noise while keeping content readable.

### `text.placeholder` — `#909399`
Used for non-primary, temporary, or disabled text.

Used for:
- Input placeholders
- Disabled field text
- Empty states
- Inactive UI labels

Communicates non-final or inactive content.

### `text.brand` — `#0F766E`
Used when text needs **brand emphasis**.

Used for:
- Editable table fields (first-time selection)
- Highlighted headings
- Important emphasized text

Reinforces brand identity in key moments.

---

## Borders

### `border.default` — `#DCDFE6`
The standard UI stroke color.

Used for:
- Input field borders
- Card outlines
- Dividers
- Secondary button borders
- Modal separators

Provides structure without being visually heavy.

### `border.light` — `#E4E7ED`
A softer, low-contrast border.

Used for:
- Table row dividers
- Light dividers
- Subtle separators

Ideal for dense UI areas like tables where visual load should stay low.

---

## Status Colors (Alerts, Validation, Feedback)

These colors are used for system feedback such as **errors, warnings, info messages, and success states**.  
Each status includes text, background, border, and icon variations for accessibility and clarity.

### ❌ Error
- **Icon:** `#F56C6C`
- **Text:** `#DC2626`
- **Background:** `#FEF0F0`
- **Border:** `#FDE2E2`

Used for:
- Error icons
- Error borders
- Input helper text
- Table error messages
- Form validation messages
- Alert backgrounds

### ⚠️ Warning (Amber)
- **Text:** `#B45309`
- **Icon:** `#D97706`
- **Background:** `#FFFBEB`
- **Border:** `#FDE68A`

Used for:
- Warning alerts
- Risk notifications
- Important but non-blocking messages

### ℹ️ Info
- **Text:** `#0284C7`
- **Icon:** `#0EA5E9`
- **Background:** `#E0F2FE`
- **Border:** `#BAE6FD`

Used for:
- Informational banners
- System messages
- Guidance alerts

### ✅ Success (Brand-aligned)
- **Text:** `#0F766E`
- **Icon:** `#0D9488`
- **Background:** `#F0FDFA`
- **Border:** `#CCFBF1`

Used for:
- Success alerts
- Confirmation messages
- Completed actions

### 🏷️ Alt Success (Tags Only)
- **Text:** `#437E25`
- **Icon:** `#529B2E`
- **Background:** `#F0F9EB`
- **Border:** `#D1EDC4`

Used for:
- Success tags
- Label chips
- Compact status indicators

---

## Status Color Usage Principles

- **Errors** → red tones for urgency  
- **Warnings** → amber tones for caution  
- **Info** → blue tones for clarity  
- **Success** → brand teal for consistency  
- **Alt Success** → reserved for tags only  

Each status color has:
- Text color  
- Icon color  
- Background color  
- Border color  

This ensures accessibility and consistent UI behavior across all components.


## Alerts 🚨

Alerts are used to communicate system feedback to users, such as errors, warnings, informational messages, and success confirmations. Each alert uses the status colors defined in the design system, ensuring consistency across the app. Refer to the **Colors section** for the exact color tokens.

### Error Alerts ❌
- **Purpose:** Communicate critical errors that require user attention.
- **Usage Examples:**
  - Input helper errors (e.g., "Required field")
  - Form validation messages
  - Error banners
  - Table error indicators

### Warning Alerts ⚠️
- **Purpose:** Provide cautionary messages that are not critical.
- **Usage Examples:**
  - Warning alerts
  - Risk notifications
  - Non-blocking caution messages

### Info Alerts ℹ️
- **Purpose:** Display general information or guidance.
- **Usage Examples:**
  - Informational banners
  - System guidance messages
  - Info alerts

### Success Alerts ✅
- **Purpose:** Indicate successful actions or confirmations.
- **Usage Examples:**
  - Success banners
  - Completed actions
  - Confirmation messages

### Alt Success Alerts 🏷️
- **Purpose:** Specifically for tags or compact success indicators.
- **Usage Examples:**
  - Success tags
  - Label chips
  - Compact status indicators

### General Rules for All Alerts
- Use `status` color tokens from the design system for **icon, text, background, and border**.  
- Border radius: `radius.sm`  
- Padding: `spacing-md`  
- Shadow: subtle  
- Typography: body 14px, regular weight  
- Icon size: 16px  
- Gap between text and icon: `spacing-sm`  
- Transition: smooth  
- Accessibility:
  - Keyboard focus: true
  - Focus ring: true
  - ARIA role: `alert`

> Note: All colors should reference the tokens in **colors.json** to ensure consistency across all alerts and UI components.

