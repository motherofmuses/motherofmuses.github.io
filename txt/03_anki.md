There are many 

Front Template:
``` 
{% raw %}
{{cloze:Text}}
{% endraw %}
``` 

Back Template:
``` 
{% raw %}
{{edit:cloze:Text}}
<hr>
{{edit:Extra}}

{{#More}}
<hr>
<a class=more href="#"onclick="this.style.display='none';
document.getElementById('more_back').style.display='inline-block';
return false;"
>Mehr</a>
<div id="more_back" class=more style="display: none">{{edit:More}}</div>
{{/More}}
{% endraw %}
``` 

Styling:

``` 
{% raw %}
.card {
    font-family: arial;
    font-size: 20px;
    text-align: center;
    color: black;
    background-color: #d3d3d3;
}

.nightMode .card {
   color: white;
   background-color: #2F2F31;
}

.cloze {
    font-weight: bold;
    color: blue;
}

.nightMode .cloze {
    color: lightblue;
}

.mobile .night_mode .cloze {
    color: lightblue;
}

body ul, body ol, body dl {
    text-align: left;
    display: inline-block;
    margin-bottom: 0;
}

.more {
  padding: 6px 40px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  border-radius: 6px;
  background-color: white; 
  color: black;
  border: 1px solid black;
  transition-duration: 0.3s;
}

.more:hover {
  background-color: transparent;
  border: 1px solid transparent;
  color: black;
}

.nightMode .more:hover {
  color: white;
}

#more_back {
    all: initial;
    * { all: unset; }
    margin-top: 7px;
    padding-top: 7px;
    color: inherit;
    font-family: inherit;
    font-size: inherit;
    text-align: center;
}

.mobile .night_mode #more_back {
    color: white;
}
{% endraw %}
``` 

[<< Back](../index.md)
