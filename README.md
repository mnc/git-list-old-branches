# git-list-old-branches
This is simple shell script for listing all git branches which were committed before specified date.
For example, you can delete those branches like:

```shell
git-list-old-branches -b 2018-07-08 | xargs git branch -D
```

## Usage

```
Usage:
    git-list-old-branches -b YYYY-MM-DD [Options]

Requires:
    -b    List branches before this date (YYYY-MM-DD)

Options:
    -v    Version
    -h    Show help of this command
    -a    List local branches and tracking branches if specified
          List only local branches if not specified
```

## Installation

### Linux

```shell
curl https://raw.githubusercontent.com/mnc/git-list-old-branches/master/git-list-old-branches | sudo tee /usr/bin/git-list-old-branches
sudo chmod +x /usr/bin/git-list-old-branches
```

### Mac

```shell
curl https://raw.githubusercontent.com/mnc/git-list-old-branches/master/git-list-old-branches | sudo tee /usr/local/bin/git-list-old-branches
sudo chmod +x /usr/local/bin/git-list-old-branches
```

## License
MIT
