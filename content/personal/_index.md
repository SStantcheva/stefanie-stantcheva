+++
title = "Personal"
weight = 0
+++


## Personal

[Xinyue Lin](https://xinyue-lin.com) - behavioral economist in training

## Recent Blog Posts

<div id="blog_posts">
<p>Loading</p>
</div>

<script>
function loadPosts() {
  var xhttp = new XMLHttpRequest();
  var posts_list = document.getElementById("blog_posts");
  xhttp.onreadystatechange = function() {
    if (this.readyState == 4 && this.status == 200) {
      var resp = JSON.parse(this.responseText)
      var posts = resp['posts']
      while (posts_list.hasChildNodes()) {
        posts_list.removeChild(posts_list.firstChild);
      }
      var ul_item = document.createElement("ul");

      for (i in posts) {
        if (i >= 5) {
	  break;
	}
        var li_item = document.createElement("li");
        var post_rellink = posts[i]['rellink']
        var post_title = posts[i]['title']
        var post_date_obj = new Date(posts[i]['date'])
        var post_date = post_date_obj.toLocaleDateString("en-US")
        li_item.innerHTML = `<a href="https://blog.leiy.me${post_rellink}" target="blank">${post_title}</a> - ${post_date}`;
        ul_item.appendChild(li_item);
      }
      posts_list.appendChild(ul_item);
    }
    else if (this.readyState == 4 && this.status != 200) {
      posts_list.innerHTML = "<p>Unable to load from <a href=\"https://blog.leiy.me\">blog.leiy.me</a></p>.";
    }
  };
  xhttp.open("GET", "https://blog.leiy.me/index.json", true);
  xhttp.send();
}
loadPosts()
</script>

## Misc

Random stuff I created. Enjoy!
