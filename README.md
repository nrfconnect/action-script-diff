# action-script-diff

* Execute given script
* Generates a diff over a given file
* Posts a comment to the PR with custom message if there is a diff
* Posts a different comment if there is no diff
* If there is diff and the PR author reacted with a defineable emote, an auto commit is added

## Usage
``` yaml

- uses: nordicbuilder/action-script-diff@v0.1
  with:
    # Token needed to post comments and add commits
    github-token: ''

    # Comment message to post when a diff was detected
    message_diff: ''

    # Comment message to post when no diff was detected
    message_success: ''

    # Relative path and script name to be executed
    script_call: ''

    # File to check for diff
    diff_file: ''

    # Path within the repo where the file to watch is present
    diff_path: ''

    # The PR number to work on
    git_target_pr: ''

    # The root folder for the git diff
    git_diff_root: ''

    # User name to be used in the auto commit (Needs to be 'Firstname' 'Lastname')
    git_user_name: '<Firstname> <Lastname>'

    # E-Mail to be used in the auto commit (Needs to be the verified e-mail of the account to be used)
    git_user_email: ''

    # Github comment remote to check if present
    # See https://docs.github.com/en/rest/reactions/reactions
    # Available emotes:
    # 👍 -1
    # 👎 -1
    # 😄 laugh
    # 😕 confused
    # ❤️ heart
    # 🎉 hooray
    # 🚀 rocket
    # 👀 eyes
    reaction_emote: ''
```
