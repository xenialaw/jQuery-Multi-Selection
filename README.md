# jQuery-Multi-Selection

This is a small jQuery plugin with out many feature but able to work with dynamic added content by JavaScript. 

There are many much powerful jQuery plugin for "multiselect" box existing on github (for detail pls refenenec from the end of this page). However, some of them cannot be worked on the dynamic content added by javascipt/jQuery and this is the reason why i write this for a project.

## Demonstration

Please reference to demo/index.html in this repository or visit 
[http://www.soyosolution.com/tools/jquery_multi_selection/index.html](http://www.soyosolution.com/tools/jquery_multi_selection/index.html)

## Getting Started

### Prerequisites

JavaScript library jQuery is required to used.

### Installing

Add these few lines to your webpage to import required CSS and JavaScript:

```
<link rel="stylesheet" type="text/css" href="res/css/jquery-multi-selection.css" />
<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
<script src="res/scripts/jQueryMultiSelection.js"></script>
```

Copy the html
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

Initial plugin
```
<script>
$(".jp-multiselect").jQueryMultiSelection();
</script>
```

An example you can reference is index.html in this repository.

## Configuration

You can pass an object to this plugin for configuration, an example:

```
$("#dynamic-form").jQueryMultiSelection({
    ajaxSourceUrl : "http://www.soyosolution.com/tools/jquery_multi_selection/github/dist/list.json",
    enableDynamicAddContent : true,
});
```
### Parameters

Let's look on list of all available parameters:

| Parameter               | Type                    | Default                  | Description                                                   |
|-------------------------|-------------------------|--------------------------|---------------------------------------------------------------|
| enableDynamicAddContent | boolean                 | false                    | If you want add content dynamicly (load json), set as true    |         
| ajaxSourceUrl           | string                  | ../dist/list.json        | Extental json file path.                                      |
| btnGetJson              | jQuery selector string  | #btn-ajax                | Text display on button which execute dynamicly add json. |
| selectMeunFrom          | jQuery selector string  | .from-panel select       | Select menu on left panel. |
| selectMeunTo            | jQuery selector string  | .to-panel select         | Select menu on right panel. |
| btnMoveAllRight         | jQuery selector string  | .btn-move-all-right      | Button element for user move all items from left panel  to right panel. |
| btnMoveSelectedRight    | jQuery selector string  | .btn-move-selected-right | Button element for user move selected item from left panel to right panel. |
| btnMoveAllLeft          | jQuery selector string  | .btn-move-all-left       | Button element for user move all items from right panel to left panel. |
| btnMoveSelectedLeft     | jQuery selector string  | .btn-move-selected-left  | Button element for user move selected item from right panel to left panel. |
| btnDelete               | jQuery selector string  | .btn-delete              | Button element to delete selected item in right panel   |
| btnMoveUp               | jQuery selector string  | .btn-up                  | Button element to changing the order: move up |
| btnMoveDown             | jQuery selector string  | .btn-down                | Button element to changing the order: move down |
| htmlMoveAllRight        | string                  | &rsaquo;&rsaquo;         | Text display on button which move all items to right panel. |
| htmlMoveSelectedRight   | string                  | &rsaquo;                 | Text display on button which move selected item to right panel. |
| htmlMoveAllLeft         | string                  | &lsaquo;&lsaquo;         | Text display on button which move all items to left panel. |
| htmlMoveSelectedLeft    | string                  | &lsaquo;                 | Text display on button which move selected item to left panel. |
| htmlDelete              | string                  | Delete                   | Text display on button execute delete action. |
| htmlMoveUp              | string                  | Up                       | Text display on button execute move up action. |
| htmlMoveDown            | string                  | Down                     | Text display on button execute move down action. |

## Built With

* [jQuery 2.2.4](https://jquery.com/) - The JavaScript library used.

## Authors

* **Adrian Crisan** - *Initial work* - [crlcu](https://github.com/crlcu/multiselect)
* **Xenia L.C Law** - *This amendment* - [xenialaw](https://github.com/xenialaw)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
