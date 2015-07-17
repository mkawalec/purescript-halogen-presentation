##  Virtual DOM

- A program-side DOM tree definition
- Propagates the smallest possible change set to the actual DOM
- Much saner to work with than real DOM
- Very performing for deep trees, less so for wide ones
- Halogen uses generic `virtual-dom` from npm
