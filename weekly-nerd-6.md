# Hidde de Vries - Modal Mischief & Dialog Dilemmas
"Toegankelijkheids expert" - Koops

Front-end + Accessibility
Freelance for Dutch government, Mozilla, W3C

Hidde was bezig met het proberen van de standaarden duidelijker te maken voor mensen

Hidde raad aan een blog te beginnen over de dingen die je leert (LOL)

In het begin van het web was content "linear" (onder elkaar)
Tegenwoordig kunnen dingen over elkaar heen liggen

Dialog element werkt sinds kort zo goed dat je het daadwerkelijk kunt gebruiken.

## Terminology

Verschil tussen modal vs non-modal (modeless?)

- Modals: het enige ding waarmee je iets kunt op de pagina, de rest van de pagina is inert (je kunt er niks mee). Voorbeeld: cookie warning. Focus blijft ook alleen binnen de modal.
- Non-modals: voorbeeld hiervan is een deel knop die vervolgens uitklapt en verschillende socials toont waar je iets op kunt delen.

> "Modal element is a dreastic measure, as the user can do nothing else. Use it sparingly!"

Verschil tussen light vs explicit dismiss

Does the element automatically hide on click outside scoll etc? (light)

Explicit dismiss -> user or script closes it

Z-index vs Top layer

With z-index you can stack elements on top of each other. Top layer ligt bovenop de z-index (aller hoogste rank basically)

The top layer is a layer above everything else. In the top layer, full screen content, dialogs and popovers (both new)

Backdrop - sometimes elements have a backdrop. Top layer elements have a built-in styleable backdrop (::backdrop)

Keyboard focus traps - Binnen een bepaald element blijven. Sometimes you want to prevent users from exiting a component with their Tab key. This is always temporary

## Patterns

Dialog - A component that contains an or some task to perform (subwindow).

Modal dialogs vs Non-modal dialogs

- Outside content made inert -> modal: yes if <dialog> open, non-modal: no
- Top later: modal - yes , non modal: no
- Clsoes on Esc key: modal dialog: yes, non modal: maybe (u add it if it makes sense)

<dialog> element comes with semantics -> top layer, inertness, close-on-Esc

div with role="dialog"m just the semantics, no behaviour

Popover - a set of behaviours that can be added to any element through the popover attribute (new)


```html
<div popover></div>
```

It just adds behaviour, it has no built-in role. Differen troles that could apply, dialog, menu, note, tooltip

Popovers voor datepickers, tooltips and toggletips, teaching UI, action menus and toasts (non-modal)

Outside content is made inert? Popovers: no, non-modal: no

popovers on top layer? yes, non-modal: no

Meerdere popovers, welke heeft prio? Kun je controleren? Er is in toplayer geen z-index, dus het gaat per qua HTML volgorde/structure

Popover sluit automatisch met esc

Dialog heeft best wat browser support (93% volgens caniuse.com)

Popover wordt eigenlijk nog nergens support, maar het komt er wel aan. 

Disclosure widgets - Elements that show and hide certain parts of the content, like FAQ or expandable divs??? -> details and summary elements in html

handmatig kan ook:
```html
aria-controls="id"
aria-expanded="true"
```

W3C has Working Groups that work to get consensus oon existing and new Web Standards (like CSS, SVG, WebRTC)

To be in a Working group you need to work for a w3c member. that why thre are community groups, where anyone can join and participate

