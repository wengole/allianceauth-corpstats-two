# CorpStats 2.0
### Electric Boogaloo!

[![Coverage Status](https://coveralls.io/repos/github/pvyParts/allianceauth-corpstats-two/badge.svg?branch=master)](https://coveralls.io/github/pvyParts/allianceauth-corpstats-two?branch=master) [![Build Status](https://travis-ci.com/pvyParts/allianceauth-corpstats-two.svg?branch=master)](https://travis-ci.com/pvyParts/allianceauth-corpstats-two)


Extended Corpstats module for [AllianceAuth](https://gitlab.com/allianceauth/allianceauth) with speed and functionality in mind.

Includes:
 * Corp level views
 * Alliance Level views
 * Member Tracking
   * Last Login and Duration
   * Last known ship

Upcoming:
  * Memberr Tracking
    * Last known location of members
 
Based on the hard work of:
 * [Ariel Rin](https://gitlab.com/soratidus999/allianceauth/tree/new-corpstats)
 * [Adarnof](https://github.com/Adarnof/allianceauth/tree/new_corpstats)

Active Devs:
 * [AaronKable](https://github.com/pvyParts)
 
## Installation
 1. Install the Repo `pip install aa-corpstats-two`
 2. Add `'corpstats',` to your `INSTALLED_APPS` in your projects `local.py`
 3. run migrations and restart auth
 3. setup your perms as documented below

## Permissions
If you are coming fromn the inbuilt module simply replace your perms from `corputils` with the matching `corpstats` perm

 Perm | Admin Site	 | Auth Site 
 --- | --- | --- 
corpstats view_corp_corpstats | None | Can view corp stats of their corporation.
corpstats view_alliance_corpstats | None | Can view corp stats of members of their alliance.
corpstats view_state_corpstats | None | Can view corp stats of members of their auth state.
corpstats view_all_corpstats | None | Can view all corp stats.
corpstats add_corpstat | Can create model | Can add new corpstats using an SSO token.
corpstats change_corpstat |Can edit model | None.
corpstats remove_corpstat | Can delete model | None.

## Usage
Is very well documented [here](https://allianceauth.readthedocs.io/en/latest/features/corpstats/#creating-a-corp-stats)

## Contributing
Make sure you have signed the [License Agreement](https://developers.eveonline.com/resource/license-agreement) by logging in at https://developers.eveonline.com before submitting any pull requests.

Todo: Make the readme nicer!