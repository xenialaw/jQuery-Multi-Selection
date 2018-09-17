# jQuery-Multi-Selection
## Introduction & Background
This is a small jQuery plugin with out many feature but able to work with dynamic added content by JavaScript. 

There are many much powerful jQuery plugin for "multiselect" box existing on github (for detail pls refenenec from the end of this page). However, some of them cannot be worked on the dynamic content added by javascipt/jQuery and this is the reason why i write this for a project.

## License
This jQuery plugin is avavilable under MIT License.

## Demonstration
Please reference to demo/index.html in this repository or visit 
[http://www.soyosolution.com/tools/jquery_multi_selection/index.html](http://www.soyosolution.com/tools/jquery_multi_selection/index.html)

## How to use
### 1) Import css and javascript
```
<link rel="stylesheet" type="text/css" href="res/css/jquery-multi-selection.css" />
<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
<script src="res/scripts/jQueryMultiSelection.js"></script>
```
### 2) Copy html
```
<div class="jp-multiselect">
    <div class="from-panel">
        <select name="from[]" class="form-control" size="8" multiple="multiple"></select>
    </div>
   <div class="move-panel">1
        <button type="button" class="btn btn-default btn btn-default btn-move-all-right"></button>
        <button type="button" class="btn btn-default btn btn-default btn-move-selected-right"></button>
        <button type="button" class="btn btn-default btn btn-default btn-move-all-left"></button>
        <button type="button" class="btn btn-default btn btn-default btn-move-selected-left"></button>
    </div>
    <div class="to-panel">
        <select name="to[]" class="form-control" size="8" multiple="multiple"></select>
    </div>
    <div class="control-panel">
        <button type="button" class="btn btn-default btn btn-default btn-delete"></button>
        <button type="button" class="btn btn-default btn btn-default btn-up"></button>
        <button type="button" class="btn btn-default btn btn-default btn-down"></button>
    </div>
</div>
```
### 3) Initial plugin
```
<script>
$(".jp-multiselect").jQueryMultiSelection();
</script>
```

# Reference
- [https://github.com/crlcu/multiselect](https://github.com/crlcu/multiselect)
- [http://www.soyosolution.com/tools/jquery_multi_selection/index.html](http://www.soyosolution.com/tools/jquery_multi_selection/index.html)
