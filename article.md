Hypertext Markup Language
=========================

Nature of Project
-----------------


The HTML specification intends to maintain and improve the HTML standard. 

The standard had been left idle since 1999, with no subsequent revisions. The [World Wide Web Consortium](http://www.w3c.org), the standards body for components of the web, had been moving toward an [(http://www.w3.org/TR/xml/) eXtensible Markup Language] vision for the web, where everything would be recast in a pure format using a pure specification. The first step was to bridge between [HTML 4.01](http://www.w3.org/TR/html401/), the last HTML standard (recommended on Dec. 24, 1999), and [XHTML1](http://www.w3.org/TR/xhtml1/), the first XML-compatible version of HTML (recommended by the W3C on Jan. 26, 2000). It merely [tightened up the syntax](http://acmeous.blogspot.com/2010/12/difference-between-xhtml-and-html4.html), the way of writing, HTML. Nothing new was added at that time. It was part of a wave of adhering to standards, in response to the browser wars. 

[XHTML 1.1]((http://www.w3.org/TR/xhtml11/) became a W3C recommendation on May 31, 2001. This was pure XML. A web server could not serve this to a web browser as HTML anymore, as Ian Hickson of Opera Software explained at the time, there are [(http://www.hixie.ch/advocacy/xhtml issues serving XHTML as HTML and not XML]. [Microsoft Internet Explorer](http://blogs.msdn.com/b/ie/archive/2005/09/15/467901.aspx), the web browser with the [largest market share at the time](http://www.thecounter.com/stats/2001/May/browser.php) (78%), could not render XML properly as  `DOCTYPE application/xml+xhtml` but could if it served as `DOCTYPE text/html`. There was the appearance that the W3C was not in touch with reality.

The tipping point came with XHTML 2. It was a pure language: without  any baggage from prior work [nor backward compatible with either current web content nor HTML](http://web.mit.edu/jmorzins/www/xhtml/dive.html). This seemed to be [at odds with the average user or designer](http://www.zeldman.com/2009/07/02/xhtml-wtf/#comment-43970). The clearest example of this was XHTML 2's replacement of the `img` tag with the `object` tag. Though the `object` tag was  "better" in how it handled content through multiple regressions through content types supported by the browser when necessary, it was putting more work into the page parsing, which would need to declare the content type of the embedded object, rather than the web server just working with the content type of the file. That, and, IE6 [did not support](http://web.mit.edu/jmorzins/www/xhtml/dive.html) the `object` tag.

The Oct. 14, 2003 [proposal for XForms](http://www.w3.org/TR/2003/REC-xforms-20031014/), a technology offered as the next version of web forms, [renewed browser makers' interest in improving HTML](http://developer.practicalecommerce.com/articles/1589-Interview-with-Ian-Hickson-on-the-HTML-5-Specification), rather than replacing it. This was mainly because implementers realized XML was mainly used for new technologies like [RSS](http://feed2.w3.org/docs/rss2.html) and Atom, than replacing existing technologies like HTML. [Web Forms 2.0](http://www.whatwg.org/specs/web-forms/2004-06-27-call-for-comments/) was created as a proof of concept and [proposed](http://www.hixie.ch/specs/html/forms/xforms-basic-1) that the new form technologies could be deployed without creating a whole new rendering engine.

At the Jun 1-2, 2004 [W3C Workshop on Web Applications and Compound Documents](http://www.w3.org/2004/04/webapps-cdf-ws/), Ian Hickson, then at Opera Software, proposed extending HTML to create web applications. This was based on Mozilla Foundation and Opera Software [position paper](http://www.w3.org/2004/04/webapps-cdf-ws/papers/opera.html) presented on the [afternoon of Jun 1, 2004](http://www.w3.org/2004/04/webapps-cdf-ws/minutes-20040601.html#topic18). The W3C rejected this on a [8 to 11 vote](http://www.w3.org/2004/04/webapps-cdf-ws/summary).

Members from Apple, Opera and Mozilla decided to create a new group to meet this need, the [Web Hypertext Application Technology Working Group](http://www.whatwg.org). They [announced the creation of the group and its mailing list on Jun. 4, 2004](http://www.whatwg.org/news/start).

Working in almost an opposite methodology than the W3C's consensus mode, WHATWG gave one editor the right to decide what went into the standard. This was done to expedite changes and move the standard along. This worked well and progress was made into what was then called HTML5. Ian Hickson, in an [interview with Practical eCommerce on Jan. 22, 2010](http://developer.practicalecommerce.com/articles/1589-Interview-with-Ian-Hickson-on-the-HTML-5-Specification), noted that the WHATWG followed a different mantra than the standards purists:

> "Many members of the standards community strongly believe that what matters is the standards, and that if the implementations don't follow the standards then the problem is by definition with the implementations. The WHATWG core principles say otherwise: the spec is just a means to an end, so if the implementations don't match the spec, that's as much a failing of the spec as of the implementations."

The W3C continued to develop XHTML 2 but progress was going nowhere fast. On Oct. 27, 2006, Tim Berners-Lee wrote [Reinventing HTML](http://dig.csail.mit.edu/breadcrumbs/node/166) in a blog post, admitting that the move to XML was not working:

> "Some things are clearer with hindsight of several years. It is necessary to evolve HTML incrementally. The attempt to get the world to switch to XML, including quotes around attribute values and slashes in empty tags and namespaces all at once didn't work."

On March 7, 2007, the W3C formed a [new charter](http://www.w3.org/2007/03/HTML-WG-charter.html) for an [HTML Working Group](http://www.w3.org/html/wg/). They adopted the work from WHATWG as the start of their work, but schizophrenically still continued to work on XHTML 2. The W3C [announced the expiration of the XHTML 2 charter](http://www.w3.org/News/2009#entry-6601) on Jul. 2, 2009. The XHTML 2 working charter [was not renewed and expired](http://www.w3.org/News/2009#item119) on Dec. 31, 2009. 

Now, the two groups continued to work in uneasy concert. On Oct. 27, 2009, WHATWG considered their [draft of HTML5 at the Last Call stage](http://blog.whatwg.org/html5-at-last-call).

The WHATWG group then realized that they could not keep going in a version development fashion and moved to an [unversioned development model](http://lists.whatwg.org/pipermail/whatwg-whatwg.org/2009-December/024477.html). This moved the WHATWG group to working on HTML as a "Living Standard". The logic used was simple: no browser developer developed a browser to meet an entire standard; they developed a browser to use features within a standard. Therefore, why use an artificial number to encapsulate a group of features that give developers and users an assumptive basis for their browsing experience?

This lead to a cacophony of protests, but, in practice, changed nothing as to how the group functioned. Nothing can be added to the standard until an implementer, a browser developer, produces an application that uses the feature proposed. This means that the standard is grounded in reality; whatever is proposed demonstrably *works*. 

Expertise of Participants
-------------------------

Apple Inc., the Mozilla Corporation and Opera Software started the WHATWG. Prominent and influential members of those companies, and now Google, constitute the membership of this working group. 

- From Opera Software:
	- [H�kon Wium Lie](http://people.opera.com/howcome/), CTO; used to work for Tim Berners-Lee, creator of the Web, at both CERN, then the W3C
	- [Anne van Kesteren](http://annevankesteren.nl/about), Developer
- From Apple Inc.:
	- [David Hyatt](http://en.wikipedia.org/wiki/Dave_Hyatt), Architect of Safari and the open-source WebKit framework
	- [Maciej Stachowiak](http://en.wikipedia.org/wiki/Maciej_Stachowiak), Developer for WebKit
- From the Mozilla Corporation:
	- [Brendan Eich](http://brendaneich.com/), CTO; creator of JavaScript
	- [David Baron](http://dbaron.org/), Developer
	- [Johnny Stenb�ck](http://en.wikipedia.org/wiki/Johnny_Stenb�ck), Developer
- From Google Inc.:
	- [Ian Hickson](http://ian.hixie.ch/), Standards Development and the Editor of the HTML standard
		- He worked at Opera and proposed to the W3C extending of HTML to create web applications. They voted him down. He then pushed for the formation of the WHATWG
- and
	- [Dean Edwards](http://dean.edwards.name/about/), JavaScript programmer known for many innovative implementations, including one that allows IE7, IE8 and IE9 to function as standards-compliant browsers
		- (No, I cannot find any reference via the web as to where he works.)

Technologies Used
-----------------

The [WHATWG Web Site](http://www.whatwg.org) serves as a single starting point about the WHATWG's work. 

Contributors submit their issues, concerns or proposals through a mailing list that they join, which uses the Python-based [MailMan](http://www.gnu.org/software/mailman/index.html) software. When changes are made and committed to the [Subversion]-based versioning system, they are updated automatically to the [HTML Tracker](http://html5.org/tools/web-apps-tracker) and simultaneously posted to the [WHATWG Twitter Feed](http://twitter.com/#!/WHATWG). 

They use a [WordPress](http://www.wordpress.org) blog called the [WHATWG Blog](http://blog.whatwg.org) that provides a review and aggregation of the week's revisions, proposals and issues from the various mailing lists. This is updated every Monday, usually by [Anne van Kesteren](http://annevankesteren.nl/about). 

Questions on the use of the standard are managed through the [WHATWG Forums](http://forums.whatwg.org), which uses  [phpBB](http://www.phpbb.org).

Development and Work Practices
------------------------------

Contributors send email to the editor through the [whatwg mailing list](http://lists.whatwg.org/htdig.cgi/whatwg-whatwg.org/). The editor reviews this [feedback](http://www.whatwg.org/issues/), along with his own research, other studies and feedback from other sources. Issues raised may get the attention of the editor faster if they are voted as popular. The editor then revises the specification that meet as broad a set of needs as possible while staying true to the language.

Changes that the editor accepts are entered as Revisions to the standard and, thus, into the Subversion repository, which will be viewable via the [HTML Tracker](http://html5.org/tools/web-apps-tracker) as well as the repository. These changes are then sent out via the Commit Watchers mailing list. Non-editorial changes are sent simultaneously via the [WHATWG Twitter Feed](http://twitter.com/#!/whatwg). 

The HTML Tracker which highlights the changes to the specification through a web interface to view of a Subversion repository. Within the HTML Tracker, each requested change is colored or highlighted in particular ways:

- All Revisions are highlighted in `background-color:#eee`.
- Revisions that are purely editorial are in gray text.
- The remaining types of Revision imply where the Revision is along the maturity (i.e. vetted, discussed) continuity:
	- Draft Content Revisions are in black text.
	- Stable Draft Revisions are highlighted in `background-color:#fcc`.
	- Stable Revisions are highlighted in `background-color:#f66`.
	- Revisions Implemented in one or more Browsers are highlighted in `background-color:#f99`. The browser that implements the change is also shown to the left of the change title.

This continues until no one is able to convince the editor to make any further revisions. This may be the case because two parties in conflict want differing implementations and the editor has already decided. There is no concensus. There is no voting. Not everyone will be happy.

This practice was selected to keep development moving forward. 

The editor may be overriden or replaced at the discretion of the [Members](http://www.whatwg.org/charter#members), and then only if they no longer believe he is making good decisions. The Members are added by invitation only.

Additional mailing lists for [Web Designer help](http://lists.whatwg.org/htdig.cgi/help-whatwg.org/) and [HTML Implementors](http://lists.whatwg.org/htdig.cgi/help-whatwg.org/) also exist to discuss issues with using and rendering HTML respectively.

====Other Communications Channels====

[WHATWG Facebook Page](http://www.facebook.com/#!/pages/WHATWG/116109708402918)
