---
layout: post
title: Markdown Syntax
---


<!-- ![_config.yml]({{ site.baseurl }}/images/config.png) -->
<!-- ![Image description](/images/my-image.jpg) -->
<!-- https://guides.github.com/features/mastering-markdown/  --> 


| Test | Test | Test |
| -----|:----:|-----:|
| test | test | test |
| test | test | test |
| test | test | test |
| test | test | test |


~~good~~  
2^(nd) time  
==highlighted==  
"quote"  
This is a sentence. [^1]  
[^1]: This is a footnote.  





[Daring Fireball Markdown documentation](https://daringfireball.net/projects/markdown/basics)  

If you want some text to show up exactly as you write it, without Markdown doing anything to it, just indent every line by at least 4 spaces (or 1 tab). As an alternative to indenting, you can use 4 or more tildes before and after the text. See examples in the [Code Highlighting](http://sourceforge.net/p/necessitas/wiki/markdown_syntax/#md_ex_code) section

    This line won't *have any markdown* formatting applied.
    I can even write <b>HTML</b> and it will show up as text.
    This is great for showing program source code, or HTML or even
    Markdown. <b>this won't show up as HTML</b> but
    exactly <i>as you see it in this text file</i>.



<br />

<span style="font-size: 14px; color: red; font-family: Georgia"> &lt;span&gt; style="font-size: 14px; color:red; font-family:Georgia" &#47;&lt;span&gt;</span>

CSS is set in _reset.scss in the ../myblog/_sass directory 
<p id="smallfont">&lt;p&gt; id="smallfont"&#47;&lt;p&gt;</p
<div class="tinyfont"> &lt;p&gt;class="tinyfont"&#47;&lt;p&gt;</div>


Markdown provides backslash escapes for the following characters:

\   backslash  
`   backtick  
*   asterisk  
_   underscore  
{}  curly braces  
[]  square brackets  
()  parentheses  
\#   hash mark  
\+   plus sign  
\-   minus sign (hyphen)  
.   dot  
!   exclamation mark  


    You can use grave accent to escape angle bracket `<blink>` tags.

This is another regular paragraph.



A First Level Header  
=====   
&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;&#61;

A Second Level Header  
------------  
&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;  




#  #This is an \<h1\> tag  
##  ##This is an \<h2\> tag  
###  ###This is an \<h3\> tag  
####  ####This is an \<h4\> tag
#####  #####This is an \<h5\> tag
######  ######This is an \<h6\> tag  


Use asterriks around words for &#42; *italic* &#42;.  
Use underscore around words for &#95;_italic also_&#95;.  

Use two asterisks for &#42;&#42; **strong emphasis**&#42;&#42; .  
Or, if you prefer, &#95;&#95;__use two underscores instead__&#95;&#95;.  


<s>&lt;s&gt;this is strikethrough text&lt;&#47;s&gt;</s>  
&#126;&#126;~~this is strikethrough also~~&#126;&#126;




I wish SmartyPants used named entities like `&mdash;`  
instead of decimal-encoded entites like `&#8212;`.  

URL links
=== 

\[This is an inline link \] \(http://example.com/  "Title") - [This is an inline link](http://exmaple.com/ "Title")

\[This is has no title attribute  \] \(http://example.com/) - [This is an inline link wtih no title attribute](http://exmaple.com/)

I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"



> This is a blockquote.
> 
> This is the second paragraph in the blockquote.
>
> ## This is an H2 in a blockquote



### Code block

Use  
> &#96;&#96;&#96;  java  
>  if (isAwesome){  
>    return true  
>  }  
> &#96;&#96;&#96;    

``` java
if (isAwesome){
  return true
}
```
    
    * an asterisk starts an unordered list
    * and this is another item in the list
    + or you can also use the + character
    - or the - character
    
    To start an ordered list, write this:
    
    1. this starts a list *with* numbers
    +  this will show as number "2"
    *  this will show as number "3."
    9. any number, +, -, or * will keep the list going.
        * just indent by 4 spaces (or tab) to make a sub-list
            1. keep indenting for more sub lists
        * here i'm back to the second level
     
 * an asterisk starts an unordered list
 * and this is another item in the list
 + or you can also use the + character
 - or the - character
 
 To start an ordered list, write this:
 
 1. this starts a list *with* numbers
 +  this will show as number "2"
 *  this will show as number "3."
 9. any number, +, -, or * will keep the list going.
     * just indent by 4 spaces (or tab) to make a sub-list
         1. keep indenting for more sub lists
     * here i'm back to the second level
 


### Code with <lauguage> line&#35;#

&#123;&#37; highlight ruby linenos &#37;&#125;
>def show
>  @widget = Widget(params[:id])  
>  respond_to do |format|  
>    format.html # show.html.erb  
>    format.json { render json: @widget }  
>  end  
>end    

&#123;&#37; endhighlight &#37;&#125;

{% highlight ruby linenos %}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}
