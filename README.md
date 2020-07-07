# github-markdown-testing
What are the limits of Github's markdown?

Github uses a whitelist for its markdown filtering. This can be found [here](https://github.com/github/html-pipeline/blob/master/lib/html/pipeline/sanitization%5Ffilter%2Erb)

# Visual Whitelist

## Headers 
h[1-8] 
<h1>Header</h1>
<h2>Header</h2>
<h3>Header</h3>
<h4>Header</h4>
<h5>Header</h5>
<h6>Header</h6>
<h7>Header</h7>
<h8>Header</h8>

## Breaks 
br
START<br>END

## Characters
b 
<b>word</b>

i 
<i>word</i>

strong
<strong>word</strong>

em
<em>word</em>

a
<a href="https://www.github.com">
<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2F78.media.tumblr.com%2F64e0843979e6458d8ed9eca74633a8db%2Ftumblr_onfjuwH2LC1v4ks6xo1_500.jpg">
</a>

<a href="https://www.github.com">Go to Github</a>

<a href="https://sampleswap.org/samples-ghost/VOCAL%20ACAPELLAS/Andres%20Franco/9836[kb]andrew-franco-Sola-Solita-cc-by.mp3.mp3">An audio file</a>

<a href="javascript:alert('Hello World!');">Execute JavaScript</a>

pre
 <div style="width:200px;overflow:auto;color:red">
<pre>smol text</pre>
</div>
 
<input type="button">
<input type="checkbox">
<input type="color">
<input type="date">
<input type="email">
<input type="datetime-local">
<input type="file">
<input type="radio">
<input type="range">
<input type="reset">
<input type="url">
Blink <blink>BLINK!</blink>
Keyboard <kbd>KeYbOaRd</kbd>
 <form oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  <input type="range" id="a" value="50">
  +<input type="number" id="b" value="25">
  =<output name="x" for="a b"></output>
</form> 
