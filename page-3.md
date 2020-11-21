---
title: Page with menubar
subtitle: Demo page with a menubar
layout: page
show_sidebar: false
menubar: example_menu
---

This is another sample page showing how a page can look with a menubar. 

## Displaying a menubar

The menubar gets its content from a data file in your site's `_data` directory. Simply set the name of your data file in the page's menubar setting in the frontmatter. 

```yml
title: Page with menubar
subtitle: Demo page with a menubar
layout: page
show_sidebar: false
menubar: example_menu
```

You will probably want to disable the show_sidebar otherwise there will be little room for the page's content. 

## Creating a menubar data file

Create a data file in the _data directory and use the following format (if using yml)

```yml
- label: Example Menu
  items:
    - name: Home
      link: /
    - name: Pages
      link: #
      items:
        - name: Page With Sidebar 
          link: /page-1/
        - name: Page Without Sidebar
          link: /page-2/
        - name: Page With Menubar
          link: /page-3/
    - name: Blog
      link: /blog/
```

### Multiple menus

You may make multiple menus in the same file, separated by the label

```yml
- label: Menu Label
  items:
    - name: Example item
      link: /example-item/
- label: Second Menu Label
  items:
    - name: Parent Item
      link: /parent-item/
      items:
        - name: Sublink 
          link: /sublink/
        - name: Sublink 2
          link: /sublink2/
- label: Third Menu Label
  items:
    - name: Another example item
      link: /another-example-item/
```

VIX 지수

<iframe id="tvc_frame_2cf3b5e506b91583c59f24e22e2232df" seamless="seamless" src="//tvcharts.investing.com/init.php?&carrier=bd2f7e982318ba67fb3f00d60919668c&time=1604386012&domain_ID=18&lang_ID=18&timezone_ID=88&pair_ID=44336&interval=86400&refresh=30&session=session&client=&user=guest&init_page=instrument&m_pids=&watchlist=&site=https://kr.investing.com" width="100%" height="500"></iframe>
