<h1 id="projects"></h1>

<h2 style="margin: 30px 0px -15px;">Projects<temp style="font-size:15px;"></temp></h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.projects.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
            <abbr class="badge">{{ link.project_short }}</abbr>
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
      <div class="author">{{ link.abstract }}</div>
      <!-- <div class="periodical"><em>{{ link.project }}</em> -->
      <div class="periodical" style="text-align: justify;">{{ link.project }}
      </div>
    <div class="links">
      {% if link.pdf %} 
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
      {% endif %}
      {% if link.code %} 
      <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
      {% endif %}
      {% if link.page %} 
      <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
      {% endif %}
      {% if link.bibtex %} 
      <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
      {% endif %}
      {% if link.web %} 
      <a href="{{ link.web }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Website</a>
      {% endif %}
      {% if link.notes %}
      <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
      <!-- <strong style="color:#e74d3c">{{ link.notes }}</strong> -->
      {% endif %}
      {% if link.others %} 
      {{ link.others }}
      {% endif %}
    </div>
  </div>
</div>
</li>

<br>

{% endfor %}


<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    <img src="./assets/img/AwesomeMarp.gif" class="teaser img-fluid z-depth-1">
            <abbr class="badge">CSS Themes</abbr>
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="https://github.com/favourhong/Awesome-Marp">Awesome Marp</a></div>
      <div class="author"></div>
      <div class="periodical" style="text-align: justify;">一整套 Marp 主题，Marp 是用 Markdown 语法来渲染创作 PPT 的工具，可以在<a href="https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode"> VS Code </a>和<a href="https://obsidian.md/"> Obsidian </a>中使用。目前 v1.3 版本提供了 6 种颜色（dark、blue、green、red、yellow、brown）和 38 种自定义样式，包括 6 种页面分栏、4 种非嵌套列表的分栏、类似 Beamer 的进度导航栏、5 种类型的封面页、3 种类型的目录页和 5 种 Callouts 引用框等。</div>
    <div class="links">
      <!-- <a href="" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a> -->
      <!-- <a href="https://github.com/yaoyao-liu/meta-transfer-learning" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a> -->
      <a href="https://github.com/favourhong/Awesome-Marp" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Website</a>
      <strong><i style="color:#e74d3c">Open Source (428 GitHub Stars)</i></strong>
    </div>
  </div>
</div>
</li>

</ol>
</div>
