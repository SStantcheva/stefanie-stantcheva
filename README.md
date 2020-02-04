### Stefanie Stantcheva's Website - Documentation

This website was built using Hugo, the Academimal theme for Hugo and elements from Lei Yang's and Gautam Rao's website.

**If you want to build your own website:** The simplest avenue is to [install Hugo](https://gohugo.io/getting-started/quick-start/), clone this GitHub repository to your computer, modify the parts you want to change and render it locally. You can then host it online using [Netlify](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/), [Render](https://gohugo.io/hosting-and-deployment/hosting-on-render/), [GitHub](https://gohugo.io/hosting-and-deployment/hosting-on-github/) or one of the many other services.


If you only want to change the content on the webpage, all you have to change is the `config.toml` file, the `content` folder and the `data/research/research.yaml` file. If you want to change the appearance of the website, you will need to edit the theme under `theme/academimal`. To find additionnal inspiration, you can look at [Gautam Rao's](https://gautam-rao.com/) and [Lei Yang's](https://people.csail.mit.edu/leiy/) webpages and their GitHub repositories.


**If you want to edit this website:**

- *In general:* You will need to clone this repository to your local device, make the changes you want to implement, test wether they render properly locally and online, and then [make a pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request). Stephanie Stantcheva will need to approve it.

- *To change the content of the `Home`, `Broader Audience Writing` and `Media` pages:* the content of these pages are respectively in `content/_index.md`, `content/writing/_index.md` and `content/media/_index.md`. You simply need to edit the file, which is written in [GitHub markdown](https://guides.github.com/features/mastering-markdown/).

- *To change the content of the `Research` page:* only the introduction to this page is in `content/research/_index.md`, while the articles are listed in the  `data/research/research.yaml` file. To add a new article, copy-paste one of the existing ones and change its attributes. Empty attributes sometimes lead to faulty appearance, so delete the one's you don't need. Articles are automatically put in the category of the list in which you entered them. To change an existing article, simply edit its current entry. Note: the order of the articles is the order in which they will show up, so keep it chronological; furthermore, do not put anything else than a year in YYYY under the "date" entry, otherwise the year-subtitles for publications will break.

- *To change the appearance of the whole site:* some options, notably fronts, colours and sizes can be edited in the `themes/academimal/static/css/style.css`; more complex edits will require you to change the `.html` of individual pages or of the sidebar, which is a far more convoluted process, notably because the code is spread across many different snippets. Tip: use "inspect element" in your browser and the "search" function in your computer generously.

**If you have any questions,** feel free to write to c.schesch@gmail.com.