# gears

Gears is a event-driven flexible site engine with hook feature.

In this project I ignore PSR-0 and many other PSR as I deprecate to many their paragraphs. Especially coding styles and code structure. I permit on using composer but do not insist upon it.

I tried to split user business logics and Core in order to ease user to create many sites (e.g. front sites as back sites) and tools over one engine. To ease the wrapping of other embedded website engines.

### Simple structure is
```
/gears/* - Core folder
/userspace/spacename/* - user's folder
/userspace/current/ - link to most recent front site (e.g. ~spacename)
/userspace/public/ - any public things such as uploads
/etc - system/global preferences
/tmp - site temporaries
/var - work engine (e.g. caches)
/lib - third-party libarries. The Core completely use one.
/static - link to static user files might be accessed as static.sitename.com in ~/userspace/static
/static/theme - link to user's theme files from ~/userspace/current/static
/public 
/doc - different documentation
```
