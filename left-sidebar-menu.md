# Main navigation

Left (in the ltr) sidebar specification. Facebook-like, it will have a number of small innovations across it to improve user experience and content discovery. 

{% method %} 

#### Collapse - expand

Navigation is responsible. We start with just 2 sizes responsive support that will work for "collapse" and "expand" states.

{% sample lang="js" -%}

* [ ] Deliberate (user-initiated) collapse/expand (this tiny long thing near the globe icon - it's height signifies what size is currently on.
* [ ] Animation for collapse-expand effect has to be well defined and worked through. 
* [ ] Logic of smart text titles / links (see XL Size and "4 new posts")

{% sample lang="go" -%}

* [ ] Animation in extra large titles (could be marque)
* [ ] Specifications for color schemes in [Colors](/colors.md)
* [ ] "Small" version of left sidebar navigation has to open on small screens (tablets and smaller) by default. This needs to be described and well tested.
* [ ] Possible switch to san francisco display font.
* [ ] Possible custom icons (user set/suggested)

{% common -%}

* [ ] Notification-in-menu (numbers of unread items in each menu item (see "4" next to News Feed)

----
| Collapse expand |
| ------------- |
| [![](/assets/Collapse-expand.png)](https://drive.google.com/a/lokieducation.org/file/d/0B-3RQRY3AlLUbmlHVlR1dzRKdWM/view?usp=sharing) |

{% endmethod %}