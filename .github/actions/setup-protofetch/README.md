# setup-protofetch Action

This action installs the [protofetch](https://github.com/coralogix/protofetch)
tool which we use for managing cross-repo protobuf dependencies. `protofetch` internally
does a `git clone` on other Knox repos in order to fetch the protobuf files, so in order
for this to work this action also sets up a git credentials hook with credentials
coming from an admin-only Github user with cross-repo read privileges.
