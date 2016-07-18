# GitMeet-template
Simple plug-n-play markdown blog website for node.js

> This template was created for my personal blog at [gitmeet.com](http://gitmeet.com). But due to it's portability and markdown writing format, I guess this help you set up your personal blog within 5 mins.

--

# System requirement
- node.js
- mongodb

--

# Install and configure
- copy latest release of this repo (download and extract .zip file)
- open cmd/terminal and run `npm install --production`
- open cmd/terminal and run `bower install` (install bower `npm install -g bower`) 
- edit `index.html` file in your parent directory.
- edit `about.html` from `/templates/`
- edit `createAdmin.js` file from `/api\__once`. Set appropriate credentials. Run this file with node (`node createAdmins.js`). This will create admin document in mongodb to create and manage your posts.
- run `web-server.js` file from parent directory with node. This will start http server at port 8881.
- **sign in** from `/admin/signin`
- **add** post from `/admin/add-post`
- **edit** post from `/admin/edit-post/post-id`. Post id is string followed by `/post/` in url of your post.
- **delete** post by clicking delete button on **edit** page.

--

# build
-  open cmd/terminal 
-  run `npm install` to install npm dependencies.
-  install gulp globally `npm install -g gulp`
-  build using `gulp build` command.

--

# disqus comments
- go to [disqus.com](disqus.com) and create a admin account. Get your **shortname**.
- if you are building the repo with gulp, replace `gitmeet` with your *shortname* in `assets/js/src/app/app.js`
- else replace `gitmeet` with your shortname in `.setShortname("gitmeet")` inside `assets/js/dist/app.min.js`.

-- 

# bug reports and contributions
- If you face any problems, create a github issue or email me on `uhiwarale@gmail.com`
- If you make any improvements or optimization, please share with us all by giving a PR.
- If you want to use it for commercial purpose, please take permission first.
