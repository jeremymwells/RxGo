RxGo (pre-alpha) <img src="https://golang.org/doc/gopher/gopherbw.png" style="float: left; height: 30px; margin-top: 8px;" />
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

To install this library , use the following command:

```
go get github.com/rxgo
```

## Goals

- Provide observable
- To model/follow the [ES7 Observable Spec](https://github.com/zenparsing/es-observable) to the observable.
- Provide more modular file structure in a variety of formats

## Building/Testing

To run tests:

`go test`

### Example

```sh
# build all the things!
npm run build_all
```

## Performance Tests

Run `npm run build_perf` or `npm run perf` to run the performance tests with `protractor`.
Run `npm run perf_micro` to run micro performance test benchmarking operator.

## Adding documentation
RxNext uses [ESDoc](https://esdoc.org/) to generate API documentation. Refer to ESDoc's documentation for syntax. Run `npm run build_docs` to generate.

## Generating PNG marble diagrams

The script `npm run tests2png` requires some native packages installed locally: `imagemagick`, `graphicsmagick`, and `ghostscript`.

For Mac OS X with [Homebrew](http://brew.sh/):

- `brew install imagemagick`
- `brew install graphicsmagick`
- `brew install ghostscript`

For Debian Linux:

- `sudo add-apt-repository ppa:dhor/myway`
- `apt-get install imagemagick`
- `apt-get install graphicsmagick`
- `apt-get install ghostscript`

For Windows and other Operating Systems, check the download instructions here:

- http://imagemagick.org
- http://www.graphicsmagick.org
- http://www.ghostscript.com/









# Roadmap: ======================================================================================>

### Necessary Basic Static Methods

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

### Necessary Basic Operators

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
- [ ] withLatestFrom
- [ ] zip
- [ ] zipAll


### Necessary Support Types

(Not including Observable and Subscriber, which are a given)

- [ ] BehaviorSubject
- [ ] ConnectableObservable (multicast)
- [ ] refCount
- [ ] Subject
- [ ] ReplaySubject

### Schedulers

- [ ] immediate
- [ ] nextTick


### Macro Performance Tests

We want to add macro performance tests for all operators that create other Observables or Subscriptions internally. (Basically anything that does a lot of allocating) We may expand this to anything that buffers or schedules. 

- [ ] combineLatest
- [ ] flatMap
- [ ] flatMap with Scalar
- [ ] groupBy
- [ ] merge
- [ ] mergeAll


### Micro Performance Tests

Micro performance tests are perhaps slightly less reliable than the macro performance tests, but still give us some insight into how we're doing. 

### Creation

- [ ] concat
- [ ] empty
- [ ] from
- [ ] fromArray
- [ ] merge
- [ ] of
- [ ] range
- [ ] return
- [ ] throw


### Operators

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
- [ ] zip


### Other Requirements

- [ ] some basic documentation
- [ ] community code of conduct
- [ ] install instructions
- [ ] build instructions
- [ ] basic build pipeline
- [ ] license
- [ ] solid version starting point (X.X.X-alpha?)