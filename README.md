# gvenkatagiri.github.io

## adding a new .md file (a new post) inside Hugo
- `$REPO_TOP/hugo_content` is where I keep the `.md` files for all the blog posts
- I've soft-linked the Hugo `quickstart/content/posts` folder to my `$REPO_TOP/hugo_content` folder
- If I want an image in my post, I put the image file in `quickstart/static` and then reference it in the post `.md` file
- Once the new `.md` file and image have been added, I just execute `hugo` inside `quickstart/`

## pushing Hugo-generated content to this pages repo
- should have already executed `hugo` inside `quickstart/`
- CWD should be the github-pages REPO_TOP
- content is already available in the hugo `quickstart/public/` folder
  - `cp -rf ../quickstart/public/* ./docs/`
  - `git add -A .` , `git commit -m "new hugo content"` , `git push`
