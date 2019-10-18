# ReDOS - link_code

## Example undefined

This markdown:

```markdown
INDEX(string, pattern[, start)` : searches for the first occurrence of pattern in string, starting from start: `INDEX("123123", "23", 3)` == `5`
`INSERT(new, old[, start][, length][, pad])` : inserts the new string into the old string after the specified position (default is 0), new string is truncated or padded (default is " ") to the specified length, if start is beyond the end of old old will be padded
`LASTPOS(pattern, string[, start])` : searches backwards for the last occurrence of pattern in string, starting from start: `LASTPOS("123123", "23", 4)` == `2`
`LINES(file)` : returns the number of lines typed ahead at the interactive stream: `push("a line"); push("second line"); lines(STDIN); /* == 2 */`
`MAX(number, number[, number,...])` : obvious
`MIN(number, number[, number,...])` : obvious
`OPEN(filehandle, filename[, "APPEND"|"READ"|"WRITE"])` : opens file, returns boolean for success: `OPEN("MyCon", "CON:160/50/320/100/MyCon/CDS")` == `1`
`OVERLAY(new, old[, start][, length][, pad])` : overlays new string onto old one at start for length chars padding with pad if necessary: `OVERLAY("4", "123", 5, 5)` == `"123-4----"`
`POS(pattern, string[, start])` : same as index

```

Should give output:

```html
<p>INDEX(string, pattern[, start)<code>: searches for the first occurrence of pattern in string, starting from start:</code>INDEX(&quot;123123&quot;, &quot;23&quot;, 3)<code>==</code>5<code></code>INSERT(new, old[, start][, length][, pad])<code>: inserts the new string into the old string after the specified position (default is 0), new string is truncated or padded (default is &quot; &quot;) to the specified length, if start is beyond the end of old old will be padded</code>LASTPOS(pattern, string[, start])<code>: searches backwards for the last occurrence of pattern in string, starting from start:</code>LASTPOS(&quot;123123&quot;, &quot;23&quot;, 4)<code>==</code>2<code></code>LINES(file)<code>: returns the number of lines typed ahead at the interactive stream:</code>push(&quot;a line&quot;); push(&quot;second line&quot;); lines(STDIN); /* == 2 */<code></code>MAX(number, number[, number,...])<code>: obvious</code>MIN(number, number[, number,...])<code>: obvious</code>OPEN(filehandle, filename[, &quot;APPEND&quot;|&quot;READ&quot;|&quot;WRITE&quot;])<code>: opens file, returns boolean for success:</code>OPEN(&quot;MyCon&quot;, &quot;CON:160/50/320/100/MyCon/CDS&quot;)<code>==</code>1<code></code>OVERLAY(new, old[, start][, length][, pad])<code>: overlays new string onto old one at start for length chars padding with pad if necessary:</code>OVERLAY(&quot;4&quot;, &quot;123&quot;, 5, 5)<code>==</code>&quot;123-4----&quot;<code></code>POS(pattern, string[, start])` : same as index</p>
```

But instead was:

```html
ERROR Problem at row 19 Expecting Problem at row 1 Expecting symbol (
```