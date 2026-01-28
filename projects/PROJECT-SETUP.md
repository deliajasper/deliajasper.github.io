# Setting Up Your Project Pages

This guide will help you create individual pages for each of your projects.

## Quick Setup

1. **Create the projects folder:**
   ```bash
   mkdir projects
   ```

2. **Copy the template for each project:**
   ```bash
   cp project-template.html projects/autonomous-rover.html
   cp project-template.html projects/smart-home-hub.html
   cp project-template.html projects/robotic-arm.html
   cp project-template.html projects/smart-grid.html
   cp project-template.html projects/hamlet-lighting.html
   cp project-template.html projects/into-the-woods-sound.html
   cp project-template.html projects/crucible-tech-director.html
   cp project-template.html projects/custom-dmx-controller.html
   ```

3. **Edit each project page** with your actual content

## What to Include in Each Project Page

### Essential Content
- **Project title and type** - Keep consistent with the home page
- **Summary** - 1-2 sentences explaining the project
- **Tech stack** - List the technologies used
- **Project image(s)** - Replace the placeholder with actual photos/screenshots
- **Overview** - What the project is and why you built it
- **Technical details** - How you built it
- **Challenges** - Problems you faced and how you solved them
- **Results** - What you achieved

### Optional Content
- Duration and timeline
- Team size and your role
- Links to GitHub repo or live demo
- Video demonstrations
- Detailed technical diagrams
- Lessons learned
- Future improvements

## Adding Images

1. Create an `images` folder in your project root:
   ```bash
   mkdir images
   ```

2. Add your project images to this folder

3. Update the image placeholder in your project HTML:
   ```html
   <!-- Replace this: -->
   <div class="project-image">
       [Project image here - replace with actual image]
   </div>

   <!-- With this: -->
   <img src="../images/your-project-image.jpg" 
        alt="Project Name" 
        class="project-image"
        style="width: 100%; height: auto; object-fit: cover;">
   ```

## Navigation Between Projects

Update the navigation links at the bottom of each project page to link to your other projects:

```html
<div class="project-nav">
    <a href="previous-project.html">← Previous Project</a>
    <a href="next-project.html">Next Project →</a>
</div>
```

## Example Structure

```
portfolio/
├── index.html
├── project-template.html
├── projects/
│   ├── autonomous-rover.html
│   ├── smart-home-hub.html
│   └── ...
├── images/
│   ├── rover-main.jpg
│   ├── rover-detail.jpg
│   └── ...
└── README.md
```

## Tips

- **Keep it consistent** - Use the same writing style across all project pages
- **Show, don't just tell** - Include images, diagrams, code snippets
- **Be specific** - Use numbers and concrete details
- **Tell the story** - What problem did you solve? How did you do it?
- **Be honest** - It's okay to talk about challenges and what you'd improve

## Deploying to GitHub Pages

After creating your project pages:

1. Commit all files:
   ```bash
   git add .
   git commit -m "Add project detail pages"
   ```

2. Push to GitHub:
   ```bash
   git push origin main
   ```

Your project pages will automatically be available at:
`https://yourusername.github.io/projects/project-name.html`
