[
  {
    "type": "issue_comment",
    "url": "https://github.com/ramaazharywibisana/hello-github-actions/issues/1#issuecomment-787031139",
    "issue": "https://github.com/ramaazharywibisana/hello-github-actions/issues/1",
    "user": "https://github.com/github-learning-lab[bot]",
    "body": "### Actions and Workflows\n\nThere are two components to using GitHub Actions that we'll cover:\n\n- the **action** itself\n- a **workflow** that uses action(s)\n\nA workflow can contain many actions. Each action has its own purpose. We'll put the files relating to the action in their own directories.\n\n### Types of Actions\n\nActions come in two types: **container actions** and **JavaScript actions**.\n\nDocker **container actions** allow the environment to be packaged with the GitHub Actions code and can only execute in the GitHub-Hosted Linux environment.\n\n**JavaScript actions** decouple the GitHub Actions code from the environment allowing faster execution but accepting greater dependency management responsibility.\n\n<!--\nUNCOMMENT WHEN THESE TWO COURSE GO LIVE AND ADD PROPER LINK DETAILS\n📖 To learn more about creating each type of action, refer to the related learning lab course:\n  - [Writing JavaScript Actions]()\n  - [Writing Docker Container Actions]() -->\n\n## Step 1: Add a `Dockerfile`\n\nOur action will use a Docker container so it will require a `Dockerfile`. Let's add it now. We won't discuss what each line means in detail, but the important thing to know is that the action will be executed in an environment defined by this file.\n\n### :keyboard: Activity: Create a `Dockerfile` and open a pull request\n\n1. Create a file titled `action-a/Dockerfile` by [using this quick link](https://github.com/ramaazharywibisana/hello-github-actions/new/main?filename=action-a/Dockerfile) or manually:\n   - Create a new branch. _Branches should be named intentionally, so a good name for this branch could be `first-action`_.\n   - On the new branch, create a directory: `action-a`. _Note:_ If you're working on GitHub.com, you can create a directory and a file at the same time by naming the file `action-a/Dockerfile`.\n   - In the `action-a` directory, create a file titled `Dockerfile`.\n1. Fill the `Dockerfile` with the content below:\n\n   ```Dockerfile\n   FROM debian:9.5-slim\n\n   ADD entrypoint.sh /entrypoint.sh\n   RUN chmod +x /entrypoint.sh\n   ENTRYPOINT [\"/entrypoint.sh\"]\n   ```\n\n1. Commit your file\n   - If you're working locally, you will also need stage your file and to push the branch to GitHub.\n1. Open a pull request with your new branch against `main`\n\n<hr>\n<h3 align=\"center\">I'll respond in your new pull request with next steps.</h3>\n",
    "formatter": "markdown",
    "created_at": "2021-02-27T07:45:23Z"
  },
  {
    "type": "issue_comment",
    "url": "https://github.com/ramaazharywibisana/github-slideshow/issues/1#issuecomment-787036484",
    "issue": "https://github.com/ramaazharywibisana/github-slideshow/issues/1",
    "user": "https://github.com/github-learning-lab[bot]",
    "body": "## Step 1: Assign yourself\n\nUnassigned issues don't have owners to look after them. When you’re assigned to an issue or pull request, it tells repository visitors and contributors that you'll be facilitating the conversation or task :muscle:.\n\n### :keyboard: Activity\n\n1. On the right side of the screen, under the \"Assignees\" section, click the gear icon and select yourself\n\nFor a printable version of the steps in this course, check out the [Quick Reference Guide](https://lab.github.com/public/introduction-to-github.pdf).\n\n<hr>\n<h3 align=\"center\">I'll respond when I detect you've assigned yourself to this issue.</h3>\n\n> _Sometimes I respond too fast for the page to update! If you perform an expected action and don't see a response from me, wait a few seconds and refresh the page for your next steps._\n",
    "formatter": "markdown",
    "created_at": "2021-02-27T08:32:00Z"
  }
]
