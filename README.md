# homebrew-git-team

Homebrew formula for [git-team](https://github.com/gblues/git-team)

This formula is a temporary work-around for git-team 1.7.0 which does not
build with go 1.18.

## What's different?

This formula lets you install git-team without needing to use `--HEAD`. This
means that new, in-progress code will not be included and potentially cause
problems.

## Installation

1. Add tap
```bash
brew tap gblues/git-team
```

2. Install git-team

Install stable release. Use `--HEAD` in case you want to install from the latest commit.
```bash
brew install gblues/git-team/git-team
```

## Development
```bash
docker run --rm -i -t \
	-v `pwd`/Formula:/home/linuxbrew/.linuxbrew/Homebrew/Library/Taps/hekmekk/homebrew-git-team/Formula \
	linuxbrew/brew:3.1.3 \
	brew install --verbose git-team
```

