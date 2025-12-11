# Homepage Layout Plan

## Header (Flexbox)
- Site title (top; centered)
- nav (bottom; Flexbox row)

## Main

### Section 1: Full-Width Image
- Mountain banner (top)

### Section 2: Animal Groups Preview (Grid – 2 columns)
- Cards (left + right, 3 rows)
- Each card:
  - Heading
  - Short description

### Section 3: Featured Habitats (Flexbox list)
- Horizontal list (Forests, Grasslands, Freshwater, Marine, Deserts, Tundra)
- Wraps on smaller screens

### Section 4: Endangered Animals Preview
- Short intro paragraph
- Link pointing to full endangered species page

## Footer (Flexbox)
- AI tool credit (left)
- Site Information (center)
- Back to top (right)

---

# Media Query Plan (Responsive Behavior)

## Header
- Desktop: title + nav in a row.
- Mobile (<600px): nav becomes stacked vertically.

## Full-Width Banner
- Desktop: large, tall image.
- Mobile: height reduced on small screens.

## Animal Groups (Grid)
- Desktop: 2-column grid.
- Mobile (<600px): switches to 1 column.

## Featured Habitats (Flexbox)
- Desktop: horizontal row of items.
- Mobile: flex-wrap makes items move to multiple rows.

## Endangered Animals Preview
- Desktop: normal spacing.
- Mobile: full-width text with smaller margins.

## Footer
- Desktop: 3-column flex layout.
- Mobile: items stack or tighten spacing.

## Standard I Will Follow
I will use the Common Media Query breakpoints from Dave Gray’s Lesson 17.

Breakpoints:
- < 481px (mobile)
- 481px – 768px (tablet)
- 769px – 1024px (small laptop)
- 1025px – 1200px (desktop)
- 1201px and greater
/* =======================
   MEDIA QUERIES
   ======================= */


/* 🔹 Mobile first – default already */


/* 🔹 Tablet (481px – 768px) */
@media (min-width: 481px) and (max-width: 768px) {

  /* Navigation wraps */
  nav ul {
    flex-wrap: wrap;
    gap: 1rem;
  }

  /* Animal Groups single column */
  .groups-grid-animals {
    grid-template-columns: 1fr;
  }

  /* Regular Groups single column */
  .groups-grid {
    grid-template-columns: 1fr;
  }

  /* Endangered text larger & stacked */
  .endangered-grid {
    grid-template-columns: 1fr;
  }

  /* Hero banner slightly smaller */
  header.hero-banner {
    height: 300px;
    font-size: 2rem;
  }
}



/* 🔹 Small Laptop (769px – 1024px) */
@media (min-width: 769px) and (max-width: 1024px) {

  /* 2 columns */
  .groups-grid-animals {
    grid-template-columns: repeat(2, 1fr);
  }

  .groups-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .endangered-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  /* Hero banner grows */
  header.hero-banner {
    height: 350px;
    font-size: 2.2rem;
  }
}



/* 🔹 Desktop (1025px – 1200px and up) */
@media (min-width: 1025px) {

  /* 2 columns, more spacing */
  .groups-grid-animals {
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
  }

  .groups-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
  }

  .endangered-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 2.5rem;
  }

  /* Hero banner biggest */
  header.hero-banner {
    height: 450px;
    font-size: 2.4rem;
  }
}
