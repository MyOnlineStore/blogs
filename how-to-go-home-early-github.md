# How to automate your workflow and go home early (Pull-requests)

_This is a blog series dedicated to becoming the fastest version of yourself by automating tasks that keep you away from actually writing code. I will talk you through how we keep our developers fast and happy at MyOnlineStore._

## Github

If you have more than 0 co-workers you are probably using some kind of platform to help you with pull-requests and reviews. If that platform of choice is Github, you're in luck. We compiled a list of tools and tricks that can help you get your commits merged in that sweet master branch as fast as possible.

### Set up a pull-request template

Writing a good pull request template can help you and teammates find a common ground on how to summarize what's in a PR. You can also add add checklist if there are some requirements that have to be met before it can be merged.

![Alt screenshot of example template](https://raw.githubusercontent.com/MyOnlineStore/blogs/how-to-go-home-early/public/pr-template.png)

### Auto label your pull-requests

With the new github actions you can automatically label your pull requests based on what files you touched in your PR. This can help a lot with the discoverability of your PR overview.

![Alt screenshot of github action on timeline](https://raw.githubusercontent.com/MyOnlineStore/blogs/how-to-go-home-early/public/labeler-timeline.png)

To set this up, go to your github repo with actions enabled, click on "New workflow" and once in the marketplace scroll down to "Automate every step in your process" where you'll find the "labeler" action:

![Alt screenshot of github action in marketplace](https://raw.githubusercontent.com/MyOnlineStore/blogs/how-to-go-home-early/public/labeler-marketplace.png)

### Automatically request reviews with "Code owners" 

We can take the automatic labeling of your PR one step further. There is a feature in github called "Code owners" which let's you assign co-workers to certain parts of your application(s) Github will use codeowners to automatically asign reviews.

![Alt screenshot of reviewers being assigned](https://raw.githubusercontent.com/MyOnlineStore/blogs/how-to-go-home-early/public/codeowners.png)

Setting up code owners is easy, check [this guide](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/about-code-owners) to get started with code owners.

### Let a panda spam your co-workers into submission for reviews.

One thing that helped our team a lot was the addition of [Pull panda](https://pullreminders.com/). It is a slack integration that automatically sends a message to your coworkers when someone requests their review. 

When you request a review, the reviewer gets a message like:
![Alt screenshot of pull panda request message](https://raw.githubusercontent.com/MyOnlineStore/blogs/how-to-go-home-early/public/panda-assigned.png)

If someone approves your pull-request, you'll be notified as well:
![Alt screenshot of pull panda request message](https://raw.githubusercontent.com/MyOnlineStore/blogs/how-to-go-home-early/public/panda-approved.png)

Even if someone comments on your pull-request, panda will show you the comments right away in slack:

![Alt screenshot of pull panda request message](https://raw.githubusercontent.com/MyOnlineStore/blogs/how-to-go-home-early/public/panda-comments.png)

### Automerge the pull-request

Our pull request got labeled automatically, the correct reviewers got assigned automatically and they got a slack message reminding them that there is work to be done. Now there is one last thing ~~we~~ the robots should do, merge the pull-request into the master branch! If your team uses any form of automated checks on pull-requests, you have probably already wasted some time blindly staring at your screen until the merge button turns green.

We can even automate the merging of our pull-request with another github action called [automerge](https://github.com/pascalgn/automerge-action). This action automatically merges your pull-request based on your team's preferences.

![Alt screenshot of github merging the pull-request](https://raw.githubusercontent.com/MyOnlineStore/blogs/how-to-go-home-early/public/automerge.png)

We configured it so that it merges a pull-request once:
- An "automerge" label is added to the pull-request
- All required checks are complete
- All the required reviews are approved

And of course after your pull-request is automatically merged, you get a message from pull panda:
![Alt screenshot of pull panda automerge message](https://raw.githubusercontent.com/MyOnlineStore/blogs/how-to-go-home-early/public/panda-automerge.png)
