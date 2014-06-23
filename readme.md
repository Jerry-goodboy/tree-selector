# Tree Selector

Bootstrap tabanlı hiyerarşik seçim listesi.

### Gereksinimler

* `jQuery 1.7.2`
* `bootstrap 3`
* `underscore 1.3.3`

### Kullanım

```html
<link href="/src/tree-selector.css" rel="stylesheet">
<script type="text/javascript" src="/src/tree-selector.js"></script>

<div class="listTree"></div>

<script type="text/javascript">

var data = [
    {
        "key": "parent1",
        "title": "Parent 1"
        "values": [
            { 
            	"key": "parent1.child1",
            	"title": "Parent 1 Child 1"
            },
            { 
            	"key": "parent1.child1",
            	"title": "Parent 1 Child 2" 
            },
        ]
    },
    {
        "key": "parent2",
        "title": "Parent 2"
        "values": []
    }
];

var dataDefaultSelected = [
    {
        "key": "parent1",
        "title": "Parent 1"
        "values": [
            { 
            	"key": "parent1.child2",
            	"title": "Parent 1 Child 2"
            },
        ]
    },
];

$('.listTree').listTree(data, { "startCollapsed": true, "selected": dataDefaultSelected });
</script>
```

### Metotlar


#### destroy()
Objeyi yok edebilirsiniz.
```javascript
$('.listTree').listTree('destroy');​
```

#### selectAll()
Tüm checkbox elemanlarını işaretli konuma getirebilirsiniz.
```javascript
$('.listTree').listTree('selectAll');​
```

#### deselectAll()
Tüm checkbox elemanlarının işaretlerini kaldırabilirsiniz.
```javascript
$('.listTree').listTree('deselectAll');​
```

#### expandAll()
Tüm seçemekleri genişletebilirsiniz.
```javascript
$('.listTree').listTree('expandAll');​
```

#### collapseAll()
Tüm seçenekleri daraltabilirsiniz.
```javascript
$('.listTree').listTree('collapseAll');​
```

#### update()
Var olan verileri yenileri ile güncelleyebilirsiniz.
```javascript
$('.listTree').listTree('update', someOtherDataObj, someOtherDataOptions);​
```

## Lisans
GPL

