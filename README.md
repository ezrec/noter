# 📝 noter

A text editor for macOS. Built using the [Ebiten](https://github.com/hajimehoshi/ebiten) game engine.

![A screenshot of the editor running. It looks like nano. It has a text file called "A Bird, came down the Walk" opened.](https://github.com/healeycodes/noter/blob/main/preview.png)

It's a little bit like `nano`.

## Guide

- command+c: copy line
- command+x: cut line
- command+v: paste
- command+x: save
- command+q: quit without saving

- command+left/right skips to start/end of line
- command+up/down is the same as page up/page down

## Development

Run the fonts build script `bash fonts.sh`

Run the editor `go run . -- "A Bird, came down the Walk.txt"`

## Build

`go build .`

## Tests

`go test ./...`

## Roadmap

- alt+arrows to skip words/spacing
- cmd+up/down should skip pages rather than move to the start of the document
- abstract away more logic into methods on Line (and a new RuneList type?)
- more tests
- search?
