Write a comment abouth the test here.
*** Parameters: ***
{}
*** Markdown input: ***
CSS: style.css

Input:
     <em>Emphasis</em>
Result: <em>Emphasis</em>

Input:
	<img src="http://jigsaw.w3.org/css-validator/images/vcss"/>
Result on span: <img src="http://jigsaw.w3.org/css-validator/images/vcss"/>

Result alone: 

<img src="http://jigsaw.w3.org/css-validator/images/vcss"/>

Without closing:

<img src="http://jigsaw.w3.org/css-validator/images/vcss">

<div markdown="1">
	This is *true* markdown text (paragraph)

	<p markdown="1">
		This is *true* markdown text (no paragraph)
	</p>
</div>

<table>
<tr>
<td markdown="1">This is *true* markdown text. (no par)</td>
<td markdown="block">This is *true* markdown text. (par)</td>
</tr>
</table>


The following is invalid HTML, and will generate an error:

<table>
<td markdown="1">This is *true* markdown text. (no par)</td>
<td markdown="block">This is *true* markdown text. (par)</td>
</tr>
</table>


*** Output of inspect ***
#<Maruku:0x111eaf8 @refs={}, @node_type=:document, @toc=Master
, @children=[#<MDElement:0x1114ee0 @node_type=:paragraph, @doc=#<Maruku:0x111eaf8 ...>, @children=["Input: ", #<MDElement:0x111a674 @node_type=:raw_html, @doc=#<Maruku:0x111eaf8 ...>, @children=[], @meta={:raw_html=>"<em>Emphasis</em> Result: <em>Emphasis</em>"}>], @meta={}>, #<MDElement:0x110cd80 @node_type=:paragraph, @doc=#<Maruku:0x111eaf8 ...>, @children=["Input: ", #<MDElement:0x11125f0 @node_type=:raw_html, @doc=#<Maruku:0x111eaf8 ...>, @children=[], @meta={:parsed_html=><UNDEFINED> ... </>, :raw_html=>"<img src=\"http://jigsaw.w3.org/css-validator/images/vcss\"/>"}>, " Result on span: ", #<MDElement:0x1110700 @node_type=:raw_html, @doc=#<Maruku:0x111eaf8 ...>, @children=[], @meta={:parsed_html=><UNDEFINED> ... </>, :raw_html=>"<img src=\"http://jigsaw.w3.org/css-validator/images/vcss\"/>"}>], @meta={}>, #<MDElement:0x110aee0 @node_type=:paragraph, @doc=#<Maruku:0x111eaf8 ...>, @children=["Result alone:"], @meta={}>, #<MDElement:0x110ab70 @node_type=:raw_html, @doc=#<Maruku:0x111eaf8 ...>, @children=[], @meta={:parsed_html=><UNDEFINED> ... </>, :raw_html=>"<img src=\"http://jigsaw.w3.org/css-validator/images/vcss\" />"}>, #<MDElement:0x1107da8 @node_type=:paragraph, @doc=#<Maruku:0x111eaf8 ...>, @children=["Without closing:"], @meta={}>, #<MDElement:0x1107bb4 @node_type=:raw_html, @doc=#<Maruku:0x111eaf8 ...>, @children=[], @meta={:parsed_html=><UNDEFINED> ... </>, :raw_html=>"<img src=\"http://jigsaw.w3.org/css-validator/images/vcss\" />"}>, #<MDElement:0x1106728 @node_type=:raw_html, @doc=#<Maruku:0x111eaf8 ...>, @children=[], @meta={:parsed_html=><UNDEFINED> ... </>, :raw_html=>"<div markdown=\"1\">\n\tThis is *true* markdown text (paragraph)\n\n\t<p markdown=\"1\">\n\t\tThis is *true* markdown text (no paragraph)\n\t</p>\n</div>"}>, #<MDElement:0x11047ac @node_type=:raw_html, @doc=#<Maruku:0x111eaf8 ...>, @children=[], @meta={:parsed_html=><UNDEFINED> ... </>, :raw_html=>"<table>\n<tr>\n<td markdown=\"1\">This is *true* markdown text. (no par)</td>\n<td markdown=\"block\">This is *true* markdown text. (par)</td>\n</tr>\n</table>"}>, #<MDElement:0x11004f4 @node_type=:paragraph, @doc=#<Maruku:0x111eaf8 ...>, @children=["The following is invalid HTML, and will generate an error:"], @meta={}>, #<MDElement:0x10ff4a0 @node_type=:raw_html, @doc=#<Maruku:0x111eaf8 ...>, @children=[], @meta={:raw_html=>"<table>\n<td markdown=\"1\">This is *true* markdown text. (no par)</td>\n<td markdown=\"block\">This is *true* markdown text. (par)</td>\n</tr>"}>, #<MDElement:0x10fc818 @node_type=:raw_html, @doc=#<Maruku:0x111eaf8 ...>, @children=[], @meta={:raw_html=>"</table>"}>], @doc=#<Maruku:0x111eaf8 ...>, @abbreviations={}, @stack=[], @meta={:css=>"style.css"}, @footnotes={}>
*** Output of to_html ***
<p>Input: <pre class='markdown-html-error' style='border: solid 3px red; background-color: pink'>HTML parse error: 
&lt;em&gt;Emphasis&lt;/em&gt; Result: &lt;em&gt;Emphasis&lt;/em&gt;</pre
    ></p
    ><p>Input: <img src='http://jigsaw.w3.org/css-validator/images/vcss'
      /> Result on span: <img src='http://jigsaw.w3.org/css-validator/images/vcss'
      /></p
    ><p>Result alone:</p
    ><img src='http://jigsaw.w3.org/css-validator/images/vcss'
    /><p>Without closing:</p
    ><img src='http://jigsaw.w3.org/css-validator/images/vcss'
    /><div
      ><p>This is <em>true</em
        > markdown text (paragraph)</p
      ><p>This is <em>true</em
        > markdown text (no paragraph)</p
    ></div
    ><table>
<tr>
<td>This is <em>true</em
          > markdown text. (no par)</td
        >
<td
          ><p>This is <em>true</em
            > markdown text. (par)</p
        ></td
        >
</tr
      >
</table
    ><p>The following is invalid HTML, and will generate an error:</p
    ><pre class='markdown-html-error' style='border: solid 3px red; background-color: pink'>HTML parse error: 
&lt;table&gt;
&lt;td markdown=&quot;1&quot;&gt;This is *true* markdown text. (no par)&lt;/td&gt;
&lt;td markdown=&quot;block&quot;&gt;This is *true* markdown text. (par)&lt;/td&gt;
&lt;/tr&gt;</pre
    ><pre class='markdown-html-error' style='border: solid 3px red; background-color: pink'>HTML parse error: 
&lt;/table&gt;</pre
  >
*** Output of to_latex ***
Input: {\bf Raw HTML removed in latex version }

Input: {\bf Raw HTML removed in latex version } Result on span: {\bf Raw HTML removed in latex version }

Result alone:

{\bf Raw HTML removed in latex version }Without closing:

{\bf Raw HTML removed in latex version }{\bf Raw HTML removed in latex version }{\bf Raw HTML removed in latex version }The following is invalid HTML, and will generate an error:

{\bf Raw HTML removed in latex version }{\bf Raw HTML removed in latex version }
*** Output of to_s ***
Input: Input:  Result on span: Result alone:Without closing:The following is invalid HTML, and will generate an error:
*** Output of to_md ***
Input: Input:  Result on span: Result alone:Without closing:The following is invalid HTML, and will generate an error:
*** EOF ***



	OK!



*** Output of Markdown.pl ***
<p>CSS: style.css</p>

<p>Input:
     <em>Emphasis</em>
Result: <em>Emphasis</em></p>

<p>Input:
    <img src="http://jigsaw.w3.org/css-validator/images/vcss"/>
Result on span: <img src="http://jigsaw.w3.org/css-validator/images/vcss"/></p>

<p>Result alone: </p>

<p><img src="http://jigsaw.w3.org/css-validator/images/vcss"/></p>

<p>Without closing:</p>

<p><img src="http://jigsaw.w3.org/css-validator/images/vcss"></p>

<div markdown="1">
    This is *true* markdown text (paragraph)

    <p markdown="1">
        This is *true* markdown text (no paragraph)
    </p>
</div>

<table>
<tr>
<td markdown="1">This is *true* markdown text. (no par)</td>
<td markdown="block">This is *true* markdown text. (par)</td>
</tr>
</table>

<p>The following is invalid HTML, and will generate an error:</p>

<table>
<td markdown="1">This is *true* markdown text. (no par)</td>
<td markdown="block">This is *true* markdown text. (par)</td>
</tr>
</table>

*** Output of Markdown.pl (parsed) ***
Error: #<REXML::ParseException: #<REXML::ParseException: Missing end tag for 'img' (got "p")
Line: 
Position: 
Last 80 unconsumed characters:
  <div markdown="1">     This is *true* markdown text (paragraph)      <p markdow>
/Volumes/Alter/Ruby/local/lib/ruby/1.8/rexml/parsers/baseparser.rb:315:in `pull'
/Volumes/Alter/Ruby/local/lib/ruby/1.8/rexml/parsers/treeparser.rb:21:in `parse'
/Volumes/Alter/Ruby/local/lib/ruby/1.8/rexml/document.rb:190:in `build'
/Volumes/Alter/Ruby/local/lib/ruby/1.8/rexml/document.rb:45:in `initialize'
bin/marutest:116:in `new'
bin/marutest:116:in `run_test'
bin/marutest:180:in `marutest'
bin/marutest:178:in `each'
bin/marutest:178:in `marutest'
bin/marutest:248
...
Missing end tag for 'img' (got "p")
Line: 
Position: 
Last 80 unconsumed characters:
  <div markdown="1">     This is *true* markdown text (paragraph)      <p markdow
Line: 
Position: 
Last 80 unconsumed characters:
  <div markdown="1">     This is *true* markdown text (paragraph)      <p markdow>