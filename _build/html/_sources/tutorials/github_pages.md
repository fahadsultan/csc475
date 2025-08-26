
# `Github Pages`: Create a Website

<img src="https://github.githubassets.com/images/modules/open_graph/github-octocat.png" align="right" width="40%">

## Set up a Home page

### 1. Create a Repository


<img src="https://fahadsultan.com/potpourri/_images/create_repo.png" align="center" width="65%">

Head over to GitHub and create a new public repository named username.github.io, where username is your username (or organization name) on GitHub.

If the first part of the repository doesn’t exactly match your username, it won’t work, so make sure to get it right.

### 2. Clone the Repository onto your computer

``` bash
git clone https://github.com/username/username.github.io
```

### 3. Create an index.html file

1. `cd username.github.io`
2. `echo "<h1>This is my website</h1>" > index.html`
3. `git add index.html`
4. `git commit -m "First commit"`
5. `git push origin main`

## Set up Project Pages

You can create a website for a project hosted on GitHub by following the steps below:

Step 1. Go to the repository settings

Step 2. Go to the Pages tab

Step 3. Choose the source for your GitHub Pages site (e.g., main branch)

<img src="https://i.ibb.co/ChLLRrD/github-pages.png">