# template.app.5ls.de



---

# Foreach new Repo:
- Enable Github Pages with custom domain "*.app.5ls.de"
- Enforce HTTPS
- Link in about with "https://"
- Favicons:
  - main SVG as "icon.svg"
    - [SVG Repo](https://www.svgrepo.com) *(but have an eye on the [licence](https://www.svgrepo.com/page/licensing) of each svg)*
  
  - [create favicons](https://realfavicongenerator.net/)
    - "Favicon for iOS - Web Clip": Add a solid #ffffff
    - "Favicon for Android Chrome": Add a solid #ffffff, App name, Options -> Start URL -> "/"
    - "Windows Metro": Use this color #960e4d, Use a white silhouette, Windows 8.1 and 10 / IE 11 and Edge -> {Small square icon, Medium square icon, Big square icon}
    - "macOS Safari": Theme color #960e4d
    - "Favicon Generator Options": Path -> "/icons", App name -> Specific app name
  - save favicon.ico,icon.svg,manifest.json in root directory
  - [create maskable icon](https://maskable.app/editor) (in Chrome)
    - add Backgroudcolor: #ffffff
    - change **only** padding such that edges are barely not touching
    - add to manifest
```
{
  …
  "icons": [
      {…},
      {
          "src": "/icons/maskable_icon.png",
          "sizes": "1024x1024",
          "type": "image/png",
          "purpose": "any maskable"
      }
  ]
  …
}
```
- add to manifest   ```  "description" : "A Template for generating new tools @app.5ls.de", ```



# Best Practises
- [Semantic Versioning](https://semver.org/)
