# Frontend Setup in Production

During the ninth weekly nerd episode, Chanel, a frontend developer at Triple, shared insights into the frontend setup in production at Triple.

## Background and Triple Clients
Chanel, a CMD graduate in 2018, expressed her love for games, board games, sports, and watching series. She works at Triple and mentioned some of the clients they collaborate with, including Ajax, Max Verstappen, Citizen M, NLZIET, Heineken, and more.

## Web Standards at Triple
Chanel emphasized the significance of adhering to web standards at Triple. She highlighted three key aspects of their frontend setup: Git, NPM, and code quality tools.

### Git

Chanel stressed the importance of using version control, such as Git, for several reasons. Git enables rollbacks to previous versions in case of emergencies, aids in debugging, and facilitates collaboration on large and long-term projects. She outlined the workflow they follow, which involves creating a feature branch from the main branch, committing and pushing changes, creating pull requests for feedback from other developers, merging the approved code into the main branch, and deployment.

### NPM

Chanel briefly mentioned NPM (Node Package Manager) and its usage in their frontend setup. However, she also highlighted the potential security risks associated with using packages from NPM. She suggested considering factors such as package maintenance, age, weekly downloads, number of contributors, package size, and preferred avoidance of package dependencies. She also emphasized the importance of checking licenses for the packages used.

### Setup and Frameworks

Chanel discussed the choice between using Vanilla JavaScript, libraries, or frameworks. While Vanilla JavaScript allows for reusability, Triple often opts for frameworks or libraries to develop faster and more scalable web applications. React and Next.js are the go-to choices at Triple, although Chanel acknowledged that React may have limitations in terms of SEO (DOM creation). She mentioned their recent shift to Svelte, which is lighter, requires less code than React, easier to learn, and closer to JavaScript. The decision to switch to Svelte was motivated by the need to support TV smart applications, where React poses challenges.

### Error Catching and Code Quality Tools

To identify issues in their code early on, Chanel highlighted the use of Typescript. It helps catch problems before they occur, ensuring code quality. They also utilize ESLint for maintaining a consistent codebase and Prettier for formatting code.

### CSS and Vite
For CSS, Chanel recommended using SASS as it provides more robust error handling and improved maintainability. Additionally, she mentioned Vite, a build tool that enables fast project startup.

### Deployment Process

Chanel addressed the deployment process, emphasizing the distinction between React (static) and Node.js. Azure and Azure DevOps were mentioned as the chosen deployment tools. Chanel described the deployment pipeline, which involves building and validating the code in each pipeline before progressing to the next stage. They follow a three-environment setup: development, acceptance (for client testing), and production.
