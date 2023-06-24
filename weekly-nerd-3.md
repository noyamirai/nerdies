# Creating Accessible and Award-Winning Websites

During the third weekly nerd episode Cyd Stumpel, a freelance creative developer, shared valuable insights into the world of web development and accessibility

## Cyd's Background and Journey

Cyd began her journey in CMD (Communication and Multimedia Design) in 2014. Her interest in animation grew during a world peace project, which involved setting up a popup shop called "World Peace in a Box" in De Pijp. After the studio she worked for went bankrupt, Cyd ventured into freelancing. In 2021, she was invited to be a jury member for Awwwards, a prestigious award program for web design and development.

## The Accessibility Gap in Award-Winning Websites

Cyd addressed the prevalent issue of award-winning websites lacking accessibility. She attributed this to many developers not being knowledgeable about accessibility, particularly those who are self-taught. Additionally, Cyd noted that even jury members sometimes struggle with evaluating accessibility when judging websites for awards.

## Common Mistakes in Creative Websites

Cyd highlighted some common mistakes found in creative websites that hinder accessibility:

- Removing the ability to select text, which limits the functionality for users who rely on text selection.
- Removing focus styles without providing suitable replacements, making it difficult for keyboard and assistive technology users to navigate.
- Disabling native scrolling functionality, often using custom virtual scrolling libraries instead, which can cause issues for users with specific browsing preferences or assistive technologies.
- Omitting alternative text for buttons, images, and other elements, preventing screen readers from conveying the necessary information.
- Neglecting to provide a text alternative for letter animations, which excludes users who cannot access the visual animation experience.
- Failing to consider user preferences, such as respecting the prefers-reduced-motion setting or other user-configurable options.

## Addressing the Curse of Bad Defaults

Cyd emphasized the need to reassess default settings, reset styles, and go-to code snippets to ensure better accessibility. By rethinking these defaults, developers can proactively create a solid foundation for accessible websites. She also encouraged adding text alternatives for letter, word, and line animations to ensure inclusivity.

## Practical Tips for Improving Accessibility

Cyd provided several practical tips to enhance accessibility in web development:

1. Incorporate native functionality when using virtual scrolling libraries, considering the preferences and needs of users.
2. Respect user settings, including animations, by using appropriate APIs like prefers-reduced-motion or other user-preference detection methods.
3. Utilize ARIA attributes, such as aria-hidden, to control whether an element should be read by screen readers.
4. Explore animation libraries like GSAP to create engaging and accessible animated experiences, demonstrating how to animate text effectively