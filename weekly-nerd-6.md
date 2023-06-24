# Modal Mischief & Dialog Dilemmas

Hidde de Vries, an accessibility expert with experience in front-end development, delivered an engaging talk on modal and non-modal components, as well as various accessibility considerations during the sixth weekly nerd episode. 

## Terminology

Hidde explained the distinction between modal and non-modal elements. Modals are components that capture user focus and restrict interaction with the rest of the page, while non-modals allow simultaneous interaction with other page elements. Examples of modals include cookie warnings, where the focus remains within the modal. Hidde emphasized the importance of using modals sparingly and considering their impact on user experience.

> "Modal element is a dreastic measure, as the user can do nothing else. Use it sparingly!"

### Light vs. Explicit Dismiss

Hidde discussed two dismissal approaches for modal elements: light and explicit dismiss. Light dismiss occurs when the element automatically hides upon clicking outside or scrolling. On the other hand, explicit dismiss requires user or script action to close the modal. The choice between the two depends on the specific use case and user needs

### Z-index and Top Layer

Hidde introduced the concept of stacking elements using z-index. The top layer, which sits above all other elements, can contain full-screen content, dialogs, and popovers. Popovers are non-modal components that provide additional functionality to an existing element, such as tooltips or datepickers. Hidde also mentioned the use of backdrops, which can be styled and applied to top layer elements.

### Keyboard Focus Traps

To enhance accessibility, Hidde highlighted the importance of keyboard focus traps. These mechanisms prevent users from inadvertently navigating outside a specific component using the Tab key. Focus traps are temporary and applied when necessary, ensuring a seamless user experience within a defined context.

## Patterns

Hidde discussed two primary patterns: dialogs and popovers. Dialogs represent subwindows that contain a specific task or content. Modal dialogs restrict interaction with the outside content, while non-modal dialogs allow concurrent interaction. Hidde highlighted the `<dialog>` element, which provides built-in semantics, including top layer placement, inertness, and automatic closing on the Esc key. Popovers, on the other hand, offer added behaviors to existing elements through attributes like `popover`. Although popovers are not widely supported yet, their functionality is expected to expand in the future.

### Disclosure Widgets

Hidde briefly touched on disclosure widgets, which involve elements that show or hide specific parts of content. Examples include FAQs or expandable sections. HTML provides the `<details>` and `<summary>` elements to create such widgets. Alternatively, developers can manually add ARIA attributes like aria-controls and aria-expanded to achieve similar functionality.

## W3C Working Groups and Community Groups:

Hidde mentioned the significance of W3C (World Wide Web Consortium) in developing and maintaining web standards. Working Groups within W3C focus on achieving consensus on existing and new standards. Hidde clarified that participation in W3C Working Groups requires employment with a W3C member organization. However, Community Groups provide an inclusive platform for anyone to join and contribute.