A fork with minor custom changes that allows to use AdNauseam in a familiar for uBO users way.

***

Below changes to `manifest.json` change the default AdNauseam popup menu to the familiar dashboard from uBO.

Was:

    "default_popup": "menu.html"

Became:

    "default_popup": "popup-fenix.html"

AdNauseam's list of clicked ads and ad vault menu is still available via the internal link which is best saved to your browser bookmarks if you still need this menu.

    chrome-extension://dkoaabhijcomjinndlgbmfnmnjnmdeeb/menu.html

It is worth going there periodically and clearing the database of clicked ads. Instead `dkoaabhijcomjinndlgbmfnmnjnmdeeb` must be your AdNauseam's extension id which can be found on `chrome://extensions` page.

Below changes to `manifest.json` extend AdNauseam's options page with more settings like in uBO.

Was:

    "options_ui": {"page": "options.html"}
  
Became:

    "options_ui": {"page": "dashboard.html"}

Note that AdNauseam allows you to import your settings from uBO.

Below changes eliminate lags and slowdowns noticeable when accessing exptension's options menu on certain low-end/mid-end configurations.

Three giant images `gray_grid.png`, `gray_grid_light.png`, `adn_clickbot_bg.jpg` in src/img folder replaced with 1x1 pixel size dummies.

***

<!-- [![Build Status](https://travis-ci.org/dhowe/AdNauseam.svg)](https://travis-ci.org/dhowe/AdNauseam) -->
![version](https://badgen.net/amo/v/adnauseam) ![stars](https://badgen.net/amo/stars/adnauseam) <a href="https://www.gnu.org/licenses/gpl-3.0.en.html"><img src="https://img.shields.io/badge/license-GPL-orange.svg" alt="gpl license"></a> [![open-collective](https://opencollective.com/adnauseam/tiers/badge.svg)](https://opencollective.com/adnauseam#category-CONTRIBUTE)

***

<div align="center">
  <a href="https://adnauseam.io">
    <img src="https://rednoise.org/images/adnauseam.png" width="150px"/>
  </a>
</div>

***

<p align="center">
<a href="https://addons.mozilla.org/en-US/firefox/addon/adnauseam/"><img src="https://user-images.githubusercontent.com/585534/107280546-7b9b2a00-6a26-11eb-8f9f-f95932f4bfec.png" alt="Get AdNauseam for Firefox"></a>
<a href="https://microsoftedge.microsoft.com/addons/detail/adnauseam/mlojlfildnehdpnlmpkeiiglhhkofhpb"><img src="https://user-images.githubusercontent.com/585534/107280673-a5ece780-6a26-11eb-9cc7-9fa9f9f81180.png" alt="Get AdNauseam for Microsoft Edge"></a>
<a href="https://addons.opera.com/en/extensions/details/adnauseam-2/"><img src="https://user-images.githubusercontent.com/585534/107280692-ac7b5f00-6a26-11eb-85c7-088926504452.png" alt="Get AdNauseam for Opera"></a>
      <br><sub><a href="https://twitter.com/gorhill/status/1033706103782170625">It is <b>not</b> recommended to use AdNauseam at the same time as other similarly-purposed blockers</a></sub>
      <!--<br><sub>See below for <a href="#installation">more installation options.</a></sub>-->
</p>

<p align="center">
<a href="https://github.com/dhowe/AdNauseam/wiki/Install-AdNauseam-on-Chrome-Without-Google's-Permission">Instructions on how to install AdNauseam in <b>Google Chrome</b></a>
<!--<sub><a href="https://github.com/uBlockOrigin/uBlock-issues/wiki/About-Google-Chrome's-%22This-extension-may-soon-no-longer-be-supported%22"><b>IMPORTANT</b>: About Google Chrome's "This extension may soon no longer be supported"</a></sub>-->
</p>

***

[AdNauseam](https://adnauseam.io) is a lightweight browser extension that blends software tool and artware intervention to actively fight back against tracking by advertising networks. AdNauseam works like an ad-blocker (it is built atop [uBlock Origin](https://github.com/gorhill/uBlock)) to silently simulate clicks on each blocked ad, confusing trackers as to one's real interests. At the same time, AdNauseam serves as a means of voicing your discontent with advertising networks that disregard privacy and engage in bulk surveillance.

In light of the industry's failure to address the excesses of network tracking, AdNauseam allows individual users to take matters into their own hands, offering active defense against surveillance, profiling and potential discrimination. The software thus represents a similar approach to that of <a href="https://rednoise.org/daniel/res/pdfs/trackmenot2009.pdf" target="_blank">TrackMeNot</a>, relocating power in the hands of individual users, rather than vast commercial entities. For further information on this approach, please see <a href="https://rednoise.org/daniel/res/pdfs/trackmenot2009.pdf" target="_blank">this paper</a>.


#### About the project
--------

* Web Site:         https://adnauseam.io
* Authors:          [Daniel C. Howe](https://rednoise.org/daniel), [Helen Nissenbaum](https://www.nyu.edu/projects/nissenbaum/) and [Mushon Zer-Aviv](http://mushon.com)
* Developers:       [Daniel C. Howe](https://rednoise.org/daniel), [Sally Chen](https://github.com/cqx931) and [Alberto Harres](https://github.com/mneunomne)
* License:          GPLv3 (see included [LICENSE.txt](https://github.com/dhowe/AdNauseam/blob/master/LICENSE.txt) file for full license)
* Github Repo:      https://github.com/dhowe/adnauseam/
* Bug Tracker:      https://github.com/dhowe/adnauseam/issues
* FAQ:              https://github.com/dhowe/adnauseam/wiki/FAQ


#### Can I contribute?
--------
Absolutely! We are looking for coders, designers, and [translators](https://crowdin.com/project/adnauseam) to help on the project.

If you are a coder or designer, just press *Fork* at the top of this github page and get started... Or, if you'd like to contribute a translation, please visit [this page](https://crowdin.com/project/adnauseam).

If you're not sure where to start, look at the issues labeled [HELP US CODE](https://github.com/dhowe/AdNauseam/labels/HELP-US-CODE). Thanks!

#### How to install the development environment

1. [Fork and clone](https://help.github.com/articles/fork-a-repo) this repository:

    ```bash
    $ git clone https://github.com/dhowe/AdNauseam.git
    ```

2. [How to build the extension for various browsers](https://github.com/dhowe/AdNauseam/wiki/Building-AdNauseam-from-source-(for-developers))

<br>

Or, support us with a monthly donation and [become a backer](https://opencollective.com/adnauseam#backer)!

<br>

[![open-collective](https://opencollective.com/adnauseam/contributors.svg?width=890)](https://github.com/dhowe/adnauseam/graphs/contributors)

##### And special thanks to our open-source support contributors!

<img src="https://pagekite.net/static/skin/i/pagekite-logo.png" width="100"/>

<br>
