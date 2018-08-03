# git-list-old-branches
This is simple shell script for listing all git branches which were committed before specified date.
You can delete those branches like:

```shell
git-list-old-branches -b 20180708 | xargs git branch -D
```

## Usage

```
Usage:
    git-list-old-branches [options]

Options:
    -v    Version
    -h    Show help of this command
    -b    List branches before this date. yyyyMMdd
```

## Installation

### Linux

```shell
curl https://raw.githubusercontent.com/mnc/git-list-old-branches/master/git-list-old-branches | sudo tee /usr/local/bin/rails-console-ecs
sudo chmod +x /usr/local/bin/git-list-old-branches
```

### Mac

```shell
curl https://raw.githubusercontent.com/mnc/git-list-old-branches/master/git-list-old-branches | sudo tee /usr/bin/git-list-old-branches
sudo chmod +x /usr/bin/git-list-old-branches
```

## License
MIT
