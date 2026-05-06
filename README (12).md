<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Deploy a Portfolio Site to AWS S3

**Project Link:** [View Project](https://learn.nextwork.org/projects/f629e259-6bbe-4ecf-9765-6f3f4b5f7ec0)

**Author:** naru uzu  
**Email:** rutu13patil@gmail.com

---

![Image](https://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/f629e259-6bbe-4ecf-9765-6f3f4b5f7ec0_rh8fajpk)

## Project Overview

### Goals and motivation

In this project, you will build a personal portfolio site with HTML and CSS. You will manage it with Git and deploy it live to AWS S3.

## Setting Up the Development Environment

### Step goals

Verify that Git and the AWS CLI are installed and configured.

Set your Git username and email for commits.

Confirm your GitHub authentication method.

![Image](https://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/f629e259-6bbe-4ecf-9765-6f3f4b5f7ec0_826ss9jy)

### GitHub authentication method

HTTPS with a personal access token: When you run git push for the first time, Git will ask for your GitHub username and a password. Use a personal access token (not your GitHub password) as the password. You can create one in GitHub under Settings > Developer settings > Personal access tokens.

SSH key: If you already have an SSH key added to your GitHub account, you can use the SSH remote URL instead of HTTPS when linking your repository later.

## Initializing a Local Repository and Pushing to GitHub

### Step goals

Create a local Git repository with a starter HTML file.

Create a new repository on GitHub.

Connect the two and push your code.

### Understanding git init and the first commit

The git init command initialize the folder as a Git repository
My first commit represents the main (first commit) to that repository.

![Image](https://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/f629e259-6bbe-4ecf-9765-6f3f4b5f7ec0_tkc771tj)

### Local repo vs. GitHub remote

The relationship
Your local repo and the GitHub repo are linked via a remote (usually called origin)
They both store the same project history (commits), but can be out of sync.

How they interact
git push → sends your local commits to GitHub
git pull → brings changes from GitHub to your local repo
git fetch → checks for updates without merging

Key idea
Local = where you make changes and commit
Remote (GitHub) = where you store, share, and collaborate


Simple analogy
Your local repo is like your notebook, and GitHub is like a cloud backup + shared workspace.

Important detail
Connecting them doesn’t automatically sync anything.
You still need to:
push your commits to upload them
pull to get others’ changes

If you want, I can show you a quick visual flow (commit → push → pull) that makes this super intuitive.

## Building the Portfolio with Feature Branches

### Step goals

Create a feature branch for your portfolio content.

Build out the HTML and CSS for your portfolio page.

Commit and push the feature branch to GitHub.

![Image](https://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/f629e259-6bbe-4ecf-9765-6f3f4b5f7ec0_22ymnthp)

### Why feature branches matter

Professional developers don't build directly on main. They create feature branches to develop new content in isolation, then merge it back when it's ready.

## Opening a Pull Request and Merging on GitHub

### Step goals

Open a pull request on GitHub for your feature branch.

Review the code diff and merge the pull request.

Pull the merged changes back to your local machine.

![Image](https://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/f629e259-6bbe-4ecf-9765-6f3f4b5f7ec0_4d3640l3)

### The role of pull requests in team workflows

A pull request lets team members see the changes you have added to the file.

## Deploying a Live Portfolio Site to AWS S3

### Step goals

Create an S3 bucket configured for public website hosting.

Upload your portfolio files to S3 using the AWS CLI.

Visit your live portfolio site in the browser.

![Image](https://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/f629e259-6bbe-4ecf-9765-6f3f4b5f7ec0_egvjf6ea)

### S3 endpoint URL and the sync command

S3 website endpoints follow this format: http://BUCKET-NAME.s3-website-REGION.amazonaws.com. 
my = http://rutup-portfolio.s3-website.ap-south-1.amazonaws.com
This is the public address anyone can use to view your site.

## Simulating and Resolving a Merge Conflict

### Triggering and resolving the conflict

In this project extension, I triggered a merge conflict by editing the same line in the main and feature repositories.
I tried to merge feature repo with main so a merge conflict emerged in VS code wich higlighted it by >>>> and <<<< and ==== difference was laos shown . I deleted the extra symblos and chose one of the changes to go with.


![Image](https://learn.nextwork.org/content_rose_beautiful_white_sapote/uploads/f629e259-6bbe-4ecf-9765-6f3f4b5f7ec0_l9ai4jnr)

## Reflections and Key Takeaways

### Tools and concepts learned

S3 bucket with static website hosting enabled and a public bucket policy.
GitHub repository (portfolio-site).
Local project folder (portfolio-site on your Desktop).

### Time and challenges

This project took me a little while but meanwhile i understood the Branch, Merge concept Push and Pull concept for Git. 

### Personal reflection

I did this project today to learn more on how to utilise git and github.

---

*Built with [NextWork](https://learn.nextwork.org) - [View this project](https://learn.nextwork.org/projects/f629e259-6bbe-4ecf-9765-6f3f4b5f7ec0)*
