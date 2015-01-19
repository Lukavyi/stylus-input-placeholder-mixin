# stylus-input-placeholder-mixin
A mixin for stylus to style placeholder content on input html elements

### Add this to your stylus base file
<pre><code>placeholder()
	&::-webkit-input-placeholder
		{block}
	&:-moz-placeholder
		{block}
	&::-moz-placeholder
		{block}
	&:-ms-input-placeholder
		{block}
</code></pre>

### Examble usage:
ps: DONT FORGET TO ADD THE "+" SIGN BEFORE THE MIXIN NAME!!!
<pre><code>input[type="submit"]
	+placeholder()
		color #fff
</code></pre>

### Outputs as:
<pre><code>.contact input[type='submit']::-webkit-input-placeholder {
	color: #fff;
}

.contact input[type='submit']:-moz-placeholder {
	color: #fff;
}

.contact input[type='submit']::-moz-placeholder {
	color: #fff;
}

.contact input[type='submit']:-ms-input-placeholder {
	color: #fff;
}
</code></pre>
