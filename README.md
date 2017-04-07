# api documentation for  [nools (v0.4.4)](http://c2fo.github.com/nools)  [![npm package](https://img.shields.io/npm/v/npmdoc-nools.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nools) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nools.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nools)
#### A rules engine for node

[![NPM](https://nodei.co/npm/nools.png?downloads=true)](https://www.npmjs.com/package/nools)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nools/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-nools_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nools/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-nools/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-nools/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Doug Martin",
        "url": "http://c2fo.com"
    },
    "bin": {
        "nools": "./bin/nools"
    },
    "bugs": {
        "url": "https://github.com/C2FO/nools/issues"
    },
    "dependencies": {
        "arguments-extended": "~0.0.3",
        "array-extended": "~0.0.4",
        "commander": "~1.1.1",
        "date-extended": "~0.0.3",
        "declare.js": "~0.0.3",
        "extended": "~0.0.3",
        "function-extended": "~0.0.3",
        "ht": "~0.0.2",
        "is-extended": "~0.0.4",
        "leafy": "~0.0.3",
        "object-extended": "~0.0.3",
        "promise-extended": "~0.0.3",
        "string-extended": "~0.0.3",
        "uglify-js": "~2.4.24"
    },
    "description": "A rules engine for node",
    "devDependencies": {
        "coddoc": "0.0.3",
        "grunt": "~0.4.1",
        "grunt-browserify": "1.2.4",
        "grunt-contrib-jshint": "~0.5.3",
        "grunt-contrib-uglify": "~0.2.0",
        "grunt-exec": "^0.4.5",
        "grunt-it": "~0.3.0",
        "it": "~0.2.0",
        "jison": "~0.4.17"
    },
    "directories": {
        "lib": "lib"
    },
    "dist": {
        "shasum": "d9f70671ee2926bd24bb62a8c605cae209199a86",
        "tarball": "https://registry.npmjs.org/nools/-/nools-0.4.4.tgz"
    },
    "engines": {
        "node": ">= 0.6.1"
    },
    "gitHead": "019cdc7d71a80a9c9f1c2dbd63b78a2e311a380b",
    "homepage": "http://c2fo.github.com/nools",
    "keywords": [
        "rules",
        "flow",
        "rules engine",
        "rools",
        "drools",
        "async",
        "flow control"
    ],
    "main": "index.js",
    "maintainers": [
        {
            "name": "damartin",
            "email": "doug@dougamartin.com"
        },
        {
            "name": "devside",
            "email": "thomas.triau@gmail.com"
        }
    ],
    "name": "nools",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/C2FO/nools.git"
    },
    "scripts": {
        "create-doc": "rm -rf docs/* && coddoc -d ./lib -f multi-html",
        "test": "it -r spec"
    },
    "testling": {
        "files": "test/browserling.js",
        "browsers": [
            "ie/8..latest",
            "chrome/20..latest",
            "firefox/14..latest",
            "safari/latest",
            "iphone/6",
            "ipad/6"
        ]
    },
    "version": "0.4.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module nools](#apidoc.module.nools)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow ()](#apidoc.element.nools.Flow)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.as (obj, name)](#apidoc.element.nools.Flow.as)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.deleteFlow (name)](#apidoc.element.nools.Flow.deleteFlow)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.deleteFlows ()](#apidoc.element.nools.Flow.deleteFlows)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.extend (proto)](#apidoc.element.nools.Flow.extend)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.get (name)](#apidoc.element.nools.Flow.get)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.init ()](#apidoc.element.nools.Flow.init)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.mixin ()](#apidoc.element.nools.Flow.mixin)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.addDefined (name, cls)](#apidoc.element.nools.Flow.prototype.addDefined)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.conflictResolution (strategies)](#apidoc.element.nools.Flow.prototype.conflictResolution)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.constructor (name, cb)](#apidoc.element.nools.Flow.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.containsRule (name)](#apidoc.element.nools.Flow.prototype.containsRule)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.getDefined (name)](#apidoc.element.nools.Flow.prototype.getDefined)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.getSession ()](#apidoc.element.nools.Flow.prototype.getSession)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.rule ()](#apidoc.element.nools.Flow.prototype.rule)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow.set (name, val)](#apidoc.element.nools.Flow.set)
