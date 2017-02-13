# bootstrap4-upgrade-guide
A Guide of how to UPGRADE bootstrap from v3 to v4

## Changes of some common classes

### pull-(left|right)
In some earlier version of bootstrap4 (before alpha.5),  
`pull-(left|right)` is replaced by `pull-(xs|sm|md|lg|xl)-(left|right)`  
so that you can design different layouts reponsively.  

However, it is modified again in alpha.5 and you should use  
`float-(xs|sm|md|lg|xl)-(left|right)`  

Simply, you can use the replacement below:
```
pull-left  => float-xs-left
pull-right => float-xs-right
```
## Changes of some elements

### \<dl\> tag
> `.dl-horizontal` has been dropped. Instead, use `.row` on `<dl>` and use grid column classes (or mixins) on its `<dt>` and `<dd>` children.

### .btn-xs
> Dropped the `.btn-xs` class entirely as `.btn-sm` is proportionally much smaller than v3’s.

```
btn-xs => btn-sm
```
