# Login to Zenodo

Next, head over to [Zenodo](http://zenodo.org/) and click the **Log in** button at the top right of the page, which gives you an option to login with your GitHub account.

![login](https://guides.github.com/activities/citable-code/zenodo-login.png)

Zenodo will redirect you back to GitHub to ask for your permission to share your email address and the ability to configure [webhooks](https://developer.github.com/webhooks/) on your repositories. Go ahead and click **Authorize application** to give Zenodo the permissions it needs.

> **Important!** If you want to archive a repository that belongs to an organization on GitHub, you will need to make sure that the organization administrator has enabled [third-party access](https://help.github.com/articles/approving-third-party-applications-for-your-organization/) to the Zenodo application.

![auth](https://guides.github.com/activities/citable-code/zenodo-authorize.png)

#### Pick the repository you want to archive

At this point, you’ve authorized Zenodo to configure the repository webhooks needed to allow for archiving and DOI-issuing. To enable this functionality, simply click the **On** toggle button next to your repository \(in this case **My-Awesome-Science-Software**\).

> **Important!** Zenodo can only access your public repositories so make sure the repository you want to archive is [public](https://help.github.com/articles/making-a-private-repository-public/).

![toggle](https://guides.github.com/activities/citable-code/zenodo-toggle-on.png)