1.  [function <span class="apidocSignatureSpan">nools.</span>agenda ()](#apidoc.element.nools.agenda)
1.  [function <span class="apidocSignatureSpan">nools.</span>compile (file, options, cb)](#apidoc.element.nools.compile)
1.  [function <span class="apidocSignatureSpan">nools.</span>context ()](#apidoc.element.nools.context)
1.  [function <span class="apidocSignatureSpan">nools.</span>deleteFlow (name)](#apidoc.element.nools.deleteFlow)
1.  [function <span class="apidocSignatureSpan">nools.</span>deleteFlows ()](#apidoc.element.nools.deleteFlows)
1.  [function <span class="apidocSignatureSpan">nools.</span>executionStrategy ()](#apidoc.element.nools.executionStrategy)
1.  [function <span class="apidocSignatureSpan">nools.</span>extended (obj)](#apidoc.element.nools.extended)
1.  [function <span class="apidocSignatureSpan">nools.</span>flow (name, cb)](#apidoc.element.nools.flow)
1.  [function <span class="apidocSignatureSpan">nools.</span>getFlow (name)](#apidoc.element.nools.getFlow)
1.  [function <span class="apidocSignatureSpan">nools.</span>hasFlow (name)](#apidoc.element.nools.hasFlow)
1.  [function <span class="apidocSignatureSpan">nools.</span>linkedList ()](#apidoc.element.nools.linkedList)
1.  [function <span class="apidocSignatureSpan">nools.</span>parse (source)](#apidoc.element.nools.parse)
1.  [function <span class="apidocSignatureSpan">nools.</span>transpile (file, options)](#apidoc.element.nools.transpile)
1.  object <span class="apidocSignatureSpan">nools.</span>Flow.prototype
1.  object <span class="apidocSignatureSpan">nools.</span>agenda.prototype
1.  object <span class="apidocSignatureSpan">nools.</span>conflict
1.  object <span class="apidocSignatureSpan">nools.</span>constraint
1.  object <span class="apidocSignatureSpan">nools.</span>constraintMatcher
1.  object <span class="apidocSignatureSpan">nools.</span>context.prototype
1.  object <span class="apidocSignatureSpan">nools.</span>executionStrategy.prototype
1.  object <span class="apidocSignatureSpan">nools.</span>flow.prototype
1.  object <span class="apidocSignatureSpan">nools.</span>linkedList.prototype
1.  object <span class="apidocSignatureSpan">nools.</span>pattern
1.  object <span class="apidocSignatureSpan">nools.</span>rule
1.  object <span class="apidocSignatureSpan">nools.</span>workingMemory

#### [module nools.Flow](#apidoc.module.nools.Flow)
1.  [function <span class="apidocSignatureSpan">nools.</span>Flow ()](#apidoc.element.nools.Flow.Flow)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>_getSuper ()](#apidoc.element.nools.Flow._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>_super (args, a)](#apidoc.element.nools.Flow._super)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>as (obj, name)](#apidoc.element.nools.Flow.as)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>create (name, cb)](#apidoc.element.nools.Flow.create)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>deleteFlow (name)](#apidoc.element.nools.Flow.deleteFlow)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>deleteFlows ()](#apidoc.element.nools.Flow.deleteFlows)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>extend (proto)](#apidoc.element.nools.Flow.extend)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>get (name)](#apidoc.element.nools.Flow.get)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>getFlow (name)](#apidoc.element.nools.Flow.getFlow)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>hasFlow (name)](#apidoc.element.nools.Flow.hasFlow)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>init ()](#apidoc.element.nools.Flow.init)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>mixin ()](#apidoc.element.nools.Flow.mixin)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>set (name, val)](#apidoc.element.nools.Flow.set)
1.  object <span class="apidocSignatureSpan">nools.Flow.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.Flow.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.Flow.</span>__setters__

#### [module nools.Flow.as](#apidoc.module.nools.Flow.as)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>as (obj, name)](#apidoc.element.nools.Flow.as.as)
1.  [function <span class="apidocSignatureSpan">nools.Flow.as.</span>_f (obj, name)](#apidoc.element.nools.Flow.as._f)

#### [module nools.Flow.deleteFlow](#apidoc.module.nools.Flow.deleteFlow)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>deleteFlow (name)](#apidoc.element.nools.Flow.deleteFlow.deleteFlow)
1.  [function <span class="apidocSignatureSpan">nools.Flow.deleteFlow.</span>_f (name)](#apidoc.element.nools.Flow.deleteFlow._f)

#### [module nools.Flow.deleteFlows](#apidoc.module.nools.Flow.deleteFlows)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>deleteFlows ()](#apidoc.element.nools.Flow.deleteFlows.deleteFlows)
1.  [function <span class="apidocSignatureSpan">nools.Flow.deleteFlows.</span>_f ()](#apidoc.element.nools.Flow.deleteFlows._f)

#### [module nools.Flow.extend](#apidoc.module.nools.Flow.extend)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>extend (proto)](#apidoc.element.nools.Flow.extend.extend)
1.  [function <span class="apidocSignatureSpan">nools.Flow.extend.</span>_f (proto)](#apidoc.element.nools.Flow.extend._f)

#### [module nools.Flow.get](#apidoc.module.nools.Flow.get)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>get (name)](#apidoc.element.nools.Flow.get.get)
1.  [function <span class="apidocSignatureSpan">nools.Flow.get.</span>_f (name)](#apidoc.element.nools.Flow.get._f)

#### [module nools.Flow.init](#apidoc.module.nools.Flow.init)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>init ()](#apidoc.element.nools.Flow.init.init)
1.  [function <span class="apidocSignatureSpan">nools.Flow.init.</span>_f ()](#apidoc.element.nools.Flow.init._f)

#### [module nools.Flow.mixin](#apidoc.module.nools.Flow.mixin)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>mixin ()](#apidoc.element.nools.Flow.mixin.mixin)
1.  [function <span class="apidocSignatureSpan">nools.Flow.mixin.</span>_f ()](#apidoc.element.nools.Flow.mixin._f)

#### [module nools.Flow.prototype](#apidoc.module.nools.Flow.prototype)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>_getSuper ()](#apidoc.element.nools.Flow.prototype._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>_static ()](#apidoc.element.nools.Flow.prototype._static)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>_super (args, a)](#apidoc.element.nools.Flow.prototype._super)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>addDefined (name, cls)](#apidoc.element.nools.Flow.prototype.addDefined)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>conflictResolution (strategies)](#apidoc.element.nools.Flow.prototype.conflictResolution)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>constructor (name, cb)](#apidoc.element.nools.Flow.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>containsRule (name)](#apidoc.element.nools.Flow.prototype.containsRule)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>getDefined (name)](#apidoc.element.nools.Flow.prototype.getDefined)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>getSession ()](#apidoc.element.nools.Flow.prototype.getSession)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>rule ()](#apidoc.element.nools.Flow.prototype.rule)
1.  object <span class="apidocSignatureSpan">nools.Flow.prototype.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.Flow.prototype.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.Flow.prototype.</span>__setters__

#### [module nools.Flow.prototype.addDefined](#apidoc.module.nools.Flow.prototype.addDefined)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>addDefined (name, cls)](#apidoc.element.nools.Flow.prototype.addDefined.addDefined)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.addDefined.</span>_f (name, cls)](#apidoc.element.nools.Flow.prototype.addDefined._f)

#### [module nools.Flow.prototype.conflictResolution](#apidoc.module.nools.Flow.prototype.conflictResolution)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>conflictResolution (strategies)](#apidoc.element.nools.Flow.prototype.conflictResolution.conflictResolution)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.conflictResolution.</span>_f (strategies)](#apidoc.element.nools.Flow.prototype.conflictResolution._f)

#### [module nools.Flow.prototype.constructor](#apidoc.module.nools.Flow.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>constructor ()](#apidoc.element.nools.Flow.prototype.constructor.constructor)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.constructor.</span>_f (name, cb)](#apidoc.element.nools.Flow.prototype.constructor._f)

#### [module nools.Flow.prototype.containsRule](#apidoc.module.nools.Flow.prototype.containsRule)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>containsRule (name)](#apidoc.element.nools.Flow.prototype.containsRule.containsRule)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.containsRule.</span>_f (name)](#apidoc.element.nools.Flow.prototype.containsRule._f)

#### [module nools.Flow.prototype.getDefined](#apidoc.module.nools.Flow.prototype.getDefined)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>getDefined (name)](#apidoc.element.nools.Flow.prototype.getDefined.getDefined)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.getDefined.</span>_f (name)](#apidoc.element.nools.Flow.prototype.getDefined._f)

#### [module nools.Flow.prototype.getSession](#apidoc.module.nools.Flow.prototype.getSession)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>getSession ()](#apidoc.element.nools.Flow.prototype.getSession.getSession)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.getSession.</span>_f ()](#apidoc.element.nools.Flow.prototype.getSession._f)

#### [module nools.Flow.prototype.rule](#apidoc.module.nools.Flow.prototype.rule)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>rule ()](#apidoc.element.nools.Flow.prototype.rule.rule)
1.  [function <span class="apidocSignatureSpan">nools.Flow.prototype.rule.</span>_f ()](#apidoc.element.nools.Flow.prototype.rule._f)

#### [module nools.Flow.set](#apidoc.module.nools.Flow.set)
1.  [function <span class="apidocSignatureSpan">nools.Flow.</span>set (name, val)](#apidoc.element.nools.Flow.set.set)
1.  [function <span class="apidocSignatureSpan">nools.Flow.set.</span>_f (name, val)](#apidoc.element.nools.Flow.set._f)

#### [module nools.agenda](#apidoc.module.nools.agenda)
1.  boolean <span class="apidocSignatureSpan">nools.agenda.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">nools.</span>agenda ()](#apidoc.element.nools.agenda.agenda)
1.  [function <span class="apidocSignatureSpan">nools.agenda.</span>EventEmitter ()](#apidoc.element.nools.agenda.EventEmitter)
1.  [function <span class="apidocSignatureSpan">nools.agenda.</span>_getSuper ()](#apidoc.element.nools.agenda._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.agenda.</span>_super (args, a)](#apidoc.element.nools.agenda._super)
1.  [function <span class="apidocSignatureSpan">nools.agenda.</span>init ()](#apidoc.element.nools.agenda.init)
1.  [function <span class="apidocSignatureSpan">nools.agenda.</span>listenerCount (emitter, type)](#apidoc.element.nools.agenda.listenerCount)
1.  number <span class="apidocSignatureSpan">nools.agenda.</span>_eventsCount
1.  number <span class="apidocSignatureSpan">nools.agenda.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">nools.agenda.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.agenda.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.agenda.</span>__setters__
1.  object <span class="apidocSignatureSpan">nools.agenda.</span>_events
1.  object <span class="apidocSignatureSpan">nools.agenda.</span>domain

#### [module nools.agenda.prototype](#apidoc.module.nools.agenda.prototype)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>_getSuper ()](#apidoc.element.nools.agenda.prototype._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>_static ()](#apidoc.element.nools.agenda.prototype._static)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>_super (args, a)](#apidoc.element.nools.agenda.prototype._super)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>addAgendaGroup (groupName)](#apidoc.element.nools.agenda.prototype.addAgendaGroup)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>constructor (flow, conflictResolution)](#apidoc.element.nools.agenda.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>dispose ()](#apidoc.element.nools.agenda.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>fireNext ()](#apidoc.element.nools.agenda.prototype.fireNext)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>getAgendaGroup (groupName)](#apidoc.element.nools.agenda.prototype.getAgendaGroup)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>getFocused ()](#apidoc.element.nools.agenda.prototype.getFocused)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>getFocusedAgenda ()](#apidoc.element.nools.agenda.prototype.getFocusedAgenda)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>insert (node, insert)](#apidoc.element.nools.agenda.prototype.insert)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>isEmpty ()](#apidoc.element.nools.agenda.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>modify (node, context)](#apidoc.element.nools.agenda.prototype.modify)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>peek ()](#apidoc.element.nools.agenda.prototype.peek)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>pop ()](#apidoc.element.nools.agenda.prototype.pop)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>register (node)](#apidoc.element.nools.agenda.prototype.register)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>retract (node, retract)](#apidoc.element.nools.agenda.prototype.retract)
1.  [function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>setFocus (agendaGroup)](#apidoc.element.nools.agenda.prototype.setFocus)
1.  object <span class="apidocSignatureSpan">nools.agenda.prototype.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.agenda.prototype.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.agenda.prototype.</span>__setters__

#### [module nools.conflict](#apidoc.module.nools.conflict)
1.  [function <span class="apidocSignatureSpan">nools.conflict.</span>strategy (strats)](#apidoc.element.nools.conflict.strategy)
1.  object <span class="apidocSignatureSpan">nools.conflict.</span>strategies

#### [module nools.constraint](#apidoc.module.nools.constraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>ComparisonConstraint ()](#apidoc.element.nools.constraint.ComparisonConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>CustomConstraint ()](#apidoc.element.nools.constraint.CustomConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>EqualityConstraint ()](#apidoc.element.nools.constraint.EqualityConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>FromConstraint ()](#apidoc.element.nools.constraint.FromConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>HashConstraint ()](#apidoc.element.nools.constraint.HashConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>InequalityConstraint ()](#apidoc.element.nools.constraint.InequalityConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>ObjectConstraint ()](#apidoc.element.nools.constraint.ObjectConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceConstraint ()](#apidoc.element.nools.constraint.ReferenceConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceEqualityConstraint ()](#apidoc.element.nools.constraint.ReferenceEqualityConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceGTConstraint ()](#apidoc.element.nools.constraint.ReferenceGTConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceGTEConstraint ()](#apidoc.element.nools.constraint.ReferenceGTEConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceInequalityConstraint ()](#apidoc.element.nools.constraint.ReferenceInequalityConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceLTConstraint ()](#apidoc.element.nools.constraint.ReferenceLTConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceLTEConstraint ()](#apidoc.element.nools.constraint.ReferenceLTEConstraint)
1.  [function <span class="apidocSignatureSpan">nools.constraint.</span>TrueConstraint ()](#apidoc.element.nools.constraint.TrueConstraint)

#### [module nools.constraintMatcher](#apidoc.module.nools.constraintMatcher)
1.  [function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>equal (c1, c2)](#apidoc.element.nools.constraintMatcher.equal)
1.  [function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>getIdentifiers (constraint)](#apidoc.element.nools.constraintMatcher.getIdentifiers)
1.  [function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>getIndexableProperties (constraint)](#apidoc.element.nools.constraintMatcher.getIndexableProperties)
1.  [function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>getMatcher (rule, options, equality)](#apidoc.element.nools.constraintMatcher.getMatcher)
1.  [function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>getSourceMatcher (rule, options, equality)](#apidoc.element.nools.constraintMatcher.getSourceMatcher)
1.  [function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>toConstraints (constraint, options)](#apidoc.element.nools.constraintMatcher.toConstraints)
1.  [function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>toJs (rule, scope, alias, equality, wrap)](#apidoc.element.nools.constraintMatcher.toJs)

#### [module nools.context](#apidoc.module.nools.context)
1.  [function <span class="apidocSignatureSpan">nools.</span>context ()](#apidoc.element.nools.context.context)
1.  [function <span class="apidocSignatureSpan">nools.context.</span>_getSuper ()](#apidoc.element.nools.context._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.context.</span>_super (args, a)](#apidoc.element.nools.context._super)
1.  [function <span class="apidocSignatureSpan">nools.context.</span>as (obj, name)](#apidoc.element.nools.context.as)
1.  [function <span class="apidocSignatureSpan">nools.context.</span>extend (proto)](#apidoc.element.nools.context.extend)
1.  [function <span class="apidocSignatureSpan">nools.context.</span>get (name)](#apidoc.element.nools.context.get)
1.  [function <span class="apidocSignatureSpan">nools.context.</span>init ()](#apidoc.element.nools.context.init)
1.  [function <span class="apidocSignatureSpan">nools.context.</span>mixin ()](#apidoc.element.nools.context.mixin)
1.  [function <span class="apidocSignatureSpan">nools.context.</span>set (name, val)](#apidoc.element.nools.context.set)
1.  object <span class="apidocSignatureSpan">nools.context.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.context.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.context.</span>__setters__

#### [module nools.context.prototype](#apidoc.module.nools.context.prototype)
1.  [function <span class="apidocSignatureSpan">nools.context.prototype.</span>_getSuper ()](#apidoc.element.nools.context.prototype._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.context.prototype.</span>_static ()](#apidoc.element.nools.context.prototype._static)
1.  [function <span class="apidocSignatureSpan">nools.context.prototype.</span>_super (args, a)](#apidoc.element.nools.context.prototype._super)
1.  [function <span class="apidocSignatureSpan">nools.context.prototype.</span>clone (fact, paths, match)](#apidoc.element.nools.context.prototype.clone)
1.  [function <span class="apidocSignatureSpan">nools.context.prototype.</span>constructor (fact, paths, mr)](#apidoc.element.nools.context.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nools.context.prototype.</span>isMatch (isMatch)](#apidoc.element.nools.context.prototype.isMatch)
1.  [function <span class="apidocSignatureSpan">nools.context.prototype.</span>mergeMatch (merge)](#apidoc.element.nools.context.prototype.mergeMatch)
1.  [function <span class="apidocSignatureSpan">nools.context.prototype.</span>set (key, value)](#apidoc.element.nools.context.prototype.set)
1.  object <span class="apidocSignatureSpan">nools.context.prototype.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.context.prototype.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.context.prototype.</span>__setters__
1.  object <span class="apidocSignatureSpan">nools.context.prototype.</span>aliases
1.  object <span class="apidocSignatureSpan">nools.context.prototype.</span>fact
1.  object <span class="apidocSignatureSpan">nools.context.prototype.</span>factHash
1.  object <span class="apidocSignatureSpan">nools.context.prototype.</span>hashCode
1.  object <span class="apidocSignatureSpan">nools.context.prototype.</span>match
1.  object <span class="apidocSignatureSpan">nools.context.prototype.</span>paths
1.  object <span class="apidocSignatureSpan">nools.context.prototype.</span>pathsHash

#### [module nools.executionStrategy](#apidoc.module.nools.executionStrategy)
1.  [function <span class="apidocSignatureSpan">nools.</span>executionStrategy ()](#apidoc.element.nools.executionStrategy.executionStrategy)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.</span>_getSuper ()](#apidoc.element.nools.executionStrategy._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.</span>_super (args, a)](#apidoc.element.nools.executionStrategy._super)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.</span>as (obj, name)](#apidoc.element.nools.executionStrategy.as)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.</span>extend (proto)](#apidoc.element.nools.executionStrategy.extend)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.</span>get (name)](#apidoc.element.nools.executionStrategy.get)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.</span>init ()](#apidoc.element.nools.executionStrategy.init)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.</span>mixin ()](#apidoc.element.nools.executionStrategy.mixin)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.</span>set (name, val)](#apidoc.element.nools.executionStrategy.set)
1.  object <span class="apidocSignatureSpan">nools.executionStrategy.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.executionStrategy.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.executionStrategy.</span>__setters__

#### [module nools.executionStrategy.prototype](#apidoc.module.nools.executionStrategy.prototype)
1.  boolean <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>looping
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>__handleAsyncNext (next)](#apidoc.element.nools.executionStrategy.prototype.__handleAsyncNext)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>__handleSyncNext (next)](#apidoc.element.nools.executionStrategy.prototype.__handleSyncNext)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>_getSuper ()](#apidoc.element.nools.executionStrategy.prototype._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>_static ()](#apidoc.element.nools.executionStrategy.prototype._static)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>_super (args, a)](#apidoc.element.nools.executionStrategy.prototype._super)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>callNext ()](#apidoc.element.nools.executionStrategy.prototype.callNext)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>callback ()](#apidoc.element.nools.executionStrategy.prototype.callback)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>constructor ()](#apidoc.element.nools.executionStrategy.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>execute ()](#apidoc.element.nools.executionStrategy.prototype.execute)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>halt ()](#apidoc.element.nools.executionStrategy.prototype.halt)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>onAlter ()](#apidoc.element.nools.executionStrategy.prototype.onAlter)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>setup ()](#apidoc.element.nools.executionStrategy.prototype.setup)
1.  [function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>tearDown ()](#apidoc.element.nools.executionStrategy.prototype.tearDown)
1.  object <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>__setters__

#### [module nools.extended](#apidoc.module.nools.extended)
1.  [function <span class="apidocSignatureSpan">nools.</span>extended (obj)](#apidoc.element.nools.extended.extended)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>AVLTree ()](#apidoc.element.nools.extended.AVLTree)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>AnderssonTree ()](#apidoc.element.nools.extended.AnderssonTree)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>BinaryTree ()](#apidoc.element.nools.extended.BinaryTree)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>HashTable ()](#apidoc.element.nools.extended.HashTable)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>LinkedList ()](#apidoc.element.nools.extended.LinkedList)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>Promise ()](#apidoc.element.nools.extended.Promise)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>PromiseList ()](#apidoc.element.nools.extended.PromiseList)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>RedBlackTree ()](#apidoc.element.nools.extended.RedBlackTree)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>Tree ()](#apidoc.element.nools.extended.Tree)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>add (date, interval, amount)](#apidoc.element.nools.extended.add)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>applyFirst (method, args)](#apidoc.element.nools.extended.applyFirst)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>avg (arr)](#apidoc.element.nools.extended.avg)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>bind (scope, method, args)](#apidoc.element.nools.extended.bind)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>bindAll (scope)](#apidoc.element.nools.extended.bindAll)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>bindIgnore (scope, method, args)](#apidoc.element.nools.extended.bindIgnore)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>cartesian (a, b)](#apidoc.element.nools.extended.cartesian)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>chain (list)](#apidoc.element.nools.extended.chain)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>compact (arr)](#apidoc.element.nools.extended.compact)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>compare (date1, date2, portion)](#apidoc.element.nools.extended.compare)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>contains (arr, obj)](#apidoc.element.nools.extended.contains)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>containsAt (arr, obj, index)](#apidoc.element.nools.extended.containsAt)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>curry (depth, cb, scope)](#apidoc.element.nools.extended.curry)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>daysAgo (val)](#apidoc.element.nools.extended.daysAgo)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>daysFromNow (val)](#apidoc.element.nools.extended.daysFromNow)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>declare (sup, proto)](#apidoc.element.nools.extended.declare)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>deepEqual (actual, expected)](#apidoc.element.nools.extended.deepEqual)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>deepMerge (obj)](#apidoc.element.nools.extended.deepMerge)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>defer ()](#apidoc.element.nools.extended.defer)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>deferredList (promises)](#apidoc.element.nools.extended.deferredList)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>define (tester, decorate)](#apidoc.element.nools.extended.define)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>diffArr (arr1, arr2)](#apidoc.element.nools.extended.diffArr)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>diffHash (h1, h2)](#apidoc.element.nools.extended.diffHash)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>difference (arr1)](#apidoc.element.nools.extended.difference)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>escape (str, except)](#apidoc.element.nools.extended.escape)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>every (arr, iterator, scope)](#apidoc.element.nools.extended.every)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>expose ()](#apidoc.element.nools.extended.expose)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>extend (supr)](#apidoc.element.nools.extended.extend)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>filter (arr, iterator, scope)](#apidoc.element.nools.extended.filter)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>flatten (arr)](#apidoc.element.nools.extended.flatten)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>forEach (arr, iterator, scope)](#apidoc.element.nools.extended.forEach)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>format (str, obj)](#apidoc.element.nools.extended.format)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>getDaysInMonth (dateObject)](#apidoc.element.nools.extended.getDaysInMonth)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>getTimezoneName (dateObject)](#apidoc.element.nools.extended.getTimezoneName)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>has (obj, prop)](#apidoc.element.nools.extended.has)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>hoursAgo (val)](#apidoc.element.nools.extended.hoursAgo)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>hoursFromNow (val)](#apidoc.element.nools.extended.hoursFromNow)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>inPlaceDifference (a, b)](#apidoc.element.nools.extended.inPlaceDifference)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>inPlaceIntersection (a, b)](#apidoc.element.nools.extended.inPlaceIntersection)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>indexOf (arr, searchElement, from)](#apidoc.element.nools.extended.indexOf)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>instanceOf (obj, clazz)](#apidoc.element.nools.extended.instanceOf)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>intersect ()](#apidoc.element.nools.extended.intersect)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>intersection (a, b)](#apidoc.element.nools.extended.intersection)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>invoke (arr, func, args)](#apidoc.element.nools.extended.invoke)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isArguments (object)](#apidoc.element.nools.extended.isArguments)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isArray ()](#apidoc.element.nools.extended.isArray)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isBoolean (obj)](#apidoc.element.nools.extended.isBoolean)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isDate (obj)](#apidoc.element.nools.extended.isDate)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isDefined (obj)](#apidoc.element.nools.extended.isDefined)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isEmpty (object)](#apidoc.element.nools.extended.isEmpty)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isEq (obj, obj2)](#apidoc.element.nools.extended.isEq)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isFalse (obj)](#apidoc.element.nools.extended.isFalse)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isFunction (obj)](#apidoc.element.nools.extended.isFunction)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isGt (obj, obj2)](#apidoc.element.nools.extended.isGt)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isGte (obj, obj2)](#apidoc.element.nools.extended.isGte)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isHash (obj)](#apidoc.element.nools.extended.isHash)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isIn (obj, arr)](#apidoc.element.nools.extended.isIn)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isLeapYear (dateObject, utc)](#apidoc.element.nools.extended.isLeapYear)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isLength (obj, l)](#apidoc.element.nools.extended.isLength)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isLike (obj, reg)](#apidoc.element.nools.extended.isLike)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isLt (obj, obj2)](#apidoc.element.nools.extended.isLt)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isLte (obj, obj2)](#apidoc.element.nools.extended.isLte)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isNeq (obj, obj2)](#apidoc.element.nools.extended.isNeq)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isNotIn (obj, arr)](#apidoc.element.nools.extended.isNotIn)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isNotLength (obj, l)](#apidoc.element.nools.extended.isNotLength)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isNotLike (obj, reg)](#apidoc.element.nools.extended.isNotLike)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isNotNull (obj)](#apidoc.element.nools.extended.isNotNull)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isNull (obj)](#apidoc.element.nools.extended.isNull)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isNumber (obj)](#apidoc.element.nools.extended.isNumber)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isObject (obj)](#apidoc.element.nools.extended.isObject)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isPromiseLike (obj)](#apidoc.element.nools.extended.isPromiseLike)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isRegExp (obj)](#apidoc.element.nools.extended.isRegExp)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isSeq (obj, obj2)](#apidoc.element.nools.extended.isSeq)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isSneq (obj, obj2)](#apidoc.element.nools.extended.isSneq)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isString (obj)](#apidoc.element.nools.extended.isString)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isTrue (obj)](#apidoc.element.nools.extended.isTrue)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isUndefined (obj)](#apidoc.element.nools.extended.isUndefined)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isUndefinedOrNull (obj)](#apidoc.element.nools.extended.isUndefinedOrNull)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>isWeekend (dateObject, utc)](#apidoc.element.nools.extended.isWeekend)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>lastIndexOf (arr, searchElement, from)](#apidoc.element.nools.extended.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>map (arr, iterator, scope)](#apidoc.element.nools.extended.map)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>max (arr, cmp)](#apidoc.element.nools.extended.max)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>merge (obj)](#apidoc.element.nools.extended.merge)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>min (arr, cmp)](#apidoc.element.nools.extended.min)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>minutesAgo (val)](#apidoc.element.nools.extended.minutesAgo)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>minutesFromNow (val)](#apidoc.element.nools.extended.minutesFromNow)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>monthsAgo (val)](#apidoc.element.nools.extended.monthsAgo)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>monthsFromNow (val)](#apidoc.element.nools.extended.monthsFromNow)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>multiply (str, times)](#apidoc.element.nools.extended.multiply)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>notContains (arr, obj)](#apidoc.element.nools.extended.notContains)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>notContainsAt (arr, obj, index)](#apidoc.element.nools.extended.notContainsAt)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>notHas (obj, prop)](#apidoc.element.nools.extended.notHas)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>omit (hash, omitted)](#apidoc.element.nools.extended.omit)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>pad (string, length, ch, end)](#apidoc.element.nools.extended.pad)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>parseDate (dateStr, format)](#apidoc.element.nools.extended.parseDate)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>partial (method, args)](#apidoc.element.nools.extended.partial)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>permutations (arr, length)](#apidoc.element.nools.extended.permutations)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>pluck (arr, prop)](#apidoc.element.nools.extended.pluck)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>plucker (prop)](#apidoc.element.nools.extended.plucker)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>powerSet (arr)](#apidoc.element.nools.extended.powerSet)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>promise ()](#apidoc.element.nools.extended.promise)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>reduce (arr, accumulator, curr)](#apidoc.element.nools.extended.reduce)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>reduceRight (arr, accumulator, curr)](#apidoc.element.nools.extended.reduceRight)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>register (alias, extendWith)](#apidoc.element.nools.extended.register)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>reject (val)](#apidoc.element.nools.extended.reject)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>removeDuplicates (arr)](#apidoc.element.nools.extended.removeDuplicates)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>resolve (val)](#apidoc.element.nools.extended.resolve)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>rotate (arr, numberOfTimes)](#apidoc.element.nools.extended.rotate)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>secondsAgo (val)](#apidoc.element.nools.extended.secondsAgo)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>secondsFromNow (val)](#apidoc.element.nools.extended.secondsFromNow)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>serial (list)](#apidoc.element.nools.extended.serial)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>some (arr, iterator, scope)](#apidoc.element.nools.extended.some)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>sort (arr, cmp)](#apidoc.element.nools.extended.sort)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>style (str, options)](#apidoc.element.nools.extended.style)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>sum (array)](#apidoc.element.nools.extended.sum)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>switcher (obj)](#apidoc.element.nools.extended.switcher)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>tester (obj)](#apidoc.element.nools.extended.tester)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>toArray (testStr, delim)](#apidoc.element.nools.extended.toArray)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>transpose (arr)](#apidoc.element.nools.extended.transpose)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>trim (str)](#apidoc.element.nools.extended.trim)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>trimLeft (str)](#apidoc.element.nools.extended.trimLeft)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>trimRight (str)](#apidoc.element.nools.extended.trimRight)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>truncate (string, length, end)](#apidoc.element.nools.extended.truncate)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>union ()](#apidoc.element.nools.extended.union)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>unionArr (arr1, arr2)](#apidoc.element.nools.extended.unionArr)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>unique (arr)](#apidoc.element.nools.extended.unique)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>valuesAt (arr, indexes)](#apidoc.element.nools.extended.valuesAt)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>wait (args, fn)](#apidoc.element.nools.extended.wait)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>when (args)](#apidoc.element.nools.extended.when)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>wrap (fn, scope)](#apidoc.element.nools.extended.wrap)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>yearsAgo (val)](#apidoc.element.nools.extended.yearsAgo)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>yearsFromNow (val)](#apidoc.element.nools.extended.yearsFromNow)
1.  [function <span class="apidocSignatureSpan">nools.extended.</span>zip ()](#apidoc.element.nools.extended.zip)
1.  object <span class="apidocSignatureSpan">nools.extended.</span>__defined__
1.  object <span class="apidocSignatureSpan">nools.extended.</span>characters
1.  object <span class="apidocSignatureSpan">nools.extended.</span>hash
1.  string <span class="apidocSignatureSpan">nools.extended.</span>IN_ORDER
1.  string <span class="apidocSignatureSpan">nools.extended.</span>POST_ORDER
1.  string <span class="apidocSignatureSpan">nools.extended.</span>PRE_ORDER
1.  string <span class="apidocSignatureSpan">nools.extended.</span>REVERSE_ORDER

#### [module nools.flow](#apidoc.module.nools.flow)
1.  [function <span class="apidocSignatureSpan">nools.</span>flow (name, cb)](#apidoc.element.nools.flow.flow)
1.  [function <span class="apidocSignatureSpan">nools.flow.</span>_f (name, cb)](#apidoc.element.nools.flow._f)

#### [module nools.flow.prototype](#apidoc.module.nools.flow.prototype)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>_getSuper ()](#apidoc.element.nools.flow.prototype._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>_static ()](#apidoc.element.nools.flow.prototype._static)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>_super (args, a)](#apidoc.element.nools.flow.prototype._super)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>assert (fact)](#apidoc.element.nools.flow.prototype.assert)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>constructor (name, conflictResolutionStrategy)](#apidoc.element.nools.flow.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>containsRule (name)](#apidoc.element.nools.flow.prototype.containsRule)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>dispose ()](#apidoc.element.nools.flow.prototype.dispose)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>focus (focused)](#apidoc.element.nools.flow.prototype.focus)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>getFact (Type)](#apidoc.element.nools.flow.prototype.getFact)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>getFacts (Type)](#apidoc.element.nools.flow.prototype.getFacts)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>halt ()](#apidoc.element.nools.flow.prototype.halt)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>match (cb)](#apidoc.element.nools.flow.prototype.match)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>matchUntilHalt (cb)](#apidoc.element.nools.flow.prototype.matchUntilHalt)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>modify (fact, cb)](#apidoc.element.nools.flow.prototype.modify)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>print ()](#apidoc.element.nools.flow.prototype.print)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>retract (fact)](#apidoc.element.nools.flow.prototype.retract)
1.  [function <span class="apidocSignatureSpan">nools.flow.prototype.</span>rule (rule)](#apidoc.element.nools.flow.prototype.rule)
1.  object <span class="apidocSignatureSpan">nools.flow.prototype.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.flow.prototype.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.flow.prototype.</span>__setters__
1.  object <span class="apidocSignatureSpan">nools.flow.prototype.</span>executionStrategy
1.  object <span class="apidocSignatureSpan">nools.flow.prototype.</span>name

#### [module nools.getFlow](#apidoc.module.nools.getFlow)
1.  [function <span class="apidocSignatureSpan">nools.</span>getFlow (name)](#apidoc.element.nools.getFlow.getFlow)
1.  [function <span class="apidocSignatureSpan">nools.getFlow.</span>_f (name)](#apidoc.element.nools.getFlow._f)

#### [module nools.hasFlow](#apidoc.module.nools.hasFlow)
1.  [function <span class="apidocSignatureSpan">nools.</span>hasFlow (name)](#apidoc.element.nools.hasFlow.hasFlow)
1.  [function <span class="apidocSignatureSpan">nools.hasFlow.</span>_f (name)](#apidoc.element.nools.hasFlow._f)

#### [module nools.linkedList](#apidoc.module.nools.linkedList)
1.  [function <span class="apidocSignatureSpan">nools.</span>linkedList ()](#apidoc.element.nools.linkedList.linkedList)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.</span>_getSuper ()](#apidoc.element.nools.linkedList._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.</span>_super (args, a)](#apidoc.element.nools.linkedList._super)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.</span>as (obj, name)](#apidoc.element.nools.linkedList.as)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.</span>extend (proto)](#apidoc.element.nools.linkedList.extend)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.</span>get (name)](#apidoc.element.nools.linkedList.get)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.</span>init ()](#apidoc.element.nools.linkedList.init)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.</span>mixin ()](#apidoc.element.nools.linkedList.mixin)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.</span>set (name, val)](#apidoc.element.nools.linkedList.set)
1.  object <span class="apidocSignatureSpan">nools.linkedList.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.linkedList.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.linkedList.</span>__setters__

#### [module nools.linkedList.prototype](#apidoc.module.nools.linkedList.prototype)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>_getSuper ()](#apidoc.element.nools.linkedList.prototype._getSuper)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>_static ()](#apidoc.element.nools.linkedList.prototype._static)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>_super (args, a)](#apidoc.element.nools.linkedList.prototype._super)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>clear ()](#apidoc.element.nools.linkedList.prototype.clear)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>constructor ()](#apidoc.element.nools.linkedList.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>forEach (cb)](#apidoc.element.nools.linkedList.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>getByData (data)](#apidoc.element.nools.linkedList.prototype.getByData)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>push (data)](#apidoc.element.nools.linkedList.prototype.push)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>remove (node)](#apidoc.element.nools.linkedList.prototype.remove)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>removeByData (data)](#apidoc.element.nools.linkedList.prototype.removeByData)
1.  [function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>toArray ()](#apidoc.element.nools.linkedList.prototype.toArray)
1.  object <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>__getters__
1.  object <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>__meta
1.  object <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>__setters__

#### [module nools.pattern](#apidoc.module.nools.pattern)
1.  [function <span class="apidocSignatureSpan">nools.pattern.</span>CompositePattern ()](#apidoc.element.nools.pattern.CompositePattern)
1.  [function <span class="apidocSignatureSpan">nools.pattern.</span>ExistsPattern ()](#apidoc.element.nools.pattern.ExistsPattern)
1.  [function <span class="apidocSignatureSpan">nools.pattern.</span>FromExistsPattern ()](#apidoc.element.nools.pattern.FromExistsPattern)
1.  [function <span class="apidocSignatureSpan">nools.pattern.</span>FromNotPattern ()](#apidoc.element.nools.pattern.FromNotPattern)
1.  [function <span class="apidocSignatureSpan">nools.pattern.</span>FromPattern ()](#apidoc.element.nools.pattern.FromPattern)
1.  [function <span class="apidocSignatureSpan">nools.pattern.</span>InitialFact ()](#apidoc.element.nools.pattern.InitialFact)
1.  [function <span class="apidocSignatureSpan">nools.pattern.</span>InitialFactPattern ()](#apidoc.element.nools.pattern.InitialFactPattern)
1.  [function <span class="apidocSignatureSpan">nools.pattern.</span>NotPattern ()](#apidoc.element.nools.pattern.NotPattern)
1.  [function <span class="apidocSignatureSpan">nools.pattern.</span>ObjectPattern ()](#apidoc.element.nools.pattern.ObjectPattern)

#### [module nools.rule](#apidoc.module.nools.rule)
1.  [function <span class="apidocSignatureSpan">nools.rule.</span>createRule (name, options, conditions, cb)](#apidoc.element.nools.rule.createRule)

#### [module nools.workingMemory](#apidoc.module.nools.workingMemory)
1.  [function <span class="apidocSignatureSpan">nools.workingMemory.</span>WorkingMemory ()](#apidoc.element.nools.workingMemory.WorkingMemory)



# <a name="apidoc.module.nools"></a>[module nools](#apidoc.module.nools)

#### <a name="apidoc.element.nools.Flow"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow ()](#apidoc.element.nools.Flow)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.as"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.as (obj, name)](#apidoc.element.nools.Flow.as)
- description and source-code
```javascript
function _export(obj, name) {
    if (obj && name) {
        obj[name] = this;
    } else {
        obj.exports = obj = this;
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.deleteFlow"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.deleteFlow (name)](#apidoc.element.nools.Flow.deleteFlow)
- description and source-code
```javascript
Flow.deleteFlow = function (name) {
    if (instanceOf(name, FlowContainer)) {
        name = name.name;
    }
    delete flows[name];
    return FlowContainer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.deleteFlows"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.deleteFlows ()](#apidoc.element.nools.Flow.deleteFlows)
- description and source-code
```javascript
Flow.deleteFlows = function () {
    for (var name in flows) {
        if (name in flows) {
            delete flows[name];
        }
    }
    return FlowContainer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.extend"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.extend (proto)](#apidoc.element.nools.Flow.extend)
- description and source-code
```javascript
function extend(proto) {
    return declare(this, proto);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.get"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.get (name)](#apidoc.element.nools.Flow.get)
- description and source-code
```javascript
function getter(name) {
    var getters = this.__getters__;
    if (getters.hasOwnProperty(name)) {
        return getters[name].apply(this);
    } else {
        return this[name];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.init"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.init ()](#apidoc.element.nools.Flow.init)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.mixin"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.mixin ()](#apidoc.element.nools.Flow.mixin)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.addDefined"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.addDefined (name, cls)](#apidoc.element.nools.Flow.prototype.addDefined)
- description and source-code
```javascript
Flow.prototype.addDefined = function (name, cls) {
    //normalize
    this.__defined[name.toLowerCase()] = cls;
    return cls;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.conflictResolution"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.conflictResolution (strategies)](#apidoc.element.nools.Flow.prototype.conflictResolution)
- description and source-code
```javascript
Flow.prototype.conflictResolution = function (strategies) {
    this.conflictResolutionStrategy = conflictStrategies.strategy(strategies);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.constructor (name, cb)](#apidoc.element.nools.Flow.prototype.constructor)
- description and source-code
```javascript
Flow.prototype.constructor = function (name, cb) {
    this.name = name;
    this.cb = cb;
    this.__rules = [];
    this.__defined = {};
    this.conflictResolutionStrategy = conflictResolution;
    if (cb) {
        cb.call(this, this);
    }
    if (!flows.hasOwnProperty(name)) {
        flows[name] = this;
    } else {
        throw new Error("Flow with " + name + " already defined");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.containsRule"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.containsRule (name)](#apidoc.element.nools.Flow.prototype.containsRule)
- description and source-code
```javascript
Flow.prototype.containsRule = function (name) {
    return extd.some(this.__rules, function (rule) {
        return rule.name === name;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.getDefined"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.getDefined (name)](#apidoc.element.nools.Flow.prototype.getDefined)
- description and source-code
```javascript
Flow.prototype.getDefined = function (name) {
    var ret = this.__defined[name.toLowerCase()];
    if (!ret) {
        throw new Error(name + " flow class is not defined");
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.getSession"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.getSession ()](#apidoc.element.nools.Flow.prototype.getSession)
- description and source-code
```javascript
Flow.prototype.getSession = function () {
    var flow = new Flow(this.name, this.conflictResolutionStrategy);
    forEach(this.__rules, function (rule) {
        flow.rule(rule);
    });
    flow.assert(new InitialFact());
    for (var i = 0, l = arguments.length; i < l; i++) {
        flow.assert(arguments[i]);
    }
    return flow;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.rule"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.prototype.rule ()](#apidoc.element.nools.Flow.prototype.rule)
- description and source-code
```javascript
Flow.prototype.rule = function () {
    this.__rules = this.__rules.concat(rule.createRule.apply(rule, arguments));
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.set"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow.set (name, val)](#apidoc.element.nools.Flow.set)
- description and source-code
```javascript
function setter(name, val) {
    var setters = this.__setters__;
    if (isHash(name)) {
        for (var i in name) {
            var prop = name[i];
            if (setters.hasOwnProperty(i)) {
                setters[name].call(this, prop);
            } else {
                this[i] = prop;
            }
        }
    } else {
        if (setters.hasOwnProperty(name)) {
            return setters[name].apply(this, argsToArray(arguments, 1));
        } else {
            return this[name] = val;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.agenda"></a>[function <span class="apidocSignatureSpan">nools.</span>agenda ()](#apidoc.element.nools.agenda)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.compile"></a>[function <span class="apidocSignatureSpan">nools.</span>compile (file, options, cb)](#apidoc.element.nools.compile)
- description and source-code
```javascript
compile = function (file, options, cb) {
    if (extd.isFunction(options)) {
        cb = options;
        options = {};
    } else {
        options = options || {};
    }
    if (extd.isString(file)) {
        options.name = options.name || (isNoolsFile(file) ? path.basename(file, path.extname(file)) : null);
        file = parse(file);
    }
    if (!options.name) {
        throw new Error("Name required when compiling nools source");
    }
    return  compile.compile(file, options, cb, FlowContainer);
}
```
- example usage
```shell
...
    }
}
'''

To use the flow

'''javascript
var flow = nools.compile(__dirname + "/helloworld.nools"),
    Message = flow.getDefined("message");
'''

### Flow Events

Each flow can have the following events emitted.
...
```

#### <a name="apidoc.element.nools.context"></a>[function <span class="apidocSignatureSpan">nools.</span>context ()](#apidoc.element.nools.context)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.deleteFlow"></a>[function <span class="apidocSignatureSpan">nools.</span>deleteFlow (name)](#apidoc.element.nools.deleteFlow)
- description and source-code
```javascript
deleteFlow = function (name) {
    FlowContainer.deleteFlow(name);
    return this;
}
```
- example usage
```shell
...
# Removing a flow

To remove a defined flow from 'nools' use the 'deleteFlow' function.

'''javascript
var myFlow = nools.flow("flow");

nools.deleteFlow("flow"); //returns nools for chaining

nools.getFlow("flow"); //undefined

'''

You may also remove a flow using the 'FlowContainer' object returned from nools.flow;
...
```

#### <a name="apidoc.element.nools.deleteFlows"></a>[function <span class="apidocSignatureSpan">nools.</span>deleteFlows ()](#apidoc.element.nools.deleteFlows)
- description and source-code
```javascript
deleteFlows = function () {
    FlowContainer.deleteFlows();
    return this;
}
```
- example usage
```shell
...
# Removing All Flows

To remove all flow from 'nools' use the 'deleteFlows' function.

'''javascript
var myFlow = nools.flow("flow");

nools.deleteFlows(); //returns nools for chaining

nools.getFlow("flow"); //undefined

'''


<a name="checking-for-flow"></a>
...
```

#### <a name="apidoc.element.nools.executionStrategy"></a>[function <span class="apidocSignatureSpan">nools.</span>executionStrategy ()](#apidoc.element.nools.executionStrategy)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended"></a>[function <span class="apidocSignatureSpan">nools.</span>extended (obj)](#apidoc.element.nools.extended)
- description and source-code
```javascript
function _extender(obj) {
    var ret = obj, i, l;
    if (!(obj instanceof Base)) {
        var OurBase = Base;
        for (i = 0, l = defined.length; i < l; i++) {
            var definer = defined[i];
            if (definer[0](obj)) {
                OurBase = OurBase.extend({instance: definer[1]});
            }
        }
        ret = new OurBase(obj);
        ret["__extender__"] = _extender;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.flow"></a>[function <span class="apidocSignatureSpan">nools.</span>flow (name, cb)](#apidoc.element.nools.flow)
- description and source-code
```javascript
flow = function (name, cb) {
    return new FlowContainer(name, cb);
}
```
- example usage
```shell
...
'''javascript
var nools = require("nools");

var Message = function (message) {
this.text = message;
};

var flow = nools.flow("Hello World", function (flow) {

//find any message that is exactly hello world
flow.rule("Hello", [Message, "m", "m.text =~ /^hello\\sworld$/"], function (facts) {
    facts.m.text = facts.m.text + " goodbye";
    this.modify(facts.m);
});
...
```

#### <a name="apidoc.element.nools.getFlow"></a>[function <span class="apidocSignatureSpan">nools.</span>getFlow (name)](#apidoc.element.nools.getFlow)
- description and source-code
```javascript
getFlow = function (name) {
    return flows[name];
}
```
- example usage
```shell
...
To remove a defined flow from 'nools' use the 'deleteFlow' function.

'''javascript
var myFlow = nools.flow("flow");

nools.deleteFlow("flow"); //returns nools for chaining

nools.getFlow("flow"); //undefined

'''

You may also remove a flow using the 'FlowContainer' object returned from nools.flow;

'''javascript
var myFlow = nools.flow("flow");
...
```

#### <a name="apidoc.element.nools.hasFlow"></a>[function <span class="apidocSignatureSpan">nools.</span>hasFlow (name)](#apidoc.element.nools.hasFlow)
- description and source-code
```javascript
hasFlow = function (name) {
    return extd.has(flows, name);
}
```
- example usage
```shell
...
# Checking If A Flow Exists

To check if a flow currently is registering with 'nools' use the 'hasFlow' function;

'''javascript
var myFlow = nools.flow("flow");

nools.hasFlow("flow"); //true

'''

<a name="agenda-groups"></a>
## Agenda Groups

Agenda groups allow for logical groups of rules within a flow.
...
```

#### <a name="apidoc.element.nools.linkedList"></a>[function <span class="apidocSignatureSpan">nools.</span>linkedList ()](#apidoc.element.nools.linkedList)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.parse"></a>[function <span class="apidocSignatureSpan">nools.</span>parse (source)](#apidoc.element.nools.parse)
- description and source-code
```javascript
function parse(source) {
    var ret;
    if (isNoolsFile(source)) {
        ret = compile.parse(fs.readFileSync(source, "utf8"), source);
    } else {
        ret = compile.parse(source);
    }
    return ret;
}
```
- example usage
```shell
...
    }
    return ret;
},

getIndexableProperties: function (rule) {
    if (rule[2] === "composite") {
        return this.getIndexableProperties(rule[0]);
    } else if (/^(\w+(\['[^']*'])*) *([!=]==?|[<>]=?) (\w+(\['[^']*'])*)$/.test(this.parse(rule))) {
        return getProps(this.__getProperties(rule)).flatten().value();
    } else {
        return [];
    }
},

getIdentifiers: function (rule) {
...
```

#### <a name="apidoc.element.nools.transpile"></a>[function <span class="apidocSignatureSpan">nools.</span>transpile (file, options)](#apidoc.element.nools.transpile)
- description and source-code
```javascript
transpile = function (file, options) {
    options = options || {};
    if (extd.isString(file)) {
        options.name = options.name || (isNoolsFile(file) ? path.basename(file, path.extname(file)) : null);
        file = parse(file);
    }
    return compile.transpile(file, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow"></a>[module nools.Flow](#apidoc.module.nools.Flow)

#### <a name="apidoc.element.nools.Flow.Flow"></a>[function <span class="apidocSignatureSpan">nools.</span>Flow ()](#apidoc.element.nools.Flow.Flow)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow._getSuper"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>_getSuper ()](#apidoc.element.nools.Flow._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow._super"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>_super (args, a)](#apidoc.element.nools.Flow._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.Flow.as"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>as (obj, name)](#apidoc.element.nools.Flow.as)
- description and source-code
```javascript
function _export(obj, name) {
    if (obj && name) {
        obj[name] = this;
    } else {
        obj.exports = obj = this;
    }
    return this;
}
```
- example usage
```shell
...
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.constraint === constraint.constraint;
}
    }
}).as(exports, "ObjectConstraint");

var EqualityConstraint = Constraint.extend({

    instance: {

type: "equality",
...
```

#### <a name="apidoc.element.nools.Flow.create"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>create (name, cb)](#apidoc.element.nools.Flow.create)
- description and source-code
```javascript
create = function (name, cb) {
    return new FlowContainer(name, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.deleteFlow"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>deleteFlow (name)](#apidoc.element.nools.Flow.deleteFlow)
- description and source-code
```javascript
deleteFlow = function (name) {
    if (instanceOf(name, FlowContainer)) {
        name = name.name;
    }
    delete flows[name];
    return FlowContainer;
}
```
- example usage
```shell
...
# Removing a flow

To remove a defined flow from 'nools' use the 'deleteFlow' function.

'''javascript
var myFlow = nools.flow("flow");

nools.deleteFlow("flow"); //returns nools for chaining

nools.getFlow("flow"); //undefined

'''

You may also remove a flow using the 'FlowContainer' object returned from nools.flow;
...
```

#### <a name="apidoc.element.nools.Flow.deleteFlows"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>deleteFlows ()](#apidoc.element.nools.Flow.deleteFlows)
- description and source-code
```javascript
deleteFlows = function () {
    for (var name in flows) {
        if (name in flows) {
            delete flows[name];
        }
    }
    return FlowContainer;
}
```
- example usage
```shell
...
# Removing All Flows

To remove all flow from 'nools' use the 'deleteFlows' function.

'''javascript
var myFlow = nools.flow("flow");

nools.deleteFlows(); //returns nools for chaining

nools.getFlow("flow"); //undefined

'''


<a name="checking-for-flow"></a>
...
```

#### <a name="apidoc.element.nools.Flow.extend"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>extend (proto)](#apidoc.element.nools.Flow.extend)
- description and source-code
```javascript
function extend(proto) {
    return declare(this, proto);
}
```
- example usage
```shell
...
    }
}


    }
});

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},
...
```

#### <a name="apidoc.element.nools.Flow.get"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>get (name)](#apidoc.element.nools.Flow.get)
- description and source-code
```javascript
function getter(name) {
    var getters = this.__getters__;
    if (getters.hasOwnProperty(name)) {
        return getters[name].apply(this);
    } else {
        return this[name];
    }
}
```
- example usage
```shell
...
},

getIndexableProperties: function () {
    return [];
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.get("alias") === constraint.get("alias") && extd.deepEqual(this.constraint
, constraint.constraint);
},

getters: {
    variables: function () {
        return [this.get("alias")];
    }
}
...
```

#### <a name="apidoc.element.nools.Flow.getFlow"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>getFlow (name)](#apidoc.element.nools.Flow.getFlow)
- description and source-code
```javascript
getFlow = function (name) {
    return flows[name];
}
```
- example usage
```shell
...
To remove a defined flow from 'nools' use the 'deleteFlow' function.

'''javascript
var myFlow = nools.flow("flow");

nools.deleteFlow("flow"); //returns nools for chaining

nools.getFlow("flow"); //undefined

'''

You may also remove a flow using the 'FlowContainer' object returned from nools.flow;

'''javascript
var myFlow = nools.flow("flow");
...
```

#### <a name="apidoc.element.nools.Flow.hasFlow"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>hasFlow (name)](#apidoc.element.nools.Flow.hasFlow)
- description and source-code
```javascript
hasFlow = function (name) {
    return extd.has(flows, name);
}
```
- example usage
```shell
...
# Checking If A Flow Exists

To check if a flow currently is registering with 'nools' use the 'hasFlow' function;

'''javascript
var myFlow = nools.flow("flow");

nools.hasFlow("flow"); //true

'''

<a name="agenda-groups"></a>
## Agenda Groups

Agenda groups allow for logical groups of rules within a flow.
...
```

#### <a name="apidoc.element.nools.Flow.init"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>init ()](#apidoc.element.nools.Flow.init)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.mixin"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>mixin ()](#apidoc.element.nools.Flow.mixin)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.set"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>set (name, val)](#apidoc.element.nools.Flow.set)
- description and source-code
```javascript
function setter(name, val) {
    var setters = this.__setters__;
    if (isHash(name)) {
        for (var i in name) {
            var prop = name[i];
            if (setters.hasOwnProperty(i)) {
                setters[name].call(this, prop);
            } else {
                this[i] = prop;
            }
        }
    } else {
        if (setters.hasOwnProperty(name)) {
            return setters[name].apply(this, argsToArray(arguments, 1));
        } else {
            return this[name] = val;
        }
    }
}
```
- example usage
```shell
...
    }
    if (store && !isEmpty(store)) {
        var atm = new constraint.HashConstraint(store);
        constraints.push(atm);
    }

    forEach(constraints, function (constraint) {
        constraint.set("alias", alias);
    });
    this.constraints = constraints;
},

getSpecificity: function () {
    var constraints = this.constraints, specificity = 0;
    for (var i = 0, l = constraints.length; i < l; i++) {
...
```



# <a name="apidoc.module.nools.Flow.as"></a>[module nools.Flow.as](#apidoc.module.nools.Flow.as)

#### <a name="apidoc.element.nools.Flow.as.as"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>as (obj, name)](#apidoc.element.nools.Flow.as.as)
- description and source-code
```javascript
function _export(obj, name) {
    if (obj && name) {
        obj[name] = this;
    } else {
        obj.exports = obj = this;
    }
    return this;
}
```
- example usage
```shell
...
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.constraint === constraint.constraint;
}
    }
}).as(exports, "ObjectConstraint");

var EqualityConstraint = Constraint.extend({

    instance: {

type: "equality",
...
```

#### <a name="apidoc.element.nools.Flow.as._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.as.</span>_f (obj, name)](#apidoc.element.nools.Flow.as._f)
- description and source-code
```javascript
function _export(obj, name) {
    if (obj && name) {
        obj[name] = this;
    } else {
        obj.exports = obj = this;
    }
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.deleteFlow"></a>[module nools.Flow.deleteFlow](#apidoc.module.nools.Flow.deleteFlow)

#### <a name="apidoc.element.nools.Flow.deleteFlow.deleteFlow"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>deleteFlow (name)](#apidoc.element.nools.Flow.deleteFlow.deleteFlow)
- description and source-code
```javascript
deleteFlow = function (name) {
    if (instanceOf(name, FlowContainer)) {
        name = name.name;
    }
    delete flows[name];
    return FlowContainer;
}
```
- example usage
```shell
...
# Removing a flow

To remove a defined flow from 'nools' use the 'deleteFlow' function.

'''javascript
var myFlow = nools.flow("flow");

nools.deleteFlow("flow"); //returns nools for chaining

nools.getFlow("flow"); //undefined

'''

You may also remove a flow using the 'FlowContainer' object returned from nools.flow;
...
```

#### <a name="apidoc.element.nools.Flow.deleteFlow._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.deleteFlow.</span>_f (name)](#apidoc.element.nools.Flow.deleteFlow._f)
- description and source-code
```javascript
_f = function (name) {
    if (instanceOf(name, FlowContainer)) {
        name = name.name;
    }
    delete flows[name];
    return FlowContainer;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.deleteFlows"></a>[module nools.Flow.deleteFlows](#apidoc.module.nools.Flow.deleteFlows)

#### <a name="apidoc.element.nools.Flow.deleteFlows.deleteFlows"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>deleteFlows ()](#apidoc.element.nools.Flow.deleteFlows.deleteFlows)
- description and source-code
```javascript
deleteFlows = function () {
    for (var name in flows) {
        if (name in flows) {
            delete flows[name];
        }
    }
    return FlowContainer;
}
```
- example usage
```shell
...
# Removing All Flows

To remove all flow from 'nools' use the 'deleteFlows' function.

'''javascript
var myFlow = nools.flow("flow");

nools.deleteFlows(); //returns nools for chaining

nools.getFlow("flow"); //undefined

'''


<a name="checking-for-flow"></a>
...
```

#### <a name="apidoc.element.nools.Flow.deleteFlows._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.deleteFlows.</span>_f ()](#apidoc.element.nools.Flow.deleteFlows._f)
- description and source-code
```javascript
_f = function () {
    for (var name in flows) {
        if (name in flows) {
            delete flows[name];
        }
    }
    return FlowContainer;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.extend"></a>[module nools.Flow.extend](#apidoc.module.nools.Flow.extend)

#### <a name="apidoc.element.nools.Flow.extend.extend"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>extend (proto)](#apidoc.element.nools.Flow.extend.extend)
- description and source-code
```javascript
function extend(proto) {
    return declare(this, proto);
}
```
- example usage
```shell
...
    }
}


    }
});

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},
...
```

#### <a name="apidoc.element.nools.Flow.extend._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.extend.</span>_f (proto)](#apidoc.element.nools.Flow.extend._f)
- description and source-code
```javascript
function extend(proto) {
    return declare(this, proto);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.get"></a>[module nools.Flow.get](#apidoc.module.nools.Flow.get)

#### <a name="apidoc.element.nools.Flow.get.get"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>get (name)](#apidoc.element.nools.Flow.get.get)
- description and source-code
```javascript
function getter(name) {
    var getters = this.__getters__;
    if (getters.hasOwnProperty(name)) {
        return getters[name].apply(this);
    } else {
        return this[name];
    }
}
```
- example usage
```shell
...
},

getIndexableProperties: function () {
    return [];
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.get("alias") === constraint.get("alias") && extd.deepEqual(this.constraint
, constraint.constraint);
},

getters: {
    variables: function () {
        return [this.get("alias")];
    }
}
...
```

#### <a name="apidoc.element.nools.Flow.get._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.get.</span>_f (name)](#apidoc.element.nools.Flow.get._f)
- description and source-code
```javascript
function getter(name) {
    var getters = this.__getters__;
    if (getters.hasOwnProperty(name)) {
        return getters[name].apply(this);
    } else {
        return this[name];
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.init"></a>[module nools.Flow.init](#apidoc.module.nools.Flow.init)

#### <a name="apidoc.element.nools.Flow.init.init"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>init ()](#apidoc.element.nools.Flow.init.init)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.init._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.init.</span>_f ()](#apidoc.element.nools.Flow.init._f)
- description and source-code
```javascript
function defaultFunction() {
    var meta = this.__meta || {},
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, arguments);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.mixin"></a>[module nools.Flow.mixin](#apidoc.module.nools.Flow.mixin)

#### <a name="apidoc.element.nools.Flow.mixin.mixin"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>mixin ()](#apidoc.element.nools.Flow.mixin.mixin)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.mixin._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.mixin.</span>_f ()](#apidoc.element.nools.Flow.mixin._f)
- description and source-code
```javascript
function mixin() {
    var args = argsToArray(arguments), l = args.length;
    var child = this.prototype;
    var childMeta = child.__meta, thisMeta = this.__meta, bases = child.__meta.bases, staticBases = bases.slice(),
        staticSupers = thisMeta.supers || [], supers = childMeta.supers || [];
    for (var i = 0; i < l; i++) {
        var m = args[i], mProto = m.prototype;
        var protoMeta = mProto.__meta, meta = m.__meta;
        !protoMeta && (protoMeta = (mProto.__meta = {proto: mProto || {}}));
        !meta && (meta = (m.__meta = {proto: m.__proto__ || {}}));
        defineMixinProps(child, protoMeta.proto || {});
        defineMixinProps(this, meta.proto || {});
        //copy the bases for static,

        mixinSupers(m.prototype, supers, bases);
        mixinSupers(m, staticSupers, staticBases);
    }
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.prototype"></a>[module nools.Flow.prototype](#apidoc.module.nools.Flow.prototype)

#### <a name="apidoc.element.nools.Flow.prototype._getSuper"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>_getSuper ()](#apidoc.element.nools.Flow.prototype._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype._static"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>_static ()](#apidoc.element.nools.Flow.prototype._static)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
...
    }

},

merge: function (that) {
    var ret = this;
    if (that instanceof ReferenceConstraint) {
        ret = new this._static([this.constraint, that.constraint, "and"], merge({}, this._options, this._options));
        ret._alias = this._alias || that._alias;
        ret.vars = this.vars.concat(that.vars);
    }
    return ret;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.Flow.prototype._super"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>_super (args, a)](#apidoc.element.nools.Flow.prototype._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.Flow.prototype.addDefined"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>addDefined (name, cls)](#apidoc.element.nools.Flow.prototype.addDefined)
- description and source-code
```javascript
addDefined = function (name, cls) {
    //normalize
    this.__defined[name.toLowerCase()] = cls;
    return cls;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.conflictResolution"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>conflictResolution (strategies)](#apidoc.element.nools.Flow.prototype.conflictResolution)
- description and source-code
```javascript
conflictResolution = function (strategies) {
    this.conflictResolutionStrategy = conflictStrategies.strategy(strategies);
    return this;
}
```
- example usage
```shell
...

To override the default strategy you can use the 'conflictResolution' method on a flow.

'''javascript

var flow = nools.flow(/**define your flow**/);

flow.conflictResolution(["salience", "factRecency", "activationRecency"]);

'''

The combination of 'salience', 'factRecency', and 'activationRecency' would do the following.

1. Check if the salience is the same, if not use the activation with the greatest salience.
2. If salience is the same check if fact recency is the same. The fact recency is determined by looping through the facts in each
 activation and until two different recencies are found. The activation with the greatest recency takes precendence.
...
```

#### <a name="apidoc.element.nools.Flow.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>constructor (name, cb)](#apidoc.element.nools.Flow.prototype.constructor)
- description and source-code
```javascript
constructor = function (name, cb) {
    this.name = name;
    this.cb = cb;
    this.__rules = [];
    this.__defined = {};
    this.conflictResolutionStrategy = conflictResolution;
    if (cb) {
        cb.call(this, this);
    }
    if (!flows.hasOwnProperty(name)) {
        flows[name] = this;
    } else {
        throw new Error("Flow with " + name + " already defined");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.containsRule"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>containsRule (name)](#apidoc.element.nools.Flow.prototype.containsRule)
- description and source-code
```javascript
containsRule = function (name) {
    return extd.some(this.__rules, function (rule) {
        return rule.name === name;
    });
}
```
- example usage
```shell
...
},

print: function () {
    this.rootNode.print();
},

containsRule: function (name) {
    return this.rootNode.containsRule(name);
},

rule: function (rule) {
    this.rootNode.assertRule(rule);
},

matchUntilHalt: function (cb) {
...
```

#### <a name="apidoc.element.nools.Flow.prototype.getDefined"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>getDefined (name)](#apidoc.element.nools.Flow.prototype.getDefined)
- description and source-code
```javascript
getDefined = function (name) {
    var ret = this.__defined[name.toLowerCase()];
    if (!ret) {
        throw new Error(name + " flow class is not defined");
    }
    return ret;
}
```
- example usage
```shell
...
}
'''

To use the flow

'''javascript
var flow = nools.compile(__dirname + "/helloworld.nools"),
    Message = flow.getDefined("message");
'''

### Flow Events

Each flow can have the following events emitted.

* 'assert (fact)' - emitted when facts are asserted
...
```

#### <a name="apidoc.element.nools.Flow.prototype.getSession"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>getSession ()](#apidoc.element.nools.Flow.prototype.getSession)
- description and source-code
```javascript
getSession = function () {
    var flow = new Flow(this.name, this.conflictResolutionStrategy);
    forEach(this.__rules, function (rule) {
        flow.rule(rule);
    });
    flow.assert(new InitialFact());
    for (var i = 0, l = arguments.length; i < l; i++) {
        flow.assert(arguments[i]);
    }
    return flow;
}
```
- example usage
```shell
...
## Working with a session

A session is an instance of the flow that contains a working memory and handles the assertion, modification, and retraction of facts
 from the engine.

To obtain an engine session from the flow invoke the  'getSession' method.

'''javascript
var session = flow.getSession();
'''

<a name="facts"></a>
## Working with facts

Facts are items that the rules should try to match.
...
```

#### <a name="apidoc.element.nools.Flow.prototype.rule"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>rule ()](#apidoc.element.nools.Flow.prototype.rule)
- description and source-code
```javascript
rule = function () {
    this.__rules = this.__rules.concat(rule.createRule.apply(rule, arguments));
    return this;
}
```
- example usage
```shell
...
var Message = function (message) {
this.text = message;
};

var flow = nools.flow("Hello World", function (flow) {

//find any message that is exactly hello world
flow.rule("Hello", [Message, "m", "m.text =~ /^hello\\sworld$/"], function (facts) {
    facts.m.text = facts.m.text + " goodbye";
    this.modify(facts.m);
});

//find all messages then end in goodbye
flow.rule("Goodbye", [Message, "m", "m.text =~ /.*goodbye$/"], function (facts) {
    console.log(facts.m.text);
...
```



# <a name="apidoc.module.nools.Flow.prototype.addDefined"></a>[module nools.Flow.prototype.addDefined](#apidoc.module.nools.Flow.prototype.addDefined)

#### <a name="apidoc.element.nools.Flow.prototype.addDefined.addDefined"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>addDefined (name, cls)](#apidoc.element.nools.Flow.prototype.addDefined.addDefined)
- description and source-code
```javascript
addDefined = function (name, cls) {
    //normalize
    this.__defined[name.toLowerCase()] = cls;
    return cls;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.addDefined._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.addDefined.</span>_f (name, cls)](#apidoc.element.nools.Flow.prototype.addDefined._f)
- description and source-code
```javascript
_f = function (name, cls) {
    //normalize
    this.__defined[name.toLowerCase()] = cls;
    return cls;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.prototype.conflictResolution"></a>[module nools.Flow.prototype.conflictResolution](#apidoc.module.nools.Flow.prototype.conflictResolution)

#### <a name="apidoc.element.nools.Flow.prototype.conflictResolution.conflictResolution"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>conflictResolution (strategies)](#apidoc.element.nools.Flow.prototype.conflictResolution.conflictResolution)
- description and source-code
```javascript
conflictResolution = function (strategies) {
    this.conflictResolutionStrategy = conflictStrategies.strategy(strategies);
    return this;
}
```
- example usage
```shell
...

To override the default strategy you can use the 'conflictResolution' method on a flow.

'''javascript

var flow = nools.flow(/**define your flow**/);

flow.conflictResolution(["salience", "factRecency", "activationRecency"]);

'''

The combination of 'salience', 'factRecency', and 'activationRecency' would do the following.

1. Check if the salience is the same, if not use the activation with the greatest salience.
2. If salience is the same check if fact recency is the same. The fact recency is determined by looping through the facts in each
 activation and until two different recencies are found. The activation with the greatest recency takes precendence.
...
```

#### <a name="apidoc.element.nools.Flow.prototype.conflictResolution._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.conflictResolution.</span>_f (strategies)](#apidoc.element.nools.Flow.prototype.conflictResolution._f)
- description and source-code
```javascript
_f = function (strategies) {
    this.conflictResolutionStrategy = conflictStrategies.strategy(strategies);
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.prototype.constructor"></a>[module nools.Flow.prototype.constructor](#apidoc.module.nools.Flow.prototype.constructor)

#### <a name="apidoc.element.nools.Flow.prototype.constructor.constructor"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>constructor ()](#apidoc.element.nools.Flow.prototype.constructor.constructor)
- description and source-code
```javascript
function Function() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.Flow.prototype.constructor._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.constructor.</span>_f (name, cb)](#apidoc.element.nools.Flow.prototype.constructor._f)
- description and source-code
```javascript
_f = function (name, cb) {
    this.name = name;
    this.cb = cb;
    this.__rules = [];
    this.__defined = {};
    this.conflictResolutionStrategy = conflictResolution;
    if (cb) {
        cb.call(this, this);
    }
    if (!flows.hasOwnProperty(name)) {
        flows[name] = this;
    } else {
        throw new Error("Flow with " + name + " already defined");
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.prototype.containsRule"></a>[module nools.Flow.prototype.containsRule](#apidoc.module.nools.Flow.prototype.containsRule)

#### <a name="apidoc.element.nools.Flow.prototype.containsRule.containsRule"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>containsRule (name)](#apidoc.element.nools.Flow.prototype.containsRule.containsRule)
- description and source-code
```javascript
containsRule = function (name) {
    return extd.some(this.__rules, function (rule) {
        return rule.name === name;
    });
}
```
- example usage
```shell
...
},

print: function () {
    this.rootNode.print();
},

containsRule: function (name) {
    return this.rootNode.containsRule(name);
},

rule: function (rule) {
    this.rootNode.assertRule(rule);
},

matchUntilHalt: function (cb) {
...
```

#### <a name="apidoc.element.nools.Flow.prototype.containsRule._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.containsRule.</span>_f (name)](#apidoc.element.nools.Flow.prototype.containsRule._f)
- description and source-code
```javascript
_f = function (name) {
    return extd.some(this.__rules, function (rule) {
        return rule.name === name;
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.prototype.getDefined"></a>[module nools.Flow.prototype.getDefined](#apidoc.module.nools.Flow.prototype.getDefined)

#### <a name="apidoc.element.nools.Flow.prototype.getDefined.getDefined"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>getDefined (name)](#apidoc.element.nools.Flow.prototype.getDefined.getDefined)
- description and source-code
```javascript
getDefined = function (name) {
    var ret = this.__defined[name.toLowerCase()];
    if (!ret) {
        throw new Error(name + " flow class is not defined");
    }
    return ret;
}
```
- example usage
```shell
...
}
'''

To use the flow

'''javascript
var flow = nools.compile(__dirname + "/helloworld.nools"),
    Message = flow.getDefined("message");
'''

### Flow Events

Each flow can have the following events emitted.

* 'assert (fact)' - emitted when facts are asserted
...
```

#### <a name="apidoc.element.nools.Flow.prototype.getDefined._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.getDefined.</span>_f (name)](#apidoc.element.nools.Flow.prototype.getDefined._f)
- description and source-code
```javascript
_f = function (name) {
    var ret = this.__defined[name.toLowerCase()];
    if (!ret) {
        throw new Error(name + " flow class is not defined");
    }
    return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.prototype.getSession"></a>[module nools.Flow.prototype.getSession](#apidoc.module.nools.Flow.prototype.getSession)

#### <a name="apidoc.element.nools.Flow.prototype.getSession.getSession"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>getSession ()](#apidoc.element.nools.Flow.prototype.getSession.getSession)
- description and source-code
```javascript
getSession = function () {
    var flow = new Flow(this.name, this.conflictResolutionStrategy);
    forEach(this.__rules, function (rule) {
        flow.rule(rule);
    });
    flow.assert(new InitialFact());
    for (var i = 0, l = arguments.length; i < l; i++) {
        flow.assert(arguments[i]);
    }
    return flow;
}
```
- example usage
```shell
...
## Working with a session

A session is an instance of the flow that contains a working memory and handles the assertion, modification, and retraction of facts
 from the engine.

To obtain an engine session from the flow invoke the  'getSession' method.

'''javascript
var session = flow.getSession();
'''

<a name="facts"></a>
## Working with facts

Facts are items that the rules should try to match.
...
```

#### <a name="apidoc.element.nools.Flow.prototype.getSession._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.getSession.</span>_f ()](#apidoc.element.nools.Flow.prototype.getSession._f)
- description and source-code
```javascript
_f = function () {
    var flow = new Flow(this.name, this.conflictResolutionStrategy);
    forEach(this.__rules, function (rule) {
        flow.rule(rule);
    });
    flow.assert(new InitialFact());
    for (var i = 0, l = arguments.length; i < l; i++) {
        flow.assert(arguments[i]);
    }
    return flow;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.prototype.rule"></a>[module nools.Flow.prototype.rule](#apidoc.module.nools.Flow.prototype.rule)

#### <a name="apidoc.element.nools.Flow.prototype.rule.rule"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.</span>rule ()](#apidoc.element.nools.Flow.prototype.rule.rule)
- description and source-code
```javascript
rule = function () {
    this.__rules = this.__rules.concat(rule.createRule.apply(rule, arguments));
    return this;
}
```
- example usage
```shell
...
var Message = function (message) {
this.text = message;
};

var flow = nools.flow("Hello World", function (flow) {

//find any message that is exactly hello world
flow.rule("Hello", [Message, "m", "m.text =~ /^hello\\sworld$/"], function (facts) {
    facts.m.text = facts.m.text + " goodbye";
    this.modify(facts.m);
});

//find all messages then end in goodbye
flow.rule("Goodbye", [Message, "m", "m.text =~ /.*goodbye$/"], function (facts) {
    console.log(facts.m.text);
...
```

#### <a name="apidoc.element.nools.Flow.prototype.rule._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.prototype.rule.</span>_f ()](#apidoc.element.nools.Flow.prototype.rule._f)
- description and source-code
```javascript
_f = function () {
    this.__rules = this.__rules.concat(rule.createRule.apply(rule, arguments));
    return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.Flow.set"></a>[module nools.Flow.set](#apidoc.module.nools.Flow.set)

#### <a name="apidoc.element.nools.Flow.set.set"></a>[function <span class="apidocSignatureSpan">nools.Flow.</span>set (name, val)](#apidoc.element.nools.Flow.set.set)
- description and source-code
```javascript
function setter(name, val) {
    var setters = this.__setters__;
    if (isHash(name)) {
        for (var i in name) {
            var prop = name[i];
            if (setters.hasOwnProperty(i)) {
                setters[name].call(this, prop);
            } else {
                this[i] = prop;
            }
        }
    } else {
        if (setters.hasOwnProperty(name)) {
            return setters[name].apply(this, argsToArray(arguments, 1));
        } else {
            return this[name] = val;
        }
    }
}
```
- example usage
```shell
...
    }
    if (store && !isEmpty(store)) {
        var atm = new constraint.HashConstraint(store);
        constraints.push(atm);
    }

    forEach(constraints, function (constraint) {
        constraint.set("alias", alias);
    });
    this.constraints = constraints;
},

getSpecificity: function () {
    var constraints = this.constraints, specificity = 0;
    for (var i = 0, l = constraints.length; i < l; i++) {
...
```

#### <a name="apidoc.element.nools.Flow.set._f"></a>[function <span class="apidocSignatureSpan">nools.Flow.set.</span>_f (name, val)](#apidoc.element.nools.Flow.set._f)
- description and source-code
```javascript
function setter(name, val) {
    var setters = this.__setters__;
    if (isHash(name)) {
        for (var i in name) {
            var prop = name[i];
            if (setters.hasOwnProperty(i)) {
                setters[name].call(this, prop);
            } else {
                this[i] = prop;
            }
        }
    } else {
        if (setters.hasOwnProperty(name)) {
            return setters[name].apply(this, argsToArray(arguments, 1));
        } else {
            return this[name] = val;
        }
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.agenda"></a>[module nools.agenda](#apidoc.module.nools.agenda)

#### <a name="apidoc.element.nools.agenda.agenda"></a>[function <span class="apidocSignatureSpan">nools.</span>agenda ()](#apidoc.element.nools.agenda.agenda)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.agenda.EventEmitter"></a>[function <span class="apidocSignatureSpan">nools.agenda.</span>EventEmitter ()](#apidoc.element.nools.agenda.EventEmitter)
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

#### <a name="apidoc.element.nools.agenda._getSuper"></a>[function <span class="apidocSignatureSpan">nools.agenda.</span>_getSuper ()](#apidoc.element.nools.agenda._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.agenda._super"></a>[function <span class="apidocSignatureSpan">nools.agenda.</span>_super (args, a)](#apidoc.element.nools.agenda._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.agenda.init"></a>[function <span class="apidocSignatureSpan">nools.agenda.</span>init ()](#apidoc.element.nools.agenda.init)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.agenda.listenerCount"></a>[function <span class="apidocSignatureSpan">nools.agenda.</span>listenerCount (emitter, type)](#apidoc.element.nools.agenda.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.agenda.prototype"></a>[module nools.agenda.prototype](#apidoc.module.nools.agenda.prototype)

#### <a name="apidoc.element.nools.agenda.prototype._getSuper"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>_getSuper ()](#apidoc.element.nools.agenda.prototype._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.agenda.prototype._static"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>_static ()](#apidoc.element.nools.agenda.prototype._static)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
...
    }

},

merge: function (that) {
    var ret = this;
    if (that instanceof ReferenceConstraint) {
        ret = new this._static([this.constraint, that.constraint, "and"], merge({}, this._options, this._options));
        ret._alias = this._alias || that._alias;
        ret.vars = this.vars.concat(that.vars);
    }
    return ret;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.agenda.prototype._super"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>_super (args, a)](#apidoc.element.nools.agenda.prototype._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.agenda.prototype.addAgendaGroup"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>addAgendaGroup (groupName)](#apidoc.element.nools.agenda.prototype.addAgendaGroup)
- description and source-code
```javascript
addAgendaGroup = function (groupName) {
    if (!extd.has(this.agendaGroups, groupName)) {
        this.agendaGroups[groupName] = new AVLTree({compare: this.comparator});
    }
}
```
- example usage
```shell
...
    instance: {
constructor: function (flow, conflictResolution) {
    this.agendaGroups = {};
    this.agendaGroupStack = [DEFAULT_AGENDA_GROUP];
    this.rules = {};
    this.flow = flow;
    this.comparator = conflictResolution;
    this.setFocus(DEFAULT_AGENDA_GROUP).addAgendaGroup(DEFAULT_AGENDA_GROUP);
},

addAgendaGroup: function (groupName) {
    if (!extd.has(this.agendaGroups, groupName)) {
        this.agendaGroups[groupName] = new AVLTree({compare: this.comparator});
    }
},
...
```

#### <a name="apidoc.element.nools.agenda.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>constructor (flow, conflictResolution)](#apidoc.element.nools.agenda.prototype.constructor)
- description and source-code
```javascript
constructor = function (flow, conflictResolution) {
    this.agendaGroups = {};
    this.agendaGroupStack = [DEFAULT_AGENDA_GROUP];
    this.rules = {};
    this.flow = flow;
    this.comparator = conflictResolution;
    this.setFocus(DEFAULT_AGENDA_GROUP).addAgendaGroup(DEFAULT_AGENDA_GROUP);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.agenda.prototype.dispose"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>dispose ()](#apidoc.element.nools.agenda.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
    for (var i in this.agendaGroups) {
        this.agendaGroups[i].clear();
    }
    var rules = this.rules;
    for (i in rules) {
        if (i in rules) {
            rules[i].tree.clear();
            rules[i].factTable.clear();

        }
    }
    this.rules = {};
}
```
- example usage
```shell
...
<a name="disposing"></a>
## Disposing of the session

When working with a lot of facts it is wise to call the 'dispose' method which will purge the current session of
all facts, this will help prevent the process from growing a large memory footprint.

'''javascript
session.dispose();
'''

<a name="removing-flow"></a>
# Removing a flow

To remove a defined flow from 'nools' use the 'deleteFlow' function.
...
```

#### <a name="apidoc.element.nools.agenda.prototype.fireNext"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>fireNext ()](#apidoc.element.nools.agenda.prototype.fireNext)
- description and source-code
```javascript
fireNext = function () {
    var agendaGroupStack = this.agendaGroupStack, ret = false;
    while (this.getFocusedAgenda().isEmpty() && this.getFocused() !== DEFAULT_AGENDA_GROUP) {
        agendaGroupStack.pop();
    }
    if (!this.getFocusedAgenda().isEmpty()) {
        var activation = this.pop();
        this.emit("fire", activation.rule.name, activation.match.factHash);
        var fired = activation.rule.fire(this.flow, activation.match);
        if (isPromise(fired)) {
            ret = fired.then(function () {
                //return true if an activation fired
                return true;
            });
        } else {
            ret = true;
        }
    }
    //return false if activation not fired
    return ret;
}
```
- example usage
```shell
...
    this.tearDown();
    this._super(arguments);
},


callNext: function () {
    this.looping = true;
    var next = this.agenda.fireNext();
    return isPromiseLike(next) ? this.__handleAsyncNext(next) : this.__handleSyncNext(next);
},

execute: function () {
    this.setup();
    this.callNext();
    return this;
...
```

#### <a name="apidoc.element.nools.agenda.prototype.getAgendaGroup"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>getAgendaGroup (groupName)](#apidoc.element.nools.agenda.prototype.getAgendaGroup)
- description and source-code
```javascript
getAgendaGroup = function (groupName) {
    return this.agendaGroups[groupName || DEFAULT_AGENDA_GROUP];
}
```
- example usage
```shell
...
},

retract: function (node, retract) {
    var rule = this.rules[node.name];
    retract.rule = node;
    var activation = rule.factTable.remove(retract);
    if (activation) {
        this.getAgendaGroup(node.rule.agendaGroup).remove(activation);
        rule.tree.remove(activation);
    }
},

insert: function (node, insert) {
    var rule = this.rules[node.name], nodeRule = node.rule, agendaGroup = nodeRule.agendaGroup;
    rule.tree.insert(insert);
...
```

#### <a name="apidoc.element.nools.agenda.prototype.getFocused"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>getFocused ()](#apidoc.element.nools.agenda.prototype.getFocused)
- description and source-code
```javascript
getFocused = function () {
    var ags = this.agendaGroupStack;
    return ags[ags.length - 1];
}
```
- example usage
```shell
...
},

getAgendaGroup: function (groupName) {
    return this.agendaGroups[groupName || DEFAULT_AGENDA_GROUP];
},

setFocus: function (agendaGroup) {
    if (agendaGroup !== this.getFocused() && this.agendaGroups[agendaGroup]) {
        this.agendaGroupStack.push(agendaGroup);
        this.emit("focused", agendaGroup);
    }
    return this;
},

getFocused: function () {
...
```

#### <a name="apidoc.element.nools.agenda.prototype.getFocusedAgenda"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>getFocusedAgenda ()](#apidoc.element.nools.agenda.prototype.getFocusedAgenda)
- description and source-code
```javascript
getFocusedAgenda = function () {
    return this.agendaGroups[this.getFocused()];
}
```
- example usage
```shell
...
    if (agendaGroup) {
        this.addAgendaGroup(agendaGroup);
    }
},

isEmpty: function () {
    var agendaGroupStack = this.agendaGroupStack, changed = false;
    while (this.getFocusedAgenda().isEmpty() && this.getFocused() !== DEFAULT_AGENDA_GROUP) {
        agendaGroupStack.pop();
        changed = true;
    }
    if (changed) {
        this.emit("focused", this.getFocused());
    }
    return this.getFocusedAgenda().isEmpty();
...
```

#### <a name="apidoc.element.nools.agenda.prototype.insert"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>insert (node, insert)](#apidoc.element.nools.agenda.prototype.insert)
- description and source-code
```javascript
insert = function (node, insert) {
    var rule = this.rules[node.name], nodeRule = node.rule, agendaGroup = nodeRule.agendaGroup;
    rule.tree.insert(insert);
    this.getAgendaGroup(agendaGroup).insert(insert);
    if (nodeRule.autoFocus) {
        this.setFocus(agendaGroup);
    }

    rule.factTable.insert(insert);
}
```
- example usage
```shell
...
        root = root.right;
    }
    return root.data;
},

modify: function (node, context) {
    this.retract(node, context);
    this.insert(node, context);
},

retract: function (node, retract) {
    var rule = this.rules[node.name];
    retract.rule = node;
    var activation = rule.factTable.remove(retract);
    if (activation) {
...
```

#### <a name="apidoc.element.nools.agenda.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>isEmpty ()](#apidoc.element.nools.agenda.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
    var agendaGroupStack = this.agendaGroupStack, changed = false;
    while (this.getFocusedAgenda().isEmpty() && this.getFocused() !== DEFAULT_AGENDA_GROUP) {
        agendaGroupStack.pop();
        changed = true;
    }
    if (changed) {
        this.emit("focused", this.getFocused());
    }
    return this.getFocusedAgenda().isEmpty();
}
```
- example usage
```shell
...
    if (agendaGroup) {
        this.addAgendaGroup(agendaGroup);
    }
},

isEmpty: function () {
    var agendaGroupStack = this.agendaGroupStack, changed = false;
    while (this.getFocusedAgenda().isEmpty() && this.getFocused() !== DEFAULT_AGENDA_GROUP) {
        agendaGroupStack.pop();
        changed = true;
    }
    if (changed) {
        this.emit("focused", this.getFocused());
    }
    return this.getFocusedAgenda().isEmpty();
...
```

#### <a name="apidoc.element.nools.agenda.prototype.modify"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>modify (node, context)](#apidoc.element.nools.agenda.prototype.modify)
- description and source-code
```javascript
modify = function (node, context) {
    this.retract(node, context);
    this.insert(node, context);
}
```
- example usage
```shell
...
};

var flow = nools.flow("Hello World", function (flow) {

    //find any message that is exactly hello world
    flow.rule("Hello", [Message, "m", "m.text =~ /^hello\\sworld$/"], function (facts) {
        facts.m.text = facts.m.text + " goodbye";
        this.modify(facts.m);
    });

    //find all messages then end in goodbye
    flow.rule("Goodbye", [Message, "m", "m.text =~ /.*goodbye$/"], function (facts) {
        console.log(facts.m.text);
    });
});
...
```

#### <a name="apidoc.element.nools.agenda.prototype.peek"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>peek ()](#apidoc.element.nools.agenda.prototype.peek)
- description and source-code
```javascript
peek = function () {
    var tree = this.getFocusedAgenda(), root = tree.__root;
    while (root.right) {
        root = root.right;
    }
    return root.data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.agenda.prototype.pop"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>pop ()](#apidoc.element.nools.agenda.prototype.pop)
- description and source-code
```javascript
pop = function () {
    var tree = this.getFocusedAgenda(), root = tree.__root;
    while (root.right) {
        root = root.right;
    }
    var v = root.data;
    tree.remove(v);
    var rule = this.rules[v.name];
    rule.tree.remove(v);
    rule.factTable.remove(v);
    return v;
}
```
- example usage
```shell
...
        this.addAgendaGroup(agendaGroup);
    }
},

isEmpty: function () {
    var agendaGroupStack = this.agendaGroupStack, changed = false;
    while (this.getFocusedAgenda().isEmpty() && this.getFocused() !== DEFAULT_AGENDA_GROUP) {
        agendaGroupStack.pop();
        changed = true;
    }
    if (changed) {
        this.emit("focused", this.getFocused());
    }
    return this.getFocusedAgenda().isEmpty();
},
...
```

#### <a name="apidoc.element.nools.agenda.prototype.register"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>register (node)](#apidoc.element.nools.agenda.prototype.register)
- description and source-code
```javascript
register = function (node) {
    var agendaGroup = node.rule.agendaGroup;
    this.rules[node.name] = {tree: new AVLTree({compare: this.comparator}), factTable: new FactHash()};
    if (agendaGroup) {
        this.addAgendaGroup(agendaGroup);
    }
}
```
- example usage
```shell
...


function union(arr1, arr2) {
return unique(arr1.concat(arr2));
}

module.exports = require("extended")()
.register(require("date-extended"))
.register(arr)
.register(require("object-extended"))
.register(require("string-extended"))
.register(require("promise-extended"))
.register(require("function-extended"))
.register(require("is-extended"))
.register("intersection", intersection)
...
```

#### <a name="apidoc.element.nools.agenda.prototype.retract"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>retract (node, retract)](#apidoc.element.nools.agenda.prototype.retract)
- description and source-code
```javascript
retract = function (node, retract) {
    var rule = this.rules[node.name];
    retract.rule = node;
    var activation = rule.factTable.remove(retract);
    if (activation) {
        this.getAgendaGroup(node.rule.agendaGroup).remove(activation);
        rule.tree.remove(activation);
    }
}
```
- example usage
```shell
...
'''javascript
var m = new Message("hello");

//assert the fact into the engine
session.assert(m);

//remove the fact from the engine
session.retract(m);

'''

**Note** 'retract' is typically used during the execution of the rules.

<a name="facts-modify"></a>
### Modify
...
```

#### <a name="apidoc.element.nools.agenda.prototype.setFocus"></a>[function <span class="apidocSignatureSpan">nools.agenda.prototype.</span>setFocus (agendaGroup)](#apidoc.element.nools.agenda.prototype.setFocus)
- description and source-code
```javascript
setFocus = function (agendaGroup) {
    if (agendaGroup !== this.getFocused() && this.agendaGroups[agendaGroup]) {
        this.agendaGroupStack.push(agendaGroup);
        this.emit("focused", agendaGroup);
    }
    return this;
}
```
- example usage
```shell
...
    instance: {
constructor: function (flow, conflictResolution) {
    this.agendaGroups = {};
    this.agendaGroupStack = [DEFAULT_AGENDA_GROUP];
    this.rules = {};
    this.flow = flow;
    this.comparator = conflictResolution;
    this.setFocus(DEFAULT_AGENDA_GROUP).addAgendaGroup(DEFAULT_AGENDA_GROUP);
},

addAgendaGroup: function (groupName) {
    if (!extd.has(this.agendaGroups, groupName)) {
        this.agendaGroups[groupName] = new AVLTree({compare: this.comparator});
    }
},
...
```



# <a name="apidoc.module.nools.conflict"></a>[module nools.conflict](#apidoc.module.nools.conflict)

#### <a name="apidoc.element.nools.conflict.strategy"></a>[function <span class="apidocSignatureSpan">nools.conflict.</span>strategy (strats)](#apidoc.element.nools.conflict.strategy)
- description and source-code
```javascript
strategy = function (strats) {
    strats = map(strats, function (s) {
        return strategies[s];
    });
    var stratsLength = strats.length;

    return function (a, b) {
        var i = -1, ret = 0;
        var equal = (a === b) || (a.name === b.name && a.hashCode === b.hashCode);
        if (!equal) {
            while (++i < stratsLength && !ret) {
                ret = strats[i](a, b);
            }
            ret = ret > 0 ? 1 : -1;
        }
        return ret;
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.constraint"></a>[module nools.constraint](#apidoc.module.nools.constraint)

#### <a name="apidoc.element.nools.constraint.ComparisonConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>ComparisonConstraint ()](#apidoc.element.nools.constraint.ComparisonConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.CustomConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>CustomConstraint ()](#apidoc.element.nools.constraint.CustomConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
...
return toJs(rule, options.scope, options.alias, equality, function (src) {
    return src;
});
};

exports.toConstraints = function (constraint, options) {
if (typeof constraint === 'function') {
    return [new atoms.CustomConstraint(constraint, options)];
}
//constraint.split("&&")
return lang.toConstraints(constraint, options);
};

exports.equal = function (c1, c2) {
return lang.equal(c1, c2);
...
```

#### <a name="apidoc.element.nools.constraint.EqualityConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>EqualityConstraint ()](#apidoc.element.nools.constraint.EqualityConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.FromConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>FromConstraint ()](#apidoc.element.nools.constraint.FromConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.HashConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>HashConstraint ()](#apidoc.element.nools.constraint.HashConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
...
if (constrnts.length) {
    constraints = constraints.concat(constrnts);
} else {
    var cnstrnt = new constraint.TrueConstraint();
    constraints.push(cnstrnt);
}
if (store && !isEmpty(store)) {
    var atm = new constraint.HashConstraint(store);
    constraints.push(atm);
}

forEach(constraints, function (constraint) {
    constraint.set("alias", alias);
});
this.constraints = constraints;
...
```

#### <a name="apidoc.element.nools.constraint.InequalityConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>InequalityConstraint ()](#apidoc.element.nools.constraint.InequalityConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.ObjectConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>ObjectConstraint ()](#apidoc.element.nools.constraint.ObjectConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
...
        constructor: function (type, alias, conditions, store, options) {
options = options || {};
this.id = id++;
this.type = type;
this.alias = alias;
this.conditions = conditions;
this.pattern = options.pattern;
var constraints = [new constraint.ObjectConstraint(type)];
var constrnts = constraintMatcher.toConstraints(conditions, merge({alias: alias}, options));
if (constrnts.length) {
    constraints = constraints.concat(constrnts);
} else {
    var cnstrnt = new constraint.TrueConstraint();
    constraints.push(cnstrnt);
}
...
```

#### <a name="apidoc.element.nools.constraint.ReferenceConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceConstraint ()](#apidoc.element.nools.constraint.ReferenceConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.ReferenceEqualityConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceEqualityConstraint ()](#apidoc.element.nools.constraint.ReferenceEqualityConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.ReferenceGTConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceGTConstraint ()](#apidoc.element.nools.constraint.ReferenceGTConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.ReferenceGTEConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceGTEConstraint ()](#apidoc.element.nools.constraint.ReferenceGTEConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.ReferenceInequalityConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceInequalityConstraint ()](#apidoc.element.nools.constraint.ReferenceInequalityConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.ReferenceLTConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceLTConstraint ()](#apidoc.element.nools.constraint.ReferenceLTConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.ReferenceLTEConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>ReferenceLTEConstraint ()](#apidoc.element.nools.constraint.ReferenceLTEConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.constraint.TrueConstraint"></a>[function <span class="apidocSignatureSpan">nools.constraint.</span>TrueConstraint ()](#apidoc.element.nools.constraint.TrueConstraint)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
...
this.conditions = conditions;
this.pattern = options.pattern;
var constraints = [new constraint.ObjectConstraint(type)];
var constrnts = constraintMatcher.toConstraints(conditions, merge({alias: alias}, options));
if (constrnts.length) {
    constraints = constraints.concat(constrnts);
} else {
    var cnstrnt = new constraint.TrueConstraint();
    constraints.push(cnstrnt);
}
if (store && !isEmpty(store)) {
    var atm = new constraint.HashConstraint(store);
    constraints.push(atm);
}
...
```



# <a name="apidoc.module.nools.constraintMatcher"></a>[module nools.constraintMatcher](#apidoc.module.nools.constraintMatcher)

#### <a name="apidoc.element.nools.constraintMatcher.equal"></a>[function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>equal (c1, c2)](#apidoc.element.nools.constraintMatcher.equal)
- description and source-code
```javascript
equal = function (c1, c2) {
    return lang.equal(c1, c2);
}
```
- example usage
```shell
...
    if (c1 === c2) {
        ret = true;
    } else {
        if (c1[2] === c2[2]) {
            if (indexOf(["string", "number", "boolean", "regexp", "identifier", "null"], c1[2]) !== -1) {
                ret = c1[0] === c2[0];
            } else if (c1[2] === "unary" || c1[2] === "logicalNot") {
                ret = this.equal(c1[0], c2[0]);
            } else {
                ret = this.equal(c1[0], c2[0]) && this.equal(c1[1], c2[1]);
            }
        }
    }
    return ret;
},
...
```

#### <a name="apidoc.element.nools.constraintMatcher.getIdentifiers"></a>[function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>getIdentifiers (constraint)](#apidoc.element.nools.constraintMatcher.getIdentifiers)
- description and source-code
```javascript
getIdentifiers = function (constraint) {
    return lang.getIdentifiers(constraint);
}
```
- example usage
```shell
...
                return this._alias;
            }
        },

        setters: {
            alias: function (alias) {
                this._alias = alias;
                this.vars = filter(constraintMatcher.getIdentifiers(this.constraint), function (v) {
                    return v !== alias;
                });
            }
        }
    }

}).as(exports, "ReferenceConstraint");
...
```

#### <a name="apidoc.element.nools.constraintMatcher.getIndexableProperties"></a>[function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>getIndexableProperties (constraint)](#apidoc.element.nools.constraintMatcher.getIndexableProperties)
- description and source-code
```javascript
getIndexableProperties = function (constraint) {
    return lang.getIndexableProperties(constraint);
}
```
- example usage
```shell
...


ReferenceConstraint.extend({
instance: {
    type: "reference_equality",
    op: "eq",
    getIndexableProperties: function () {
        return constraintMatcher.getIndexableProperties(this.constraint);
    }
}
}).as(exports, "ReferenceEqualityConstraint")
.extend({instance: {type: "reference_inequality", op: "neq"}}).as(exports, "ReferenceInequalityConstraint")
.extend({instance: {type: "reference_gt", op: "gt"}}).as(exports, "ReferenceGTConstraint")
.extend({instance: {type: "reference_gte", op: "gte"}}).as(exports, "ReferenceGTEConstraint")
.extend({instance: {type: "reference_lt", op: "lt"}}).as(exports, "ReferenceLTConstraint")
...
```

#### <a name="apidoc.element.nools.constraintMatcher.getMatcher"></a>[function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>getMatcher (rule, options, equality)](#apidoc.element.nools.constraintMatcher.getMatcher)
- description and source-code
```javascript
getMatcher = function (rule, options, equality) {
    options = options || {};
    return toJs(rule, options.scope, options.alias, equality, function (src) {
        return "!!(" + src + ")";
    });
}
```
- example usage
```shell
...

        type: "equality",

        constructor: function (constraint, options) {
            this._super([constraint]);
            options = options || {};
            this.pattern = options.pattern;
            this._matcher = constraintMatcher.getMatcher(constraint, options, true);
        },

        "assert": function (values) {
            return this._matcher(values);
        }
    }
}).as(exports, "EqualityConstraint");
...
```

#### <a name="apidoc.element.nools.constraintMatcher.getSourceMatcher"></a>[function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>getSourceMatcher (rule, options, equality)](#apidoc.element.nools.constraintMatcher.getSourceMatcher)
- description and source-code
```javascript
getSourceMatcher = function (rule, options, equality) {
    options = options || {};
    return toJs(rule, options.scope, options.alias, equality, function (src) {
        return src;
    });
}
```
- example usage
```shell
...
    }
}).as(exports, "HashConstraint");

Constraint.extend({
    instance: {
constructor: function (constraints, options) {
    this.type = "from";
    this.constraints = constraintMatcher.getSourceMatcher(constraints, (options || {}), true);
    extd.bindAll(this, ["assert"]);
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.get("alias") === constraint.get("alias") && deepEqual(this.constraints,
constraint.constraints);
},
...
```

#### <a name="apidoc.element.nools.constraintMatcher.toConstraints"></a>[function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>toConstraints (constraint, options)](#apidoc.element.nools.constraintMatcher.toConstraints)
- description and source-code
```javascript
toConstraints = function (constraint, options) {
    if (typeof constraint === 'function') {
        return [new atoms.CustomConstraint(constraint, options)];
    }
    //constraint.split("&&")
    return lang.toConstraints(constraint, options);
}
```
- example usage
```shell
...
    alias = options.alias,
    scope = options.scope || {};

var rule2 = rule[2];


if (rule2 === "and") {
    ret = ret.concat(this.toConstraints(rule[0], options)).concat(this.toConstraints(rule[1], options));
} else if (
    rule2 === "composite" ||
    rule2 === "or" ||
    rule2 === "lt" ||
    rule2 === "gt" ||
    rule2 === "lte" ||
    rule2 === "gte" ||
...
```

#### <a name="apidoc.element.nools.constraintMatcher.toJs"></a>[function <span class="apidocSignatureSpan">nools.constraintMatcher.</span>toJs (rule, scope, alias, equality, wrap)](#apidoc.element.nools.constraintMatcher.toJs)
- description and source-code
```javascript
toJs = function (rule, scope, alias, equality, wrap) {
<span class="apidocCodeCommentSpan">    /*jshint evil:true*/
</span>    var js = lang.parse(rule);
    scope = scope || {};
    var vars = lang.getIdentifiers(rule);
    var closureVars = ["var indexOf = definedFuncs.indexOf; var hasOwnProperty = Object.prototype.hasOwnProperty;"], funcVars = [];
    extd(vars).filter(function (v) {
        var ret = ["var ", v, " = "];
        if (definedFuncs.hasOwnProperty(v)) {
            ret.push("definedFuncs['", v, "']");
        } else if (scope.hasOwnProperty(v)) {
            ret.push("scope['", v, "']");
        } else {
            return true;
        }
        ret.push(";");
        closureVars.push(ret.join(""));
        return false;
    }).forEach(function (v) {
        var ret = ["var ", v, " = "];
        if (equality || v !== alias) {
            ret.push("fact." + v);
        } else if (v === alias) {
            ret.push("hash.", v, "");
        }
        ret.push(";");
        funcVars.push(ret.join(""));
    });
    var closureBody = closureVars.join("") + "return function matcher" + (matcherCount++) + (!equality ? "(fact, hash){" : "(fact
){") + funcVars.join("") + " return " + (wrap ? wrap(js) : js) + ";}";
    var f = new Function("definedFuncs, scope", closureBody)(definedFuncs, scope);
    //console.log(f.toString());
    return f;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.context"></a>[module nools.context](#apidoc.module.nools.context)

#### <a name="apidoc.element.nools.context.context"></a>[function <span class="apidocSignatureSpan">nools.</span>context ()](#apidoc.element.nools.context.context)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.context._getSuper"></a>[function <span class="apidocSignatureSpan">nools.context.</span>_getSuper ()](#apidoc.element.nools.context._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.context._super"></a>[function <span class="apidocSignatureSpan">nools.context.</span>_super (args, a)](#apidoc.element.nools.context._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.context.as"></a>[function <span class="apidocSignatureSpan">nools.context.</span>as (obj, name)](#apidoc.element.nools.context.as)
- description and source-code
```javascript
function _export(obj, name) {
    if (obj && name) {
        obj[name] = this;
    } else {
        obj.exports = obj = this;
    }
    return this;
}
```
- example usage
```shell
...
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.constraint === constraint.constraint;
}
    }
}).as(exports, "ObjectConstraint");

var EqualityConstraint = Constraint.extend({

    instance: {

type: "equality",
...
```

#### <a name="apidoc.element.nools.context.extend"></a>[function <span class="apidocSignatureSpan">nools.context.</span>extend (proto)](#apidoc.element.nools.context.extend)
- description and source-code
```javascript
function extend(proto) {
    return declare(this, proto);
}
```
- example usage
```shell
...
    }
}


    }
});

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},
...
```

#### <a name="apidoc.element.nools.context.get"></a>[function <span class="apidocSignatureSpan">nools.context.</span>get (name)](#apidoc.element.nools.context.get)
- description and source-code
```javascript
function getter(name) {
    var getters = this.__getters__;
    if (getters.hasOwnProperty(name)) {
        return getters[name].apply(this);
    } else {
        return this[name];
    }
}
```
- example usage
```shell
...
},

getIndexableProperties: function () {
    return [];
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.get("alias") === constraint.get("alias") && extd.deepEqual(this.constraint
, constraint.constraint);
},

getters: {
    variables: function () {
        return [this.get("alias")];
    }
}
...
```

#### <a name="apidoc.element.nools.context.init"></a>[function <span class="apidocSignatureSpan">nools.context.</span>init ()](#apidoc.element.nools.context.init)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.context.mixin"></a>[function <span class="apidocSignatureSpan">nools.context.</span>mixin ()](#apidoc.element.nools.context.mixin)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.context.set"></a>[function <span class="apidocSignatureSpan">nools.context.</span>set (name, val)](#apidoc.element.nools.context.set)
- description and source-code
```javascript
function setter(name, val) {
    var setters = this.__setters__;
    if (isHash(name)) {
        for (var i in name) {
            var prop = name[i];
            if (setters.hasOwnProperty(i)) {
                setters[name].call(this, prop);
            } else {
                this[i] = prop;
            }
        }
    } else {
        if (setters.hasOwnProperty(name)) {
            return setters[name].apply(this, argsToArray(arguments, 1));
        } else {
            return this[name] = val;
        }
    }
}
```
- example usage
```shell
...
    }
    if (store && !isEmpty(store)) {
        var atm = new constraint.HashConstraint(store);
        constraints.push(atm);
    }

    forEach(constraints, function (constraint) {
        constraint.set("alias", alias);
    });
    this.constraints = constraints;
},

getSpecificity: function () {
    var constraints = this.constraints, specificity = 0;
    for (var i = 0, l = constraints.length; i < l; i++) {
...
```



# <a name="apidoc.module.nools.context.prototype"></a>[module nools.context.prototype](#apidoc.module.nools.context.prototype)

#### <a name="apidoc.element.nools.context.prototype._getSuper"></a>[function <span class="apidocSignatureSpan">nools.context.prototype.</span>_getSuper ()](#apidoc.element.nools.context.prototype._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.context.prototype._static"></a>[function <span class="apidocSignatureSpan">nools.context.prototype.</span>_static ()](#apidoc.element.nools.context.prototype._static)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
...
    }

},

merge: function (that) {
    var ret = this;
    if (that instanceof ReferenceConstraint) {
        ret = new this._static([this.constraint, that.constraint, "and"], merge({}, this._options, this._options));
        ret._alias = this._alias || that._alias;
        ret.vars = this.vars.concat(that.vars);
    }
    return ret;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.context.prototype._super"></a>[function <span class="apidocSignatureSpan">nools.context.prototype.</span>_super (args, a)](#apidoc.element.nools.context.prototype._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.context.prototype.clone"></a>[function <span class="apidocSignatureSpan">nools.context.prototype.</span>clone (fact, paths, match)](#apidoc.element.nools.context.prototype.clone)
- description and source-code
```javascript
clone = function (fact, paths, match) {
    return new Context(fact || this.fact, paths || this.path, match || this.match);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.context.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nools.context.prototype.</span>constructor (fact, paths, mr)](#apidoc.element.nools.context.prototype.constructor)
- description and source-code
```javascript
constructor = function (fact, paths, mr) {
    this.fact = fact;
    if (mr) {
        this.match = mr;
    } else {
        this.match = new Match().addFact(fact);
    }
    this.factHash = this.match.factHash;
    this.aliases = this.match.aliases;
    this.hashCode = this.match.hashCode;
    if (paths) {
        this.paths = paths;
        this.pathsHash = createContextHash(paths, this.hashCode);
    } else {
        this.pathsHash = this.hashCode;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.context.prototype.isMatch"></a>[function <span class="apidocSignatureSpan">nools.context.prototype.</span>isMatch (isMatch)](#apidoc.element.nools.context.prototype.isMatch)
- description and source-code
```javascript
isMatch = function (isMatch) {
    if (isBoolean(isMatch)) {
        this.match.isMatch = isMatch;
    } else {
        return this.match.isMatch;
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.context.prototype.mergeMatch"></a>[function <span class="apidocSignatureSpan">nools.context.prototype.</span>mergeMatch (merge)](#apidoc.element.nools.context.prototype.mergeMatch)
- description and source-code
```javascript
mergeMatch = function (merge) {
    var match = this.match = this.match.merge(merge);
    this.factHash = match.factHash;
    this.hashCode = match.hashCode;
    this.aliases = match.aliases;
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.context.prototype.set"></a>[function <span class="apidocSignatureSpan">nools.context.prototype.</span>set (key, value)](#apidoc.element.nools.context.prototype.set)
- description and source-code
```javascript
set = function (key, value) {
    this.factHash[key] = value;
    this.aliases.push(key);
    return this;
}
```
- example usage
```shell
...
    }
    if (store && !isEmpty(store)) {
        var atm = new constraint.HashConstraint(store);
        constraints.push(atm);
    }

    forEach(constraints, function (constraint) {
        constraint.set("alias", alias);
    });
    this.constraints = constraints;
},

getSpecificity: function () {
    var constraints = this.constraints, specificity = 0;
    for (var i = 0, l = constraints.length; i < l; i++) {
...
```



# <a name="apidoc.module.nools.executionStrategy"></a>[module nools.executionStrategy](#apidoc.module.nools.executionStrategy)

#### <a name="apidoc.element.nools.executionStrategy.executionStrategy"></a>[function <span class="apidocSignatureSpan">nools.</span>executionStrategy ()](#apidoc.element.nools.executionStrategy.executionStrategy)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.executionStrategy._getSuper"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.</span>_getSuper ()](#apidoc.element.nools.executionStrategy._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.executionStrategy._super"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.</span>_super (args, a)](#apidoc.element.nools.executionStrategy._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.executionStrategy.as"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.</span>as (obj, name)](#apidoc.element.nools.executionStrategy.as)
- description and source-code
```javascript
function _export(obj, name) {
    if (obj && name) {
        obj[name] = this;
    } else {
        obj.exports = obj = this;
    }
    return this;
}
```
- example usage
```shell
...
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.constraint === constraint.constraint;
}
    }
}).as(exports, "ObjectConstraint");

var EqualityConstraint = Constraint.extend({

    instance: {

type: "equality",
...
```

#### <a name="apidoc.element.nools.executionStrategy.extend"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.</span>extend (proto)](#apidoc.element.nools.executionStrategy.extend)
- description and source-code
```javascript
function extend(proto) {
    return declare(this, proto);
}
```
- example usage
```shell
...
    }
}


    }
});

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},
...
```

#### <a name="apidoc.element.nools.executionStrategy.get"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.</span>get (name)](#apidoc.element.nools.executionStrategy.get)
- description and source-code
```javascript
function getter(name) {
    var getters = this.__getters__;
    if (getters.hasOwnProperty(name)) {
        return getters[name].apply(this);
    } else {
        return this[name];
    }
}
```
- example usage
```shell
...
},

getIndexableProperties: function () {
    return [];
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.get("alias") === constraint.get("alias") && extd.deepEqual(this.constraint
, constraint.constraint);
},

getters: {
    variables: function () {
        return [this.get("alias")];
    }
}
...
```

#### <a name="apidoc.element.nools.executionStrategy.init"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.</span>init ()](#apidoc.element.nools.executionStrategy.init)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.executionStrategy.mixin"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.</span>mixin ()](#apidoc.element.nools.executionStrategy.mixin)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.executionStrategy.set"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.</span>set (name, val)](#apidoc.element.nools.executionStrategy.set)
- description and source-code
```javascript
function setter(name, val) {
    var setters = this.__setters__;
    if (isHash(name)) {
        for (var i in name) {
            var prop = name[i];
            if (setters.hasOwnProperty(i)) {
                setters[name].call(this, prop);
            } else {
                this[i] = prop;
            }
        }
    } else {
        if (setters.hasOwnProperty(name)) {
            return setters[name].apply(this, argsToArray(arguments, 1));
        } else {
            return this[name] = val;
        }
    }
}
```
- example usage
```shell
...
    }
    if (store && !isEmpty(store)) {
        var atm = new constraint.HashConstraint(store);
        constraints.push(atm);
    }

    forEach(constraints, function (constraint) {
        constraint.set("alias", alias);
    });
    this.constraints = constraints;
},

getSpecificity: function () {
    var constraints = this.constraints, specificity = 0;
    for (var i = 0, l = constraints.length; i < l; i++) {
...
```



# <a name="apidoc.module.nools.executionStrategy.prototype"></a>[module nools.executionStrategy.prototype](#apidoc.module.nools.executionStrategy.prototype)

#### <a name="apidoc.element.nools.executionStrategy.prototype.__handleAsyncNext"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>__handleAsyncNext (next)](#apidoc.element.nools.executionStrategy.prototype.__handleAsyncNext)
- description and source-code
```javascript
__handleAsyncNext = function (next) {
    var self = this, agenda = self.agenda;
    return next.then(function () {
        self.looping = false;
        if (!agenda.isEmpty()) {
            if (self.flowAltered) {
                self.rootNode.incrementCounter();
                self.flowAltered = false;
            }
            if (!self.__halted) {
                self.callNext();
            } else {
                self.callback();
            }
        } else if (!self.matchUntilHalt || self.__halted) {
            self.callback();
        }
        self = null;
    }, this.errback);
}
```
- example usage
```shell
...
    this._super(arguments);
},


callNext: function () {
    this.looping = true;
    var next = this.agenda.fireNext();
    return isPromiseLike(next) ? this.__handleAsyncNext(next) : this.__handleSyncNext(next);
},

execute: function () {
    this.setup();
    this.callNext();
    return this;
}
...
```

#### <a name="apidoc.element.nools.executionStrategy.prototype.__handleSyncNext"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>__handleSyncNext (next)](#apidoc.element.nools.executionStrategy.prototype.__handleSyncNext)
- description and source-code
```javascript
__handleSyncNext = function (next) {
    this.looping = false;
    if (!this.agenda.isEmpty()) {
        if (this.flowAltered) {
            this.rootNode.incrementCounter();
            this.flowAltered = false;
        }
    }
    if (next && !this.__halted) {
        nextTick(this.callNext);
    } else if (!this.matchUntilHalt || this.__halted) {
        this.callback();
    }
    return next;
}
```
- example usage
```shell
...
    this._super(arguments);
},


callNext: function () {
    this.looping = true;
    var next = this.agenda.fireNext();
    return isPromiseLike(next) ? this.__handleAsyncNext(next) : this.__handleSyncNext(next);
},

execute: function () {
    this.setup();
    this.callNext();
    return this;
}
...
```

#### <a name="apidoc.element.nools.executionStrategy.prototype._getSuper"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>_getSuper ()](#apidoc.element.nools.executionStrategy.prototype._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.executionStrategy.prototype._static"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>_static ()](#apidoc.element.nools.executionStrategy.prototype._static)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
...
    }

},

merge: function (that) {
    var ret = this;
    if (that instanceof ReferenceConstraint) {
        ret = new this._static([this.constraint, that.constraint, "and"], merge({}, this._options, this._options));
        ret._alias = this._alias || that._alias;
        ret.vars = this.vars.concat(that.vars);
    }
    return ret;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.executionStrategy.prototype._super"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>_super (args, a)](#apidoc.element.nools.executionStrategy.prototype._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.executionStrategy.prototype.callNext"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>callNext ()](#apidoc.element.nools.executionStrategy.prototype.callNext)
- description and source-code
```javascript
callNext = function () {
    this.looping = true;
    var next = this.agenda.fireNext();
    return isPromiseLike(next) ? this.__handleAsyncNext(next) : this.__handleSyncNext(next);
}
```
- example usage
```shell
...
        this.callback();
    }
},

onAlter: function () {
    this.flowAltered = true;
    if (!this.looping && this.matchUntilHalt && !this.__halted) {
        this.callNext();
    }
},

setup: function () {
    var flow = this.flow;
    this.rootNode.resetCounter();
    flow.on("assert", this.onAlter);
...
```

#### <a name="apidoc.element.nools.executionStrategy.prototype.callback"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>callback ()](#apidoc.element.nools.executionStrategy.prototype.callback)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
...
    this.matchUntilHalt = !!(matchUntilHalt);
    extd.bindAll(this, ["onAlter", "callNext"]);
},

halt: function () {
    this.__halted = true;
    if (!this.looping) {
        this.callback();
    }
},

onAlter: function () {
    this.flowAltered = true;
    if (!this.looping && this.matchUntilHalt && !this.__halted) {
        this.callNext();
...
```

#### <a name="apidoc.element.nools.executionStrategy.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>constructor ()](#apidoc.element.nools.executionStrategy.prototype.constructor)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.executionStrategy.prototype.execute"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>execute ()](#apidoc.element.nools.executionStrategy.prototype.execute)
- description and source-code
```javascript
execute = function () {
    this.setup();
    this.callNext();
    return this;
}
```
- example usage
```shell
...
    },

    rule: function (rule) {
        this.rootNode.assertRule(rule);
    },

    matchUntilHalt: function (cb) {
        return (this.executionStrategy = new ExecutionStragegy(this, true)).execute().classic(cb).promise();
    },

    match: function (cb) {
        return (this.executionStrategy = new ExecutionStragegy(this)).execute().classic(cb).promise();
    }

}
...
```

#### <a name="apidoc.element.nools.executionStrategy.prototype.halt"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>halt ()](#apidoc.element.nools.executionStrategy.prototype.halt)
- description and source-code
```javascript
halt = function () {
    this.__halted = true;
    if (!this.looping) {
        this.callback();
    }
}
```
- example usage
```shell
...

focus: function (focused) {
    this.agenda.setFocus(focused);
    return this;
},

halt: function () {
    this.executionStrategy.halt();
    return this;
},

dispose: function () {
    this.workingMemory.dispose();
    this.agenda.dispose();
    this.rootNode.dispose();
...
```

#### <a name="apidoc.element.nools.executionStrategy.prototype.onAlter"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>onAlter ()](#apidoc.element.nools.executionStrategy.prototype.onAlter)
- description and source-code
```javascript
onAlter = function () {
    this.flowAltered = true;
    if (!this.looping && this.matchUntilHalt && !this.__halted) {
        this.callNext();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.executionStrategy.prototype.setup"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>setup ()](#apidoc.element.nools.executionStrategy.prototype.setup)
- description and source-code
```javascript
setup = function () {
    var flow = this.flow;
    this.rootNode.resetCounter();
    flow.on("assert", this.onAlter);
    flow.on("modify", this.onAlter);
    flow.on("retract", this.onAlter);
}
```
- example usage
```shell
...
        callNext: function () {
            this.looping = true;
            var next = this.agenda.fireNext();
            return isPromiseLike(next) ? this.__handleAsyncNext(next) : this.__handleSyncNext(next);
        },

        execute: function () {
            this.setup();
            this.callNext();
            return this;
        }
    }
}).as(module);
...
```

#### <a name="apidoc.element.nools.executionStrategy.prototype.tearDown"></a>[function <span class="apidocSignatureSpan">nools.executionStrategy.prototype.</span>tearDown ()](#apidoc.element.nools.executionStrategy.prototype.tearDown)
- description and source-code
```javascript
tearDown = function () {
    var flow = this.flow;
    flow.removeListener("assert", this.onAlter);
    flow.removeListener("modify", this.onAlter);
    flow.removeListener("retract", this.onAlter);
}
```
- example usage
```shell
...
    } else if (!this.matchUntilHalt || this.__halted) {
        this.callback();
    }
    return next;
},

callback: function () {
    this.tearDown();
    this._super(arguments);
},


callNext: function () {
    this.looping = true;
    var next = this.agenda.fireNext();
...
```



# <a name="apidoc.module.nools.extended"></a>[module nools.extended](#apidoc.module.nools.extended)

#### <a name="apidoc.element.nools.extended.extended"></a>[function <span class="apidocSignatureSpan">nools.</span>extended (obj)](#apidoc.element.nools.extended.extended)
- description and source-code
```javascript
function _extender(obj) {
    var ret = obj, i, l;
    if (!(obj instanceof Base)) {
        var OurBase = Base;
        for (i = 0, l = defined.length; i < l; i++) {
            var definer = defined[i];
            if (definer[0](obj)) {
                OurBase = OurBase.extend({instance: definer[1]});
            }
        }
        ret = new OurBase(obj);
        ret["__extender__"] = _extender;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.AVLTree"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>AVLTree ()](#apidoc.element.nools.extended.AVLTree)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.AnderssonTree"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>AnderssonTree ()](#apidoc.element.nools.extended.AnderssonTree)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.BinaryTree"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>BinaryTree ()](#apidoc.element.nools.extended.BinaryTree)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.HashTable"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>HashTable ()](#apidoc.element.nools.extended.HashTable)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.LinkedList"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>LinkedList ()](#apidoc.element.nools.extended.LinkedList)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.Promise"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>Promise ()](#apidoc.element.nools.extended.Promise)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.PromiseList"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>PromiseList ()](#apidoc.element.nools.extended.PromiseList)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.RedBlackTree"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>RedBlackTree ()](#apidoc.element.nools.extended.RedBlackTree)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.Tree"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>Tree ()](#apidoc.element.nools.extended.Tree)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.add"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>add (date, interval, amount)](#apidoc.element.nools.extended.add)
- description and source-code
```javascript
add = function (date, interval, amount) {
    var res = addTransform(interval, date, amount || 0);
    amount = res[0];
    var property = res[1];
    var sum = new Date(+date);
    var fixOvershoot = res[2];
    if (property) {
        sum["set" + property](sum["get" + property]() + amount);
    }

    if (fixOvershoot && (sum.getDate() < date.getDate())) {
        sum.setDate(0);
    }

    return sum; // Date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.applyFirst"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>applyFirst (method, args)](#apidoc.element.nools.extended.applyFirst)
- description and source-code
```javascript
function applyFirst(method, args) {
    args = argsToArray(arguments, 1);
    if (!isString(method) && !isFunction(method)) {
        throw new Error(method + " must be the name of a property or function to execute");
    }
    if (isString(method)) {
        return function () {
            var scopeArgs = argsToArray(arguments), scope = scopeArgs.shift();
            var func = scope[method];
            if (isFunction(func)) {
                scopeArgs = args.concat(scopeArgs);
                return spreadArgs(func, scopeArgs, scope);
            } else {
                return func;
            }
        };
    } else {
        return function () {
            var scopeArgs = argsToArray(arguments), scope = scopeArgs.shift();
            scopeArgs = args.concat(scopeArgs);
            return spreadArgs(method, scopeArgs, scope);
        };
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.avg"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>avg (arr)](#apidoc.element.nools.extended.avg)
- description and source-code
```javascript
function avg(arr) {
    arr = arr || [];
    if (arr.length) {
        var total = sum(arr);
        if (is.isNumber(total)) {
            return  total / arr.length;
        } else {
            throw new Error("Cannot average an array of non numbers.");
        }
    } else {
        return 0;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.bind"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>bind (scope, method, args)](#apidoc.element.nools.extended.bind)
- description and source-code
```javascript
function hitch(scope, method, args) {
    args = argsToArray(arguments, 2);
    if ((isString(method) && !(method in scope))) {
        throw new Error(method + " property not defined in scope");
    } else if (!isString(method) && !isFunction(method)) {
        throw new Error(method + " is not a function");
    }
    if (isString(method)) {
        return function () {
            var func = scope[method];
            if (isFunction(func)) {
                return spreadArgs(func, args.concat(argsToArray(arguments)), scope);
            } else {
                return func;
            }
        };
    } else {
        if (args.length) {
            return function () {
                return spreadArgs(method, args.concat(argsToArray(arguments)), scope);
            };
        } else {

            return function () {
                return spreadArgs(method, arguments, scope);
            };
        }
    }
}
```
- example usage
```shell
...

/*global setImmediate, window, MessageChannel*/
var extd = require("./extended");
var nextTick;
if (typeof setImmediate === "function") {
    // In IE10, or use https://github.com/NobleJS/setImmediate
    if (typeof window !== "undefined") {
        nextTick = extd.bind(window, setImmediate);
    } else {
        nextTick = setImmediate;
    }
} else if (typeof process !== "undefined") {
    // node
    nextTick = process.nextTick;
} else if (typeof MessageChannel !== "undefined") {
...
```

#### <a name="apidoc.element.nools.extended.bindAll"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>bindAll (scope)](#apidoc.element.nools.extended.bindAll)
- description and source-code
```javascript
function hitchAll(scope) {
    var funcs = argsToArray(arguments, 1);
    if (!isObject(scope) && !isFunction(scope)) {
        throw new TypeError("scope must be an object");
    }
    if (funcs.length === 1 && isArray(funcs[0])) {
        funcs = funcs[0];
    }
    if (!funcs.length) {
        funcs = [];
        for (var k in scope) {
            if (scope.hasOwnProperty(k) && isFunction(scope[k])) {
                funcs.push(k);
            }
        }
    }
    for (var i = 0, l = funcs.length; i < l; i++) {
        scope[funcs[i]] = hitch(scope, scope[funcs[i]]);
    }
    return scope;
}
```
- example usage
```shell
...
    instance: {
constructor: function (constraint) {
    if (!constraintMatcher) {
        constraintMatcher = require("./constraintMatcher");
    }
    this.id = id++;
    this.constraint = constraint;
    extd.bindAll(this, ["assert"]);
},
"assert": function () {
    throw new Error("not implemented");
},

getIndexableProperties: function () {
    return [];
...
```

#### <a name="apidoc.element.nools.extended.bindIgnore"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>bindIgnore (scope, method, args)](#apidoc.element.nools.extended.bindIgnore)
- description and source-code
```javascript
function hitchIgnore(scope, method, args) {
    args = argsToArray(arguments, 2);
    if ((isString(method) && !(method in scope))) {
        throw new Error(method + " property not defined in scope");
    } else if (!isString(method) && !isFunction(method)) {
        throw new Error(method + " is not a function");
    }
    if (isString(method)) {
        return function () {
            var func = scope[method];
            if (isFunction(func)) {
                return spreadArgs(func, args, scope);
            } else {
                return func;
            }
        };
    } else {
        return function () {
            return spreadArgs(method, args, scope);
        };
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.cartesian"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>cartesian (a, b)](#apidoc.element.nools.extended.cartesian)
- description and source-code
```javascript
function cartesian(a, b) {
    var ret = [];
    if (isArray(a) && isArray(b) && a.length && b.length) {
        ret = cross(a[0], b).concat(cartesian(a.slice(1), b));
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.chain"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>chain (list)](#apidoc.element.nools.extended.chain)
- description and source-code
```javascript
function chain(list) {
    if (isArray(list)) {
        return callNext(list, [], true);
    } else {
        throw new Error("When calling promise.serial the first argument must be an array");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.compact"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>compact (arr)](#apidoc.element.nools.extended.compact)
- description and source-code
```javascript
function compact(arr) {
    var ret = [];
    if (isArray(arr) && arr.length) {
        ret = filter(arr, function (item) {
            return !is.isUndefinedOrNull(item);
        });
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.compare"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>compare (date1, date2, portion)](#apidoc.element.nools.extended.compare)
- description and source-code
```javascript
compare = function (date1, date2, portion) {
    date1 = new Date(+date1);
    date2 = new Date(+(date2 || new Date()));

    if (portion === "date") {
        // Ignore times and compare dates.
        date1.setHours(0, 0, 0, 0);
        date2.setHours(0, 0, 0, 0);
    } else if (portion === "time") {
        // Ignore dates and compare times.
        date1.setFullYear(0, 0, 0);
        date2.setFullYear(0, 0, 0);
    }
    return date1 > date2 ? 1 : date1 < date2 ? -1 : 0;
}
```
- example usage
```shell
...
},

isNotNull: function (actual) {
    return actual !== null;
},

dateCmp: function (dt1, dt2) {
    return extd.compare(dt1, dt2);
}

};

forEach(["years", "days", "months", "hours", "minutes", "seconds"], function (k) {
definedFuncs[k + "FromNow"] = extd[k + "FromNow"];
definedFuncs[k + "Ago"] = extd[k + "Ago"];
...
```

#### <a name="apidoc.element.nools.extended.contains"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>contains (arr, obj)](#apidoc.element.nools.extended.contains)
- description and source-code
```javascript
function contains(arr, obj) {
    return isIn(obj, arr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.containsAt"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>containsAt (arr, obj, index)](#apidoc.element.nools.extended.containsAt)
- description and source-code
```javascript
function containsAt(arr, obj, index) {
    if (isArray(arr) && arr.length > index) {
        return isEq(arr[index], obj);
    }
    return false;
}
```
- example usage
```shell
...
    .switcher();

return _getParamType(type);
};

var parsePattern = extd
.switcher()
.containsAt("or", 0, function (condition) {
    condition.shift();
    return extd(condition).map(function (cond) {
        cond.scope = condition.scope;
        return parsePattern(cond);
    }).flatten().value();
})
.containsAt("not", 0, function (condition) {
...
```

#### <a name="apidoc.element.nools.extended.curry"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>curry (depth, cb, scope)](#apidoc.element.nools.extended.curry)
- description and source-code
```javascript
function curry(depth, cb, scope) {
    var f;
    if (scope) {
        f = hitch(scope, cb);
    } else {
        f = cb;
    }
    if (depth) {
        var len = depth - 1;
        for (var i = len; i >= 0; i--) {
            f = curryFunc(f, i === len);
        }
    }
    return f;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.daysAgo"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>daysAgo (val)](#apidoc.element.nools.extended.daysAgo)
- description and source-code
```javascript
daysAgo = function (val) {
    return date.add(new Date(), interval, -val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.daysFromNow"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>daysFromNow (val)](#apidoc.element.nools.extended.daysFromNow)
- description and source-code
```javascript
daysFromNow = function (val) {
    return date.add(new Date(), interval, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.declare"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>declare (sup, proto)](#apidoc.element.nools.extended.declare)
- description and source-code
```javascript
function declare(sup, proto) {
    function declared() {
        switch (arguments.length) {
        case 0:
            this.constructor.call(this);
            break;
        case 1:
            this.constructor.call(this, arguments[0]);
            break;
        case 2:
            this.constructor.call(this, arguments[0], arguments[1]);
            break;
        case 3:
            this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
            break;
        default:
            this.constructor.apply(this, arguments);
        }
    }

    __declare(declared, sup, proto);
    return declared.init() || declared;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.deepEqual"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>deepEqual (actual, expected)](#apidoc.element.nools.extended.deepEqual)
- description and source-code
```javascript
function deepEqual(actual, expected) {
    // 7.1. All identical values are equivalent, as determined by ===.
    if (actual === expected) {
        return true;

    } else if (typeof Buffer !== "undefined" && Buffer.isBuffer(actual) && Buffer.isBuffer(expected)) {
        if (actual.length !== expected.length) {
            return false;
        }
        for (var i = 0; i < actual.length; i++) {
            if (actual[i] !== expected[i]) {
                return false;
            }
        }
        return true;

        // 7.2. If the expected value is a Date object, the actual value is
        // equivalent if it is also a Date object that refers to the same time.
    } else if (isDate(actual) && isDate(expected)) {
        return actual.getTime() === expected.getTime();

        // 7.3 If the expected value is a RegExp object, the actual value is
        // equivalent if it is also a RegExp object with the same source and
        // properties ('global', 'multiline', 'lastIndex', 'ignoreCase').
    } else if (isRegExp(actual) && isRegExp(expected)) {
        return actual.source === expected.source &&
            actual.global === expected.global &&
            actual.multiline === expected.multiline &&
            actual.lastIndex === expected.lastIndex &&
            actual.ignoreCase === expected.ignoreCase;

        // 7.4. Other pairs that do not both pass typeof value == 'object',
        // equivalence is determined by ==.
    } else if (isString(actual) && isString(expected) && actual !== expected) {
        return false;
    } else if (typeof actual !== 'object' && typeof expected !== 'object') {
        return actual === expected;

        // 7.5 For all other Object pairs, including Array objects, equivalence is
        // determined by having the same number of owned properties (as verified
        // with Object.prototype.hasOwnProperty.call), the same set of keys
        // (although not necessarily the same order), equivalent values for every
        // corresponding key, and an identical 'prototype' property. Note: this
        // accounts for both named and indexed properties on Arrays.
    } else {
        return objEquiv(actual, expected);
    }
}
```
- example usage
```shell
...
},

getIndexableProperties: function () {
    return [];
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.get("alias") === constraint.get("alias") && extd.deepEqual(this.constraint
, constraint.constraint);
},

getters: {
    variables: function () {
        return [this.get("alias")];
    }
}
...
```

#### <a name="apidoc.element.nools.extended.deepMerge"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>deepMerge (obj)](#apidoc.element.nools.extended.deepMerge)
- description and source-code
```javascript
function deepMerge(obj) {
    if (!obj) {
        obj = {};
    }
    for (var i = 1, l = arguments.length; i < l; i++) {
        _deepMerge(obj, arguments[i]);
    }
    return obj; // Object
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.defer"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>defer ()](#apidoc.element.nools.extended.defer)
- description and source-code
```javascript
function createPromise() {
    return new Promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.deferredList"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>deferredList (promises)](#apidoc.element.nools.extended.deferredList)
- description and source-code
```javascript
function createPromiseList(promises) {
    return new PromiseList(promises, true).promise();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.define"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>define (tester, decorate)](#apidoc.element.nools.extended.define)
- description and source-code
```javascript
function define(tester, decorate) {
    if (arguments.length) {
        if (typeof tester === "object") {
            decorate = tester;
            tester = always;
        }
        decorate = decorate || {};
        var proto = {};
        decorateProto(proto, decorate);
        //handle browsers like which skip over the constructor while looping
        if (!proto.hasOwnProperty("constructor")) {
            if (decorate.hasOwnProperty("constructor")) {
                addMethod(proto, "constructor", decorate.constructor);
            } else {
                proto.constructor = function () {
                    this._super(arguments);
                };
            }
        }
        defined.push([tester, proto]);
    }
    return _extender;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.diffArr"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>diffArr (arr1, arr2)](#apidoc.element.nools.extended.diffArr)
- description and source-code
```javascript
function diffArr(arr1, arr2) {
    var ret = [], i = -1, j, l2 = arr2.length, l1 = arr1.length, a, found;
    if (l2 > l1) {
        ret = arr1.slice();
        while (++i < l2) {
            a = arr2[i];
            j = -1;
            l1 = ret.length;
            while (++j < l1) {
                if (ret[j] === a) {
                    ret.splice(j, 1);
                    break;
                }
            }
        }
    } else {
        while (++i < l1) {
            a = arr1[i];
            j = -1;
            found = false;
            while (++j < l2) {
                if (arr2[j] === a) {
                    found = true;
                    break;
                }
            }
            if (!found) {
                ret.push(a);
            }
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.diffHash"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>diffHash (h1, h2)](#apidoc.element.nools.extended.diffHash)
- description and source-code
```javascript
function diffHash(h1, h2) {
    var ret = {};
    for (var i in h1) {
        if (!hasOwnProperty.call(h2, i)) {
            ret[i] = h1[i];
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.difference"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>difference (arr1)](#apidoc.element.nools.extended.difference)
- description and source-code
```javascript
function difference(arr1) {
    var ret = arr1, args = flatten(argsToArray(arguments, 1));
    if (isArray(arr1)) {
        ret = filter(arr1, function (a) {
            return indexOf(args, a) === -1;
        });
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.escape"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>escape (str, except)](#apidoc.element.nools.extended.escape)
- description and source-code
```javascript
function escape(str, except) {
    return str.replace(/([\.$?*|{}\(\)\[\]\\\/\+^])/g, function (ch) {
        if (except && arr.indexOf(except, ch) !== -1) {
            return ch;
        }
        return "\\" + ch;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.every"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>every (arr, iterator, scope)](#apidoc.element.nools.extended.every)
- description and source-code
```javascript
function every(arr, iterator, scope) {
    if (arr && arrayEvery && arrayEvery === arr.every) {
        return arr.every(iterator, scope);
    }
    if (!isArray(arr) || typeof iterator !== "function") {
        throw new TypeError();
    }
    var t = Object(arr);
    var len = t.length >>> 0;
    for (var i = 0; i < len; i++) {
        if (i in t && !iterator.call(scope, t[i], i, t)) {
            return false;
        }
    }
    return true;
}
```
- example usage
```shell
...
function createRule(name, options, conditions, cb) {
if (isArray(options)) {
    cb = conditions;
    conditions = options;
} else {
    options = options || {};
}
var isRules = extd.every(conditions, function (cond) {
    return isArray(cond);
});
if (isRules && conditions.length === 1) {
    conditions = conditions[0];
    isRules = false;
}
var rules = [];
...
```

#### <a name="apidoc.element.nools.extended.expose"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>expose ()](#apidoc.element.nools.extended.expose)
- description and source-code
```javascript
function expose() {
    var methods;
    for (var i = 0, l = arguments.length; i < l; i++) {
        methods = arguments[i];
        if (typeof methods === "object") {
            merge(_extender, methods, ["define", "extend", "expose", "__defined__"]);
        }
    }
    return _extender;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.extend"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>extend (supr)](#apidoc.element.nools.extended.extend)
- description and source-code
```javascript
function extend(supr) {
    if (supr && supr.hasOwnProperty("__defined__")) {
        _extender["__defined__"] = defined = defined.concat(supr["__defined__"]);
    }
    merge(_extender, supr, ["define", "extend", "expose", "__defined__"]);
    return _extender;
}
```
- example usage
```shell
...
    }
}


    }
});

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},
...
```

#### <a name="apidoc.element.nools.extended.filter"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>filter (arr, iterator, scope)](#apidoc.element.nools.extended.filter)
- description and source-code
```javascript
function filter(arr, iterator, scope) {
    if (arr && arrayFilter && arrayFilter === arr.filter) {
        return arr.filter(iterator, scope);
    }
    if (!isArray(arr) || typeof iterator !== "function") {
        throw new TypeError();
    }

    var t = Object(arr);
    var len = t.length >>> 0;
    var res = [];
    for (var i = 0; i < len; i++) {
        if (i in t) {
            var val = t[i]; // in case fun mutates this
            if (iterator.call(scope, val, i, t)) {
                res.push(val);
            }
        }
    }
    return res;
}
```
- example usage
```shell
...
isNumber = extd.isNumber,
removeDups = extd.removeDuplicates,
atoms = require("./constraint");

function getProps(val) {
return extd(val).map(function mapper(val) {
    return isArray(val) ? isArray(val[0]) ? getProps(val).value() : val.reverse().join(".") : val;
}).flatten().filter(function (v) {
    return !!v;
});
}

var definedFuncs = {
indexOf: extd.indexOf,
now: function () {
...
```

#### <a name="apidoc.element.nools.extended.flatten"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>flatten (arr)](#apidoc.element.nools.extended.flatten)
- description and source-code
```javascript
function flatten(arr) {
    var set;
    var args = argsToArray(arguments);
    if (args.length > 1) {
        //assume we are intersections all the lists in the array
        set = args;
    } else {
        set = toArray(arr);
    }
    return reduce(set, function (a, b) {
        return a.concat(b);
    }, []);
}
```
- example usage
```shell
...
isNumber = extd.isNumber,
removeDups = extd.removeDuplicates,
atoms = require("./constraint");

function getProps(val) {
return extd(val).map(function mapper(val) {
    return isArray(val) ? isArray(val[0]) ? getProps(val).value() : val.reverse().join(".") : val;
}).flatten().filter(function (v) {
    return !!v;
});
}

var definedFuncs = {
indexOf: extd.indexOf,
now: function () {
...
```

#### <a name="apidoc.element.nools.extended.forEach"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>forEach (arr, iterator, scope)](#apidoc.element.nools.extended.forEach)
- description and source-code
```javascript
function forEach(arr, iterator, scope) {
    if (!isArray(arr) || typeof iterator !== "function") {
        throw new TypeError();
    }
    if (arr && arrayForEach && arrayForEach === arr.forEach) {
        arr.forEach(iterator, scope);
        return arr;
    }
    for (var i = 0, len = arr.length; i < len; ++i) {
        iterator.call(scope || arr, arr[i], i, arr);
    }

    return arr;
}
```
- example usage
```shell
...
        count--;
        if (!count) {
            done();
        }
    }
}

files.forEach(function (file) {
    var base = path.basename(file, ".nools"),
        out = path.resolve(path.dirname(file), base + "-compiled.js");
    child.exec(path.resolve(__dirname, "./bin/nools") + " compile " + file + " -l ../../ -n " + base + "-compiled", function (err
, output) {
        if (!err) {
            grunt.file.write(out, output.toString());
        }
        counter(err);
...
```

#### <a name="apidoc.element.nools.extended.format"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>format (str, obj)](#apidoc.element.nools.extended.format)
- description and source-code
```javascript
function format(str, obj) {
    if (obj instanceof Array) {
        var i = 0, len = obj.length;
        //find the matches
        return str.replace(FORMAT_REGEX, function (m, format, type) {
            var replacer, ret;
            if (i < len) {
                replacer = obj[i++];
            } else {
                //we are out of things to replace with so
                //just return the match?
                return m;
            }
            if (m === "%s" || m === "%d" || m === "%D") {
                //fast path!
                ret = replacer + "";
            } else if (m === "%Z") {
                ret = replacer.toUTCString();
            } else if (m === "%j") {
                try {
                    ret = stringify(replacer);
                } catch (e) {
                    throw new Error("stringExtended.format : Unable to parse json from ", replacer);
                }
            } else {
                format = format.replace(/^\[|\]$/g, "");
                switch (type) {
                case "s":
                    ret = formatString(replacer, format);
                    break;
                case "d":
                    ret = formatNumber(replacer, format);
                    break;
                case "j":
                    ret = formatObject(replacer, format);
                    break;
                case "D":
                    ret = date.format(replacer, format);
                    break;
                case "Z":
                    ret = date.format(replacer, format, true);
                    break;
                }
            }
            return ret;
        });
    } else if (isHash(obj)) {
        return str.replace(INTERP_REGEX, function (m, format, value) {
            value = obj[value];
            if (!is.isUndefined(value)) {
                if (format) {
                    if (is.isString(value)) {
                        return formatString(value, format);
                    } else if (is.isNumber(value)) {
                        return formatNumber(value, format);
                    } else if (is.isDate(value)) {
                        return date.format(value, format);
                    } else if (is.isObject(value)) {
                        return formatObject(value, format);
                    }
                } else {
                    return "" + value;
                }
            }
            return m;
        });
    } else {
        var args = aSlice.call(arguments).slice(1);
        return format(str, args);
    }
}
```
- example usage
```shell
...
        hasConstraint: function (type) {
            return extd.some(this.constraints, function (c) {
                return c instanceof type;
            });
        },

        hashCode: function () {
            return [this.type, this.alias, extd.format("%j", this.conditions)].join(":");
        },

        toString: function () {
            return extd.format("%j", this.constraints);
        }
    }
}).as(exports, "ObjectPattern");
...
```

#### <a name="apidoc.element.nools.extended.getDaysInMonth"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>getDaysInMonth (dateObject)](#apidoc.element.nools.extended.getDaysInMonth)
- description and source-code
```javascript
getDaysInMonth = function (dateObject) {
    //	summary:
    //		Returns the number of days in the month used by dateObject
    var month = dateObject.getMonth();
    var days = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31];
    if (month === 1 && date.isLeapYear(dateObject)) {
        return 29;
    } // Number
    return days[month]; // Number
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.getTimezoneName"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>getTimezoneName (dateObject)](#apidoc.element.nools.extended.getTimezoneName)
- description and source-code
```javascript
function getTimezoneName(dateObject) {
    var str = dateObject.toString();
    var tz = '';
    var pos = str.indexOf('(');
    if (pos > -1) {
        tz = str.substring(++pos, str.indexOf(')'));
    }
    return tz; // String
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.has"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>has (obj, prop)](#apidoc.element.nools.extended.has)
- description and source-code
```javascript
function has(obj, prop) {
    return hasOwn.call(obj, prop);
}
```
- example usage
```shell
...
    this.rules = {};
    this.flow = flow;
    this.comparator = conflictResolution;
    this.setFocus(DEFAULT_AGENDA_GROUP).addAgendaGroup(DEFAULT_AGENDA_GROUP);
},

addAgendaGroup: function (groupName) {
    if (!extd.has(this.agendaGroups, groupName)) {
        this.agendaGroups[groupName] = new AVLTree({compare: this.comparator});
    }
},

getAgendaGroup: function (groupName) {
    return this.agendaGroups[groupName || DEFAULT_AGENDA_GROUP];
},
...
```

#### <a name="apidoc.element.nools.extended.hoursAgo"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>hoursAgo (val)](#apidoc.element.nools.extended.hoursAgo)
- description and source-code
```javascript
hoursAgo = function (val) {
    return date.add(new Date(), interval, -val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.hoursFromNow"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>hoursFromNow (val)](#apidoc.element.nools.extended.hoursFromNow)
- description and source-code
```javascript
hoursFromNow = function (val) {
    return date.add(new Date(), interval, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.inPlaceDifference"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>inPlaceDifference (a, b)](#apidoc.element.nools.extended.inPlaceDifference)
- description and source-code
```javascript
function inPlaceDifference(a, b) {
    var aOne, i = -1, l;
    l = a.length;
    while (++i < l) {
        aOne = a[i];
        if (indexOf(b, aOne) !== -1) {
            pSplice.call(a, i--, 1);
            l--;
        }
    }
    return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.inPlaceIntersection"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>inPlaceIntersection (a, b)](#apidoc.element.nools.extended.inPlaceIntersection)
- description and source-code
```javascript
function inPlaceIntersection(a, b) {
    var aOne, i = -1, l;
    l = a.length;
    while (++i < l) {
        aOne = a[i];
        if (indexOf(b, aOne) === -1) {
            pSplice.call(a, i--, 1);
            l--;
        }
    }
    return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.indexOf"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>indexOf (arr, searchElement, from)](#apidoc.element.nools.extended.indexOf)
- description and source-code
```javascript
function indexOf(arr, searchElement, from) {
    var index = (from || 0) - 1,
        length = arr.length;
    while (++index < length) {
        if (arr[index] === searchElement) {
            return index;
        }
    }
    return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.instanceOf"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>instanceOf (obj, clazz)](#apidoc.element.nools.extended.instanceOf)
- description and source-code
```javascript
function isInstanceOf(obj, clazz) {
    if (isFunction(clazz)) {
        return obj instanceof clazz;
    } else {
        return false;
    }
}
```
- example usage
```shell
...
type: "hash",

constructor: function (hash) {
    this._super([hash]);
},

equal: function (constraint) {
    return extd.instanceOf(constraint, this._static) && this.get("alias") === constraint.get("alias") && extd.deepEqual(this.constraint
, constraint.constraint);
},

"assert": function () {
    return true;
},

getters: {
...
```

#### <a name="apidoc.element.nools.extended.intersect"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>intersect ()](#apidoc.element.nools.extended.intersect)
- description and source-code
```javascript
function intersect() {
    var collect = [], sets, i = -1 , l;
    if (arguments.length > 1) {
        //assume we are intersections all the lists in the array
        sets = argsToArray(arguments);
    } else {
        sets = arguments[0];
    }
    if (isArray(sets)) {
        collect = sets[0];
        i = 0;
        l = sets.length;
        while (++i < l) {
            collect = intersection(collect, sets[i]);
        }
    }
    return removeDuplicates(collect);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.intersection"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>intersection (a, b)](#apidoc.element.nools.extended.intersection)
- description and source-code
```javascript
function intersection(a, b) {
    a = pSlice.call(a);
    var aOne, i = -1, l;
    l = a.length;
    while (++i < l) {
        aOne = a[i];
        if (indexOf(b, aOne) === -1) {
            pSplice.call(a, i--, 1);
            l--;
        }
    }
    return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.invoke"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>invoke (arr, func, args)](#apidoc.element.nools.extended.invoke)
- description and source-code
```javascript
function invoke(arr, func, args) {
    args = argsToArray(arguments, 2);
    return map(arr, function (item) {
        var exec = isString(func) ? item[func] : func;
        return exec.apply(item, args);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isArguments"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isArguments (object)](#apidoc.element.nools.extended.isArguments)
- description and source-code
```javascript
function _isArguments(object) {
    return toStr.call(object) === '[object Arguments]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isArray"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isArray ()](#apidoc.element.nools.extended.isArray)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isBoolean"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isBoolean (obj)](#apidoc.element.nools.extended.isBoolean)
- description and source-code
```javascript
function isBoolean(obj) {
    return obj === true || obj === false || toStr.call(obj) === "[object Boolean]";
}
```
- example usage
```shell
...
    instance: {
constructor: function (name, options, pattern, cb) {
    this.name = name;
    this.pattern = pattern;
    this.cb = cb;
    if (options.agendaGroup) {
        this.agendaGroup = options.agendaGroup;
        this.autoFocus = extd.isBoolean(options.autoFocus) ? options.autoFocus : false;
    }
    this.priority = options.priority || options.salience || 0;
},

fire: function (flow, match) {
    var ret = new Promise(), cb = this.cb;
    try {
...
```

#### <a name="apidoc.element.nools.extended.isDate"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isDate (obj)](#apidoc.element.nools.extended.isDate)
- description and source-code
```javascript
function isDate(obj) {
    return toStr.call(obj) === '[object Date]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isDefined"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isDefined (obj)](#apidoc.element.nools.extended.isDefined)
- description and source-code
```javascript
function isDefined(obj) {
    return !isUndefined(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isEmpty"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isEmpty (object)](#apidoc.element.nools.extended.isEmpty)
- description and source-code
```javascript
function isEmpty(object) {
    if (isArguments(object)) {
        return object.length === 0;
    } else if (isObject(object)) {
        return keys(object).length === 0;
    } else if (isString(object) || isArray(object)) {
        return object.length === 0;
    }
    return true;
}
```
- example usage
```shell
...
    if (agendaGroup) {
        this.addAgendaGroup(agendaGroup);
    }
},

isEmpty: function () {
    var agendaGroupStack = this.agendaGroupStack, changed = false;
    while (this.getFocusedAgenda().isEmpty() && this.getFocused() !== DEFAULT_AGENDA_GROUP) {
        agendaGroupStack.pop();
        changed = true;
    }
    if (changed) {
        this.emit("focused", this.getFocused());
    }
    return this.getFocusedAgenda().isEmpty();
...
```

#### <a name="apidoc.element.nools.extended.isEq"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isEq (obj, obj2)](#apidoc.element.nools.extended.isEq)
- description and source-code
```javascript
function isEq(obj, obj2) {
<span class="apidocCodeCommentSpan">    /*jshint eqeqeq:false*/
</span>    return obj == obj2;
}
```
- example usage
```shell
...
})
.switcher();

var getParamType = function getParamType(type, scope) {
scope = scope || {};
var getParamTypeSwitch = extd
    .switcher()
    .isEq("string", function () {
        return String;
    })
    .isEq("date", function () {
        return Date;
    })
    .isEq("array", function () {
        return Array;
...
```

#### <a name="apidoc.element.nools.extended.isFalse"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isFalse (obj)](#apidoc.element.nools.extended.isFalse)
- description and source-code
```javascript
function isFalse(obj) {
    return obj === false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isFunction"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isFunction (obj)](#apidoc.element.nools.extended.isFunction)
- description and source-code
```javascript
isFunction = function (obj) {
    return toStr.call(obj) === '[object Function]';
}
```
- example usage
```shell
...
    var t = scope[param];
    if (!t) {
        return getParamTypeSwitch(param.toLowerCase());
    } else {
        return t;
    }
})
.isFunction(function (func) {
    return func;
})
.deepEqual([], function () {
    return Array;
})
.def(function (param) {
    throw  new Error("invalid param type " + param);
...
```

#### <a name="apidoc.element.nools.extended.isGt"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isGt (obj, obj2)](#apidoc.element.nools.extended.isGt)
- description and source-code
```javascript
function isGt(obj, obj2) {
    return obj > obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isGte"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isGte (obj, obj2)](#apidoc.element.nools.extended.isGte)
- description and source-code
```javascript
function isGte(obj, obj2) {
    return obj >= obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isHash"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isHash (obj)](#apidoc.element.nools.extended.isHash)
- description and source-code
```javascript
function isHash(obj) {
    var ret = isObject(obj);
    return ret && obj.constructor === Object && !obj.nodeType && !obj.setInterval;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isIn"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isIn (obj, arr)](#apidoc.element.nools.extended.isIn)
- description and source-code
```javascript
function isIn(obj, arr) {
    if ((isArray(arr) && Array.prototype.indexOf) || isString(arr)) {
        return arr.indexOf(obj) > -1;
    } else if (isArray(arr)) {
        for (var i = 0, l = arr.length; i < l; i++) {
            if (isEq(obj, arr[i])) {
                return true;
            }
        }
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isLeapYear"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isLeapYear (dateObject, utc)](#apidoc.element.nools.extended.isLeapYear)
- description and source-code
```javascript
isLeapYear = function (dateObject, utc) {
    var year = dateObject[utc ? "getUTCFullYear" : "getFullYear"]();
    return (year % 400 === 0) || (year % 4 === 0 && year % 100 !== 0);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isLength"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isLength (obj, l)](#apidoc.element.nools.extended.isLength)
- description and source-code
```javascript
function length(obj, l) {
    if (has(obj, "length")) {
        return obj.length === l;
    }
    return false;
}
```
- example usage
```shell
...
.def(function (o) {
    throw new Error("invalid rule constraint option " + o);
})
.switcher();

var normailizeConstraint = extd
.switcher()
.isLength(1, function (c) {
    throw new Error("invalid rule constraint " + format("%j", [c]));
})
.isLength(2, function (c) {
    c.push("true");
    return c;
})
//handle case where c[2] is a hash rather than a constraint string
...
```

#### <a name="apidoc.element.nools.extended.isLike"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isLike (obj, reg)](#apidoc.element.nools.extended.isLike)
- description and source-code
```javascript
function isLike(obj, reg) {
    if (isString(reg)) {
        return ("" + obj).match(reg) !== null;
    } else if (isRegExp(reg)) {
        return reg.test(obj);
    }
    return false;
}
```
- example usage
```shell
...
};

var parseExtra = extd
.switcher()
.isUndefinedOrNull(function () {
    return null;
})
.isLike(/^from +/, function (s) {
    return {from: s.replace(/^from +/, "").replace(/^\s*|\s*$/g, "")};
})
.def(function (o) {
    throw new Error("invalid rule constraint option " + o);
})
.switcher();
...
```

#### <a name="apidoc.element.nools.extended.isLt"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isLt (obj, obj2)](#apidoc.element.nools.extended.isLt)
- description and source-code
```javascript
function isLt(obj, obj2) {
    return obj < obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isLte"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isLte (obj, obj2)](#apidoc.element.nools.extended.isLte)
- description and source-code
```javascript
function isLte(obj, obj2) {
    return obj <= obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isNeq"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isNeq (obj, obj2)](#apidoc.element.nools.extended.isNeq)
- description and source-code
```javascript
function isNeq(obj, obj2) {
<span class="apidocCodeCommentSpan">    /*jshint eqeqeq:false*/
</span>    return obj != obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isNotIn"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isNotIn (obj, arr)](#apidoc.element.nools.extended.isNotIn)
- description and source-code
```javascript
function isNotIn(obj, arr) {
    return !isIn(obj, arr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isNotLength"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isNotLength (obj, l)](#apidoc.element.nools.extended.isNotLength)
- description and source-code
```javascript
function notLength(obj, l) {
    if (has(obj, "length")) {
        return obj.length !== l;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isNotLike"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isNotLike (obj, reg)](#apidoc.element.nools.extended.isNotLike)
- description and source-code
```javascript
function isNotLike(obj, reg) {
    return !isLike(obj, reg);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isNotNull"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isNotNull (obj)](#apidoc.element.nools.extended.isNotNull)
- description and source-code
```javascript
function isNotNull(obj) {
    return !isNull(obj);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isNull"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isNull (obj)](#apidoc.element.nools.extended.isNull)
- description and source-code
```javascript
function isNull(obj) {
    return obj === null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isNumber"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isNumber (obj)](#apidoc.element.nools.extended.isNumber)
- description and source-code
```javascript
function isNumber(obj) {
    return toStr.call(obj) === '[object Number]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isObject"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isObject (obj)](#apidoc.element.nools.extended.isObject)
- description and source-code
```javascript
function isObject(obj) {
    var undef;
    return obj !== null && typeof obj === "object";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isPromiseLike"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isPromiseLike (obj)](#apidoc.element.nools.extended.isPromiseLike)
- description and source-code
```javascript
function isPromiseLike(obj) {
    return !isUndefinedOrNull(obj) && (isFunction(obj.then));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isRegExp"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isRegExp (obj)](#apidoc.element.nools.extended.isRegExp)
- description and source-code
```javascript
function isRegExp(obj) {
    return toStr.call(obj) === '[object RegExp]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isSeq"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isSeq (obj, obj2)](#apidoc.element.nools.extended.isSeq)
- description and source-code
```javascript
function isSeq(obj, obj2) {
    return obj === obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isSneq"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isSneq (obj, obj2)](#apidoc.element.nools.extended.isSneq)
- description and source-code
```javascript
function isSneq(obj, obj2) {
    return obj !== obj2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isString"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isString (obj)](#apidoc.element.nools.extended.isString)
- description and source-code
```javascript
function isString(obj) {
    return toStr.call(obj) === '[object String]';
}
```
- example usage
```shell
...
    .def(function (param) {
        throw new TypeError("invalid param type " + param);
    })
    .switcher();

var _getParamType = extd
    .switcher()
    .isString(function (param) {
        var t = scope[param];
        if (!t) {
            return getParamTypeSwitch(param.toLowerCase());
        } else {
            return t;
        }
    })
...
```

#### <a name="apidoc.element.nools.extended.isTrue"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isTrue (obj)](#apidoc.element.nools.extended.isTrue)
- description and source-code
```javascript
function isTrue(obj) {
    return obj === true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isUndefined"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isUndefined (obj)](#apidoc.element.nools.extended.isUndefined)
- description and source-code
```javascript
function isUndefined(obj) {
    return typeof obj === 'undefined';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.isUndefinedOrNull"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isUndefinedOrNull (obj)](#apidoc.element.nools.extended.isUndefinedOrNull)
- description and source-code
```javascript
function isUndefinedOrNull(obj) {
    return isUndefined(obj) || isNull(obj);
}
```
- example usage
```shell
...
    return constraint;
}
return parser.parseConstraint(constraint);
};

var parseExtra = extd
.switcher()
.isUndefinedOrNull(function () {
    return null;
})
.isLike(/^from +/, function (s) {
    return {from: s.replace(/^from +/, "").replace(/^\s*|\s*$/g, "")};
})
.def(function (o) {
    throw new Error("invalid rule constraint option " + o);
...
```

#### <a name="apidoc.element.nools.extended.isWeekend"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>isWeekend (dateObject, utc)](#apidoc.element.nools.extended.isWeekend)
- description and source-code
```javascript
isWeekend = function (dateObject, utc) {
    // summary:
    //	Determines if the date falls on a weekend, according to local custom.
    var day = (dateObject || new Date())[utc ? "getUTCDay" : "getDay"]();
    return day === 0 || day === 6;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.lastIndexOf"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>lastIndexOf (arr, searchElement, from)](#apidoc.element.nools.extended.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf(arr, searchElement, from) {
    if (!isArray(arr)) {
        throw new TypeError();
    }

    var t = Object(arr);
    var len = t.length >>> 0;
    if (len === 0) {
        return -1;
    }

    var n = len;
    if (arguments.length > 2) {
        n = Number(arguments[2]);
        if (n !== n) {
            n = 0;
        } else if (n !== 0 && n !== (1 / 0) && n !== -(1 / 0)) {
            n = (n > 0 || -1) * floor(abs(n));
        }
    }

    var k = n >= 0 ? mathMin(n, len - 1) : len - abs(n);

    for (; k >= 0; k--) {
        if (k in t && t[k] === searchElement) {
            return k;
        }
    }
    return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.map"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>map (arr, iterator, scope)](#apidoc.element.nools.extended.map)
- description and source-code
```javascript
function map(arr, iterator, scope) {
    if (arr && arrayMap && arrayMap === arr.map) {
        return arr.map(iterator, scope);
    }
    if (!isArray(arr) || typeof iterator !== "function") {
        throw new TypeError();
    }

    var t = Object(arr);
    var len = t.length >>> 0;
    var res = [];
    for (var i = 0; i < len; i++) {
        if (i in t) {
            res.push(iterator.call(scope, t[i], i, t));
        }
    }
    return res;
}
```
- example usage
```shell
...
    some = extd.some,
    indexOf = extd.indexOf,
    isNumber = extd.isNumber,
    removeDups = extd.removeDuplicates,
    atoms = require("./constraint");

function getProps(val) {
    return extd(val).map(function mapper(val) {
        return isArray(val) ? isArray(val[0]) ? getProps(val).value() : val.reverse().join(".") : val;
    }).flatten().filter(function (v) {
        return !!v;
    });
}

var definedFuncs = {
...
```

#### <a name="apidoc.element.nools.extended.max"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>max (arr, cmp)](#apidoc.element.nools.extended.max)
- description and source-code
```javascript
function max(arr, cmp) {
    return _sort(arr, cmp)[arr.length - 1];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.merge"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>merge (obj)](#apidoc.element.nools.extended.merge)
- description and source-code
```javascript
function merge(obj) {
    if (!obj) {
        obj = {};
    }
    for (var i = 1, l = arguments.length; i < l; i++) {
        _merge(obj, arguments[i]);
    }
    return obj; // Object
}
```
- example usage
```shell
...
    } else {
        return this.match.isMatch;
    }
    return this;
},

mergeMatch: function (merge) {
    var match = this.match = this.match.merge(merge);
    this.factHash = match.factHash;
    this.hashCode = match.hashCode;
    this.aliases = match.aliases;
    return this;
},

clone: function (fact, paths, match) {
...
```

#### <a name="apidoc.element.nools.extended.min"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>min (arr, cmp)](#apidoc.element.nools.extended.min)
- description and source-code
```javascript
function min(arr, cmp) {
    return _sort(arr, cmp)[0];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.minutesAgo"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>minutesAgo (val)](#apidoc.element.nools.extended.minutesAgo)
- description and source-code
```javascript
minutesAgo = function (val) {
    return date.add(new Date(), interval, -val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.minutesFromNow"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>minutesFromNow (val)](#apidoc.element.nools.extended.minutesFromNow)
- description and source-code
```javascript
minutesFromNow = function (val) {
    return date.add(new Date(), interval, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.monthsAgo"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>monthsAgo (val)](#apidoc.element.nools.extended.monthsAgo)
- description and source-code
```javascript
monthsAgo = function (val) {
    return date.add(new Date(), interval, -val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.monthsFromNow"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>monthsFromNow (val)](#apidoc.element.nools.extended.monthsFromNow)
- description and source-code
```javascript
monthsFromNow = function (val) {
    return date.add(new Date(), interval, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.multiply"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>multiply (str, times)](#apidoc.element.nools.extended.multiply)
- description and source-code
```javascript
function multiply(str, times) {
    var ret = [];
    if (times) {
        for (var i = 0; i < times; i++) {
            ret.push(str);
        }
    }
    return ret.join("");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.notContains"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>notContains (arr, obj)](#apidoc.element.nools.extended.notContains)
- description and source-code
```javascript
function notContains(arr, obj) {
    return !isIn(obj, arr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.notContainsAt"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>notContainsAt (arr, obj, index)](#apidoc.element.nools.extended.notContainsAt)
- description and source-code
```javascript
function notContainsAt(arr, obj, index) {
    if (isArray(arr)) {
        return !isEq(arr[index], obj);
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.notHas"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>notHas (obj, prop)](#apidoc.element.nools.extended.notHas)
- description and source-code
```javascript
function notHas(obj, prop) {
    return !has(obj, prop);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.omit"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>omit (hash, omitted)](#apidoc.element.nools.extended.omit)
- description and source-code
```javascript
function omit(hash, omitted) {
    if (!isHash(hash)) {
        throw new TypeError();
    }
    if (isString(omitted)) {
        omitted = [omitted];
    }
    var objKeys = difference(keys(hash), omitted), key, ret = {};
    for (var i = 0, len = objKeys.length; i < len; ++i) {
        key = objKeys[i];
        ret[key] = hash[key];
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.pad"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>pad (string, length, ch, end)](#apidoc.element.nools.extended.pad)
- description and source-code
```javascript
function pad(string, length, ch, end) {
    string = "" + string; //check for numbers
    ch = ch || " ";
    var strLen = string.length;
    while (strLen < length) {
        if (end) {
            string += ch;
        } else {
            string = ch + string;
        }
        strLen++;
    }
    return string;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.parseDate"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>parseDate (dateStr, format)](#apidoc.element.nools.extended.parseDate)
- description and source-code
```javascript
parseDate = function (dateStr, format) {
    if (!format) {
        throw new Error('format required when calling dateExtender.parse');
    }
    var tokens = [], regexp = buildDateEXP(format, tokens),
        re = new RegExp("^" + regexp + "$", "i"),
        match = re.exec(dateStr);
    if (!match) {
        return null;
    } // null
    var result = [1970, 0, 1, 0, 0, 0, 0], // will get converted to a Date at the end
        amPm = "",
        valid = every(match, function (v, i) {
            if (i) {
                var token = tokens[i - 1];
                var l = token.length, type = token.charAt(0);
                if (type === 'y') {
                    if (v < 100) {
                        v = parseInt(v, 10);
                        //choose century to apply, according to a sliding window
                        //of 80 years before and 20 years after present year
                        var year = '' + new Date().getFullYear(),
                            century = year.substring(0, 2) * 100,
                            cutoff = min(year.substring(2, 4) + 20, 99);
                        result[0] = (v < cutoff) ? century + v : century - 100 + v;
                    } else {
                        result[0] = v;
                    }
                } else if (type === "M") {
                    if (l > 2) {
                        var months = monthNames, j, k;
                        if (l === 3) {
                            months = monthAbbr;
                        }
                        //Tolerate abbreviating period in month part
                        //Case-insensitive comparison
                        v = v.replace(".", "").toLowerCase();
                        var contains = false;
                        for (j = 0, k = months.length; j < k && !contains; j++) {
                            var s = months[j].replace(".", "").toLocaleLowerCase();
                            if (s === v) {
                                v = j;
                                contains = true;
                            }
                        }
                        if (!contains) {
                            return false;
                        }
                    } else {
                        v--;
                    }
                    result[1] = v;
                } else if (type === "E" || type === "e") {
                    var days = dayNames;
                    if (l === 3) {
                        days = dayAbbr;
                    }
                    //Case-insensitive comparison
                    v = v.toLowerCase();
                    days = array.map(days, function (d) {
                        return d.toLowerCase();
                    });
                    var d = array.indexOf(days, v);
                    if (d === -1) {
                        v = parseInt(v, 10);
                        if (isNaN(v) || v > days.length) {
                            return false;
                        }
                    } else {
                        v = d;
                    }
                } else if (type === 'D' || type === "d") {
                    if (type === "D") {
                        result[1] = 0;
                    }
                    result[2] = v;
                } else if (type === "a") {
                    var am = "am";
                    var pm = "pm";
                    var period = /\./g;
                    v = v.replace(period, '').toLowerCase();
                    // we might not have seen the hours field yet, so store the state and apply hour change later
                    amPm = (v === pm) ? 'p' : (v === am) ? 'a' : '';
                } else if (type === "k" || type === "h" || type === "H" || type === "K") {
                    if (type === "k" && (+v) === 24) {
                        v = 0;
                    }
                    result[3] = v;
                } else if (type === "m") {
                    result[4] = v;
                } else if (type === "s") {
                    result[5] = v;
                } else if (type === "S") { ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.partial"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>partial (method, args)](#apidoc.element.nools.extended.partial)
- description and source-code
```javascript
function partial(method, args) {
    args = argsToArray(arguments, 1);
    if (!isString(method) && !isFunction(method)) {
        throw new Error(method + " must be the name of a property or function to execute");
    }
    if (isString(method)) {
        return function () {
            var func = this[method];
            if (isFunction(func)) {
                var scopeArgs = args.concat(argsToArray(arguments));
                return spreadArgs(func, scopeArgs, this);
            } else {
                return func;
            }
        };
    } else {
        return function () {
            var scopeArgs = args.concat(argsToArray(arguments));
            return spreadArgs(method, scopeArgs, this);
        };
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.permutations"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>permutations (arr, length)](#apidoc.element.nools.extended.permutations)
- description and source-code
```javascript
function permutations(arr, length) {
    var ret = [];
    if (isArray(arr)) {
        var copy = arr.slice(0);
        if (typeof length !== "number") {
            length = arr.length;
        }
        if (!length) {
            ret = [
                []
            ];
        } else if (length <= arr.length) {
            ret = reduce(arr, function (a, b, i) {
                var ret;
                if (length > 1) {
                    ret = permute(b, rotate(copy, i).slice(1), length);
                } else {
                    ret = [
                        [b]
                    ];
                }
                return a.concat(ret);
            }, []);
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.pluck"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>pluck (arr, prop)](#apidoc.element.nools.extended.pluck)
- description and source-code
```javascript
function pluck(arr, prop) {
    prop = prop.split(".");
    var result = arr.slice(0);
    forEach(prop, function (prop) {
        var exec = prop.match(/(\w+)\(\)$/);
        result = map(result, function (item) {
            return exec ? item[exec[1]]() : item[prop];
        });
    });
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.plucker"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>plucker (prop)](#apidoc.element.nools.extended.plucker)
- description and source-code
```javascript
function plucker(prop) {
    prop = prop.split(".");
    if (prop.length === 1) {
        return plucked(prop[0]);
    } else {
        var pluckers = map(prop, function (prop) {
            return plucked(prop);
        });
        var l = pluckers.length;
        return function (item) {
            var i = -1, res = item;
            while (++i < l) {
                res = pluckers[i](res);
            }
            return res;
        };
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.powerSet"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>powerSet (arr)](#apidoc.element.nools.extended.powerSet)
- description and source-code
```javascript
function powerSet(arr) {
    var ret = [];
    if (isArray(arr) && arr.length) {
        ret = reduce(arr, function (a, b) {
            var ret = map(a, function (c) {
                return c.concat(b);
            });
            return a.concat(ret);
        }, [
            []
        ]);
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.promise"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>promise ()](#apidoc.element.nools.extended.promise)
- description and source-code
```javascript
function createPromise() {
    return new Promise();
}
```
- example usage
```shell
...
    },

    rule: function (rule) {
        this.rootNode.assertRule(rule);
    },

    matchUntilHalt: function (cb) {
        return (this.executionStrategy = new ExecutionStragegy(this, true)).execute().classic(cb).promise();
    },

    match: function (cb) {
        return (this.executionStrategy = new ExecutionStragegy(this)).execute().classic(cb).promise();
    }

}
...
```

#### <a name="apidoc.element.nools.extended.reduce"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>reduce (arr, accumulator, curr)](#apidoc.element.nools.extended.reduce)
- description and source-code
```javascript
function reduce(arr, accumulator, curr) {
    var initial = arguments.length > 2;
    if (arr && arrayReduce && arrayReduce === arr.reduce) {
        return initial ? arr.reduce(accumulator, curr) : arr.reduce(accumulator);
    }
    if (!isArray(arr) || typeof accumulator !== "function") {
        throw new TypeError();
    }
    var i = 0, l = arr.length >> 0;
    if (arguments.length < 3) {
        if (l === 0) {
            throw new TypeError("Array length is 0 and no second argument");
        }
        curr = arr[0];
        i = 1; // start accumulating at the second element
    } else {
        curr = arguments[2];
    }
    while (i < l) {
        if (i in arr) {
            curr = accumulator.call(undefined, curr, arr[i], i, arr);
        }
        ++i;
    }
    return curr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.reduceRight"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>reduceRight (arr, accumulator, curr)](#apidoc.element.nools.extended.reduceRight)
- description and source-code
```javascript
function reduceRight(arr, accumulator, curr) {
    var initial = arguments.length > 2;
    if (arr && arrayReduceRight && arrayReduceRight === arr.reduceRight) {
        return initial ? arr.reduceRight(accumulator, curr) : arr.reduceRight(accumulator);
    }
    if (!isArray(arr) || typeof accumulator !== "function") {
        throw new TypeError();
    }

    var t = Object(arr);
    var len = t.length >>> 0;

    // no value to return if no initial value, empty array
    if (len === 0 && arguments.length === 2) {
        throw new TypeError();
    }

    var k = len - 1;
    if (arguments.length >= 3) {
        curr = arguments[2];
    } else {
        do {
            if (k in arr) {
                curr = arr[k--];
                break;
            }
        }
        while (true);
    }
    while (k >= 0) {
        if (k in t) {
            curr = accumulator.call(undefined, curr, t[k], k, t);
        }
        k--;
    }
    return curr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.register"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>register (alias, extendWith)](#apidoc.element.nools.extended.register)
- description and source-code
```javascript
function register(alias, extendWith) {
    if (!extendWith) {
        extendWith = alias;
        alias = null;
    }
    var type = typeof extendWith;
    if (alias) {
        extended[alias] = extendWith;
    } else if (extendWith && type === "function") {
        extended.extend(extendWith);
    } else if (type === "object") {
        extended.expose(extendWith);
    } else {
        throw new TypeError("extended.register must be called with an extender function");
    }
    return extended;
}
```
- example usage
```shell
...


function union(arr1, arr2) {
return unique(arr1.concat(arr2));
}

module.exports = require("extended")()
.register(require("date-extended"))
.register(arr)
.register(require("object-extended"))
.register(require("string-extended"))
.register(require("promise-extended"))
.register(require("function-extended"))
.register(require("is-extended"))
.register("intersection", intersection)
...
```

#### <a name="apidoc.element.nools.extended.reject"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>reject (val)](#apidoc.element.nools.extended.reject)
- description and source-code
```javascript
function createRejected(val) {
    return createPromise().errback(val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.removeDuplicates"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>removeDuplicates (arr)](#apidoc.element.nools.extended.removeDuplicates)
- description and source-code
```javascript
function removeDuplicates(arr) {
    var ret = [], i = -1, l, retLength = 0;
    if (arr) {
        l = arr.length;
        while (++i < l) {
            var item = arr[i];
            if (indexOf(ret, item) === -1) {
                ret[retLength++] = item;
            }
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.resolve"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>resolve (val)](#apidoc.element.nools.extended.resolve)
- description and source-code
```javascript
function createResolved(val) {
    return createPromise().callback(val);
}
```
- example usage
```shell
...
            done();
        }
    }
}

files.forEach(function (file) {
    var base = path.basename(file, ".nools"),
        out = path.resolve(path.dirname(file), base + "-compiled.js");
    child.exec(path.resolve(__dirname, "./bin/nools") + " compile " + file + " -l ../../ -n " + base + "-compiled", function (err
, output) {
        if (!err) {
            grunt.file.write(out, output.toString());
        }
        counter(err);
    });
});
...
```

#### <a name="apidoc.element.nools.extended.rotate"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>rotate (arr, numberOfTimes)](#apidoc.element.nools.extended.rotate)
- description and source-code
```javascript
function rotate(arr, numberOfTimes) {
    var ret = arr.slice();
    if (typeof numberOfTimes !== "number") {
        numberOfTimes = 1;
    }
    if (numberOfTimes && isArray(arr)) {
        if (numberOfTimes > 0) {
            ret.push(ret.shift());
            numberOfTimes--;
        } else {
            ret.unshift(ret.pop());
            numberOfTimes++;
        }
        return rotate(ret, numberOfTimes);
    } else {
        return ret;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.secondsAgo"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>secondsAgo (val)](#apidoc.element.nools.extended.secondsAgo)
- description and source-code
```javascript
secondsAgo = function (val) {
    return date.add(new Date(), interval, -val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.secondsFromNow"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>secondsFromNow (val)](#apidoc.element.nools.extended.secondsFromNow)
- description and source-code
```javascript
secondsFromNow = function (val) {
    return date.add(new Date(), interval, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.serial"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>serial (list)](#apidoc.element.nools.extended.serial)
- description and source-code
```javascript
function serial(list) {
    if (isArray(list)) {
        return callNext(list, [], false);
    } else {
        throw new Error("When calling promise.serial the first argument must be an array");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.some"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>some (arr, iterator, scope)](#apidoc.element.nools.extended.some)
- description and source-code
```javascript
function some(arr, iterator, scope) {
    if (arr && arraySome && arraySome === arr.some) {
        return arr.some(iterator, scope);
    }
    if (!isArray(arr) || typeof iterator !== "function") {
        throw new TypeError();
    }
    var t = Object(arr);
    var len = t.length >>> 0;
    for (var i = 0; i < len; i++) {
        if (i in t && iterator.call(scope, t[i], i, t)) {
            return true;
        }
    }
    return false;
}
```
- example usage
```shell
...
            specificity++;
        }
    }
    return specificity;
},

hasConstraint: function (type) {
    return extd.some(this.constraints, function (c) {
        return c instanceof type;
    });
},

hashCode: function () {
    return [this.type, this.alias, extd.format("%j", this.conditions)].join(":");
},
...
```

#### <a name="apidoc.element.nools.extended.sort"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>sort (arr, cmp)](#apidoc.element.nools.extended.sort)
- description and source-code
```javascript
function sort(arr, cmp) {
    return _sort(arr, cmp);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.style"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>style (str, options)](#apidoc.element.nools.extended.style)
- description and source-code
```javascript
function style(str, options) {
    var ret, i, l;
    if (options) {
        if (is.isArray(str)) {
            ret = [];
            for (i = 0, l = str.length; i < l; i++) {
                ret.push(style(str[i], options));
            }
        } else if (options instanceof Array) {
            ret = str;
            for (i = 0, l = options.length; i < l; i++) {
                ret = style(ret, options[i]);
            }
        } else if (options in styles) {
            ret = '\x1B[' + styles[options] + 'm' + str + '\x1B[0m';
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.sum"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>sum (array)](#apidoc.element.nools.extended.sum)
- description and source-code
```javascript
function sum(array) {
    array = array || [];
    if (array.length) {
        return reduce(array, function (a, b) {
            return a + b;
        });
    } else {
        return 0;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.switcher"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>switcher (obj)](#apidoc.element.nools.extended.switcher)
- description and source-code
```javascript
function _extender(obj) {
    var ret = obj, i, l;
    if (!(obj instanceof Base)) {
        var OurBase = Base;
        for (i = 0, l = defined.length; i < l; i++) {
            var definer = defined[i];
            if (definer[0](obj)) {
                OurBase = OurBase.extend({instance: definer[1]});
            }
        }
        ret = new OurBase(obj);
        ret["__extender__"] = _extender;
    }
    return ret;
}
```
- example usage
```shell
...
    // No parsing is needed for constraint functions
    return constraint;
}
return parser.parseConstraint(constraint);
};

var parseExtra = extd
.switcher()
.isUndefinedOrNull(function () {
    return null;
})
.isLike(/^from +/, function (s) {
    return {from: s.replace(/^from +/, "").replace(/^\s*|\s*$/g, "")};
})
.def(function (o) {
...
```

#### <a name="apidoc.element.nools.extended.tester"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>tester (obj)](#apidoc.element.nools.extended.tester)
- description and source-code
```javascript
function _extender(obj) {
    var ret = obj, i, l;
    if (!(obj instanceof Base)) {
        var OurBase = Base;
        for (i = 0, l = defined.length; i < l; i++) {
            var definer = defined[i];
            if (definer[0](obj)) {
                OurBase = OurBase.extend({instance: definer[1]});
            }
        }
        ret = new OurBase(obj);
        ret["__extender__"] = _extender;
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.toArray"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>toArray (testStr, delim)](#apidoc.element.nools.extended.toArray)
- description and source-code
```javascript
function toArray(testStr, delim) {
    var ret = [];
    if (testStr) {
        if (testStr.indexOf(delim) > 0) {
            ret = testStr.replace(/\s+/g, "").split(delim);
        }
        else {
            ret.push(testStr);
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.transpose"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>transpose (arr)](#apidoc.element.nools.extended.transpose)
- description and source-code
```javascript
function transpose(arr) {
    var ret = [];
    if (isArray(arr) && arr.length) {
        var last;
        forEach(arr, function (a) {
            if (isArray(a) && (!last || a.length === last.length)) {
                forEach(a, function (b, i) {
                    if (!ret[i]) {
                        ret[i] = [];
                    }
                    ret[i].push(b);
                });
                last = a;
            }
        });
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.trim"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>trim (str)](#apidoc.element.nools.extended.trim)
- description and source-code
```javascript
function trim(str) {
    return str.replace(/^\s*|\s*$/g, "");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.trimLeft"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>trimLeft (str)](#apidoc.element.nools.extended.trimLeft)
- description and source-code
```javascript
function trimLeft(str) {
    return str.replace(/^\s*/, "");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.trimRight"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>trimRight (str)](#apidoc.element.nools.extended.trimRight)
- description and source-code
```javascript
function trimRight(str) {
    return str.replace(/\s*$/, "");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.truncate"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>truncate (string, length, end)](#apidoc.element.nools.extended.truncate)
- description and source-code
```javascript
function truncate(string, length, end) {
    var ret = string;
    if (is.isString(ret)) {
        if (string.length > length) {
            if (end) {
                var l = string.length;
                ret = string.substring(l - length, l);
            } else {
                ret = string.substring(0, length);
            }
        }
    } else {
        ret = truncate("" + ret, length);
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.union"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>union ()](#apidoc.element.nools.extended.union)
- description and source-code
```javascript
function union() {
    var ret = [];
    var arrs = argsToArray(arguments);
    if (arrs.length > 1) {
        for (var i = 0, l = arrs.length; i < l; i++) {
            ret = ret.concat(arrs[i]);
        }
        ret = removeDuplicates(ret);
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.unionArr"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>unionArr (arr1, arr2)](#apidoc.element.nools.extended.unionArr)
- description and source-code
```javascript
function union(arr1, arr2) {
    return unique(arr1.concat(arr2));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.unique"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>unique (arr)](#apidoc.element.nools.extended.unique)
- description and source-code
```javascript
function unique(arr) {
    return removeDuplicates(arr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.valuesAt"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>valuesAt (arr, indexes)](#apidoc.element.nools.extended.valuesAt)
- description and source-code
```javascript
function valuesAt(arr, indexes) {
    var ret = [];
    indexes = argsToArray(arguments);
    arr = indexes.shift();
    if (isArray(arr) && indexes.length) {
        for (var i = 0, l = indexes.length; i < l; i++) {
            ret.push(arr[indexes[i]] || null);
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.wait"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>wait (args, fn)](#apidoc.element.nools.extended.wait)
- description and source-code
```javascript
function wait(args, fn) {
    args = argsToArray(arguments);
    var resolved = false;
    fn = args.pop();
    var p = when(args);
    return function waiter() {
        if (!resolved) {
            args = arguments;
            return p.then(bind(this, function doneWaiting() {
                resolved = true;
                return fn.apply(this, args);
            }));
        } else {
            return when(fn.apply(this, arguments));
        }
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.when"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>when (args)](#apidoc.element.nools.extended.when)
- description and source-code
```javascript
function when(args) {
    var p;
    args = argsToArray(arguments);
    if (!args.length) {
        p = new Promise().callback(args).promise();
    } else if (args.length === 1) {
        args = args.pop();
        if (isPromiseLike(args)) {
            if (args.addCallback && args.addErrback) {
                p = new Promise();
                args.addCallback(p.callback);
                args.addErrback(p.errback);
            } else {
                p = wrapThenPromise(args);
            }
        } else if (isArray(args) && array.every(args, isPromiseLike)) {
            p = new PromiseList(args, true).promise();
        } else {
            p = new Promise().callback(args);
        }
    } else {
        p = new PromiseList(array.map(args, function (a) {
            return when(a);
        }), true).promise();
    }
    return p;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.wrap"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>wrap (fn, scope)](#apidoc.element.nools.extended.wrap)
- description and source-code
```javascript
function wrap(fn, scope) {
    return function _wrap() {
        var ret = new Promise();
        var args = argsToArray(arguments);
        args.push(ret.resolve);
        fn.apply(scope || this, args);
        return ret.promise();
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.yearsAgo"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>yearsAgo (val)](#apidoc.element.nools.extended.yearsAgo)
- description and source-code
```javascript
yearsAgo = function (val) {
    return date.add(new Date(), interval, -val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.yearsFromNow"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>yearsFromNow (val)](#apidoc.element.nools.extended.yearsFromNow)
- description and source-code
```javascript
yearsFromNow = function (val) {
    return date.add(new Date(), interval, val);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.extended.zip"></a>[function <span class="apidocSignatureSpan">nools.extended.</span>zip ()](#apidoc.element.nools.extended.zip)
- description and source-code
```javascript
function zip() {
    var ret = [];
    var arrs = argsToArray(arguments);
    if (arrs.length > 1) {
        var arr1 = arrs.shift();
        if (isArray(arr1)) {
            ret = reduce(arr1, function (a, b, i) {
                var curr = [b];
                for (var j = 0; j < arrs.length; j++) {
                    var currArr = arrs[j];
                    if (isArray(currArr) && !is.isUndefined(currArr[i])) {
                        curr.push(currArr[i]);
                    } else {
                        curr.push(null);
                    }
                }
                a.push(curr);
                return a;
            }, []);
        }
    }
    return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.flow"></a>[module nools.flow](#apidoc.module.nools.flow)

#### <a name="apidoc.element.nools.flow.flow"></a>[function <span class="apidocSignatureSpan">nools.</span>flow (name, cb)](#apidoc.element.nools.flow.flow)
- description and source-code
```javascript
flow = function (name, cb) {
    return new FlowContainer(name, cb);
}
```
- example usage
```shell
...
'''javascript
var nools = require("nools");

var Message = function (message) {
this.text = message;
};

var flow = nools.flow("Hello World", function (flow) {

//find any message that is exactly hello world
flow.rule("Hello", [Message, "m", "m.text =~ /^hello\\sworld$/"], function (facts) {
    facts.m.text = facts.m.text + " goodbye";
    this.modify(facts.m);
});
...
```

#### <a name="apidoc.element.nools.flow._f"></a>[function <span class="apidocSignatureSpan">nools.flow.</span>_f (name, cb)](#apidoc.element.nools.flow._f)
- description and source-code
```javascript
_f = function (name, cb) {
    return new FlowContainer(name, cb);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.flow.prototype"></a>[module nools.flow.prototype](#apidoc.module.nools.flow.prototype)

#### <a name="apidoc.element.nools.flow.prototype._getSuper"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>_getSuper ()](#apidoc.element.nools.flow.prototype._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.flow.prototype._static"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>_static ()](#apidoc.element.nools.flow.prototype._static)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
...
    }

},

merge: function (that) {
    var ret = this;
    if (that instanceof ReferenceConstraint) {
        ret = new this._static([this.constraint, that.constraint, "and"], merge({}, this._options, this._options));
        ret._alias = this._alias || that._alias;
        ret.vars = this.vars.concat(that.vars);
    }
    return ret;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.flow.prototype._super"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>_super (args, a)](#apidoc.element.nools.flow.prototype._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.flow.prototype.assert"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>assert (fact)](#apidoc.element.nools.flow.prototype.assert)
- description and source-code
```javascript
assert = function (fact) {
    this.rootNode.assertFact(this.workingMemory.assertFact(fact));
    this.emit("assert", fact);
    return fact;
}
```
- example usage
```shell
...

<a name="facts-assert"></a>
### Assert

To add facts to the session use 'assert' method.

'''javascript
session.assert(new Message("hello"));
session.assert(new Message("hello world"));
session.assert(new Message("goodbye"));
'''

As a convenience any object passed into **getSession** will also be asserted.

**Note** assert is typically used pre engine execution and during the execution of the rules.
...
```

#### <a name="apidoc.element.nools.flow.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>constructor (name, conflictResolutionStrategy)](#apidoc.element.nools.flow.prototype.constructor)
- description and source-code
```javascript
constructor = function (name, conflictResolutionStrategy) {
    this.env = null;
    this.name = name;
    this.__rules = {};
    this.conflictResolutionStrategy = conflictResolutionStrategy;
    this.workingMemory = new WorkingMemory();
    this.agenda = new AgendaTree(this, conflictResolutionStrategy);
    this.agenda.on("fire", bind(this, "emit", "fire"));
    this.agenda.on("focused", bind(this, "emit", "focused"));
    this.rootNode = new nodes.RootNode(this.workingMemory, this.agenda);
    extd.bindAll(this, "halt", "assert", "retract", "modify", "focus",
      "emit", "getFacts", "getFact");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.flow.prototype.containsRule"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>containsRule (name)](#apidoc.element.nools.flow.prototype.containsRule)
- description and source-code
```javascript
containsRule = function (name) {
    return this.rootNode.containsRule(name);
}
```
- example usage
```shell
...
},

print: function () {
    this.rootNode.print();
},

containsRule: function (name) {
    return this.rootNode.containsRule(name);
},

rule: function (rule) {
    this.rootNode.assertRule(rule);
},

matchUntilHalt: function (cb) {
...
```

#### <a name="apidoc.element.nools.flow.prototype.dispose"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>dispose ()](#apidoc.element.nools.flow.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
    this.workingMemory.dispose();
    this.agenda.dispose();
    this.rootNode.dispose();
}
```
- example usage
```shell
...
<a name="disposing"></a>
## Disposing of the session

When working with a lot of facts it is wise to call the 'dispose' method which will purge the current session of
all facts, this will help prevent the process from growing a large memory footprint.

'''javascript
session.dispose();
'''

<a name="removing-flow"></a>
# Removing a flow

To remove a defined flow from 'nools' use the 'deleteFlow' function.
...
```

#### <a name="apidoc.element.nools.flow.prototype.focus"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>focus (focused)](#apidoc.element.nools.flow.prototype.focus)
- description and source-code
```javascript
focus = function (focused) {
    this.agenda.setFocus(focused);
    return this;
}
```
- example usage
```shell
...

When running your rules and you want a particular agenda group to run you must call 'focus' on the session of the flow and specify
 the 'agenda-group' to add to the stack.

'''
//assuming a flow with the rules specified above.
var fired = [];
flow.getSession(new Message("hello"))
    .focus("ag1")
    .on("fire", function (ruleName) {
        fired.push(ruleName);
    })
    .match(function () {
        console.log(fired);  //[ 'Hello World' ]
    });
'''
...
```

#### <a name="apidoc.element.nools.flow.prototype.getFact"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>getFact (Type)](#apidoc.element.nools.flow.prototype.getFact)
- description and source-code
```javascript
getFact = function (Type) {
    var ret;
    if (Type) {
        ret = this.workingMemory.getFactsByType(Type);
    } else {
        ret = this.workingMemory.getFacts();
    }
    return ret && ret[0];
}
```
- example usage
```shell
...
    this.rootNode.assertFact(this.workingMemory.assertFact(fact));
    this.emit("assert", fact);
    return fact;
},

// This method is called to remove an existing fact from working memory
retract: function (fact) {
    //fact = this.workingMemory.getFact(fact);
    this.rootNode.retractFact(this.workingMemory.retractFact(fact));
    this.emit("retract", fact);
    return fact;
},

// This method is called to alter an existing fact.  It is essentially a
// retract followed by an assert.
...
```

#### <a name="apidoc.element.nools.flow.prototype.getFacts"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>getFacts (Type)](#apidoc.element.nools.flow.prototype.getFacts)
- description and source-code
```javascript
getFacts = function (Type) {
    var ret;
    if (Type) {
        ret = this.workingMemory.getFactsByType(Type);
    } else {
        ret = this.workingMemory.getFacts();
    }
    return ret;
}
```
- example usage
```shell
...

'''javascript
session.assert(1);
session.assert("A");
session.assert("B");
session.assert(2);

session.getFacts(); //[1, "A", "B", 2];
'''

You may also pass in a 'Type' to 'getFacts' which will return facts only of the given type.

'''javascript
session.assert(1);
session.assert("A");
...
```

#### <a name="apidoc.element.nools.flow.prototype.halt"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>halt ()](#apidoc.element.nools.flow.prototype.halt)
- description and source-code
```javascript
halt = function () {
    this.executionStrategy.halt();
    return this;
}
```
- example usage
```shell
...

focus: function (focused) {
    this.agenda.setFocus(focused);
    return this;
},

halt: function () {
    this.executionStrategy.halt();
    return this;
},

dispose: function () {
    this.workingMemory.dispose();
    this.agenda.dispose();
    this.rootNode.dispose();
...
```

#### <a name="apidoc.element.nools.flow.prototype.match"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>match (cb)](#apidoc.element.nools.flow.prototype.match)
- description and source-code
```javascript
match = function (cb) {
    return (this.executionStrategy = new ExecutionStragegy(this)).execute().classic(cb).promise();
}
```
- example usage
```shell
...
var session = flow.getSession();
//assert your different messages
session.assert(new Message("goodbye"));
session.assert(new Message("hello"));
session.assert(new Message("hello world"));

//now fire the rules
session.match(function(err){
    if(err){
        console.error(err.stack);
    }else{
        console.log("done");
    }
})
'''
...
```

#### <a name="apidoc.element.nools.flow.prototype.matchUntilHalt"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>matchUntilHalt (cb)](#apidoc.element.nools.flow.prototype.matchUntilHalt)
- description and source-code
```javascript
matchUntilHalt = function (cb) {
    return (this.executionStrategy = new ExecutionStragegy(this, true)).execute().classic(cb).promise();
}
```
- example usage
```shell
...
        });
    }
}

'''

'''javascript
flow.getSession().matchUntilHalt(function(err){
    if(err){
        console.log(err.stack);
        return;
    }
    //halt finally invoked
});
'''
...
```

#### <a name="apidoc.element.nools.flow.prototype.modify"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>modify (fact, cb)](#apidoc.element.nools.flow.prototype.modify)
- description and source-code
```javascript
modify = function (fact, cb) {
    //fact = this.workingMemory.getFact(fact);
    if ("function" === typeof cb) {
        cb.call(fact, fact);
    }
    this.rootNode.modifyFact(this.workingMemory.modifyFact(fact));
    this.emit("modify", fact);
    return fact;
}
```
- example usage
```shell
...
};

var flow = nools.flow("Hello World", function (flow) {

    //find any message that is exactly hello world
    flow.rule("Hello", [Message, "m", "m.text =~ /^hello\\sworld$/"], function (facts) {
        facts.m.text = facts.m.text + " goodbye";
        this.modify(facts.m);
    });

    //find all messages then end in goodbye
    flow.rule("Goodbye", [Message, "m", "m.text =~ /.*goodbye$/"], function (facts) {
        console.log(facts.m.text);
    });
});
...
```

#### <a name="apidoc.element.nools.flow.prototype.print"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>print ()](#apidoc.element.nools.flow.prototype.print)
- description and source-code
```javascript
print = function () {
    this.rootNode.print();
}
```
- example usage
```shell
...
    }
    this.rootNode.modifyFact(this.workingMemory.modifyFact(fact));
    this.emit("modify", fact);
    return fact;
},

print: function () {
    this.rootNode.print();
},

containsRule: function (name) {
    return this.rootNode.containsRule(name);
},

rule: function (rule) {
...
```

#### <a name="apidoc.element.nools.flow.prototype.retract"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>retract (fact)](#apidoc.element.nools.flow.prototype.retract)
- description and source-code
```javascript
retract = function (fact) {
    //fact = this.workingMemory.getFact(fact);
    this.rootNode.retractFact(this.workingMemory.retractFact(fact));
    this.emit("retract", fact);
    return fact;
}
```
- example usage
```shell
...
'''javascript
var m = new Message("hello");

//assert the fact into the engine
session.assert(m);

//remove the fact from the engine
session.retract(m);

'''

**Note** 'retract' is typically used during the execution of the rules.

<a name="facts-modify"></a>
### Modify
...
```

#### <a name="apidoc.element.nools.flow.prototype.rule"></a>[function <span class="apidocSignatureSpan">nools.flow.prototype.</span>rule (rule)](#apidoc.element.nools.flow.prototype.rule)
- description and source-code
```javascript
rule = function (rule) {
    this.rootNode.assertRule(rule);
}
```
- example usage
```shell
...
var Message = function (message) {
this.text = message;
};

var flow = nools.flow("Hello World", function (flow) {

//find any message that is exactly hello world
flow.rule("Hello", [Message, "m", "m.text =~ /^hello\\sworld$/"], function (facts) {
    facts.m.text = facts.m.text + " goodbye";
    this.modify(facts.m);
});

//find all messages then end in goodbye
flow.rule("Goodbye", [Message, "m", "m.text =~ /.*goodbye$/"], function (facts) {
    console.log(facts.m.text);
...
```



# <a name="apidoc.module.nools.getFlow"></a>[module nools.getFlow](#apidoc.module.nools.getFlow)

#### <a name="apidoc.element.nools.getFlow.getFlow"></a>[function <span class="apidocSignatureSpan">nools.</span>getFlow (name)](#apidoc.element.nools.getFlow.getFlow)
- description and source-code
```javascript
getFlow = function (name) {
    return flows[name];
}
```
- example usage
```shell
...
To remove a defined flow from 'nools' use the 'deleteFlow' function.

'''javascript
var myFlow = nools.flow("flow");

nools.deleteFlow("flow"); //returns nools for chaining

nools.getFlow("flow"); //undefined

'''

You may also remove a flow using the 'FlowContainer' object returned from nools.flow;

'''javascript
var myFlow = nools.flow("flow");
...
```

#### <a name="apidoc.element.nools.getFlow._f"></a>[function <span class="apidocSignatureSpan">nools.getFlow.</span>_f (name)](#apidoc.element.nools.getFlow._f)
- description and source-code
```javascript
_f = function (name) {
    return flows[name];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.hasFlow"></a>[module nools.hasFlow](#apidoc.module.nools.hasFlow)

#### <a name="apidoc.element.nools.hasFlow.hasFlow"></a>[function <span class="apidocSignatureSpan">nools.</span>hasFlow (name)](#apidoc.element.nools.hasFlow.hasFlow)
- description and source-code
```javascript
hasFlow = function (name) {
    return extd.has(flows, name);
}
```
- example usage
```shell
...
# Checking If A Flow Exists

To check if a flow currently is registering with 'nools' use the 'hasFlow' function;

'''javascript
var myFlow = nools.flow("flow");

nools.hasFlow("flow"); //true

'''

<a name="agenda-groups"></a>
## Agenda Groups

Agenda groups allow for logical groups of rules within a flow.
...
```

#### <a name="apidoc.element.nools.hasFlow._f"></a>[function <span class="apidocSignatureSpan">nools.hasFlow.</span>_f (name)](#apidoc.element.nools.hasFlow._f)
- description and source-code
```javascript
_f = function (name) {
    return extd.has(flows, name);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.linkedList"></a>[module nools.linkedList](#apidoc.module.nools.linkedList)

#### <a name="apidoc.element.nools.linkedList.linkedList"></a>[function <span class="apidocSignatureSpan">nools.</span>linkedList ()](#apidoc.element.nools.linkedList.linkedList)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.linkedList._getSuper"></a>[function <span class="apidocSignatureSpan">nools.linkedList.</span>_getSuper ()](#apidoc.element.nools.linkedList._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.linkedList._super"></a>[function <span class="apidocSignatureSpan">nools.linkedList.</span>_super (args, a)](#apidoc.element.nools.linkedList._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.linkedList.as"></a>[function <span class="apidocSignatureSpan">nools.linkedList.</span>as (obj, name)](#apidoc.element.nools.linkedList.as)
- description and source-code
```javascript
function _export(obj, name) {
    if (obj && name) {
        obj[name] = this;
    } else {
        obj.exports = obj = this;
    }
    return this;
}
```
- example usage
```shell
...
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.constraint === constraint.constraint;
}
    }
}).as(exports, "ObjectConstraint");

var EqualityConstraint = Constraint.extend({

    instance: {

type: "equality",
...
```

#### <a name="apidoc.element.nools.linkedList.extend"></a>[function <span class="apidocSignatureSpan">nools.linkedList.</span>extend (proto)](#apidoc.element.nools.linkedList.extend)
- description and source-code
```javascript
function extend(proto) {
    return declare(this, proto);
}
```
- example usage
```shell
...
    }
}


    }
});

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},
...
```

#### <a name="apidoc.element.nools.linkedList.get"></a>[function <span class="apidocSignatureSpan">nools.linkedList.</span>get (name)](#apidoc.element.nools.linkedList.get)
- description and source-code
```javascript
function getter(name) {
    var getters = this.__getters__;
    if (getters.hasOwnProperty(name)) {
        return getters[name].apply(this);
    } else {
        return this[name];
    }
}
```
- example usage
```shell
...
},

getIndexableProperties: function () {
    return [];
},

equal: function (constraint) {
    return instanceOf(constraint, this._static) && this.get("alias") === constraint.get("alias") && extd.deepEqual(this.constraint
, constraint.constraint);
},

getters: {
    variables: function () {
        return [this.get("alias")];
    }
}
...
```

#### <a name="apidoc.element.nools.linkedList.init"></a>[function <span class="apidocSignatureSpan">nools.linkedList.</span>init ()](#apidoc.element.nools.linkedList.init)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.linkedList.mixin"></a>[function <span class="apidocSignatureSpan">nools.linkedList.</span>mixin ()](#apidoc.element.nools.linkedList.mixin)
- description and source-code
```javascript
function wrapper() {
    var ret, meta = this.__meta || {};
    var orig = meta.superMeta;
    meta.superMeta = {f: f, pos: 0, name: name};
    switch (arguments.length) {
    case 0:
        ret = f.call(this);
        break;
    case 1:
        ret = f.call(this, arguments[0]);
        break;
    case 2:
        ret = f.call(this, arguments[0], arguments[1]);
        break;

    case 3:
        ret = f.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        ret = f.apply(this, arguments);
    }
    meta.superMeta = orig;
    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.linkedList.set"></a>[function <span class="apidocSignatureSpan">nools.linkedList.</span>set (name, val)](#apidoc.element.nools.linkedList.set)
- description and source-code
```javascript
function setter(name, val) {
    var setters = this.__setters__;
    if (isHash(name)) {
        for (var i in name) {
            var prop = name[i];
            if (setters.hasOwnProperty(i)) {
                setters[name].call(this, prop);
            } else {
                this[i] = prop;
            }
        }
    } else {
        if (setters.hasOwnProperty(name)) {
            return setters[name].apply(this, argsToArray(arguments, 1));
        } else {
            return this[name] = val;
        }
    }
}
```
- example usage
```shell
...
    }
    if (store && !isEmpty(store)) {
        var atm = new constraint.HashConstraint(store);
        constraints.push(atm);
    }

    forEach(constraints, function (constraint) {
        constraint.set("alias", alias);
    });
    this.constraints = constraints;
},

getSpecificity: function () {
    var constraints = this.constraints, specificity = 0;
    for (var i = 0, l = constraints.length; i < l; i++) {
...
```



# <a name="apidoc.module.nools.linkedList.prototype"></a>[module nools.linkedList.prototype](#apidoc.module.nools.linkedList.prototype)

#### <a name="apidoc.element.nools.linkedList.prototype._getSuper"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>_getSuper ()](#apidoc.element.nools.linkedList.prototype._getSuper)
- description and source-code
```javascript
function getSuper() {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.bind(this);
            }
        } while (l > ++pos);
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.linkedList.prototype._static"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>_static ()](#apidoc.element.nools.linkedList.prototype._static)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
...
    }

},

merge: function (that) {
    var ret = this;
    if (that instanceof ReferenceConstraint) {
        ret = new this._static([this.constraint, that.constraint, "and"], merge({}, this._options, this._options));
        ret._alias = this._alias || that._alias;
        ret.vars = this.vars.concat(that.vars);
    }
    return ret;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.linkedList.prototype._super"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>_super (args, a)](#apidoc.element.nools.linkedList.prototype._super)
- description and source-code
```javascript
function callSuper(args, a) {
    var meta = this.__meta,
        supers = meta.supers,
        l = supers.length, superMeta = meta.superMeta, pos = superMeta.pos;
    if (l > pos) {
        args = !args ? [] : (!isArguments(args) && !isArray(args)) ? [args] : args;
        var name = superMeta.name, f = superMeta.f, m;
        do {
            m = supers[pos][name];
            if ("function" === typeof m && (m = m._f || m) !== f) {
                superMeta.pos = 1 + pos;
                return m.apply(this, args);
            }
        } while (l > ++pos);
    }

    return null;
}
```
- example usage
```shell
...

Constraint.extend({
    instance: {

type: "object",

constructor: function (type) {
    this._super([type]);
},

"assert": function (param) {
    return param instanceof this.constraint || param.constructor === this.constraint;
},

equal: function (constraint) {
...
```

#### <a name="apidoc.element.nools.linkedList.prototype.clear"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>clear ()](#apidoc.element.nools.linkedList.prototype.clear)
- description and source-code
```javascript
clear = function () {
    this.head = this.tail = null;
    this.length = 0;
}
```
- example usage
```shell
...
    instance: {
constructor: function () {
    this.memory = {};
    this.memoryValues = new LinkedList();
},

clear: function () {
    this.memoryValues.clear();
    this.memory = {};
},


remove: function (v) {
    var hashCode = v.hashCode,
        memory = this.memory,
...
```

#### <a name="apidoc.element.nools.linkedList.prototype.constructor"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>constructor ()](#apidoc.element.nools.linkedList.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    this.head = null;
    this.tail = null;
    this.length = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.linkedList.prototype.forEach"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>forEach (cb)](#apidoc.element.nools.linkedList.prototype.forEach)
- description and source-code
```javascript
forEach = function (cb) {
    var head = {next: this.head};
    while ((head = head.next)) {
        cb(head.data);
    }
}
```
- example usage
```shell
...
        count--;
        if (!count) {
            done();
        }
    }
}

files.forEach(function (file) {
    var base = path.basename(file, ".nools"),
        out = path.resolve(path.dirname(file), base + "-compiled.js");
    child.exec(path.resolve(__dirname, "./bin/nools") + " compile " + file + " -l ../../ -n " + base + "-compiled", function (err
, output) {
        if (!err) {
            grunt.file.write(out, output.toString());
        }
        counter(err);
...
```

#### <a name="apidoc.element.nools.linkedList.prototype.getByData"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>getByData (data)](#apidoc.element.nools.linkedList.prototype.getByData)
- description and source-code
```javascript
getByData = function (data) {
    var head = {next: this.head};
    while ((head = head.next)) {
        if (head.data === data) {
            return head;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.linkedList.prototype.push"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>push (data)](#apidoc.element.nools.linkedList.prototype.push)
- description and source-code
```javascript
push = function (data) {
    var tail = this.tail, head = this.head, node = {data: data, prev: tail, next: null};
    if (tail) {
        this.tail.next = node;
    }
    this.tail = node;
    if (!head) {
        this.head = node;
    }
    this.length++;
    return node;
}
```
- example usage
```shell
...

'''
//assuming a flow with the rules specified above.
var fired = [];
flow.getSession(new Message("hello"))
    .focus("ag1")
    .on("fire", function (ruleName) {
        fired.push(ruleName);
    })
    .match(function () {
        console.log(fired);  //[ 'Hello World' ]
    });
'''

Or you can add multiple 'agenda-groups' to the focus stack.
...
```

#### <a name="apidoc.element.nools.linkedList.prototype.remove"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>remove (node)](#apidoc.element.nools.linkedList.prototype.remove)
- description and source-code
```javascript
remove = function (node) {
    if (node.prev) {
        node.prev.next = node.next;
    } else {
        this.head = node.next;
    }
    if (node.next) {
        node.next.prev = node.prev;
    } else {
        this.tail = node.prev;
    }
    //node.data = node.prev = node.next = null;
    this.length--;
}
```
- example usage
```shell
...


remove: function (v) {
    var hashCode = v.hashCode,
        memory = this.memory,
        ret = memory[hashCode];
    if (ret) {
        this.memoryValues.remove(ret);
        delete memory[hashCode];
    }
    return ret;
},

insert: function (insert) {
    var hashCode = insert.hashCode;
...
```

#### <a name="apidoc.element.nools.linkedList.prototype.removeByData"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>removeByData (data)](#apidoc.element.nools.linkedList.prototype.removeByData)
- description and source-code
```javascript
removeByData = function (data) {
    var head = {next: this.head};
    while ((head = head.next)) {
        if (head.data === data) {
            this.remove(head);
            break;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.linkedList.prototype.toArray"></a>[function <span class="apidocSignatureSpan">nools.linkedList.prototype.</span>toArray ()](#apidoc.element.nools.linkedList.prototype.toArray)
- description and source-code
```javascript
toArray = function () {
    var head = {next: this.head}, ret = [];
    while ((head = head.next)) {
        ret.push(head);
    }
    return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.pattern"></a>[module nools.pattern](#apidoc.module.nools.pattern)

#### <a name="apidoc.element.nools.pattern.CompositePattern"></a>[function <span class="apidocSignatureSpan">nools.pattern.</span>CompositePattern ()](#apidoc.element.nools.pattern.CompositePattern)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.pattern.ExistsPattern"></a>[function <span class="apidocSignatureSpan">nools.pattern.</span>ExistsPattern ()](#apidoc.element.nools.pattern.ExistsPattern)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.pattern.FromExistsPattern"></a>[function <span class="apidocSignatureSpan">nools.pattern.</span>FromExistsPattern ()](#apidoc.element.nools.pattern.FromExistsPattern)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.pattern.FromNotPattern"></a>[function <span class="apidocSignatureSpan">nools.pattern.</span>FromNotPattern ()](#apidoc.element.nools.pattern.FromNotPattern)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.pattern.FromPattern"></a>[function <span class="apidocSignatureSpan">nools.pattern.</span>FromPattern ()](#apidoc.element.nools.pattern.FromPattern)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.pattern.InitialFact"></a>[function <span class="apidocSignatureSpan">nools.pattern.</span>InitialFact ()](#apidoc.element.nools.pattern.InitialFact)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.pattern.InitialFactPattern"></a>[function <span class="apidocSignatureSpan">nools.pattern.</span>InitialFactPattern ()](#apidoc.element.nools.pattern.InitialFactPattern)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.pattern.NotPattern"></a>[function <span class="apidocSignatureSpan">nools.pattern.</span>NotPattern ()](#apidoc.element.nools.pattern.NotPattern)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nools.pattern.ObjectPattern"></a>[function <span class="apidocSignatureSpan">nools.pattern.</span>ObjectPattern ()](#apidoc.element.nools.pattern.ObjectPattern)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.rule"></a>[module nools.rule](#apidoc.module.nools.rule)

#### <a name="apidoc.element.nools.rule.createRule"></a>[function <span class="apidocSignatureSpan">nools.rule.</span>createRule (name, options, conditions, cb)](#apidoc.element.nools.rule.createRule)
- description and source-code
```javascript
function createRule(name, options, conditions, cb) {
    if (isArray(options)) {
        cb = conditions;
        conditions = options;
    } else {
        options = options || {};
    }
    var isRules = extd.every(conditions, function (cond) {
        return isArray(cond);
    });
    if (isRules && conditions.length === 1) {
        conditions = conditions[0];
        isRules = false;
    }
    var rules = [];
    var scope = options.scope || {};
    conditions.scope = scope;
    if (isRules) {
        var _mergePatterns = function (patt, i) {
            if (!patterns[i]) {
                patterns[i] = i === 0 ? [] : patterns[i - 1].slice();
                //remove dup
                if (i !== 0) {
                    patterns[i].pop();
                }
                patterns[i].push(patt);
            } else {
                extd(patterns).forEach(function (p) {
                    p.push(patt);
                });
            }

        };
        var l = conditions.length, patterns = [], condition;
        for (var i = 0; i < l; i++) {
            condition = conditions[i];
            condition.scope = scope;
            extd.forEach(parsePattern(condition), _mergePatterns);

        }
        rules = extd.map(patterns, function (patterns) {
            var compPat = null;
            for (var i = 0; i < patterns.length; i++) {
                if (compPat === null) {
                    compPat = new CompositePattern(patterns[i++], patterns[i]);
                } else {
                    compPat = new CompositePattern(compPat, patterns[i]);
                }
            }
            return new Rule(name, options, compPat, cb);
        });
    } else {
        rules = extd.map(parsePattern(conditions), function (cond) {
            return new Rule(name, options, cond, cb);
        });
    }
    return rules;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nools.workingMemory"></a>[module nools.workingMemory](#apidoc.module.nools.workingMemory)

#### <a name="apidoc.element.nools.workingMemory.WorkingMemory"></a>[function <span class="apidocSignatureSpan">nools.workingMemory.</span>WorkingMemory ()](#apidoc.element.nools.workingMemory.WorkingMemory)
- description and source-code
```javascript
function declared() {
    switch (arguments.length) {
    case 0:
        this.constructor.call(this);
        break;
    case 1:
        this.constructor.call(this, arguments[0]);
        break;
    case 2:
        this.constructor.call(this, arguments[0], arguments[1]);
        break;
    case 3:
        this.constructor.call(this, arguments[0], arguments[1], arguments[2]);
        break;
    default:
        this.constructor.apply(this, arguments);
    }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
