
This is a collection of style guides for Go.

Be sure to read about [writing engineering
guidelines](https://medium.com/@dgryski/writing-engineering-guidelines-24fdda53a3f0)
before trying to adopt one of these wholesale.

(For more commentary on these, see my blog post [Idiomatic Go Resources](https://medium.com/@dgryski/idiomatic-go-resources-966535376dba))

### The Classics

* [Effective Go](https://golang.org/doc/effective_go.html)
* [CodeReviewComments](https://github.com/golang/go/wiki/CodeReviewComments)
* [Go Proverbs](https://go-proverbs.github.io)

### Googler Talks

* [What’s in a name?](https://talks.golang.org/2014/names.slide#1)
* [Package Names](https://blog.golang.org/package-names)
* [When in Go, do as Gophers do](https://talks.golang.org/2014/readability.slide#1)
* [Twelve Go Best Practices](https://talks.golang.org/2013/bestpractices.slide#1)
* [Style guidelines for Go packages](https://rakyll.org/style-packages/)
* [Idiomatic Go](https://dmitri.shuralyov.com/idiomatic-go)

### Go Wiki Pages

* [Target-specific code](https://github.com/golang/go/wiki/TargetSpecific)
* [Assembly Policy](https://github.com/golang/go/wiki/AssemblyPolicy)
* [Commit Messages](https://github.com/golang/go/wiki/CommitMessage)
* [TestComments](https://github.com/golang/go/wiki/TestComments)

### Non-Googlers

* [Go Best Practices 2016](https://peter.bourgon.org/go-best-practices-2016/)
* [Go for Industrial Programming](https://peter.bourgon.org/go-for-industrial-programming/)
* [Practical Go: Real world advice for writing maintainable Go programs](https://dave.cheney.net/practical-go/presentations/qcon-china.html)
* [The Zen of Go](https://dave.cheney.net/2020/02/23/the-zen-of-go)
* [godocgo: Effective Go documentation](https://godoc.org/github.com/natefinch/godocgo)

### Further Reading

* [The Ideas That Shaped Go](https://medium.com/@dgryski/the-ideas-that-shaped-go-21850a74295f)
* [Software Engineering at Google](https://arxiv.org/abs/1702.01715)

### Corporate/Project-specific Style Guildes

* [bahlo/go-styleguide](https://github.com/bahlo/go-styleguide)
* [CockroachDB](https://github.com/cockroachdb/cockroach/blob/master/docs/style.md)
* [Edge X Foundry](https://wiki.edgexfoundry.org/display/FA/Contributor%27s+Guide+-+Go+Lang)
* [GitLab](https://docs.gitlab.com/ee/development/go_guide/)
* [Hyperledger](https://github.com/hyperledger/fabric/blob/release-1.4/docs/source/style-guides/go-style.rst)
* [Magnetico](https://github.com/boramalper/magnetico/wiki/magnetico-Design-Specification)
* [Sourcegraph](https://about.sourcegraph.com/handbook/engineering/go_style_guide)
* [Thanos](https://thanos.io/tip/contributing/coding-style-guide.md/)
* [Uber](https://github.com/uber-go/guide/blob/master/style.md)

General tips for Code Reviews:

* [Vitess.io Code Reviews](https://vitess.io/docs/contributing/code-reviews/)
* [Google Engineering Practices](https://google.github.io/eng-practices/)
* [How to Do Code Reviews Like a Human](https://mtlynch.io/human-code-reviews-1/)

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
to stay static while maintainers move over time.  Similarly, including dates or
release versions in the comment can ensure TODOs are revisisted at appropriate
times.

*Find this useful? [Buy me a coffee!](https://www.buymeacoffee.com/dgryski)*
