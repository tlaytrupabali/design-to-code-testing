# Design-to-code approach with Figma Low-Code & Luisa

### Introduction:

The Luisa framework is an OpenSource project that turns Figma and Quant-UX designs into fully functional VUE applications. It focuses solely on the front-end code (HTML and CSS) of a user interface, and leaves the implementation of the business logic in code. The Luisa works currently with VUE.js, and is just another NPN dependency.

The Figma-Low-Code project is open-source and free to use. The project enables a new kind of collaboration between developers and designers and reduces the friction between both roles. The visual design maintains the single source of truth, and allows the front-end developers to focus on business logic and backend connectivity. Design changes are automatically updated in the UI, without jeopardizing the existing code base.

Once an initial design is ready, the developers use the Figma-Low-Code plugin to specify which UI elements to use (e.g. input fields, DropDowns, Text Area, etc.) by adding metadata to the design. This metadata contains the wiring between the design and the application data and business logic. The Low-Code components must be imported into the VUE application and configured with a link to the Figma design. The design is automatically rendered without a single line of UI code.
Luisa loads the Figma design from a file (or during development from the Figma API) and creates the required DOM elements and CSS styles on the fly. 

The data exchange between the LowCode component and the application is based on a ViewModel and data binding.

### How it works:

1. Create your design in Figma and use the Figma-Low-Code Plugin to define which elements will be rendered as real input elements in the browser.
2. Install the luisa-vue package in your VUE project and use the <Luisa> component to render your design on the fly. Design changes are updated instantaneously.
3. Write custom business methods and wire them to the right elements. Define a view model and bind it to Figma elements to show dynamic data and read user input.
4. Once your application is ready, freeze the design and deploy the app. All apps are fully self contained and run as fast as normal single page applications build with VUE.

> As a result, the development process is simplified as there is no hand-off and the amount of front-end code is drastically reduced.
>