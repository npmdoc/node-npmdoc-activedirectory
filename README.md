# api documentation for  [activedirectory (v0.7.2)](https://github.com/gheeres/node-activedirectory#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-activedirectory.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-activedirectory) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-activedirectory.svg)](https://travis-ci.org/npmdoc/node-npmdoc-activedirectory)
#### ActiveDirectory is an ldapjs client for authN (authentication) and authZ (authorization) for Microsoft Active Directory with range retrieval support for large Active Directory installations.

[![NPM](https://nodei.co/npm/activedirectory.png?downloads=true)](https://www.npmjs.com/package/activedirectory)

[![apidoc](https://npmdoc.github.io/node-npmdoc-activedirectory/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-activedirectory_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-activedirectory/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-activedirectory/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-activedirectory/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "George Heeres",
        "email": "gheeres@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/gheeres/node-activedirectory/issues"
    },
    "dependencies": {
        "async": ">= 0.1.22",
        "bunyan": ">= 1.3.5",
        "ldapjs": ">= 0.7.1",
        "underscore": ">= 1.4.3"
    },
    "description": "ActiveDirectory is an ldapjs client for authN (authentication) and authZ (authorization) for Microsoft Active Directory with range retrieval support for large Active Directory installations.",
    "devDependencies": {
        "mocha": "^2.2.5"
    },
    "directories": {
        "lib": "./lib"
    },
    "dist": {
        "shasum": "19286d10c6b24a98cc906dc638256191686fa91f",
        "tarball": "https://registry.npmjs.org/activedirectory/-/activedirectory-0.7.2.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "gitHead": "416b201e188d7748bbaaaf888eba131c4bf6ebd4",
    "homepage": "https://github.com/gheeres/node-activedirectory#readme",
    "keywords": [
        "ldap",
        "active directory"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "gheeres",
            "email": "npm@heeresonline.com"
        }
    ],
    "name": "activedirectory",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/gheeres/node-activedirectory.git"
    },
    "scripts": {},
    "version": "0.7.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module activedirectory](#apidoc.module.activedirectory)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>filters.AndFilter (options)](#apidoc.element.activedirectory.filters.AndFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>filters.ApproximateFilter (options)](#apidoc.element.activedirectory.filters.ApproximateFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>filters.EqualityFilter (options)](#apidoc.element.activedirectory.filters.EqualityFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>filters.ExtensibleFilter (options)](#apidoc.element.activedirectory.filters.ExtensibleFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>filters.GreaterThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>filters.LessThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>filters.NotFilter (options)](#apidoc.element.activedirectory.filters.NotFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>filters.OrFilter (options)](#apidoc.element.activedirectory.filters.OrFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>filters.PresenceFilter (options)](#apidoc.element.activedirectory.filters.PresenceFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>filters.SubstringFilter (options)](#apidoc.element.activedirectory.filters.SubstringFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.</span>super_ ()](#apidoc.element.activedirectory.super_)
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.AndFilter.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.AndFilter.super_.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.ApproximateFilter.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.ApproximateFilter.super_.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.EqualityFilter.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.EqualityFilter.super_.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.ExtensibleFilter.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.ExtensibleFilter.super_.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.GreaterThanEqualsFilter.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.GreaterThanEqualsFilter.super_.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.LessThanEqualsFilter.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.LessThanEqualsFilter.super_.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.NotFilter.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.NotFilter.super_.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.OrFilter.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.OrFilter.super_.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.PresenceFilter.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.PresenceFilter.super_.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.SubstringFilter.prototype
1.  object <span class="apidocSignatureSpan">activedirectory.</span>filters.SubstringFilter.super_.prototype

#### [module activedirectory.filters](#apidoc.module.activedirectory.filters)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>AndFilter (options)](#apidoc.element.activedirectory.filters.AndFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>ApproximateFilter (options)](#apidoc.element.activedirectory.filters.ApproximateFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>EqualityFilter (options)](#apidoc.element.activedirectory.filters.EqualityFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>ExtensibleFilter (options)](#apidoc.element.activedirectory.filters.ExtensibleFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>GreaterThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>LessThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>NotFilter (options)](#apidoc.element.activedirectory.filters.NotFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>OrFilter (options)](#apidoc.element.activedirectory.filters.OrFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>PresenceFilter (options)](#apidoc.element.activedirectory.filters.PresenceFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>SubstringFilter (options)](#apidoc.element.activedirectory.filters.SubstringFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>isFilter (filter)](#apidoc.element.activedirectory.filters.isFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>parse (ber)](#apidoc.element.activedirectory.filters.parse)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>parseString (str)](#apidoc.element.activedirectory.filters.parseString)

#### [module activedirectory.filters.AndFilter](#apidoc.module.activedirectory.filters.AndFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>AndFilter (options)](#apidoc.element.activedirectory.filters.AndFilter.AndFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.AndFilter.super_)

#### [module activedirectory.filters.AndFilter.prototype](#apidoc.module.activedirectory.filters.AndFilter.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.AndFilter.prototype._toBer)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.AndFilter.prototype.toBer)

#### [module activedirectory.filters.AndFilter.super_.prototype](#apidoc.module.activedirectory.filters.AndFilter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.super_.prototype.</span>addFilter (filter)](#apidoc.element.activedirectory.filters.AndFilter.super_.prototype.addFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.AndFilter.super_.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.AndFilter.super_.prototype.toString)

#### [module activedirectory.filters.ApproximateFilter](#apidoc.module.activedirectory.filters.ApproximateFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>ApproximateFilter (options)](#apidoc.element.activedirectory.filters.ApproximateFilter.ApproximateFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.ApproximateFilter.super_)

#### [module activedirectory.filters.ApproximateFilter.prototype](#apidoc.module.activedirectory.filters.ApproximateFilter.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.ApproximateFilter.prototype._toBer)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.ApproximateFilter.prototype.parse)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.ApproximateFilter.prototype.toBer)

#### [module activedirectory.filters.ApproximateFilter.super_.prototype](#apidoc.module.activedirectory.filters.ApproximateFilter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.super_.prototype.</span>matches ()](#apidoc.element.activedirectory.filters.ApproximateFilter.super_.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.ApproximateFilter.super_.prototype.toString)

#### [module activedirectory.filters.EqualityFilter](#apidoc.module.activedirectory.filters.EqualityFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>EqualityFilter (options)](#apidoc.element.activedirectory.filters.EqualityFilter.EqualityFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.EqualityFilter.super_)

#### [module activedirectory.filters.EqualityFilter.prototype](#apidoc.module.activedirectory.filters.EqualityFilter.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.EqualityFilter.prototype._toBer)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.EqualityFilter.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.EqualityFilter.prototype.parse)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.EqualityFilter.prototype.toBer)

#### [module activedirectory.filters.EqualityFilter.super_.prototype](#apidoc.module.activedirectory.filters.EqualityFilter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.EqualityFilter.super_.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.EqualityFilter.super_.prototype.toString)

#### [module activedirectory.filters.ExtensibleFilter](#apidoc.module.activedirectory.filters.ExtensibleFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>ExtensibleFilter (options)](#apidoc.element.activedirectory.filters.ExtensibleFilter.ExtensibleFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.ExtensibleFilter.super_)

#### [module activedirectory.filters.ExtensibleFilter.prototype](#apidoc.module.activedirectory.filters.ExtensibleFilter.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.ExtensibleFilter.prototype._toBer)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.ExtensibleFilter.prototype.parse)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.ExtensibleFilter.prototype.toBer)

#### [module activedirectory.filters.ExtensibleFilter.super_.prototype](#apidoc.module.activedirectory.filters.ExtensibleFilter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.super_.prototype.</span>matches ()](#apidoc.element.activedirectory.filters.ExtensibleFilter.super_.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.ExtensibleFilter.super_.prototype.toString)

#### [module activedirectory.filters.GreaterThanEqualsFilter](#apidoc.module.activedirectory.filters.GreaterThanEqualsFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>GreaterThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.GreaterThanEqualsFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.super_)

#### [module activedirectory.filters.GreaterThanEqualsFilter.prototype](#apidoc.module.activedirectory.filters.GreaterThanEqualsFilter.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.prototype._toBer)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.prototype.parse)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.prototype.toBer)

#### [module activedirectory.filters.GreaterThanEqualsFilter.super_.prototype](#apidoc.module.activedirectory.filters.GreaterThanEqualsFilter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.super_.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.super_.prototype.toString)

#### [module activedirectory.filters.LessThanEqualsFilter](#apidoc.module.activedirectory.filters.LessThanEqualsFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>LessThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.LessThanEqualsFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.super_)

#### [module activedirectory.filters.LessThanEqualsFilter.prototype](#apidoc.module.activedirectory.filters.LessThanEqualsFilter.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.prototype._toBer)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.prototype.parse)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.prototype.toBer)

#### [module activedirectory.filters.LessThanEqualsFilter.super_.prototype](#apidoc.module.activedirectory.filters.LessThanEqualsFilter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.super_.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.super_.prototype.toString)

#### [module activedirectory.filters.NotFilter](#apidoc.module.activedirectory.filters.NotFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>NotFilter (options)](#apidoc.element.activedirectory.filters.NotFilter.NotFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.NotFilter.super_)

#### [module activedirectory.filters.NotFilter.prototype](#apidoc.module.activedirectory.filters.NotFilter.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.NotFilter.prototype._toBer)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.NotFilter.prototype.toBer)

#### [module activedirectory.filters.NotFilter.super_.prototype](#apidoc.module.activedirectory.filters.NotFilter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.super_.prototype.</span>addFilter (filter)](#apidoc.element.activedirectory.filters.NotFilter.super_.prototype.addFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.NotFilter.super_.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.NotFilter.super_.prototype.toString)

#### [module activedirectory.filters.OrFilter](#apidoc.module.activedirectory.filters.OrFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>OrFilter (options)](#apidoc.element.activedirectory.filters.OrFilter.OrFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.OrFilter.super_)

#### [module activedirectory.filters.OrFilter.prototype](#apidoc.module.activedirectory.filters.OrFilter.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.OrFilter.prototype._toBer)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.OrFilter.prototype.toBer)

#### [module activedirectory.filters.OrFilter.super_.prototype](#apidoc.module.activedirectory.filters.OrFilter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.super_.prototype.</span>addFilter (filter)](#apidoc.element.activedirectory.filters.OrFilter.super_.prototype.addFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.OrFilter.super_.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.OrFilter.super_.prototype.toString)

#### [module activedirectory.filters.PresenceFilter](#apidoc.module.activedirectory.filters.PresenceFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>PresenceFilter (options)](#apidoc.element.activedirectory.filters.PresenceFilter.PresenceFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.PresenceFilter.super_)

#### [module activedirectory.filters.PresenceFilter.prototype](#apidoc.module.activedirectory.filters.PresenceFilter.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.PresenceFilter.prototype._toBer)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.PresenceFilter.prototype.parse)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.PresenceFilter.prototype.toBer)

#### [module activedirectory.filters.PresenceFilter.super_.prototype](#apidoc.module.activedirectory.filters.PresenceFilter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.PresenceFilter.super_.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.PresenceFilter.super_.prototype.toString)

#### [module activedirectory.filters.SubstringFilter](#apidoc.module.activedirectory.filters.SubstringFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.</span>SubstringFilter (options)](#apidoc.element.activedirectory.filters.SubstringFilter.SubstringFilter)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.SubstringFilter.super_)

#### [module activedirectory.filters.SubstringFilter.prototype](#apidoc.module.activedirectory.filters.SubstringFilter.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.SubstringFilter.prototype._toBer)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.SubstringFilter.prototype.parse)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.SubstringFilter.prototype.toBer)

#### [module activedirectory.filters.SubstringFilter.super_.prototype](#apidoc.module.activedirectory.filters.SubstringFilter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.SubstringFilter.super_.prototype.matches)
1.  [function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.SubstringFilter.super_.prototype.toString)



# <a name="apidoc.module.activedirectory"></a>[module activedirectory](#apidoc.module.activedirectory)

#### <a name="apidoc.element.activedirectory.filters.AndFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>filters.AndFilter (options)](#apidoc.element.activedirectory.filters.AndFilter)
- description and source-code
```javascript
function AndFilter(options) {
  parents.AndFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ApproximateFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>filters.ApproximateFilter (options)](#apidoc.element.activedirectory.filters.ApproximateFilter)
- description and source-code
```javascript
function ApproximateFilter(options) {
  parents.ApproximateFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.EqualityFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>filters.EqualityFilter (options)](#apidoc.element.activedirectory.filters.EqualityFilter)
- description and source-code
```javascript
function EqualityFilter(options) {
  parents.EqualityFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ExtensibleFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>filters.ExtensibleFilter (options)](#apidoc.element.activedirectory.filters.ExtensibleFilter)
- description and source-code
```javascript
function ExtensibleFilter(options) {
  parents.ExtensibleFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.GreaterThanEqualsFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>filters.GreaterThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter)
- description and source-code
```javascript
function GreaterThanEqualsFilter(options) {
  parents.GreaterThanEqualsFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.LessThanEqualsFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>filters.LessThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter)
- description and source-code
```javascript
function LessThanEqualsFilter(options) {
  parents.LessThanEqualsFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.NotFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>filters.NotFilter (options)](#apidoc.element.activedirectory.filters.NotFilter)
- description and source-code
```javascript
function NotFilter(options) {
  parents.NotFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.OrFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>filters.OrFilter (options)](#apidoc.element.activedirectory.filters.OrFilter)
- description and source-code
```javascript
function OrFilter(options) {
  parents.OrFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.PresenceFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>filters.PresenceFilter (options)](#apidoc.element.activedirectory.filters.PresenceFilter)
- description and source-code
```javascript
function PresenceFilter(options) {
  parents.PresenceFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.SubstringFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>filters.SubstringFilter (options)](#apidoc.element.activedirectory.filters.SubstringFilter)
- description and source-code
```javascript
function SubstringFilter(options) {
  parents.SubstringFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.</span>super_ ()](#apidoc.element.activedirectory.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters"></a>[module activedirectory.filters](#apidoc.module.activedirectory.filters)

#### <a name="apidoc.element.activedirectory.filters.AndFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>AndFilter (options)](#apidoc.element.activedirectory.filters.AndFilter)
- description and source-code
```javascript
function AndFilter(options) {
  parents.AndFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ApproximateFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>ApproximateFilter (options)](#apidoc.element.activedirectory.filters.ApproximateFilter)
- description and source-code
```javascript
function ApproximateFilter(options) {
  parents.ApproximateFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.EqualityFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>EqualityFilter (options)](#apidoc.element.activedirectory.filters.EqualityFilter)
- description and source-code
```javascript
function EqualityFilter(options) {
  parents.EqualityFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ExtensibleFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>ExtensibleFilter (options)](#apidoc.element.activedirectory.filters.ExtensibleFilter)
- description and source-code
```javascript
function ExtensibleFilter(options) {
  parents.ExtensibleFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.GreaterThanEqualsFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>GreaterThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter)
- description and source-code
```javascript
function GreaterThanEqualsFilter(options) {
  parents.GreaterThanEqualsFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.LessThanEqualsFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>LessThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter)
- description and source-code
```javascript
function LessThanEqualsFilter(options) {
  parents.LessThanEqualsFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.NotFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>NotFilter (options)](#apidoc.element.activedirectory.filters.NotFilter)
- description and source-code
```javascript
function NotFilter(options) {
  parents.NotFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.OrFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>OrFilter (options)](#apidoc.element.activedirectory.filters.OrFilter)
- description and source-code
```javascript
function OrFilter(options) {
  parents.OrFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.PresenceFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>PresenceFilter (options)](#apidoc.element.activedirectory.filters.PresenceFilter)
- description and source-code
```javascript
function PresenceFilter(options) {
  parents.PresenceFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.SubstringFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>SubstringFilter (options)](#apidoc.element.activedirectory.filters.SubstringFilter)
- description and source-code
```javascript
function SubstringFilter(options) {
  parents.SubstringFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.isFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>isFilter (filter)](#apidoc.element.activedirectory.filters.isFilter)
- description and source-code
```javascript
function isFilter(filter) {
  if (!filter || typeof (filter) !== 'object') {
    return false;
  }
  // Do our best to duck-type it
  if (typeof (filter.toBer) === 'function' &&
      typeof (filter.matches) === 'function' &&
      TYPES[filter.type] !== undefined) {
    return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.parse"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>parse (ber)](#apidoc.element.activedirectory.filters.parse)
- description and source-code
```javascript
parse = function (ber) {
  if (!ber || !(ber instanceof BerReader))
    throw new TypeError('ber (BerReader) required');

  return _parse(ber);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.parseString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>parseString (str)](#apidoc.element.activedirectory.filters.parseString)
- description and source-code
```javascript
function parseString(str) {
  var generic = parents.parse(str);
  // The filter object(s) return from ldap-filter.parse lack the toBer/parse
  // decoration that native ldapjs filter possess.  cloneFilter adds that back.
  return cloneFilter(generic);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.AndFilter"></a>[module activedirectory.filters.AndFilter](#apidoc.module.activedirectory.filters.AndFilter)

#### <a name="apidoc.element.activedirectory.filters.AndFilter.AndFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>AndFilter (options)](#apidoc.element.activedirectory.filters.AndFilter.AndFilter)
- description and source-code
```javascript
function AndFilter(options) {
  parents.AndFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.AndFilter.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.AndFilter.super_)
- description and source-code
```javascript
function AndFilter(options) {
  if (typeof (options) === 'object') {
    assert.arrayOfObject(options.filters, 'options.filters');
  } else {
    options = {};
  }

  this.__defineGetter__('type', function () { return 'and'; });
  this.filters = options.filters ? options.filters.slice() : [];

  var self = this;
  this.__defineGetter__('json', function () {
    return {
      type: 'And',
      filters: self.filters
    };
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.AndFilter.prototype"></a>[module activedirectory.filters.AndFilter.prototype](#apidoc.module.activedirectory.filters.AndFilter.prototype)

#### <a name="apidoc.element.activedirectory.filters.AndFilter.prototype._toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.AndFilter.prototype._toBer)
- description and source-code
```javascript
_toBer = function (ber) {
  assert.ok(ber);

  this.filters.forEach(function (f) {
    ber = f.toBer(ber);
  });

  return ber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.AndFilter.prototype.toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.AndFilter.prototype.toBer)
- description and source-code
```javascript
function toBer(ber) {
  if (!ber || !(ber instanceof BerWriter))
    throw new TypeError('ber (BerWriter) required');

  ber.startSequence(TYPES[this.type]);
  ber = this._toBer(ber);
  ber.endSequence();
  return ber;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.AndFilter.super_.prototype"></a>[module activedirectory.filters.AndFilter.super_.prototype](#apidoc.module.activedirectory.filters.AndFilter.super_.prototype)

#### <a name="apidoc.element.activedirectory.filters.AndFilter.super_.prototype.addFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.super_.prototype.</span>addFilter (filter)](#apidoc.element.activedirectory.filters.AndFilter.super_.prototype.addFilter)
- description and source-code
```javascript
addFilter = function (filter) {
  assert.object(filter, 'filter');

  this.filters.push(filter);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.AndFilter.super_.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.AndFilter.super_.prototype.matches)
- description and source-code
```javascript
matches = function (target, strictAttrCase) {
  assert.object(target, 'target');

  if (this.filters.length === 0) {
<span class="apidocCodeCommentSpan">    /* true per RFC4526 */
</span>    return true;
  }

  for (var i = 0; i < this.filters.length; i++) {
    if (!this.filters[i].matches(target, strictAttrCase))
      return false;
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.AndFilter.super_.prototype.toString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.AndFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.AndFilter.super_.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var str = '(&';
  this.filters.forEach(function (f) {
    str += f.toString();
  });
  str += ')';

  return str;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.ApproximateFilter"></a>[module activedirectory.filters.ApproximateFilter](#apidoc.module.activedirectory.filters.ApproximateFilter)

#### <a name="apidoc.element.activedirectory.filters.ApproximateFilter.ApproximateFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>ApproximateFilter (options)](#apidoc.element.activedirectory.filters.ApproximateFilter.ApproximateFilter)
- description and source-code
```javascript
function ApproximateFilter(options) {
  parents.ApproximateFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ApproximateFilter.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.ApproximateFilter.super_)
- description and source-code
```javascript
function ApproximateFilter(options) {
  if (typeof (options) === 'object') {
    assert.string(options.attribute, 'options.attribute');
    assert.string(options.value, 'options.value');
    this.attribute = options.attribute;
    this.value = options.value;
  }

  var self = this;
  this.__defineGetter__('type', function () { return 'approx'; });
  this.__defineGetter__('json', function () {
    return {
      type: 'ApproximateMatch',
      attribute: self.attribute,
      value: self.value
    };
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.ApproximateFilter.prototype"></a>[module activedirectory.filters.ApproximateFilter.prototype](#apidoc.module.activedirectory.filters.ApproximateFilter.prototype)

#### <a name="apidoc.element.activedirectory.filters.ApproximateFilter.prototype._toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.ApproximateFilter.prototype._toBer)
- description and source-code
```javascript
_toBer = function (ber) {
  assert.ok(ber);

  ber.writeString(this.attribute);
  ber.writeString(this.value);

  return ber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ApproximateFilter.prototype.parse"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.ApproximateFilter.prototype.parse)
- description and source-code
```javascript
parse = function (ber) {
  assert.ok(ber);

  this.attribute = ber.readString().toLowerCase();
  this.value = ber.readString();

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ApproximateFilter.prototype.toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.ApproximateFilter.prototype.toBer)
- description and source-code
```javascript
function toBer(ber) {
  if (!ber || !(ber instanceof BerWriter))
    throw new TypeError('ber (BerWriter) required');

  ber.startSequence(TYPES[this.type]);
  ber = this._toBer(ber);
  ber.endSequence();
  return ber;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.ApproximateFilter.super_.prototype"></a>[module activedirectory.filters.ApproximateFilter.super_.prototype](#apidoc.module.activedirectory.filters.ApproximateFilter.super_.prototype)

#### <a name="apidoc.element.activedirectory.filters.ApproximateFilter.super_.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.super_.prototype.</span>matches ()](#apidoc.element.activedirectory.filters.ApproximateFilter.super_.prototype.matches)
- description and source-code
```javascript
matches = function () {
  // Consumers must implement this themselves
  throw new Error('approx match implementation missing');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ApproximateFilter.super_.prototype.toString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ApproximateFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.ApproximateFilter.super_.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return ('(' + helpers.escape(this.attribute) +
          '~=' + helpers.escape(this.value) + ')');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.EqualityFilter"></a>[module activedirectory.filters.EqualityFilter](#apidoc.module.activedirectory.filters.EqualityFilter)

#### <a name="apidoc.element.activedirectory.filters.EqualityFilter.EqualityFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>EqualityFilter (options)](#apidoc.element.activedirectory.filters.EqualityFilter.EqualityFilter)
- description and source-code
```javascript
function EqualityFilter(options) {
  parents.EqualityFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.EqualityFilter.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.EqualityFilter.super_)
- description and source-code
```javascript
function EqualityFilter(options) {
  if (typeof (options) === 'object') {
    assert.string(options.attribute, 'options.attribute');
    this.attribute = options.attribute;
    // Prefer Buffers over strings to make filter cloning easier
    if (options.raw) {
      this.raw = options.raw;
    } else {
      this.raw = new Buffer(options.value);
    }
  } else {
    this.raw = new Buffer(0);
  }

  var self = this;
  this.__defineGetter__('type', function () { return 'equal'; });
  this.__defineGetter__('value', function () {
    return (Buffer.isBuffer(self.raw)) ? self.raw.toString() : self.raw;
  });
  this.__defineSetter__('value', function (data) {
    if (typeof (data) === 'string') {
      self.raw = new Buffer(data);
    } else if (Buffer.isBuffer(data)) {
      self.raw = new Buffer(data.length);
      data.copy(self.raw);
    } else {
      self.raw = data;
    }
  });
  this.__defineGetter__('json', function () {
    return {
      type: 'EqualityMatch',
      attribute: self.attribute,
      value: self.value
    };
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.EqualityFilter.prototype"></a>[module activedirectory.filters.EqualityFilter.prototype](#apidoc.module.activedirectory.filters.EqualityFilter.prototype)

#### <a name="apidoc.element.activedirectory.filters.EqualityFilter.prototype._toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.EqualityFilter.prototype._toBer)
- description and source-code
```javascript
_toBer = function (ber) {
  assert.ok(ber);

  ber.writeString(this.attribute);
  ber.writeBuffer(this.raw, ASN1.OctetString);

  return ber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.EqualityFilter.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.EqualityFilter.prototype.matches)
- description and source-code
```javascript
matches = function (target, strictAttrCase) {
  assert.object(target, 'target');

  var tv = parents.getAttrValue(target, this.attribute, strictAttrCase);
  var value = this.value;

  if (this.attribute.toLowerCase() === 'objectclass') {
<span class="apidocCodeCommentSpan">    /*
     * Perform case-insensitive match for objectClass since nearly every LDAP
     * implementation behaves in this manner.
     */
</span>    value = value.toLowerCase();
    return parents.testValues(function (v) {
      return value === v.toLowerCase();
    }, tv);
  } else {
    return parents.testValues(function (v) {
      return value === v;
    }, tv);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.EqualityFilter.prototype.parse"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.EqualityFilter.prototype.parse)
- description and source-code
```javascript
parse = function (ber) {
  assert.ok(ber);

  this.attribute = ber.readString().toLowerCase();
  this.value = ber.readString(ASN1.OctetString, true);

  if (this.attribute === 'objectclass')
    this.value = this.value.toLowerCase();

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.EqualityFilter.prototype.toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.EqualityFilter.prototype.toBer)
- description and source-code
```javascript
function toBer(ber) {
  if (!ber || !(ber instanceof BerWriter))
    throw new TypeError('ber (BerWriter) required');

  ber.startSequence(TYPES[this.type]);
  ber = this._toBer(ber);
  ber.endSequence();
  return ber;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.EqualityFilter.super_.prototype"></a>[module activedirectory.filters.EqualityFilter.super_.prototype](#apidoc.module.activedirectory.filters.EqualityFilter.super_.prototype)

#### <a name="apidoc.element.activedirectory.filters.EqualityFilter.super_.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.EqualityFilter.super_.prototype.matches)
- description and source-code
```javascript
matches = function (target, strictAttrCase) {
  assert.object(target, 'target');

  var tv = helpers.getAttrValue(target, this.attribute, strictAttrCase);
  var value = this.value;

  return helpers.testValues(function (v) {
    return value === v;
  }, tv);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.EqualityFilter.super_.prototype.toString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.EqualityFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.EqualityFilter.super_.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return ('(' + helpers.escape(this.attribute) +
          '=' + helpers.escape(this.value) + ')');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.ExtensibleFilter"></a>[module activedirectory.filters.ExtensibleFilter](#apidoc.module.activedirectory.filters.ExtensibleFilter)

#### <a name="apidoc.element.activedirectory.filters.ExtensibleFilter.ExtensibleFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>ExtensibleFilter (options)](#apidoc.element.activedirectory.filters.ExtensibleFilter.ExtensibleFilter)
- description and source-code
```javascript
function ExtensibleFilter(options) {
  parents.ExtensibleFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ExtensibleFilter.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.ExtensibleFilter.super_)
- description and source-code
```javascript
function ExtensibleFilter(options) {
  if (typeof (options) === 'object') {
    assert.optionalString(options.rule, 'options.rule');
    assert.optionalString(options.matchType, 'options.matchType');
    assert.optionalString(options.attribute, 'options.attribute');
    assert.optionalString(options.value, 'options.value');
  } else {
    options = {};
  }

  if (options.matchType !== undefined) {
    this.matchType = options.matchType;
  } else {
    this.matchType = options.attribute;
  }
  this.dnAttributes = options.dnAttributes || false;
  this.rule = options.rule;
  this.value = (options.value !== undefined) ? options.value : '';

  var self = this;
  this.__defineGetter__('type', function () { return 'ext'; });
  this.__defineGetter__('json', function () {
    return {
      type: 'ExtensibleMatch',
      matchRule: self.rule,
      matchType: self.matchType,
      matchValue: self.value,
      dnAttributes: self.dnAttributes
    };
  });
  this.__defineGetter__('matchingRule', function () {
    return self.rule;
  });
  this.__defineGetter__('matchValue', function () {
    return self.value;
  });
  this.__defineGetter__('attribute', function () {
    return this.matchType;
  });
  this.__defineSetter__('attribute', function (value) {
    this.matchType = value;
  });

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.ExtensibleFilter.prototype"></a>[module activedirectory.filters.ExtensibleFilter.prototype](#apidoc.module.activedirectory.filters.ExtensibleFilter.prototype)

#### <a name="apidoc.element.activedirectory.filters.ExtensibleFilter.prototype._toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.ExtensibleFilter.prototype._toBer)
- description and source-code
```javascript
_toBer = function (ber) {
  assert.ok(ber);

  if (this.rule)
    ber.writeString(this.rule, 0x81);
  if (this.matchType)
    ber.writeString(this.matchType, 0x82);

  ber.writeString(this.value, 0x83);
  if (this.dnAttributes)
    ber.writeBoolean(this.dnAttributes, 0x84);

  return ber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ExtensibleFilter.prototype.parse"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.ExtensibleFilter.prototype.parse)
- description and source-code
```javascript
parse = function (ber) {
  var end = ber.offset + ber.length;
  while (ber.offset < end) {
    var tag = ber.peek();
    switch (tag) {
    case 0x81:
      this.rule = ber.readString(tag);
      break;
    case 0x82:
      this.matchType = ber.readString(tag);
      break;
    case 0x83:
      this.value = ber.readString(tag);
      break;
    case 0x84:
      this.dnAttributes = ber.readBoolean(tag);
      break;
    default:
      throw new Error('Invalid ext_match filter type: 0x' + tag.toString(16));
    }
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ExtensibleFilter.prototype.toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.ExtensibleFilter.prototype.toBer)
- description and source-code
```javascript
function toBer(ber) {
  if (!ber || !(ber instanceof BerWriter))
    throw new TypeError('ber (BerWriter) required');

  ber.startSequence(TYPES[this.type]);
  ber = this._toBer(ber);
  ber.endSequence();
  return ber;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.ExtensibleFilter.super_.prototype"></a>[module activedirectory.filters.ExtensibleFilter.super_.prototype](#apidoc.module.activedirectory.filters.ExtensibleFilter.super_.prototype)

#### <a name="apidoc.element.activedirectory.filters.ExtensibleFilter.super_.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.super_.prototype.</span>matches ()](#apidoc.element.activedirectory.filters.ExtensibleFilter.super_.prototype.matches)
- description and source-code
```javascript
matches = function () {
  // Consumers must implement this themselves
  throw new Error('ext match implementation missing');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.ExtensibleFilter.super_.prototype.toString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.ExtensibleFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.ExtensibleFilter.super_.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var str = '(';

  if (this.matchType)
    str += this.matchType;

  str += ':';

  if (this.dnAttributes)
    str += 'dn:';

  if (this.rule)
    str += this.rule + ':';

  return (str + '=' + this.value + ')');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.GreaterThanEqualsFilter"></a>[module activedirectory.filters.GreaterThanEqualsFilter](#apidoc.module.activedirectory.filters.GreaterThanEqualsFilter)

#### <a name="apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.GreaterThanEqualsFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>GreaterThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.GreaterThanEqualsFilter)
- description and source-code
```javascript
function GreaterThanEqualsFilter(options) {
  parents.GreaterThanEqualsFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.super_)
- description and source-code
```javascript
function GreaterThanEqualsFilter(options) {
  if (typeof (options) === 'object') {
    assert.string(options.attribute, 'options.attribute');
    assert.string(options.value, 'options.value');
    this.attribute = options.attribute;
    this.value = options.value;
  }

  var self = this;
  this.__defineGetter__('type', function () { return 'ge'; });
  this.__defineGetter__('json', function () {
    return {
      type: 'GreaterThanEqualsMatch',
      attribute: self.attribute,
      value: self.value
    };
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.GreaterThanEqualsFilter.prototype"></a>[module activedirectory.filters.GreaterThanEqualsFilter.prototype](#apidoc.module.activedirectory.filters.GreaterThanEqualsFilter.prototype)

#### <a name="apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.prototype._toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.prototype._toBer)
- description and source-code
```javascript
_toBer = function (ber) {
  assert.ok(ber);

  ber.writeString(this.attribute);
  ber.writeString(this.value);

  return ber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.prototype.parse"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.prototype.parse)
- description and source-code
```javascript
parse = function (ber) {
  assert.ok(ber);

  this.attribute = ber.readString().toLowerCase();
  this.value = ber.readString();

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.prototype.toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.prototype.toBer)
- description and source-code
```javascript
function toBer(ber) {
  if (!ber || !(ber instanceof BerWriter))
    throw new TypeError('ber (BerWriter) required');

  ber.startSequence(TYPES[this.type]);
  ber = this._toBer(ber);
  ber.endSequence();
  return ber;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.GreaterThanEqualsFilter.super_.prototype"></a>[module activedirectory.filters.GreaterThanEqualsFilter.super_.prototype](#apidoc.module.activedirectory.filters.GreaterThanEqualsFilter.super_.prototype)

#### <a name="apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.super_.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.super_.prototype.matches)
- description and source-code
```javascript
matches = function (target, strictAttrCase) {
  assert.object(target, 'target');

  var tv = helpers.getAttrValue(target, this.attribute, strictAttrCase);
  var value = this.value;

  return helpers.testValues(function (v) {
    return value <= v;
  }, tv);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.super_.prototype.toString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.GreaterThanEqualsFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.GreaterThanEqualsFilter.super_.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return ('(' + helpers.escape(this.attribute) +
          '>=' + helpers.escape(this.value) + ')');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.LessThanEqualsFilter"></a>[module activedirectory.filters.LessThanEqualsFilter](#apidoc.module.activedirectory.filters.LessThanEqualsFilter)

#### <a name="apidoc.element.activedirectory.filters.LessThanEqualsFilter.LessThanEqualsFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>LessThanEqualsFilter (options)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.LessThanEqualsFilter)
- description and source-code
```javascript
function LessThanEqualsFilter(options) {
  parents.LessThanEqualsFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.LessThanEqualsFilter.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.super_)
- description and source-code
```javascript
function LessThanEqualsFilter(options) {
  if (typeof (options) === 'object') {
    assert.string(options.attribute, 'options.attribute');
    assert.string(options.value, 'options.attribute');
    this.attribute = options.attribute;
    this.value = options.value;
  }

  var self = this;
  this.__defineGetter__('type', function () { return 'le'; });
  this.__defineGetter__('json', function () {
    return {
      type: 'LessThanEqualsMatch',
      attribute: self.attribute,
      value: self.value
    };
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.LessThanEqualsFilter.prototype"></a>[module activedirectory.filters.LessThanEqualsFilter.prototype](#apidoc.module.activedirectory.filters.LessThanEqualsFilter.prototype)

#### <a name="apidoc.element.activedirectory.filters.LessThanEqualsFilter.prototype._toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.prototype._toBer)
- description and source-code
```javascript
_toBer = function (ber) {
  assert.ok(ber);

  ber.writeString(this.attribute);
  ber.writeString(this.value);

  return ber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.LessThanEqualsFilter.prototype.parse"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.prototype.parse)
- description and source-code
```javascript
parse = function (ber) {
  assert.ok(ber);

  this.attribute = ber.readString().toLowerCase();
  this.value = ber.readString();

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.LessThanEqualsFilter.prototype.toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.prototype.toBer)
- description and source-code
```javascript
function toBer(ber) {
  if (!ber || !(ber instanceof BerWriter))
    throw new TypeError('ber (BerWriter) required');

  ber.startSequence(TYPES[this.type]);
  ber = this._toBer(ber);
  ber.endSequence();
  return ber;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.LessThanEqualsFilter.super_.prototype"></a>[module activedirectory.filters.LessThanEqualsFilter.super_.prototype](#apidoc.module.activedirectory.filters.LessThanEqualsFilter.super_.prototype)

#### <a name="apidoc.element.activedirectory.filters.LessThanEqualsFilter.super_.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.super_.prototype.matches)
- description and source-code
```javascript
matches = function (target, strictAttrCase) {
  assert.object(target, 'target');

  var tv = helpers.getAttrValue(target, this.attribute, strictAttrCase);
  var value = this.value;

  return helpers.testValues(function (v) {
    return value >= v;
  }, tv);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.LessThanEqualsFilter.super_.prototype.toString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.LessThanEqualsFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.LessThanEqualsFilter.super_.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return ('(' + helpers.escape(this.attribute) +
          '<=' + helpers.escape(this.value) + ')');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.NotFilter"></a>[module activedirectory.filters.NotFilter](#apidoc.module.activedirectory.filters.NotFilter)

#### <a name="apidoc.element.activedirectory.filters.NotFilter.NotFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>NotFilter (options)](#apidoc.element.activedirectory.filters.NotFilter.NotFilter)
- description and source-code
```javascript
function NotFilter(options) {
  parents.NotFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.NotFilter.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.NotFilter.super_)
- description and source-code
```javascript
function NotFilter(options) {
  if (typeof (options) === 'object') {
    assert.object(options.filter, 'options.filter');
  } else {
    options = {};
  }

  this.filter = options.filter || {};

  var self = this;
  this.__defineGetter__('type', function () { return 'not'; });
  this.__defineGetter__('json', function () {
    return {
      type: 'Not',
      filter: self.filter
    };
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.NotFilter.prototype"></a>[module activedirectory.filters.NotFilter.prototype](#apidoc.module.activedirectory.filters.NotFilter.prototype)

#### <a name="apidoc.element.activedirectory.filters.NotFilter.prototype._toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.NotFilter.prototype._toBer)
- description and source-code
```javascript
_toBer = function (ber) {
  assert.ok(ber);

  return this.filter.toBer(ber);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.NotFilter.prototype.toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.NotFilter.prototype.toBer)
- description and source-code
```javascript
function toBer(ber) {
  if (!ber || !(ber instanceof BerWriter))
    throw new TypeError('ber (BerWriter) required');

  ber.startSequence(TYPES[this.type]);
  ber = this._toBer(ber);
  ber.endSequence();
  return ber;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.NotFilter.super_.prototype"></a>[module activedirectory.filters.NotFilter.super_.prototype](#apidoc.module.activedirectory.filters.NotFilter.super_.prototype)

#### <a name="apidoc.element.activedirectory.filters.NotFilter.super_.prototype.addFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.super_.prototype.</span>addFilter (filter)](#apidoc.element.activedirectory.filters.NotFilter.super_.prototype.addFilter)
- description and source-code
```javascript
addFilter = function (filter) {
  assert.object(filter, 'filter');
  this.filter = filter;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.NotFilter.super_.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.NotFilter.super_.prototype.matches)
- description and source-code
```javascript
matches = function (target, strictAttrCase) {
  return !this.filter.matches(target, strictAttrCase);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.NotFilter.super_.prototype.toString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.NotFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.NotFilter.super_.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return '(!' + this.filter.toString() + ')';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.OrFilter"></a>[module activedirectory.filters.OrFilter](#apidoc.module.activedirectory.filters.OrFilter)

#### <a name="apidoc.element.activedirectory.filters.OrFilter.OrFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>OrFilter (options)](#apidoc.element.activedirectory.filters.OrFilter.OrFilter)
- description and source-code
```javascript
function OrFilter(options) {
  parents.OrFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.OrFilter.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.OrFilter.super_)
- description and source-code
```javascript
function OrFilter(options) {
  if (typeof (options) === 'object') {
    assert.arrayOfObject(options.filters, 'options.filters');
  } else {
    options = {};
  }

  this.filters = options.filters ? options.filters.slice() : [];

  var self = this;
  this.__defineGetter__('type', function () { return 'or'; });
  this.__defineGetter__('json', function () {
    return {
      type: 'Or',
      filters: self.filters
    };
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.OrFilter.prototype"></a>[module activedirectory.filters.OrFilter.prototype](#apidoc.module.activedirectory.filters.OrFilter.prototype)

#### <a name="apidoc.element.activedirectory.filters.OrFilter.prototype._toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.OrFilter.prototype._toBer)
- description and source-code
```javascript
_toBer = function (ber) {
  assert.ok(ber);

  this.filters.forEach(function (f) {
    ber = f.toBer(ber);
  });

  return ber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.OrFilter.prototype.toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.OrFilter.prototype.toBer)
- description and source-code
```javascript
function toBer(ber) {
  if (!ber || !(ber instanceof BerWriter))
    throw new TypeError('ber (BerWriter) required');

  ber.startSequence(TYPES[this.type]);
  ber = this._toBer(ber);
  ber.endSequence();
  return ber;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.OrFilter.super_.prototype"></a>[module activedirectory.filters.OrFilter.super_.prototype](#apidoc.module.activedirectory.filters.OrFilter.super_.prototype)

#### <a name="apidoc.element.activedirectory.filters.OrFilter.super_.prototype.addFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.super_.prototype.</span>addFilter (filter)](#apidoc.element.activedirectory.filters.OrFilter.super_.prototype.addFilter)
- description and source-code
```javascript
addFilter = function (filter) {
  assert.object(filter, 'filter');

  this.filters.push(filter);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.OrFilter.super_.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.OrFilter.super_.prototype.matches)
- description and source-code
```javascript
matches = function (target, strictAttrCase) {
  assert.object(target, 'target');

  for (var i = 0; i < this.filters.length; i++) {
    if (this.filters[i].matches(target, strictAttrCase))
      return true;
  }

  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.OrFilter.super_.prototype.toString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.OrFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.OrFilter.super_.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var str = '(|';
  this.filters.forEach(function (f) {
    str += f.toString();
  });
  str += ')';

  return str;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.PresenceFilter"></a>[module activedirectory.filters.PresenceFilter](#apidoc.module.activedirectory.filters.PresenceFilter)

#### <a name="apidoc.element.activedirectory.filters.PresenceFilter.PresenceFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>PresenceFilter (options)](#apidoc.element.activedirectory.filters.PresenceFilter.PresenceFilter)
- description and source-code
```javascript
function PresenceFilter(options) {
  parents.PresenceFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.PresenceFilter.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.PresenceFilter.super_)
- description and source-code
```javascript
function PresenceFilter(options) {
  if (typeof (options) === 'object') {
    assert.string(options.attribute, 'options.attribute');
    this.attribute = options.attribute;
  }


  var self = this;
  this.__defineGetter__('type', function () { return 'present'; });
  this.__defineGetter__('json', function () {
    return {
      type: 'PresenceMatch',
      attribute: self.attribute
    };
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.PresenceFilter.prototype"></a>[module activedirectory.filters.PresenceFilter.prototype](#apidoc.module.activedirectory.filters.PresenceFilter.prototype)

#### <a name="apidoc.element.activedirectory.filters.PresenceFilter.prototype._toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.PresenceFilter.prototype._toBer)
- description and source-code
```javascript
_toBer = function (ber) {
  assert.ok(ber);

  for (var i = 0; i < this.attribute.length; i++)
    ber.writeByte(this.attribute.charCodeAt(i));

  return ber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.PresenceFilter.prototype.parse"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.PresenceFilter.prototype.parse)
- description and source-code
```javascript
parse = function (ber) {
  assert.ok(ber);

  this.attribute =
    ber.buffer.slice(0, ber.length).toString('utf8').toLowerCase();

  ber._offset += ber.length;

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.PresenceFilter.prototype.toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.PresenceFilter.prototype.toBer)
- description and source-code
```javascript
function toBer(ber) {
  if (!ber || !(ber instanceof BerWriter))
    throw new TypeError('ber (BerWriter) required');

  ber.startSequence(TYPES[this.type]);
  ber = this._toBer(ber);
  ber.endSequence();
  return ber;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.PresenceFilter.super_.prototype"></a>[module activedirectory.filters.PresenceFilter.super_.prototype](#apidoc.module.activedirectory.filters.PresenceFilter.super_.prototype)

#### <a name="apidoc.element.activedirectory.filters.PresenceFilter.super_.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.PresenceFilter.super_.prototype.matches)
- description and source-code
```javascript
matches = function (target, strictAttrCase) {
  assert.object(target, 'target');

  var value = helpers.getAttrValue(target, this.attribute, strictAttrCase);

  return (value !== undefined && value !== null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.PresenceFilter.super_.prototype.toString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.PresenceFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.PresenceFilter.super_.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return '(' + helpers.escape(this.attribute) + '=*)';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.SubstringFilter"></a>[module activedirectory.filters.SubstringFilter](#apidoc.module.activedirectory.filters.SubstringFilter)

#### <a name="apidoc.element.activedirectory.filters.SubstringFilter.SubstringFilter"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.</span>SubstringFilter (options)](#apidoc.element.activedirectory.filters.SubstringFilter.SubstringFilter)
- description and source-code
```javascript
function SubstringFilter(options) {
  parents.SubstringFilter.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.SubstringFilter.super_"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.</span>super_ (options)](#apidoc.element.activedirectory.filters.SubstringFilter.super_)
- description and source-code
```javascript
function SubstringFilter(options) {
  if (typeof (options) === 'object') {
    assert.string(options.attribute, 'options.attribute');

    this.attribute = options.attribute;
    this.initial = options.initial;
    this.any = options.any ? options.any.slice(0) : [];
    this.final = options.final;
  } else {
    this.any = [];
  }

  var self = this;
  this.__defineGetter__('type', function () { return 'substring'; });
  this.__defineGetter__('json', function () {
    return {
      type: 'SubstringMatch',
      initial: self.initial,
      any: self.any,
      final: self.final
    };
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.SubstringFilter.prototype"></a>[module activedirectory.filters.SubstringFilter.prototype](#apidoc.module.activedirectory.filters.SubstringFilter.prototype)

#### <a name="apidoc.element.activedirectory.filters.SubstringFilter.prototype._toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.prototype.</span>_toBer (ber)](#apidoc.element.activedirectory.filters.SubstringFilter.prototype._toBer)
- description and source-code
```javascript
_toBer = function (ber) {
  assert.ok(ber);

  ber.writeString(this.attribute);
  ber.startSequence();

  if (this.initial)
    ber.writeString(this.initial, 0x80);

  if (this.any && this.any.length)
    this.any.forEach(function (s) {
      ber.writeString(s, 0x81);
    });

  if (this.final)
    ber.writeString(this.final, 0x82);

  ber.endSequence();

  return ber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.SubstringFilter.prototype.parse"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.prototype.</span>parse (ber)](#apidoc.element.activedirectory.filters.SubstringFilter.prototype.parse)
- description and source-code
```javascript
parse = function (ber) {
  assert.ok(ber);

  this.attribute = ber.readString().toLowerCase();
  ber.readSequence();
  var end = ber.offset + ber.length;

  while (ber.offset < end) {
    var tag = ber.peek();
    switch (tag) {
    case 0x80: // Initial
      this.initial = ber.readString(tag);
      if (this.attribute === 'objectclass')
        this.initial = this.initial.toLowerCase();
      break;
    case 0x81: // Any
      var anyVal = ber.readString(tag);
      if (this.attribute === 'objectclass')
        anyVal = anyVal.toLowerCase();
      this.any.push(anyVal);
      break;
    case 0x82: // Final
      this.final = ber.readString(tag);
      if (this.attribute === 'objectclass')
        this.final = this.final.toLowerCase();
      break;
    default:
      throw new Error('Invalid substrings filter type: 0x' + tag.toString(16));
    }
  }

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.SubstringFilter.prototype.toBer"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.prototype.</span>toBer (ber)](#apidoc.element.activedirectory.filters.SubstringFilter.prototype.toBer)
- description and source-code
```javascript
function toBer(ber) {
  if (!ber || !(ber instanceof BerWriter))
    throw new TypeError('ber (BerWriter) required');

  ber.startSequence(TYPES[this.type]);
  ber = this._toBer(ber);
  ber.endSequence();
  return ber;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.activedirectory.filters.SubstringFilter.super_.prototype"></a>[module activedirectory.filters.SubstringFilter.super_.prototype](#apidoc.module.activedirectory.filters.SubstringFilter.super_.prototype)

#### <a name="apidoc.element.activedirectory.filters.SubstringFilter.super_.prototype.matches"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.super_.prototype.</span>matches (target, strictAttrCase)](#apidoc.element.activedirectory.filters.SubstringFilter.super_.prototype.matches)
- description and source-code
```javascript
matches = function (target, strictAttrCase) {
  assert.object(target, 'target');

  var tv = helpers.getAttrValue(target, this.attribute, strictAttrCase);

  if (tv !== undefined && tv !== null) {
    var re = '';

    if (this.initial)
      re += '^' + escapeRegExp(this.initial) + '.*';
    this.any.forEach(function (s) {
      re += escapeRegExp(s) + '.*';
    });
    if (this.final)
      re += escapeRegExp(this.final) + '$';

    var matcher = new RegExp(re);
    return helpers.testValues(function (v) {
      return matcher.test(v);
    }, tv);
  }

  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.activedirectory.filters.SubstringFilter.super_.prototype.toString"></a>[function <span class="apidocSignatureSpan">activedirectory.filters.SubstringFilter.super_.prototype.</span>toString ()](#apidoc.element.activedirectory.filters.SubstringFilter.super_.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var str = '(' + helpers.escape(this.attribute) + '=';

  if (this.initial)
    str += helpers.escape(this.initial);

  str += '*';

  this.any.forEach(function (s) {
    str += helpers.escape(s) + '*';
  });

  if (this.final)
    str += helpers.escape(this.final);

  str += ')';

  return str;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
