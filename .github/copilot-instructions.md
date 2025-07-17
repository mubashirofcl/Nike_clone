# Copilot Instructions for Nike HTML/CSS Project

## Project Overview
This is a static front-end project for a Nike-themed website, built with HTML and CSS. The project structure is organized for rapid prototyping and visual experimentation, with a focus on modern, responsive layouts and interactive carousels.

## Key Files and Structure
- `index.html`: Main entry point. Contains all page sections, including navigation, hero banners, featured products, video, and carousels.
- `style.css`: Centralized stylesheet. All layout, typography, and component styles are defined here.
- `images/`: Contains all static assets, organized by feature (e.g., `shoes/`, `slider/`, `grid/`).

## UI Patterns and Conventions
- **Section Classes**: Each major section uses a `Section`-suffixed class (e.g., `.featuredSection`, `.VideoSection`, `.shoesSlider`).
- **Cards and Carousels**: Product carousels use `.carousel`, `.carousel2`, `.card`, `.card2` classes. Navigation buttons are `.carousel-btn`, `.carousel-btn2`.
- **Absolute Positioning**: Overlays (e.g., `.hero2` in `.cal`) use `position: absolute` inside a `position: relative` parent.
- **Responsive Layout**: Flexbox is used for most layout containers (e.g., `.featured`, `.carousel-wrapper`).

## JavaScript Interactivity
- Carousel scrolling is handled by simple JS in `<script>` tags at the bottom of `index.html`.
- Button selectors are class-based (e.g., `.carousel-btn.next`, `.carousel-btn2.prev`).
- Example: 
  ```js
  next2.addEventListener('click', () => {
      carousel2.scrollBy({ left: 200, behavior: 'smooth' });
  });
  ```

## Customization and Extension
- To add new sections, follow the existing section and class naming conventions.
- For new carousels, duplicate the structure and update IDs/classes as needed.
- All images should be placed in the appropriate subfolder under `images/`.

## No Build or Test Workflow
- This project is static: no build, test, or dependency management is required.
- Open `index.html` directly in a browser to view changes.

## Tips for AI Agents
- Always update both HTML and CSS for new UI features.
- Maintain consistent class naming and section structure.
- When adding interactivity, use unobtrusive JS at the end of `index.html`.
- Reference existing patterns for overlays, carousels, and responsive design.

## Key Example
- To overlay text on an image in a grid cell:
  - Set parent `.cal` to `position: relative;`
  - Set child `.hero2` to `position: absolute; top: 0; left: 0; width: 100%; height: 100%`

---

If you add new patterns or workflows, update this file to help future contributors and AI agents.
