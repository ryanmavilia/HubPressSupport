=== Installation
==== Fork the repository
Click the Fork icon image:http://hubpress.io/img/fork-icon.png[Fork,80] to create a copy of this repository within your GitHub account.

==== Use the github.io domain

If you have never used your GitHub Pages domain before, you can use this procedure to quickly set up HubPress. With this method, only a few steps are required to get HubPress deployed and ready for use.

IMPORTANT: If you are currently using your `username.github.io` GitHub Pages domain for another project, or if you want to use a custom domain name, skip to the next procedure for instructions.

. Rename your repository to `<username>.github.io`

. Set values in `hubpress/config.json`
+
image:http://hubpress.io/img/edit-config.png[Edit config]
+
The following parameters are mandatory :
+
* `username`, which is your GitHub user name,
* `repositoryName`, which is the new name of the repository fork, `<username>.github.io`.
. Commit the changes, and open the GitHub Pages domain:  `http://<username>.github.io/`.
. The following screen indicates you have correctly configured HubPress
+
image:http://hubpress.io/img/home-install.png[Install complete,300]

==== Use a Custom Domain or GitHub Page Domain Already In Use

If you want your blog to be available on a custom domain, or you are already using your GitHub Pages domain to host another project, some extra configuration is required.

. In the repository settings, set the default branch to `gh-pages` :
+
image:http://hubpress.io/img/settings-gh-pages.png[Settings gh-pages,400]
. Switch your repository to the branch *gh-pages*
+
image:http://hubpress.io/img/switch-gh-pages.png[Install complete,300]
+
. Set the required values in `hubpress/config.json
+
image:http://hubpress.io/img/edit-config-gh-pages.png[Edit config]
+
The following parameters are mandatory :
+
* `username`, which is your GitHub user name,
* `repositoryName`, which is the repository fork. For example, `hubpress.io` if you did not rename it.
. Commit the changes, and open the GitHub Pages domain:  `http://<username>.github.io/<repositoryName>/`.
. The following screen indicates you have correctly configured HubPress
+
image:http://hubpress.io/img/home-install.png[Install complete,300]

== Administration Console

The HubPress Administration Console is available at */hubpress*

* `http://<username>.github.io/hubpress/` for GitHub Hosted blogs, or
* `http://<username>.github.io/<repositoryName>/hubpress/` for Domain Hosted blogs.

=== Log Into the Administration Console

image:http://hubpress.io/img/login.png[Install complete,300]

Enter your GitHub credentials to log into HubPress Admin.

Once you authenticate, a personal token is created for future calls from HubPress to the GitHub API.

This is synchronized across all sessions of HubPress, so if you open the Administration Console on your PC and then your Tablet, the token is applicable to all devices.

=== Settings Page

You can configure basic blog settings (such as CNAME and Pagination) and social media accounts you want to connect to your blog.
