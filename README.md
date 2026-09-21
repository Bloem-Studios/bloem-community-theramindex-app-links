## Bloem community build

This is Bloem's community build of [theramindex/silo-plugin-app-links](https://github.com/theramindex/silo-plugin-app-links) by **theramindex**
(contributors: theramindex). It is ported to the Bloem plugin SDK and listed in the
Bloem community plugin catalog. All credit for the plugin goes to its author; please
report plugin behavior issues upstream. See [NOTICE](NOTICE) for provenance.

---

# Silo App Links

Silo plugin that adds an Apps launcher for external services. Admins manage links in a custom admin panel. Users open links in a Silo-hosted fullscreen iframe shell or in a new tab.

## Storage

Links are stored in JSON. By default the plugin writes:

`/var/lib/continuum/plugins/silo.ramindex.app-links/app-links.json`

Override with:

`APP_LINKS_DATA_FILE=/path/to/app-links.json`

## Routes

- User app: `/app-links`
- Fullscreen iframe shell: `/app-links/open?id=<link-id>`
- Admin manager: `/app-links/admin`
