# Speedwriter

**Speedwriter** makes it *look like* you write like a world-leading hacker or a New York Times best seller!

This nifty little tool will be a building block in [Mammon](https://github.com/bep/mammon), a hacking scene factory for movie and television producers. 

Just pick your text and start typing random letters as fast as you can! As any good magician will know: People will not notice the keys you press as long as the pace is in sync and the result is correct!

## Install

**Speedwriter** is a Go application. The easiest way to intall it is via `go get`:

```bash
 go get -v github.com/bep/speedwriter
```

## Is it any good?

[Yes.](https://news.ycombinator.com/item?id=3067434)

## Use

Usage: `speedwriter [FILE]`
		
An alternative to the above, is to pipe the text to stdin, e.g.:
	
```bash	
cat myfile.txt | speedwriter
```
	
This makes it easy to make it look like you're coding like Linus Torvalds:

```bash
curl -s https://raw.githubusercontent.com/git/git/master/block-sha1/sha1.c | egrep -v "^(//|/\*| \*)" | tail -n +153 | speedwriter
```

## Limitations

This application has been confirmed to work fine on OS X, but should work fine on most *nixes. Will have to be checked out/adapted to Windows.
