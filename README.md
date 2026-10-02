# LaitHaus PNG website

Website for **LaitHaus PNG Ltd**, the telecommunications tower company and subsidiary of Wantok Radio Light. The company runs tower sites at Burns Peak, Port Moresby, and 11 Mile, Lae.

It is a static site: one `index.html` file plus images. There is no build step and nothing to install.

## Pages

The menu links to five pages. They all live in `index.html` and are reached with links like `#about`:

- Home
- About (`#about`)
- Infrastructure (`#infrastructure`)
- Clients (`#clients`)
- Contact (`#contact`)

## Folder layout

```
index.html        the whole site (styles, fonts and scripts are inside it)
img/              photos
img/clients/      partner logos
img/team/         staff photos
404.html          sends wrong addresses back to the home page
.nojekyll         tells GitHub Pages to serve the files as they are
```

## Publish with GitHub Pages

1. Create a new repository on GitHub, for example `laithaus-png-website`.
2. Upload everything in this folder, including the hidden `.nojekyll` file, to the root of the repository.
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**. Choose the branch `main` and the folder `/ (root)`, then click **Save**.
5. After a minute or two the site is live at `https://<your-github-username>.github.io/laithaus-png-website/`.

### Use your own domain (optional)

1. In **Settings → Pages → Custom domain**, enter your domain (for example `www.laithauspng.com.pg`) and click **Save**.
2. At your domain registrar, add a `CNAME` record that points `www` to `<your-github-username>.github.io`.
3. Once the domain works, tick **Enforce HTTPS**.

## After the site is live

- In `index.html`, change `og:image` and `og:url` to full addresses, such as `https://www.laithauspng.com.pg/img/hero.jpg`. This makes the preview image appear when the link is shared on Facebook or WhatsApp.
- The two YouTube videos only play on the page once the site has a real web address. Opening `index.html` straight from your computer shows a "watch on YouTube" message instead.
- The contact form gets the visitor's message ready for them to send by email. For messages to arrive automatically, connect a form service such as Formspree.

## Updating content

- **Text:** edit `index.html` in any text editor.
- **Partner list:** edit the `clients` list near the bottom of `index.html`.
- **Images:** replace a file in `img/` with another file of the same name.
