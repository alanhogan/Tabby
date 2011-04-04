# Tabby

This jQuery plugin is by [Ted Devito], originally found at  <http://teddevito.com/demos/textarea.html>. There did not seem to be a GitHub repo for it yet, so I made one.

### Purpose

Ted:

> The "Tabby" Javascript jQuery plugin … [allows use of the Tab key] in regular `textarea`s to make them suitable for in-browser coding [in] languages like HTML, CSS, Javascript, or your favorite server-side language. The idea is to be able to use a press of the TAB button or SHIFT+TAB to indent or outdent your code.

It pretty well for Markdown editors, too.

### Usage

Can’t be any simpler:

	$('.my-textarea').tabby();
	
To use e.g. four spaces instead of the default tab character:

	var tabby_opts = {tabString:'    '};
	$('.my-textarea').tabby(tabby_opts);

### Demo

Please see [Ted’s demo here][ted].

### Differences from original

I made a small change to better support alternate tag strings besides the actual tab character `\t` (e.g. four spaces).

### Caveats

Outdenting only works properly with one single kind of tab string (spaces or tabs).  You should probably standardize input to your preferred kind of tabs (soft or hard) before presenting a Tabby-enabled `textarea` to your users.

### See Also

For a description of the problem and how this solution is implemented, please see [Ted’s original description][ted].

[ted]: http://teddevito.com/demos/textarea.html "Original website and demo"
[Ted Devito]: http://teddevito.com/ "Ted’s website"