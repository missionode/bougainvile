# Implementation Plan: Bougainvillea HTML Prototype

The goal is to expand the existing single-page landing page into a comprehensive, multi-page HTML prototype for "Bougainvillea," a luxury lifestyle brand.

## Objective
Create a functional, high-fidelity prototype with linked pages, consistent branding, and refined UI/UX components.

## Site Architecture
We will implement the following structure:
1.  **Home (`index.html`):** The existing landing page, updated with correct links.
2.  **Collections (`collections.html`):** A landing page showcasing different categories (e.g., The Linen Series, Modern Tailoring).
3.  **Collection Detail (`collection-detail.html`):** A focused view of a specific collection.
4.  **Boutique (`shop.html`):** Product listing page with filters (mocked).
5.  **Product Detail (`product.html`):** A detailed view for a single item.
6.  **Our Story (`about.html`):** Brand heritage and mission page.
7.  **Journal (`journal.html`):** Editorial/Blog listing.
8.  **Contact (`contact.html`):** Contact form and boutique locator.

## Implementation Steps

### Phase 1: Foundation & Refactoring
1.  **Shared Components:** Extract the `Header` and `Footer` logic. Since this is a pure HTML prototype without a build system, we will use a small helper script to load these components dynamically or duplicate them with clear "start/end" comments for easy maintenance.
2.  **Navigation Fix:** Update the `index.html` navigation links to point to the new files.
3.  **Dark Mode Fix:** Standardize dark mode support across all pages by ensuring the `body` background uses Tailwind classes instead of hardcoded CSS.

### Phase 2: Page Development
1.  **Collections Page:** 
    *   Implement a high-impact visual grid for collection categories.
    *   Use the established "bento" style for consistency.
2.  **Boutique (Shop):**
    *   Create a product grid with hover effects.
    *   Add a sidebar or top-bar for mock filtering (Category, Size, Color).
3.  **Our Story:**
    *   Design a layout focused on long-form typography and editorial imagery.
    *   Include a "Timeline" or "Values" section.
4.  **Journal:**
    *   Implement a card-based layout for editorial stories.

### Phase 3: Interactivity & Polish
1.  **Mobile Menu:** Implement the JavaScript logic to open/close the mobile navigation drawer.
2.  **Transitions:** Add smooth page transitions or scroll-reveal animations using Tailwind's `transition` classes and potentially a tiny bit of GSAP or Intersection Observer.
3.  **Forms:** Create a stylized contact/newsletter form with validation states.

## Verification & Testing
*   **Link Check:** Ensure all internal links resolve correctly between files.
*   **Responsive Audit:** Verify all new pages are fully responsive (Mobile, Tablet, Desktop).
*   **Accessibility:** Check contrast ratios and ensure interactive elements have proper hover/focus states.
*   **Dark Mode:** Toggle dark mode on all pages to ensure no hardcoded colors break the theme.
