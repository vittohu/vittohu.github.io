<!DOCTYPE HTML>
<html lang="en">

<head>
  <title>{{ site.name }}</title>

  <meta content="text/html; charset=utf-8" http-equiv="Content-Type">

  <meta name="author" content="{{ site.name }}" />
  <meta name="viewport" content="width=device-width, initial-scale=1">

  <link rel="stylesheet" type="text/css" href="{{ site.baseurl }}/style.css" />
  <link rel="canonical" href="{{ page.url | replace:'index.html','' | prepend: site.baseurl | prepend: site.url }}">
  <link href="https://fonts.googleapis.com/css?family=Lato:400,700,400italic,700italic" rel="stylesheet" type="text/css">

</head>



<body>
  <table style="width:100%;max-width:800px;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
    <tr style="padding:0px">
      <td style="padding:0px">
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
          <tr style="padding:0px">
            <td style="padding:2.5%;width:60%;vertical-align:middle">
              <h1>
                Weitao Hu（胡伟涛）
              </h1>
              <p>I am a graduate student at the <a href="http://rlab.sia.cas.cn/">State Key Laboratory of Robotics</a>, part of the <a href="http://www.sia.cn/">Shenyang Institute of Automation</a> at <a href="https://www.ucas.ac.cn/">University of Chinese Academy of Sciences</a>, where I work on compliant control. My master advisor is <a href="https://people.ucas.ac.cn/~panxinan">Xinan Pan</a>.
              </p>
              <p>
                I received my B.Eng. degree from <a href="https://www.csu.edu.cn/">Central South University</a>.
              </p>
              <p style="text-align:center">
                <a target="_blank" href="huweitao@sia.cn"> Email</a> &nbsp;/&nbsp;
                <a href="https://github.com/vittohu">GitHub</a> &nbsp;/&nbsp;
                <!-- <a href="https://scholar.google.com/citations?user=GCYG4GoAAAAJ">Google Scholar</a> &nbsp;/&nbsp;
                <a href="https://www.linkedin.com/in/lkeselman"> LinkedIn </a> -->
              </p>
            </td>
            <td style="padding:2.5%;width:40%;max-width:40%">
              <img style="width:100%;max-width:100%" alt="profile photo" src="images/hwt.jpg">
            </td>
          </tr>
        </table>


        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
          <tr>
            <td style="padding:2.5%;width:100%;vertical-align:middle">
              <h2>Research</h2>
              <p>
                I'm interested in robotics.
              </p>
            </td>
          </tr>
        </table>
        <!--
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">

          {% for post in site.posts %}
          {% for cat in post.categories %}
          {% if cat == 'research' %}
          <tr>
            <td style="padding:2.5%;width:25%;vertical-align:middle;min-width:120px">
              <img src="/tn{{post.image}}" alt="project image" style="width:auto; height:auto; max-width:100%;" />
            </td>
            <td style="padding:2.5%;width:75%;vertical-align:middle">
              <h3>{{post.title}}</h3>
              <br>
              {{post.authors}}

              <br>
              <em>{{post.venue}}</em>, {{ post.date | date: "%Y" }}
              <br>
              {% if post.arxiv %}
              <a href="{{post.arxiv}}">arxiv</a> /
              {% endif %}
              {% if post.video %}
              <a href="{{post.video}}">video</a> /
              {% endif %}
              {% if post.code %}
              <a href="{{post.code}}">code</a> /
              {% endif %}
              {% if post.poster %}
              <a href="{{post.poster}}">poster</a> /
              {% endif %}
              {% if post.slides %}
              <a href="{{post.slides}}">slides</a> /
              {% endif %}
              <p></p>
              {{ post.excerpt }}
            </td>
          </tr>
          {% endif %}
          {% endfor %}
          {% endfor %}
        </table>
        <br>
        <br>
        <br>
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
          <tr>
            <td style="padding:2.5%;width:100%;vertical-align:middle">
              <h2>Publications</h2>
              <p>Besides my work on the RealSense depth sensors and the publications above, a sampling of my publicly disclosed work
              </p>
            </td>
          </tr>
        </table>
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">

          {% for post in site.posts %}
          {% for cat in post.categories %}
          {% if cat == 'Publications' %}
          <tr>
            <td style="padding:2.5%;width:25%;vertical-align:middle;min-width:120px">
              <img src="/tn{{post.image}}" alt="project image" style="width:auto; height:auto; max-width:100%;" />
            </td>
            <td style="padding:2.5%;width:75%;vertical-align:middle">
              <h3>{{post.title}}</h3>
              <br>
              <em>{{post.categories}} {{post.course}}</em>
              <br>
              {{ post.date | date: "%Y-%m-%d" }}

              <br>
              {% if post.website %}
              <a href="{{post.website}}">website</a> /
              {% endif %}
              {% if post.paper %}
              <a href="{{post.paper}}">paper</a> /
              {% endif %}
              {% if post.patent %}
              <a href="{{post.patent}}">patent</a> /
              {% endif %}
              {% if post.patent2 %}
              <a href="{{post.patent2}}">patent #2</a> /
              {% endif %}
              {% if post.patent3 %}
              <a href="{{post.patent3}}">patent #3</a> /
              {% endif %}
              {% if post.video %}
              <a href="{{post.video}}">video</a> /
              {% endif %}
              {% if post.video2 %}
              <a href="{{post.video2}}">video #2</a> /
              {% endif %}
              {% if post.code %}
              <a href="{{post.code}}">code</a> /
              {% endif %}
              {% if post.poster %}
              <a href="{{post.poster}}">poster</a> /
              {% endif %}
              {% if post.slides %}
              <a href="{{post.slides}}">slides</a> /
              {% endif %}
              <p></p>
              {{ post.excerpt }}
            </td>
          </tr>
          {% endif %}
          {% endfor %}
          {% endfor %}
        </table>
        <br>
        <br>
        <br>
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
          <tr>
            <td style="padding:2.5%;width:100%;vertical-align:middle">
              <h2>Honors and Awards</h2>
            </td>
          </tr>
        </table>
        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">

          {% for post in site.posts %}
          {% for cat in post.categories %}
          {% if cat = 'Honor' or cat = 'Award' %}
          <tr>
            <td style="padding:2.5%;width:25%;vertical-align:middle;min-width:120px">
              <img src="/tn{{post.image}}" alt="project image" style="width:auto; height:auto; max-width:100%;" />
            </td>
            <td style="padding:2.5%;width:75%;vertical-align:middle">
              <h3>{{post.title}}</h3>
              <br>
              <em>{{post.categories}} {{post.course}}</em>
              <br>
              {{ post.date | date: "%Y-%m-%d" }}

              <br>
              {% if post.website %}
              <a href="{{post.website}}">website</a> /
              {% endif %}
              {% if post.paper %}
              <a href="{{post.paper}}">paper</a> /
              {% endif %}
              {% if post.patent %}
              <a href="{{post.patent}}">patent</a> /
              {% endif %}
              {% if post.patent2 %}
              <a href="{{post.patent2}}">patent #2</a> /
              {% endif %}
              {% if post.patent3 %}
              <a href="{{post.patent3}}">patent #3</a> /
              {% endif %}
              {% if post.video %}
              <a href="{{post.video}}">video</a> /
              {% endif %}
              {% if post.video2 %}
              <a href="{{post.video2}}">video #2</a> /
              {% endif %}
              {% if post.code %}
              <a href="{{post.code}}">code</a> /
              {% endif %}
              {% if post.poster %}
              <a href="{{post.poster}}">poster</a> /
              {% endif %}
              {% if post.slides %}
              <a href="{{post.slides}}">slides</a> /
              {% endif %}
              <p></p>
              {{ post.excerpt }}
            </td>
          </tr>
          {% endif %}
          {% endfor %}
          {% endfor %}
        </table>        -->

        <table style="width:100%;border:0px;border-spacing:0px;border-collapse:separate;margin-right:auto;margin-left:auto;">
          <tr>
            <td style="padding:0px">
              <br>
              <p style="text-align:center;font-size:small;">
                Design and source code from <a style="font-size:small;" href="https://jonbarron.info">Jon Barron's website</a>
              </p>
            </td>
          </tr>
        </table>
      </td>
    </tr>
  </table>
</body>

</html>
