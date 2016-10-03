
<div class="editor-content">

	<p>Here you can download all of the <abbr title="Global Experience Language"><a href="http://sldigitalhub.com/digital-playbooks/accessibility/Pages/default.aspx">GEL</a>br> boilerplate assets including <a href="http://sass-lang.com/">SASS</a>, <a href="http://sldigitalhub.com/digital-playbooks/accessibility/Pages/CSS-and-Markup.aspx">CSS</a>, Javascript, images and webfonts. An example index.html file with the correct asset references is also included</p>

	<a href="https://github.com/SLDG/gel/archive/0.2.2.zip" class="btn btn--primary btn--icon no-external">

		Download Version 0.2.2

		<i class="icon icon-download"></i>

	</a>

	<h2>

		Updating the Styleguide

	</h2>

	<p>The styleguide is constructed using <a href="http://warpspire.com/kss/"><abbr title="Knyle Style Sheets">KSS</abbr></a> documentation within the <a href="http://sass-lang.com/">SASS</a> files. To rebuild the styleguide after making updates, you will need to install  <a href="http://howtonode.org/introduction-to-npm"><abbr title="Node Package Manager">npm</abbr></a> and <a href="https://github.com/hughsk/kss-node#installation">kss-node</a>.

	<p>To rebuild the styleguide, run these commands:</p>

	<pre>cd PATH_TO_PATTERNS_DIRECTORY</pre>

	<pre>kss-node content/sass --template styleguide-template/ --css content/css/all.css</pre>

	<p>The updated styleguide can then be viewed by opening <code>styleguide/index.html</code> in a browser.</p>

	<h2>Github</h2>

	<p>The code is hosted in a <a href="http://github.com/SLDG/gel">Github repository</a>.</p>


	<p>To find out more information about using git with Github, see the <a href="https://help.github.com/articles/set-up-git">Github help </a>.</p>

	<h3>Creating a Github Release</h3>

	<p>To create a release of the boilerplate code, add a tag:</p>

	<pre>git tag v0.1.9</pre>

	<p>Create a zip file of the content folder with an index.html including references for <a href="http://sldigitalhub.com/digital-playbooks/accessibility/Pages/CSS-and-Markup.aspx">CSS</a>, Javascript and any other assets required.</p>

	<p>Then <a href="https://github.com/SLDG/gel/releases/new">create a release </a> for the tag version and upload the zip file.</p>

	<p>Once the release has been created, the download link in the styleguide should be updated.</p>


	<h2>Code guidelines</h2>

	<h3>About the patterns</h3>

	<p>A responsive system to support Standard Life designers, developers and teams to begin the build of products, apps and services based on a core collection of flexible consistent elements. </p>

	<h3>CSS and Sass</h3>

	<p>The site's <a href="http://sldigitalhub.com/digital-playbooks/accessibility/Pages/CSS-and-Markup.aspx">CSS</a> is compiled and minified using <a href="http://sass-lang.com/">Sass </a>. Two files are compiled from many: all.css and all-old-ie.css. All.css is served to all modern browsers and uses a responsive grid and media queries.All-old-ie.css is served only to IE8 (and below although IE versions before 8 are not officially supported) and uses a fixed width grid with no media queries. The <a href="http://sass-lang.com/">SASS</a> code is split between many files so it easy to find the code you need.</p>

	<p>The <a href="http://sldigitalhub.com/digital-playbooks/accessibility/Pages/CSS-and-Markup.aspx">CSS</a> is built in a modular way and covers a huge variety of design patterns, so adding <a href="http://sldigitalhub.com/digital-playbooks/accessibility/Pages/CSS-and-Markup.aspx">CSS</a> will be needed often. If you are adding new <a href="http://sldigitalhub.com/digital-playbooks/accessibility/Pages/CSS-and-Markup.aspx">CSS</a> for a new section of the site, create a new partial <a href="http://sass-lang.com/">SASS</a> file (preceded by an underscore, .scss filetype) and add it to the sass directory. Then open all.scss and add a new import with the name of your file. Add it at the end of the file.</p>

	<p><a href="http://sass-lang.com/">Learn more about installing and compiling Sass</a></p>

	<h3>Mixins</h3>

	<p>The <a href="http://sass-lang.com/">SASS</a> code contains several mixins and variables to make development easier, quicker and more consistent. Look in sass/mixins.css for the full list.</p>

	<h4>Examples</h4>

	<pre>@include border-radius(4px);</pre>

	<p>becomes</p>

	<pre>
-moz-border-radius: 4px;
-webkit-border-radius: 4px;
-ms-border-radius: 4px;
border-radius: 4px;
	</pre>

</div>

