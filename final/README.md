# Project

## Selecting a Topic

I chose to build a website about animals and wildlife because I’ve always found animals interesting and there is so much variety to learn about. Animals play an important role in our world, from helping ecosystems stay balanced to being part of different cultures and environments. I also like this topic because it allows me to organize information in a clear and educational way without worrying about copyrighted characters or media.

This project explores different animal groups, the environments they live in, and the ones that are most endangered. It provides simple examples and information that anyone can understand, and it allows me to practice good website structure using HTML.

## Outline

**Prompt to ChatGPT:**  
`I want to make an educational website about animals for a school HTML project. It should include animal groups, fun facts, and learning sections. Can you help me come up with a site name and short description?`

**ChatGPT Response:**  
**Wildlife Discovery** — *“Explore the amazing world of animals — from tiny insects to powerful mammals. Learn about habitats, species groups, and a list of the most endangered.”*

I chose this idea because it fits the educational style of the project and lets me include different types of animals and information.

## Menu

1. **Home** – Introduction to animals and the purpose of the site  
2. **Animal Groups** – Mammals, Birds, Reptiles, Fish, Amphibians  
3. **Habitats** – Forests, Oceans, Deserts, Grasslands  
4. **Most Endangered Species** – List of highly endangered animals  
5. **Climate Change** – *New Phase 3 page covering environmental impacts*  
6. **About / Contact** – Basic site information & fictional contact

---

# Typography Enhancements

For this part of the project, I made sure all typography and link styles are consistent across every page:

- Base **font-size (16px)**, **font-family (Arial/Helvetica)**, and **line-height** applied globally.
- Clear hierarchy using **h1–h4** with adjusted sizes and spacing.
- Heading color: `#1a3a53`.
- Link styling:
  - **hover:** underline + darker blue  
  - **focus:** visible outline (accessibility)  
  - **visited:** purple (`#5a2a8a`)
- Navigation links styled with Flexbox, bold text, and hover underline.
- No inline styles or ID selectors — everything uses clean classes and inheritance.

These improvements make the entire website readable, clean, and consistent.

---

# Decorative or Positional Enhancements

I used three CSS positioning techniques required for the project:

## My Responsiveness using Media Queries
My layout will change at these breakpoints. The navigation and content will stack vertically at smaller widths. On tablets, content stays in one column but spacing increases. On laptops and larger screens, content is displayed in two columns, spacing increases, and images adjust to the available width.

## Hero Image Design

For my hero image, I chose a mountain landscape because it represents the theme of my website: nature, wildlife, and the outdoors. The image appears at the top of my home page and contact page as a large banner section.

I used background-size: cover to make sure the image fills the entire width of the header area and stays responsive on different screen sizes. I also centered the image using background-position: center so the most important part of the scene is always visible.

To keep the text readable, I used darker heading styling and added spacing so that the title stands out clearly on top of the image.
