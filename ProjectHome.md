# tumblrBadge #
Use this JavaScript badge to present Tumblr posts in a web page. Supports text, photo, quote, link and chat posts. An example of the badge in action can be found at [the tumblrBadge demo page](http://www.robertnyman.com/tumblrbadge/tumblr-example.html).

## Settings ##
Include the script file in your page, and just set the values you want for the script to retrieve:

```
var settings = {
	userName : "robertnyman", // Your Tumblr user name
	itemsToShow : 10, // Number of Tumblr posts to retrieve
	itemToAddBadgeTo : "tumblr-badge", // Id of HTML element to put badge code into
	imageSize : 100, // Values can be 75, 100, 250, 400 or 500
	shortPublishDate : true, // Whether the publishing date should be cut shorter
	timeToWait : 2000 // Milliseconds, 1000 = 1 second
};
```

## Generated HTML ##
The generated HTML from the script is an unordered list, with link, images and em elements. It could look something like this:

```
<ul class="tumblr">
	<li>
		“I roll and i tumble, cried the whole night long”
		<em>— Muddy Waters</em>
		<a class="tumblr-post-date" href="http://robertnyman.tumblr.com/post/39813835">25 Jun 2008 19:38</a>
	</li>
	<li>
		<p>“We’re sorry, but your Gmail account is currently experiencing errors.”</p>
		<p>NO ONE wants to see such an error</p><a class="tumblr-post-date" href="http://robertnyman.tumblr.com/post/39813135">25 Jun 2008 19:32</a>
	</li>
	<li>
		“Tear here” on different packages can only be for spite
		<a class="tumblr-post-date" href="http://robertnyman.tumblr.com/post/39629828">24 Jun 2008 12:16</a>
	</li>
	<li>
		<a href="http://robertnyman.tumblr.com/post/39572421">
			<img width="100" src="http://media.tumblr.com/xTmFqJEX7al8er5sKdasUEsI_100.jpg"/>
		</a>
		<em>A morning can’t get more beautiful than this!</em>
		<a class="tumblr-post-date" href="http://robertnyman.tumblr.com/post/39572421">24 Jun 2008 01:10</a>
	</li>
	<li>
		<a href="http://robertnyman.tumblr.com/post/39569872">
			<img width="100" src="http://media.tumblr.com/xTmFqJEX7al7a8m4Bc5ASMVQ_100.jpg"/>
		</a>
		<em>Midsummer</em>
		<a class="tumblr-post-date" href="http://robertnyman.tumblr.com/post/39569872">24 Jun 2008 00:39</a>
	</li>
</ul>
```


## Example CSS to go with that ##

```
.tumblr {
	list-style: none;
	width: 150px;
	margin-bottom: 1em;
	padding: 0;
}
.tumblr li {
	margin-bottom: 1em;
}
.tumblr p {
	margin: 0;
}
.tumblr img {
	display: block;
}
.tumblr em {
	display: block;
	margin-top: 0.2em;
}
.tumblr .tumblr-post-date{
	display: block;
	font-size: 0.9em;
	margin-top: 0.5em;
}
```