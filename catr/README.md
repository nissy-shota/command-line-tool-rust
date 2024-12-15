# catr

catr is a Rust version of the coreutils cat.
catr has two options whichi is number and nonblank number.

## exmaple

### default

```bash
cargo run tests/inputs/spiders.txt
```

out

```bash
Don't worry, spiders,
I keep house
casually.
```

### number option

```bash
$ cargo run -- -n tests/inputs/the-bustle.txt
```

out

```bash
1  The bustle in a house
2  The morning after death
3  Is solemnest of industries
4  Enacted upon earth,
5
6  The sweeping up the heart,
7  And putting love away
8  We shall not want to use again
9  Until eternity.
```

### nonblank line option

```bash
$ cargo run -- -b tests/inputs/the-bustle.txt
```

```bash
1  The bustle in a house
2  The morning after death
3  Is solemnest of industries
4  Enacted upon earth,
5  The sweeping up the heart,
6  And putting love away
7  We shall not want to use again
8  Until eternity.
```

## test

```bash
cargo test
```
