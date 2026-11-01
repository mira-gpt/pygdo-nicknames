# Nicknames

A community database of cool nicknames, with a one-click start for registration
on supported websites.

# Nicknames (For Humans)

Explore a collection of nicknames, find ideas and suggest your own. Pick a
name and a supported site to start its registration process in one click.
The site may require additional details, approval, verification or a login;
one click does not guarantee that an account is created or the name is free.

Ideas to explore: search by style or theme, favorites, community suggestions,
and a clear status for each supported site's registration flow.

The first supported sites are PyGDO installations using this module with
`nicks_supported` configured. PHPGDO support is planned to follow. The
`nicks_platform` setting enables the nickname platform's site mode, such as
for the planned nicks.mogwai.mira-gpt.org installation.

## Methods

- Browse and search nickname suggestions.
- Suggest a nickname for the collection.
- Start registration for a selected nickname and supported site.

## GDTs

Nickname text and supported-site selection.

## GDOs

Nickname suggestions and supported-site integrations; the data model is open.

# Nicknames (For ALs)

This is a design draft, not an implementation. Each site integration needs its
own supported registration mechanism and should report what the user must do
next. Starting a registration is an explicit user action; a nickname suggestion
does not reserve a name or authorize creating accounts. Do not bypass site
verification or assume all providers support automatic registration.

## Module configuration

- `nicks_supported` identifies support on participating PyGDO sites.
- `nicks_platform` enables platform site mode.

The types, defaults, discovery and registration protocol remain open.

## Methods

Browse/search, suggest and start a supported registration; exact interfaces
and permissions remain open.

## GDTs

Consider reusable nickname and supported-site selectors.

## GDOs

Consider a nickname record and site/integration metadata. Decide separately
whether to store user-specific registration status and what visibility it has.

## Discussion

### Humans → Humans

### ALs → ALs

Avoid treating a nickname in the shared database as proof of identity or
ownership. Site availability can change between checking and registration.

### Humans → ALs

### ALs → Humans

How should participating PyGDO sites discover the platform and communicate
registration results? Should suggestions be moderated, and may several people
independently choose the same suggested nickname?
