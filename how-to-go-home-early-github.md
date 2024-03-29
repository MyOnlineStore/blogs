# How to automate your GitHub workflow and go home early

_If you have more than zero co-workers you are probably using some kind of platform to help you with pull requests and reviews. If your platform of choice is GitHub, you're in luck. We compiled a list of tools and tricks that can help you get your commits merged in that sweet master branch as fast as possible._

### Set up a pull request template

Writing a good pull request template can help you and teammates find a common ground on how to summarize what's in a PR. You can also add a checklist if there are some requirements that have to be met before it can be merged.

![Alt screenshot of example template](https://raw.githubusercontent.com/MyOnlineStore/blogs/master/public/pr-template.png)

### Auto label your pull requests

With the new GitHub actions you can automatically label your pull requests based on what files you touched in your pull request. This can help a lot with the discoverability of your pull request overview.

![Alt screenshot of GitHub action on timeline](https://raw.githubusercontent.com/MyOnlineStore/blogs/master/public/labeler-timeline.png)

To set this up, go to your GitHub repo with actions enabled, click on "New workflow" and once in the marketplace scroll down to "Automate every step in your process" where you'll find the "labeler" action:

![Alt screenshot of GitHub action in marketplace](https://raw.githubusercontent.com/MyOnlineStore/blogs/master/public/labeler-marketplace.png)

### Automatically request reviews with "Code owners" 

We can take the automatic labeling of your pull request one step further. There is a feature in GitHub called "code owners" which lets you assign co-workers to certain parts of your application(s). GitHub will use code owners to automatically assign reviews.

![Alt screenshot of reviewers being assigned](https://raw.githubusercontent.com/MyOnlineStore/blogs/master/public/codeowners.png)

Setting up code owners is easy, check [this guide](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/about-code-owners) to get started with code owners.

### Let a panda spam your co-workers into submission for reviews.

One thing that has been very helpful to our team is the addition of [Pull panda](https://pullreminders.com/). It is a Slack integration that automatically sends a message to your co-workers when someone requests their review. 

When you request a review, the reviewer gets a message like:

![Alt screenshot of pull panda request message](https://raw.githubusercontent.com/MyOnlineStore/blogs/master/public/panda-assigned.png)

If someone approves your pull request, you'll be notified as well:

![Alt screenshot of pull panda request message](https://raw.githubusercontent.com/MyOnlineStore/blogs/master/public/panda-approved.png)

Even if someone comments on your pull request, panda will show you the comments right away in Slack:

![Alt screenshot of pull panda request message](https://raw.githubusercontent.com/MyOnlineStore/blogs/master/public/panda-comments.png)

### Automatically merge the pull request

After applying all these steps, Our pull request get's labeled automatically, the correct reviewers get assigned automatically and they receive a Slack message reminding them that there is work to be done. Now there is one final thing for ~~us~~ the robots to do, merge the pull request into the master branch! If your team uses any form of automated checks on pull requests, you have probably already wasted some time blindly staring at your screen until the merge button turns green.

With another GitHub action called [automerge](https://github.com/pascalgn/automerge-action), this is a thing of the past. This action automatically merges your pull request based the preferences of your team.

![Alt screenshot of GitHub merging the pull request](https://raw.githubusercontent.com/MyOnlineStore/blogs/master/public/automerge.png)

For instance: We set up automerge to merge a pull request once:
- An "automerge" label is added to the pull request
- All required checks are complete and successful
- All the required reviews are approved

And of course after your pull request is automatically merged, you get a message from pull panda:

![Alt screenshot of pull panda automerge message](https://raw.githubusercontent.com/MyOnlineStore/blogs/master/public/panda-automerge.png)

### Conclusion

I hope this list gives you some inspiration on how to automate the little things in your workflow. Even though these steps are probably not the worst bottlenecks for the speed of your team, saving a few minutes per pull request can quickly add up to something worthwhile.

---
If you liked this blog, please let us know by giving us some claps, retweets or likes.

If you think working at MyOnlineStore would be something for you, here are our [job openings](https://www.mijnwebwinkel.nl/vacatures) (NL).

If you have questions about this blog or just want to get in touch, you can tweet to me at https://twitter.com/CarloPalinckx

You can find more of our blogs on [Medium](https://medium.com/myonlinestore) 

Cheers 👋 
