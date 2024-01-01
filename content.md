# Load a Grades project with Codespaces

On the forked repository page, ensure that your on the `main` branch, click the "Code" drop-down button, click the "Codespaces" tab, and click "Create codespace on main":

![](/assets/launch-codespace.png)
{: .bleed-full }

**Note:** Unless you specifically intend to work on another branch of the project, you should make a codespace on `main`. If you don't see that option for `main`, use the `+` icon in the "Code" > "Codespaces" tab to create the codespace _specifically_ on the `main` branch rather than another branch of the repository. You may need to use the drop down selection menu on the left side to switch the viewing branch to `main` before you click through the "Code" > "Codespaces" steps.

This will open a "Setting up your codespace page". 

**Be patient. The first time you setup a codespace for a repository takes about two minutes. But subsequent loads of the codespace will be much faster.**

More details on using codespaces can be found below: 

* [workflow for a codespaces project](#workflow-for-a-codespaces-project){: target="_self"}, 
* [closing and reopening a workspace](#closing-and-reopening-a-workspace){: target="_self"}, 
* [increasing the cores](#increasing-cores-on-a-codespace){: target="_self"}, and
* [sharing snapshots of your work](#sharing-a-codespace-snapshot){: target="_self"}

## Workflow for a codespaces project

The general steps for working on most projects for this course are:

1. Start the web server by running `rackup`, `ruby app.rb`, or `bin/dev` (depending on the project instructions) at the bash prompt, and navigate to your live application preview from the "Ports" tab:

    <!-- ![](/assets/codespace-setup-6.png) -->
    ![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1686013613/codespace-setup-6_db2mdo.png)
    {: .bleed-full }

    <!-- ![](/assets/codespace-setup-7.png) -->
    ![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1680218006/codespace-setup-7_onufud.png)
    {: .bleed-full }

2. As you work, remember to use **Git source control** and **Always Be Committing (ABC)**. Also periodically push your work to GitHub so it is saved there. [See more details on our git workflow here](https://learn.firstdraft.com/lessons/50-git-commit-and-push).

3. Keep your browser tabs organized: lesson, workspace, live preview, target, and a tab for grading results.

4. Run `rake grade` as often as you like at a bash prompt to see how you are doing, but make sure you *test your app manually first* to make sure it matches the target's behavior. [See more details about `rake grade` in this lesson](https://learn.firstdraft.com/lessons/125-using-rake-grade).

You will become very comfortable with these steps while working on several projects for the course.

## Closing and reopening a workspace

Remember to keep the codespace and live application browser tabs open as you work. If you close the workspace window, you can always navigate to [github.com/codespaces](https://github.com/codespaces) to reopen it.

To close a workspace just navigate to [github.com/codespaces](https://github.com/codespaces), scroll down to find the codespace you want to stop, click the `...` menu, and select "Stop codespace". Reopen the codespace by clicking the `...` menu again, and selecting "Open in ..." then "Open in browser":

![](/assets/manage-codespaces.png)
{: .bleed-full }

In this same management menu, you can also un-check the "Auto-delete codespace" option to prevent deletion of the codespace after 30 days of inactivity. But, **as long as you are making git commits and pushing your work to save your progress**, you can always spin up a new codespace directly from the GitHub repository if your current codespace gets deleted.

## Increasing cores on a codespace

If you note poor performance of your codespace, you can increase the number of cores used. By default codespaces are started on a 2-core machine.

### For a new codespace

When you start a codespace for the first time, you can configure this setting by clicking on the menu icon and selecting "+ New with options":

<!-- ![](/assets/codespace-increase-cores-1.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1683650473/codespace-increase-cores-1_xi3awk.png)
{: .bleed-full }

On the next screen, use the drop-down menu to select a 4-core machine (8- or 16-core is not necessary and we do not recommend this right now). After this is selected, click "Create codespace":

<!-- ![](/assets/codespace-increase-cores-2.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1683650486/codespace-increase-cores-2_egselv.png)
{: .bleed-full }

### For an existing codespace

If you want to increase the cores on an existing codespace, navigate to [github.com/codespaces](https://github.com/codespaces), scroll down to find the codespace you want to increase the cores on, and select "Change machine type" from the drop-down menu:

<!-- ![](/assets/codespace-increase-cores-3.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1683650502/codespace-increase-cores-3_jj9erf.png)
{: .bleed-full }

On the next screen, select 4-core and then "Update codespace":

<!-- ![](/assets/codespace-increase-cores-4.png) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1683650510/codespace-increase-cores-4_hobvno.png)
{: .bleed-full }

## Sharing a codespace snapshot

With codespaces, we don't have the ability to [share Gitpod snapshots](https://learn.firstdraft.com/lessons/48-gitpod-setup#sharing-a-gitpod-snapshot) for instructor feedback and debugging. But there's an (even better!) alternative, with Git commits!

Simply follow the [instructions in this lesson](https://learn.firstdraft.com/lessons/50-git-commit-and-push) to make a new commit with your broken code. For the commit message, use **Broken code snapshot X** with X replaced by the number of times you are asking for help on a project (e.g., **Broken code snapshot 1**, **Broken code snapshot 2**, etc.). Be sure to also push the commit to publish it on GitHub with the "Sync" button.

Now you can just send the instructor the URL of your GitHub repository (i.e., your fork of the project at `github.com/<your-username>/<project-name>`) along with the commit message, and we can browse your code at that point in time and try to provide helpful suggestions. 

You can even continue working on your code independently and making additional commits while you wait for the instructor feedback. You won't be overwriting your code from the **Broken code snapshot X** commit that your shared
