
# ct (card tracker)

ct is a Python command line interface application, which makes it easy to keep track of collectable trading cards.


## Features

- Multiple user support
- Check cards into a database using their unique identification code or card name
- Duplicate cards are flagged to user and not checked into the database
- Display total number of unique cards a user has
- Remove cards from a user database
- Remove user from database
- Display all users card counts

## Demo



## Support

Only tested on Linux OS running Python 3.7.2



## Installation

Using the linux command line. Install ct from github into a Python virtual environment.

```bash
  cd ~
  python3 -m venv .venv        # create virtual environment
  source .venv/bin/activate    # activate environment
  python3 -m pip install git+https://github.com/mpflynnx/ct.git     # install from git

```
    
## Usage/Examples

On the Linux command line enter:

```bash

# Check cards into database
ct checkin # prompts user for their firstname, creates new user account if one doesn't exist

ct checkin --name <user-name> # avoid user name prompt

# Display card count for user
ct count # prompts user for name

ct count --name <user-name> # avoid user name prompt

# Remove card from user database
ct remove --card # prompts user for name and card identification code

ct remove --card --name <user-name> # avoid user name prompt

# Remove user account from database
ct remove --user

ct remove --user --name <user-name> # avoid user name prompt

# Display a list of all users and their card count total
ct users

```


## Roadmap

- Microsoft Windows support.
- Automated tests


## Badges

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)
