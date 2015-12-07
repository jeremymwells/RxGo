<img src="https://golang.org/doc/gopher/gopherbw.png" height="30px" margin-top="5px"/>RxGo (pre-alpha) 
====

Reactive Extensions implementation for the Go Programming Language

[Apache 2.0 License](LICENSE.txt)

- [Code of Conduct](CODE_OF_CONDUCT.md)
- [Contribution Guidelines](CONTRIBUTING.md)
- [Maintainer Guidelines](doc/maintainer-guidelines.md)
- [Creating Operators](doc/operator-creation.md)

## Important

By contributing or commenting on issues in this repository, whether you've read them or not, you're agreeing to the [Contributor Code of Conduct](CODE_OF_CONDUCT.md). Much like traffic laws, ignorance doesn't grant you immunity.

## Installation and Usage

To install this library , use the following command: (doesn't work yet)

```
go get github.com/rxgo 
```

## Goals

- Provide RxGO

## Building/Testing

To run tests:

`go test something`

# Alpha roadmap

##Necessary Basic Static Methods

I'm cherry-picking from current ReactiveX/RxJS

- [ ] concat
- [ ] empty
- [ ] from
- [ ] fromArray
- [ ] fromEvent
- [ ] fromEventPattern
- [ ] fromPromise
- [ ] interval
- [ ] just/value
- [ ] merge
- [ ] never
- [ ] of
- [ ] range
- [ ] return
- [ ] throw
- [ ] timer
- [ ] zip

##Necessary Basic Operators

I'm cherry-picking operators from ReactiveX/RxJS

- [ ] buffer
- [ ] bufferCount (bufferWithCount)
- [ ] bufferTime (bufferWithTime)
- [ ] bufferToggle (buffer(obs, fn))
- [ ] bufferWhen (buffer(fn))
- [ ] catch
- [ ] combineLatest
- [ ] concat
- [ ] concatAll
- [ ] defaultIfEmpty
- [ ] delay
- [ ] flatMap
- [ ] filter
- [ ] forkJoin
- [ ] groupBy
- [ ] groupByUntil
- [ ] map
- [ ] mapTo
- [ ] merge
- [ ] mergeAll
- [ ] multicast
- [ ] observeOn
- [ ] publish
- [ ] reduce
- [ ] repeat
- [ ] retry
- [ ] retryWhen
- [ ] scan
- [ ] skip
- [ ] skipUntil
- [ ] startWith
- [ ] subscribeOn
- [ ] switchMap (flatMapLatest)
- [ ] take
- [ ] takeUntil
- [ ] timeout
- [ ] toArray
- [ ] toPromise
- [ ] withLatestFrom
- [ ] zip
- [ ] zipAll

##Necessary Support Types

- [ ] Observable
- [ ] Subscriber
- [ ] BehaviorSubject
- [ ] ConnectableObservable (multicast)
- [ ] refCount
- [ ] Subject
- [ ] ReplaySubject

##Schedulers

- [ ] immediate
- [ ] nextTick

##Macro Performance Tests

We want to add macro performance tests for all operators that create other Observables or Subscriptions internally. (Basically anything that does a lot of allocating) We may expand this to anything that buffers or schedules. These should be contrasted against their predecessors.

- [ ] combineLatest
- [ ] flatMap
- [ ] flatMap with Scalar
- [ ] groupBy
- [ ] merge
- [ ] mergeAll
- [ ] windowCount (windowWithCount)
//need more here...

Micro Performance Tests

Micro performance tests are perhaps slightly less reliable than the macro performance tests, but still give us some insight into how we're doing.

##Creation

- [ ] concat
- [ ] empty
- [ ] from
- [ ] fromArray
- [ ] merge
- [ ] of
- [ ] range
- [ ] return
- [ ] throw
//need more here...


##Operators

- [ ] bufferCount (bufferWithCount)
- [ ] catch
- [ ] combineLatest
- [ ] concat
- [ ] concatAll
- [ ] defaultIfEmpty
- [ ] flatMap
- [ ] filter
- [ ] groupBy
- [ ] groupByUntil
- [ ] map
- [ ] merge
- [ ] mergeAll
- [ ] reduce
- [ ] repeat
- [ ] scan
- [ ] skip
- [ ] startWith
- [ ] take
- [ ] toArray
- [ ] windowCount (windowWithCount)
- [ ] zip
//need more here...

##TODO: figure out benchmarking

##Other Requirements

- [ ] some basic documentation
- [ ] community code of conduct
- [ ] install instructions
- [ ] build instructions
- [ ] basic build pipeline
- [ ] license
- [ ] solid version starting point (0.0.1)
- [ ] interop points from some canonical spec


