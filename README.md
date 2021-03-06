# git-tags-testing
[Git Basics - Tagging](https://git-scm.com/book/en/v2/Git-Basics-Tagging)

- Add tag to the current state:
	`git tag <tagname>`
- Add tag to the current state with anotations: 
	`git tag -a <tagname> -m <"notes">`
- Add tag to a specific commit:
	`git tag -a <tagname> <commit>`
- List all tags:
	`git tag`
- List all tags matching a pattern:
	`git tag -l <"pattern">`
- Show tag information:
    `git tag <tagname>`
- Push tag to remote server:
	`git push <remote> <tagname>`
- Push all tags to remote server:
	`git push <remote> --tags`
- Delete tag:
	`git tag -d <tagname>`
- Delete remote tag:
	`git tag --delete <tagname>`
- Tags that were deleted from remote repository won't be removed on a git pull. Some tricks are necessary for this: [Remove local git tags that are no longer on the remote repository](https://stackoverflow.com/questions/1841341/remove-local-git-tags-that-are-no-longer-on-the-remote-repository#5373319)
- To see and/or make changes at an other tag:
	`git checkout <tagname>`
- To fix a bug at an older tag, create a new branch:
	`git checkout -b <newbranch> <oldtagname>`
- Than commit the patch:
	`git commit -am <"message">`

## GitHub Releases

- GitHub releases are based on Git tags.
- You can subscribe to receive notifications when new releases are published.
- To create a release, select/create a tag, give the release a title and a description.
- A title may have: date, version number etc.
- A description may have new features, bug fixes, list of commits, links, nothing etc.
- The description is writen using the Markdown syntax.
- If a release is not ready for production, it can be set as a pre-release.
- You can download the source code of a release.
