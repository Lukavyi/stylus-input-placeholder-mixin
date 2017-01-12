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
<pre><code>
.contact
	input
		+placeholder()
			color #fff
</code></pre>
The reason behind + sign: http://stylus-lang.com/docs/mixins.html#block-mixins

### Outputs as:
<pre><code>.contact input::-webkit-input-placeholder {
	color: #fff;
}

.contact input:-moz-placeholder {
	color: #fff;
}

.contact input::-moz-placeholder {
	color: #fff;
}

.contact input:-ms-input-placeholder {
	color: #fff;
}
</code></pre>
