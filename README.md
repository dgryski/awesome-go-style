
** This is also part of avelino/awesome-go: https://github.com/avelino/awesome-go#style-guides **

This is a collection of style guides for Go.

Be sure to read about [writing engineering
guidelines](https://medium.com/@dgryski/writing-engineering-guidelines-24fdda53a3f0)
before trying to adopt one of these wholesale.

There are also a number of semi-official guides linked from [Idiomatic Go Resources](https://medium.com/@dgryski/idiomatic-go-resources-966535376dba)

* [bahlo/go-styleguide](https://github.com/bahlo/go-styleguide)
* [CockroachDB](https://github.com/cockroachdb/cockroach/blob/master/docs/style.md)
* [Edge X Foundry](https://wiki.edgexfoundry.org/display/FA/Contributor%27s+Guide+-+Go+Lang)
* [GitLab](https://docs.gitlab.com/ee/development/go_guide/)
* [Hyperledger](https://github.com/hyperledger/fabric/blob/release-1.4/docs/source/style-guides/go-style.rst)
* [Magnetico](https://github.com/boramalper/magnetico/wiki/magnetico-Design-Specification)
* [Sourcegraph](https://about.sourcegraph.com/handbook/engineering/go_style_guide)
* [Thanos](https://thanos.io/contributing/coding-style-guide.md/)
* [Uber](https://github.com/uber-go/guide/blob/master/style.md)
* [Zen of Go](https://dave.cheney.net/2020/02/23/the-zen-of-go)

General tips for Code Reviews:

* [Vitess.io Code Reviews](https://vitess.io/docs/contributing/code-reviews/)
* [Google Engineering Practices](https://google.github.io/eng-practices/)


My own attempt at best practices for TODO comments (extracted from existing Go
practices, but otherwise mostly undocumented):


```
// For TODOs, BUGs, and NOTEs please use the standard form:
//
//    // TODO(username): ...
//
// The username (generally yours) means "for more information see", not
// "I claim responsibility for fixing this." Please use TODO rather than FIXME,
// XXX, HACK, etc.  This limits the number of things to grep for.
//
//    * TODO denotes missing features or functionality
//    * BUG denotes known broken code; these are displayed in godoc
//    * NOTE is used to highlight a particularly important or subtle section of code
//    * SECURITY and SECBUG are used for security related notes and issues
```

If you have a bug tracker, TODO(bug#) is probalby more useful as they're likely
to stay static while maintainers move over time.
