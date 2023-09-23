# CasaOS (Edge) AppStore

[![GitHub issues by-label](https://img.shields.io/github/issues/IceWhaleTech/CasaOS-AppStore/help%20wanted?label=help%20wanted&style=for-the-badge)](https://github.com/IceWhaleTech/CasaOS-AppStore/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) [![GitHub contributors](https://img.shields.io/github/contributors/IceWhaleTech/CasaOS-AppStore?style=for-the-badge)](https://github.com/IceWhaleTech/CasaOS-AppStore/graphs/contributors)

[![Number of installs](https://visitly.paodayag.dev/edge.zip/badge?label=Installs)](https://visitly.paodayag.dev)

CasaOS AppStore needs your help to grow:

- See [CONTRIBUTING.md](https://github.com/IceWhaleTech/CasaOS-AppStore/blob/main/CONTRIBUTING.md) for how to contribute CasaOS Apps in Docker Compose format.
- Check `help wanted` for which issues you can help with.

Thank you!

---

### Support me by treating me to a cup of coffee 🥰

[![Buy me a coffee](https://raw.githubusercontent.com/WisdomSky/CasaOS-Coolstore/main/buy-me-a-coffee.png)](https://www.buymeacoffee.com/wisdomsky)


---
## 💡 Information

This is an `Edge` version of the [Official CasaOS Appstore](https://github.com/IceWhaleTech/CasaOS-AppStore/blob/main/CONTRIBUTING.md). 

This version of the CasaOS Appstore attempts to automatically update all the listed apps into their more recent (stable) versions if possible.

The list will update every 24 hours.

## 🚨 Disclaimer

This appstore cannot guarantee that the newer version of an app it automatically resolved to is fully stable and working. 

If there is a new update available, it is best to verify from other sources (reddit, github repo) first if the current (more recent) tag referenced in each app is safe to update to.

---

## 🔥 Installation

Unregister the Official CasaOS Appstore:

    casaos-cli app-management unregister app-store 0

Register the edge version of CasaOS appstore:

    casaos-cli app-management register app-store https://casaos-appstore.paodayag.dev/edge.zip

Done.


---
## 🔃 Restoring back the Official CasaOS Appstore

Get the assigned `ID` of the CasaOS Edge Appstore:

    casaos-cli app-management list app-stores

Unregister the  CasaOS Edge Appstore:

    casaos-cli app-management unregister app-store <casaos-edge-appstore-id>

> NOTE: Replace `<casaos-edge-appstore-id>` with the corresponding `ID` of the CasaOS Edge Appstore.

Register the Official CasaOS appstore:

    casaos-cli app-management register app-store https://github.com/IceWhaleTech/CasaOS-AppStore/archive/refs/heads/main.zip

Done.

---

## 🛠 Troubleshooting

* **I followed and run all the instructions but it seems not working**

    **Solution:** 
    
    _Adding third-party appstores only works on CasaOS v0.4.4 and above._
    
    _Upgrade your CasaOS to at least [v0.4.4](https://blog.casaos.io/blog/23.html)_

* **I receive an Error 404 Not found when running the register command.**

    **Solution:**
    
    _It could be that your CasaOS is running on a port other than port `80`._ 
    
    _You need to tell the command which port your CasaOS is running by passing the `-u` flag together with the `host` and `port`._

    _For example, if my CasaOS is running on port `90`:_

        casaos-cli app-management register app-store https://casaos-appstore.paodayag.dev/edge.zip -u "localhost:90"

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->
