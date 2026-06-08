-- Project Description For Landing Page --

This project is a responsive product landing page created for the Sony WH-1000XM4 wireless noise-cancelling headphones. The goal was to design a modern marketing page that highlights the product's key features, benefits, color options, pricing comparison, and promotional video while maintaining accessibility and responsive design principles. The page includes a hero section, feature highlights, product showcase cards, comparison table, embedded promotional video, and footer navigation links.

-- CSS Transform Info --

The project uses a CSS transform on the video section to create a subtle hover interaction.

.video-wrapper:hover,
.video-wrapper:focus-within {
    transform: scale(1.02);
}

This effect slightly enlarges the video container when users hover over it, helping draw attention to the promotional content and creating a more interactive experience.

-- CSS Animation Info -- 

The project includes a custom animation called table-scroll-hint.

@keyframes table-scroll-hint {
    0% {
        transform: translateX(0);
    }

    45% {
        transform: translateX(-0.75rem);
    }

    100% {
        transform: translateX(0);
    }
}

This animation is applied to the comparison table container to provide a visual hint that the table can be scrolled horizontally on smaller screens.

.table-scroll {
    animation: table-scroll-hint 900ms ease-out 450ms 1;
}

-- Table Content -- 

The table used in this project is a feature comparison table.

It compares the Sony WH-1000XM4 headphones against generic headphones using several categories:

- Battery Life
- Noise Cancellation
- Multipoint Connection
- Touch Controls
- Fast Charging

This allows users to quickly evaluate the advantages of the Sony XM4 headphones.

-- Challenges Encountered --

One challenge was creating a layout that worked well across desktop, tablet, and mobile devices. Large images and multiple-column sections looked good on larger screens but required adjustments for smaller displays. The solution was media queries were used to switch grid layouts into single-column layouts and resize typography and images appropriately.

Another challenge was, large comparison tables can become difficult to view on smaller screens. So my solution was a horizontally scrollable container was added around the table, along with a subtle animation to indicate that additional content is available through scrolling.

-- Key Learnings -- 

- Build responsive layouts using CSS Grid.
- Create reusable design systems using CSS custom properties (variables).
- Apply CSS transforms and animations to improve user interaction.
- Design accessible navigation and semantic HTML structures.
- Create responsive tables that remain usable on mobile devices.
- Embed external media while maintaining a consistent visual design.
- Balance visual aesthetics with usability and accessibility considerations.