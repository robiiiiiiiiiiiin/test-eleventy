# Test 11ty 🦝🎈
Could be a "Base 11ty" in a near future.

## 📝 Todo
- Data fetching
- Add JS minification

## 💿 Installation and build / run
1. Clone the repo
2. Run `npm i`
3. Run `npm run watch` or `npm run build`

## 👾 How it works
### Styling
The project uses [Tailwind CSS](https://tailwindcss.com/) for styling.
### JS
At the moment, every file in the `src/assets/js` folder are simply copied in the build directory using `addPassthroughCopy()` in `eleventy.config.js`.
### Image optimisation
`eleventyImageTransformPlugin` automatically generates multiple image sizes and formats (webp, abif, jpg) at build time.  
When you use an `<img>` tag, it will automatically generate a `<picture>` element with the full srcset etc.  
  
The images' `src` attribute needs to be relative (unfortunately).
### Environment variables
The project uses cross-env to set environment variables.  
The variable is set in the `package.json` scripts.  
The code is not minified in dev mode, etc
