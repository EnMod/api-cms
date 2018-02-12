# Using any raw HTML API to make the world's smallest CMS

Turn any html page into a Markdown-driven CMS using services such as [txti.es](http://txti.es) or [Canvas](https://usecanvas.com), with just 25 lines of JavaScript. 

## Step 1

Create an HTML file. Each element that you would like to populate with HTML from an API call should get an attribute of `data-src="http://item's.html.endpoint/here"`.  Additionally, add a `data-srv="serviceName"` attribute to change how the JS will parse the received data:
- For txti.es: `txti` or leave blank as this is the default
- For Canvas: `canvas`

If you haven't created the desired site content yet on your preferred service, do so in this step.

## Step 2

Include the `api-cms` script above the `</body>` tag of your HTML file. You're done! You should get nice, clean HTML delivered from your request. (You can also include or paste the code from the api-cms.min.js file for a compressed version)

Because this solution requires JavaScript, it's recommended you put some helpful text with a link to the hosted entry inside of the element in case the user has JavaScript disabled. By requesting raw HTML you shouldn't have any dynamic components, such as JavaScript, so make sure your preferred service's entry is publicly visible.


