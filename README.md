# AWC-Maps-Redirect

This is a personal project to manage my multiple map links for AniList AWC challenges in one place. It provides a single, permanent set of URLs that can be updated at any time from one file.

---

## 📁 Structure

<pre>
maps-redirect/
├── index.html          → Main directory page (lists all redirect pages)
├── redirects.js        → Central file that stores all redirect targets
└── redirect.html       → Redirect page (reads query and navigates)
</pre>

## 🔧 How it works

- The **main page** (`index.html`) lists all the maps.  
- The **redirects** are defined in one shared file called `redirects.js`.  
- `redirect.html` reads the to query parameter, looks it up in `redirects.js`, and navigates to the corresponding URL in the same tab.
- Updating `redirects.js` automatically updates all redirect links without changing `index.html` or `redirect.html`.

