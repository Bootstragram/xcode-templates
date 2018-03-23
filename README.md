# Xcode Templates

This repository contains some custom Xcode file templates.

## Why use custom templates?

1. Save time when creating files in Xcode
1. Who needs a file header?

Some blog posts inspired me to start using my own templates:

* [Xcode 9 File Templates](http://jeanetienne.net/2017/09/10/xcode-templates.html) by jeanetienne.net
* [Customizing the file header comment and other text macros in Xcode 9](https://oleb.net/blog/2017/07/xcode-9-text-macros/)

And some references to write them:

* Xcode Help's [Text macros reference](https://help.apple.com/xcode/mac/9.0/index.html?localePath=en.lproj#/dev7fe737ce0)
* Xcode Help's [Text macro format reference](https://help.apple.com/xcode/mac/9.0/index.html?localePath=en.lproj#/devc8a500cb9)

## The Templates

### Swift File Template

The Swift File template is just an empty file:

* I don't want some header
* I don't want to decide if I'm going to write a `struct`, a `class` or an `enum` just yet

Why not just use the empty file template? Because it started not empty but, over time, it became empty. I want to keep that in mind.

### Quick File Template

The Quick File Template looks like:

    import Quick
    import Nimble
    @testable import MyTarget

    class FileSpec: QuickSpec {
        override func spec() {
            describe("my spec") {
                it("has a dummy test") {
                    expect(true).to(beTrue())
                }
            }
        }
    }
