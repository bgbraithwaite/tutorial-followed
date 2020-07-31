# [Pure JavaScript — Building A Real-World Application From Scratch](https://medium.com/codingthesmartway-com-blog/pure-javascript-building-a-real-world-application-from-scratch-5213591cfcd6)

Tutorial followed from the article by Sebastian Eschweiler, published on January 30, 2017.

## Notes

- I was interested in this tutorial because it uses vanilla JS to solve some common business problems, rather than jumping straight to a full framework. It still uses libraries, which does indeed make a lot of sense because I am not going to wander off into rolling my own crypto or pretending I can do CSS better than Twitter. Yet.

- Tutorial uses: Bootstrap, jQuery, ChanceJS library (for UUID generation). I didn't install `live-server` manually, since I have the VSCode extension installed already, but if I were using vim or some other pure editor, I'd probably do Debian package management rather than a manual install regardless. Maybe if I were using Windows.

- I tried to only copy & paste if it was a URL or text blob. I want to pay attention to each (reusable in a different context) significant character. Also, I want to get used to my editor (VSCode on this project). I fixed minor typos in the tutorial text, and I basically ignored the tab formatting & left it to VSCode to auto-format.

## Debugging

```
SyntaxError: missing ; before statement[Learn More]  main.js:21:92
ReferenceError: fetchIssues is not defined[Learn More]  CodingTheSmartWay:1:1
	onload http://127.0.0.1:5500/CodingTheSmartWay/:1:1
```

So I fixed my errors after submitting a test ticket and viewing the JS Console in Firefox.

Error 1 was typing:

```
'<a href="#" class="btn btn-danger" onclick="deleteIssue(\''id+'\')">Delete</a>'+
```

instead of:

```
'<a href="#" class="btn btn-danger" onclick="deleteIssue(\''+id+'\')">Delete</a>'+
```

That missing `+` really got me.

```
ReferenceError: chance is not defined[Learn More]  main.js:29:9
TypeError: issues is null[Learn More]  main.js:7:21
```

Error 2 is something to do with the the ChangeJS library. Hokay.

So I learned that the original guy made a `chance.js` file with the appropriate stuff in it. I uh. Don't know. So I just copied the file from the [github repo](https://github.com/seeschweiler/jsissuetracker) and altered the `src` in `index.html`, and it works now. Woo!?!?

## Things I Don't Understand (Yet)

- **Why all `div`s?** Maybe it's a Bootstrap thing? Or force of habit? I feel like some of these could have been more semantically useful on their face, although the form elements all seemed pretty straightforward.

- **Why all `var`s?** I'm guessing from ES6 not fully supported in 2017. This could be a quick practice rewrite for ES6 once I get more knowledge & practice under my belt?

- **"Finally, we need to execute e.preventDefault() to avoid that the default submission of the form is taking place."** ... what?

- I don't understand the `chance.js` business not working.

## Enlightenment?

- I definitely am feeling that building an HTML skeleton upon which all the JS hangs is a huge part of what I will be doing for a living.

- I followed all of the JS except for that `e` variable magic.

- It works! Eventually! Hooray! Now on to the fuller thing. And also to make this a proper git repo.
