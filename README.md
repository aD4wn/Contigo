# KCauldron
### KCauldron - continuation of Cauldron minecraft server
[![Donate PayPal USD][donate_paypal_usd_img]][donate_paypal_usd_url] [![Donate PayPal RUB][donate_paypal_rub_img]][donate_paypal_rub_url]

## Building KCauldron
* Checkout project
  * You can use your's IDE gui or clone from console:
  `git clone https://prok.pw/git/prototik/kcauldron.git`
* Init submodules
  * Since this project is merger of two other we need both.
  * Again, you can use IDE gui or do it from console:
  `git submodule update --init --recursive`
* Setup initial workspace
  * This process download minecraft and apply patches
  * If you have gradle integration in IDE - you can still use gui
  `./gradlew setupCauldron`
* Build server & installer
  `./gradlew buildPackages`

## Updating sources
If you're once checkout source - you not need to do it again
* Update sources
  * `git pull origin master`
* Reapply patches & build binaries
  * `./gradle clean setupCauldron buildPackages`


## Issue submitting rule
* First check the bug in single player and vanilla forge, if bug still present - mod issue
* Check with minimal server environment
  * Remove all unnecessary plugins and mods
  * Reset all configs to default
  If bug present - mod compatibility issue
* If you're using beta-release of KCauldron - check on latest stable
  * All versions situated [there](https://prok.pw/git/Prototik/KCauldron/releases)
* If bug still present - KCauldron issue
  * Make sure that similar issue not exists already
  * Please fill [issue form](https://prok.pw/git/Prototik/KCauldron/issues/new) else

[donate_paypal_usd_url]: https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=me%40prok%2epw&lc=US&item_name=ProK&item_number=KCauldron%20USD&currency_code=USD&bn=PP%2dDonationsBF%3adonate_paypal_usd%2epng%3aNonHosted
[donate_paypal_usd_img]: https://prok.pw/donate_paypal_usd.png
[donate_paypal_rub_url]: https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=me%40prok%2epw&lc=US&item_name=ProK&item_number=KCauldron%20RUB&currency_code=RUB&bn=PP%2dDonationsBF%3adonate_paypal_rub%2epng%3aNonHosted
[donate_paypal_rub_img]: https://prok.pw/donate_paypal_rub.png
