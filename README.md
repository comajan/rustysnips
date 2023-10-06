# rustysnips
Various VS Code snippets for the Rust language.

# Support for Selected Text

Many of the snippets will automagically surround the currently _selected text_ with the snippet template code, _but_ in order to get this to work in VS Code, you will need to do the following _one-time_ configuration change:

1. Open VS Code
1. Press `Ctrl + K` followed by `Ctrl + S` (this should open the VS Code keyboard shortcuts page)
1. Search for `surround with snippet`
1. Assign a keybind of your choosing or use `Ctrl + K Ctrl + M`

## Standard Process for Surrounding Selected Text with Snippet

After you have configured VS Code (see previous steps) and you have some _selected text_ you want to surround a snippet with, then do the following:

1. Press the keybinding you configured previously
1. Type the snippet name or shortcut
1. Select the appropriate snippet
1. Press `Enter`
 
# VS Code Snippets

## block

What you type:

* `{`
* `block`

What you get:

```rs
{
  // new code block ...
}
```

Any _selected text_ will be included in the new code block.  Also, this snippet is _smart_ and will automatically add a `;` automatically if needed (e.g. you selected some text after the arrow in a `match` arm you want to turn into a code block).

## error match

What you type:

* `error-match`
* `em`

What you get:

```rs
match <first tab position here> {
  Ok(<second tab position here>) => <third tab position here>,
  Err(<fourth tab position here>) => <fifth tab position here>
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## for in enumerate()

What you type:

* `for-in-enumerate`
* `fien`

What you get:

```rs
for (i, <first tab position here with default &item>) in <second tab position here; choose: iter(),into_iter(),iter_mut()>.enumerate() {
  <selected text goes here>
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## for in loop

What you type:

* `for-in-loop`
* `floop`

What you get:

```rs
for <first tab position here> in <second tab position here> {
  <selected text goes here>
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## if

What you type:

* `if`

What you get:

```rs
if <first tab position here> {
  <selected text goes here>
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## if/else

What you type:

* `if-else`
* `ife`

What you get:

```rs
if <first tab position here> {
  <selected text goes here>
} else {
  
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## if let

What you type:

* `if-let`
* `ifl`

What you get:

```rs
if let <first tab position here; select: Some(), Err()> = <second tab position here> {
  <selected text goes here>
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## loop

What you type:

* `loop`
* `lp`

What you get:

```rs
loop {
  <selected text goes here>
}
```

## match

What you type:

* `match`
* `mt`

What you get:

```rs
match <first tab position here> {
  <second tab position here> => <third tab position here>,
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## optional match

What you type:

* `optional-match`
* `match?`
* `mt?`

```rs
match <first tab position here> {
  Some(<second tab position here>) => <third tab position here>,
  None => <fourth tab position here>
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## optional while

What you type:

* `optional-while`
* `while?`
* `ow?`

What you get:

```rs
while let Some(<first tab position here with default: value>) = <second tab position here> {
  <selected text goes here>
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## println! macro

What you type:

* `print-line`
* `println`
* `pln`

What you get:

```rs
println!("<cursor is here>");
```

## struct declaration

What you type:

* `declare-struct`
* `define-struct`
* `ds`
* `struct`
* `stc`

What you get:

```rs
struct <first tab position here with default: name> {
  <second tab position here>
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## trait declaration

What you type:

* `trait`
* `tr`

What you get:

```rs
trait <first tab position here with default: name> {
  <second tab position here>
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.

## while

What you type:

* `while-loop`
* `wl`

What you get:

```rs
while <first tab position here> {
  <selected text goes here>
}
```

Once the code snippet fills in the above code template, use the `Tab` key to quickly fill in the code.
