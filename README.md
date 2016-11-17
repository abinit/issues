## About 

This is a github repository for issues and bugs related to [Abinit](http://www.abinit.org/). 
Users are invited to commit input files that can be used by developers to reproduce the issue,
confirm the bug and work on the bug fix. 
Please note that the purpose of this repository is to facilitate the exchange of input files
between Abinit users and developers. 
This repo is **not** meant to replace our [support forum](http://forum.abinit.org/)
that represents the official reference to be consulted if you are encountering
a problem or you need some help.

## Submitting

### Before you start:

* Search the [forum](http://forum.abinit.org/) and the github 
  [issue tracker](https://github.com/abinit/abinit_issues/issues)
  to ensure that your issue is not a duplicate

* If you think you've discovered a real bug, fork the repository and create 
  a new issue on github (follow the instructions reported below)

### Create a new issue:

* Select the [Issues tab](https://github.com/abinit/abinit_issues/issues)
  on the github interface and click the `New Issue` button.

* Give a meaningful Title to your post that may help us to find/remember your post easily. 

* Fill the sections in the issue template. Be clear and concise in your description and 
  take advantage of [GitHub Flavored Markdown](https://help.github.com/categories/writing-on-github/)

* Submit the issue and take note of the issue identifier generated by github. 
  At this point, you can add the files needed to reproduce the issue. 
  Please follow the instruction reported in the next section.

### Add the files needed to reproduce the issue:

* Fork the repository on github and get a local copy with:
  ```
  git clone git@github.com:YOURNAME/abinit_issues.git
  ```

* Create a new directory named `issue_id` where `id` is the identifier associated 
  to the the issue you've just created on github.

* Please provide whole/complete files neeeded to reproduce the error. More specifically:

    * Abinit input files and files file
    * Pseudopotential files
    * The configuration options and the `config.log` file produced by `configure` (if available)
      or, alternatively, a file with the output of `abinit -b` 
    * Abinit output and log files (optional)
    * Please **do not** add binary files to the repo, we only need the files needed to run
      the code

* Add the files to the repo with `git add issue_id` where `issue_id` is the directory containing your file.

* Commit the changes with `git commit -a` and push them to github with `git push`

* Send us a pull request on github and mention the issue on the Abinit forum (just cut&paste
  the github issue and put a link to it so that other users of the forum will be aware of the problem)
