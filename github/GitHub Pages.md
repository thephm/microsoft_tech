# GitHub Pages

GitHub Pages  is a **static site hosting service** provided by GitHub. It allows you to host **HTML, CSS, and JavaScript** files directly from a GitHub repository, making it easy to create and publish personal websites, project documentation, or blogs.
## How GitHub Pages Works

1. **Source Repository** – You create a repository on [[github]] with your website's files (HTML, CSS, JS).
2. **Branch Selection** – GitHub Pages can serve content from specific branches:
    - `main` branch
    - `gh-pages` branch (often used for project-specific pages)
    - `/docs` folder within the repository
3. **Automatic Deployment** – When you push changes to the selected branch, GitHub Pages automatically builds and deploys the site.
4. **Public URL** – Your site is available at:
    
    `https://<username>.github.io/<repository-name>/`
    
##  Types of GitHub Pages Sites

1. **User/Organization Site**
	1. Repository must be named **<username>.github.io
	2. Available at: `https://<username>.github.io/`
	- Only one user/organization site per GitHub account

2. **Project Site**
    
    - Can be created from any repository
    - URL format:
        
        php-template
        
        CopyEdit
        
        `https://<username>.github.io/<repository-name>/`
        
3. **Custom Domain**
    
    - You can configure a custom domain (like `www.example.com`) in the repository settings.

##  Setup Example

### Create a Repository

- Create a new GitHub repository.
- Add your static site files (like `index.html`, `style.css`, `script.js`).

### 2. Enable GitHub Pages

- Go to **Settings → Pages** in the repository.
- Under **"Branch"**, select the branch to use (e.g., `main` or `gh-pages`).
- Save settings - GitHub will generate a public URL.

### 3. Access Your Site

- Visit the generated URL, e.g.,
    
    `https://<username>.github.io/<repository-name>/`
    

## Example: Basic `index.html`

html

CopyEdit

```html
<!DOCTYPE html>
<html>
<head>
    <title>My GitHub Page</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>Welcome to my GitHub Page!</p>
</body>
</html>

```

## Jekyll Support

- GitHub Pages also supports [[Jekyll]] — a static site generator written in Ruby.
- If you include a `_config.yml` file, GitHub will build the site using Jekyll automatically.
- You can use Jekyll themes to style your site without writing CSS from scratch.

## ✅ When to Use GitHub Pages

✔️ Hosting project documentation  
✔️ Personal portfolio or resume site  
✔️ Simple blogs (via Jekyll)  
✔️ Open-source project pages

## 🚀 Advantages

✅ Free for public repositories  
✅ Automatic HTTPS (secure)  
✅ No need for a separate hosting service  
✅ Direct integration with GitHub workflow

## ❌ Limitations

- No backend support — **static files only** (no PHP, Python, etc.)
- Some plugins and Jekyll features are restricted for security reasons
- Bandwidth limit of **100 GB/month** and **10 builds/hour**

### ⭐ Summary

GitHub Pages is ideal for hosting static websites directly from a GitHub repository. It’s simple to set up, secure (with HTTPS), and integrates smoothly with version control. Perfect for personal sites, project documentation, and small web apps! 😎