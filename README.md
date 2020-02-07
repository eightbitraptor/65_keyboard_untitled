# 65_keyboard_untitled

My as yet unnamed 65% keyboard design

## Project structure

- [`layouts`](layouts/) - contains all the layout options I explored and the related artifacts. Generated using [Keyboard Layout Editor](https://www.keyboard-layout-editor.com)

## Layout

**tl;dr - pretty standard 65% layout WKL bottom row and split backspace**

This keyboard is a 65% board. Which means it's basically a 60% layout that's been extended by 1 column which allows us to comfortably incorporate an arrow cluster and a couple of the useful navigation keys. It's a fixed layout because it's being built just for me as a personal project. So don't expect any allowances in plate or case design for other layouts.

It's using a HHKB style layout (ANSI base with split backspace, Esc next to the 1), a Winkeyless style bottom row with a 7u spacebar, and a 1u logo blocker in the top right (because aesthetics). The right shift has been shrunk to 1.75u to allow for the up arrow. It looks like this:

![65% WKL Layout](layouts/65-wkl.png)

NOTE: To make the process easier later. I'm using the Tsangan layout to generate the platefile dxf. Tsangan is the same as WKL but with a 1u key instead of a blocker. I'm generating it this way as it makes the top case easier to design as it gives me the markings for the key that I can use as anchors in my cad program to situate the blocker.

## Plate

Platefile was generated using [this fork of ai03's another plate file generator](https://github.com/fox-lab/another-keyboard-builder/commits/master)

`cat plate_2d/wkl-kle-raw | python3 plategen.py --stab-type large-cuts -at typical > wkl-platefile.dxf`