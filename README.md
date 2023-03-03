![Mi-Table](./assets/mitable.png)
# Mi-Table a Full-Featured datatable made with Javascript by Florian L&auml;mmlein
#### Creates an interactive table.
#### The Mi-Table script has over 20 functions in the current stable version witch you can use.
&nbsp;
&nbsp;
## Mi-Table Features
- Easy to use, super fast and smooth.
- Sort with default order.
- Multiple fixed headers.
- Pagination.
- Scrollbar.
- And much more!

&nbsp;
&nbsp;
## Why Mi-Table
- <strong style="color: #ff6b6b;">It is much faster than any other script. (1 Mio rows in 10 ms)</strong>
- It supports much more functions than any other script.
- It uses minmal memory and cpu.
- And much more!


&nbsp;
&nbsp;
## How to get Mi-Table
- Just send me an message or click on <a href="https://www.buymeacoffee.com/flory1"><img align="right" src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=flory1&button_colour=FFDD00&font_colour=000000&font_family=Cookie&outline_colour=000000&coffee_colour=ffffff" /></a>

&nbsp;
&nbsp;
## All config <a id="options">options</a> in the Mi-Table
| <strong style="color: #6ba0ff;">Option</strong> | <strong style="color: #6ba0ff;">Attribute</strong> | <strong style="color: #6ba0ff;">Special</strong> | <strong style="color: #6ba0ff;">Description</strong> | <strong style="color: #6ba0ff;">Type</strong> | <strong style="color: #6ba0ff;">Default value</strong> |
| --- | --- | --- | --- | --- | --- |
| `on` | | [events](#events) | Table events to call | | |
| `section` | | | Table section | | |
| | active | | Activate this option | Boolean | false |
| | check | | Holds the check options | Object | {} |
| | cell_class | | Holds the cell class if `check` is true | Object | {} |
| | cell_kwarg | | Holds the cell kwargs if `check` is true | Object | {} |
| | row_class | | Holds the row class if `check` is true | Object | {} |
| | row_kwarg | | Holds the row kwargs if `check` is true | Object | {} |
| | column_class | | Holds the column class if `check` is true | Object | {} |
| | column_kwarg | | Holds the column kwargs if `check` is true | Object | {} |
| | | | | | |
| `selection` | | | Table selection | | |
| | active | | Activate this option | Boolean | false |
| | actions | | Selection actions (`copy`, `remove`, `empty`, `duplicate`, `export`) | Array[String] | ["copy", "remove", "empty", "duplicate", "export"] |
| | maxRows | | Max selected rows | Number | 1 |
| | exportUrl | | Url to export if `export` action is set | String | "" |
| | | | | | |
| `pagination` | | | Table pagination | | |
| | active | | Activate this option | Boolean | true |
| | next | | Next and prev buttons if true (`table render is faster`) | Boolean | true |
| | class | | Classes for this option | String | "" |
| | kwargs | | Holds anything you want for this option | String | "" |
| | `buttons` | | pagination buttons | | |
| | | class | Classes for this option | String | "" |
| | | kwargs | Holds anything you want for this option | String | "" |
| | | | | | |
| `search` | | | Table search | | |
| | active | | Activate this option | Boolean | true |
| | minInputLength | |Min input length before auto search | Number | 3 |
| | inputDelay | | Input dealy time before search | Number | 500 |
| | casesens | | Case sensetive search | Boolean | true |
| | class | | Classes for this option | String | "" |
| | kwargs | | Holds anything you want for this option | String | "" |
| | | | | | |
| `length` | | | Table length | | |
| | active | | Activate this option | Boolean | true |
| | values | | Length values | Array | [10, 25, 50, -1] |
| | labels | | Length labels the -1 from `values` will be `All` | Array | [10, 25, 50] |
| | class | | Classes for this option | String | "" |
| | kwargs | | Holds anything you want for this option | String | "" |
| | | | | | |
| `sort` | | | Table sort | | |
| | active | | Activate this option | Boolean | true |
| | columns | | Columns that can be sorted | Array | null |
| | resetOrder | | Reset the order after any change on the table | Boolean | false |
| | class | | Classes for this option | String | "" |
| | kwargs | | Holds anything you want for this option | String | "" |
| | | | | | |
| `export` | | | Table export | | |
| | active | | Activate this option | Boolean | false |
| | url | | Ajay url to send the json data | String | "" |
| | class | | Classes for this option | String | "" |
| | kwargs | | Holds anything you want for this option | String | "" |
| | | | | | |
| `columns` | | | Table columns | | |
| | visableActive | | Activate the visable option | Boolean | false |
| | visable | | Columns that can be hidden dynamically | Array[Number] | null |
| | fixedActive | | Activate the fixed option | Boolean | false |
| | fixed | | Columns that can be fixed dynamically | Number | 0 |
| | calcActive | | Activate the calc option | Boolean | false |
| | `calc` | | Columns that can be calc dynamically | Array | [["", 0, ""]] |
| | | index | String inserted before the number | String | "" |
| | | index | The column index that will be calculated | Number | 0 |
| | | index | String inserted after the number | String | "" |
| | orderActive | | Activate the order option | Boolean | false |
| | order | | Columns that can be orderd dynamically | Array[Number] | null |
| | class | | Classes for this option | String | "" |
| | kwargs | | Holds anything you want for this option | String | "" |
| | | | | | |
| `cells` | | | Table cells | | |
| | editorActive | | Activate the editor option | Boolean | false |
| | editor | | Columns that can be edit dynamically | Array[Number] | null |
| | | | | | |
| `options` | | | Table options | | |
| | scroll | | Activate the table scroll | Boolean | false |
| | scrollY | | Max height of the table | String | "" |
| | scrollX | | Max width of the table | String | "" |
| | templateActive | | Use the template to render | Boolean | false |
| | template | | Table template design | String | "HL:\<l>\<e>\<o>\<se>,HR:\<v>\<s>,FL:\<f>,FR:\<p>" |
| | language | | Tabel language for any renderd text (`de`, `en`) | String | "en" |

&nbsp;
&nbsp;
## All config <a id="events">events</a> in the Mi-Table
| <strong style="color: #6ba0ff;">Event</strong> | <strong style="color: #6ba0ff;">Description</strong> |
| --- | --- |
| `initComplete` | After table is configured |
| `tableComplete` | After table is renderd |

&nbsp;
&nbsp;
## All api <a id="events">events</a> in the Mi-Table
| <strong style="color: #6ba0ff;">Event</strong> | <strong style="color: #6ba0ff;">Action</strong> | <strong style="color: #6ba0ff;">Return Params / Attributes</strong> | <strong style="color: #6ba0ff;">Description</strong> | <strong style="color: #6ba0ff;">Type</strong> |
| --- | --- | --- | --- | --- |
| `cellEditing` | `on` | row, column, valueOld, valueNew | After cell editing | Number, Number, String, String |
| `search` | `on` | value | After search | String |
| `length` | `on` | lengths | After length change | Array[Number] |
| `sort` | `on` | index, value | After sorting | Number, Number |
| `visable` | `on` | visables | After column hidde click | Array[Boolean] |
| `pagination` | `on` | page | After pagination click | Number |
| `order` | `on` | orders | After ordering | Array[Number] |
| `add` | `emit` | data | Append data to table | Array |
| `search` | `emit` | data | Search the table | String |

&nbsp;
&nbsp;
## How to use Mi-Table
### Basic example (slow):
###### &nbsp;&nbsp;&nbsp; Desc: The basic version is the old way to render the table.
```html
<link rel="stylesheet" href="designs/default.css" />
<link rel="stylesheet" href="table.css" />

<table id="example">
    <thead>
        <tr>
            <th>Name</th>
            <th>Position</th>
            <th>Office</th>
            <th>Age</th>
            <th>Start date</th>
            <th>Salary</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Tiger Nixon</td>
            <td>System Architect</td>
            <td>Edinburgh</td>
            <td>61</td>
            <td>2011-04-25</td>
            <td>$320,800</td>
        </tr>
        ...
    </tbody>
</table>

<script src="table.js"></script>
<script>
    window.onload = function () {
        new Table("example");
    };
</script>
```
&nbsp;
### Data example (fast):
###### &nbsp;&nbsp;&nbsp; Desc: The data version is the standard way to render the table.
```html
<link rel="stylesheet" href="designs/default.css" />
<link rel="stylesheet" href="table.css" />

<table id="example">
    <thead>
        <tr>
            <th>Name</th>
            <th>Position</th>
            <th>Office</th>
            <th>Age</th>
            <th>Start date</th>
            <th>Salary</th>
        </tr>
    </thead>
</table>

<script src="table.js"></script>
<script>
    window.onload = function () {
        new Table("example", {}, [
            ["Tiger Nixon", "System Architect", "Edinburgh", "61", "2011-04-25", "$320,800"]
        ]);
    };
</script>
```
&nbsp;
### Data Object example (fastest):
###### &nbsp;&nbsp;&nbsp; Desc: The Object version is the new way to render the table.
```html
<link rel="stylesheet" href="designs/default.css" />
<link rel="stylesheet" href="table.css" />

<table id="example">
    <thead>
        <tr>
            <th>Name</th>
            <th>Position</th>
            <th>Office</th>
            <th>Age</th>
            <th>Start date</th>
            <th>Salary</th>
        </tr>
    </thead>
</table>

<script src="table.js"></script>
<script>
    window.onload = function () {
        new Table("example", {}, [
            {data: ["Tiger Nixon", "System Architect", "Edinburgh", "61", "2011-04-25", "$320,800"]}
        ]);
    };
</script>
```
&nbsp;
### Options example:
###### &nbsp;&nbsp;&nbsp; Desc: Setup all [options](#options) you want.
```html
<link rel="stylesheet" href="designs/default.css" />
<link rel="stylesheet" href="table.css" />

<table id="example">
    <thead>
        <tr>
            <th>Name</th>
            <th>Position</th>
            <th>Office</th>
            <th>Age</th>
            <th>Start date</th>
            <th>Salary</th>
        </tr>
    </thead>
    ...data
</table>

<script src="table.js"></script>
<script>
    window.onload = function () {
        new Table("example", {
            pagination: {
                class: "text-danger"
            },
            search: {
                casesens: false
            },
            sort: {
                columns: [0, 2]
            }
        }, ...data);
    };
</script>
```
&nbsp;
### Config events example:
###### &nbsp;&nbsp;&nbsp; Desc: Setup all [options](#options) you want.
```html
<link rel="stylesheet" href="designs/default.css" />
<link rel="stylesheet" href="table.css" />

<table id="example">
    <thead>
        <tr>
            <th>Name</th>
            <th>Position</th>
            <th>Office</th>
            <th>Age</th>
            <th>Start date</th>
            <th>Salary</th>
        </tr>
    </thead>
    ...data
</table>

<script src="table.js"></script>
<script>
    window.onload = function () {
        let startTimer = performance.now();
        new Table("example", {
            on: {
                initComplete: () => {
                    let endTimer = performance.now();
                    console.log(`Table took: ${endTimer - startTimer} ms`);
                }
            }
            ...
        }, ...data);
    };
</script>
```
&nbsp;
### Api Events example:
###### &nbsp;&nbsp;&nbsp; Desc: Setup all [options](#options) you want.
```html
<link rel="stylesheet" href="designs/default.css" />
<link rel="stylesheet" href="table.css" />

<table id="example">
    <thead>
        <tr>
            <th>Name</th>
            <th>Position</th>
            <th>Office</th>
            <th>Age</th>
            <th>Start date</th>
            <th>Salary</th>
        </tr>
    </thead>
    ...data
</table>

<script src="table.js"></script>
<script>
    window.onload = function () {
        let table = new Table("example", {
            ...
        }, ...data);
        table.on("cellEditing", (row, column, valueOld, valueNew) => {
            console.log(row, column, valueOld, valueNew);
        });
        table.on("search", (value) => {
            console.log(value);
        });
    };
</script>
```
&nbsp;
### Section example:
###### &nbsp;&nbsp;&nbsp; Desc: Setup all [options](#options) you want.
```html
<link rel="stylesheet" href="designs/default.css" />
<link rel="stylesheet" href="table.css" />

<style>
    .text-warning {
        color: orange;
    }
    .text-danger {
        color: #db1e1e;
    }
    .text-success {
        color: #1cd61c;
    }
    .font {
        font-style: italic;
    }
</style>

<table id="example">
    <thead>
        <tr>
            <th>Name</th>
            <th>Position</th>
            <th>Office</th>
            <th>Age</th>
            <th>Start date</th>
            <th>Salary</th>
        </tr>
    </thead>
    ...data
</table>

<script src="table.js"></script>
<script>
    window.onload = function () {
        new Table("example", {
            section: {
                active: true,
                check: {2: {str: "Edinburgh"}, 3: {str: "61"}, 0: {str: "Ashton Cox"}, 1: {str: "Sales Assistant"}, 5: {int: ["<200000", ">300000"]}},
                cell_class: {2: "text-warning", 5: ["text-danger", "text-success"]},
                cell_kwarg: {3: "style='color: red;'"},
                row_class: {3: "font"},
                row_kwarg: {0: "style='background: #c7c7c7;'"},
                column_class: {},
                column_kwarg: {1: "style='background: #d1b3b3;'", 3: "style='color: blue;'"},
            },
            ...
        }, ...data);
    };
</script>
```
&nbsp;
&nbsp;
## Legacy versions
This version of the Mi-Table are the current stable version which is supported for feature updates.

## Do you have any Ideas, Changes or Bugs ?
Please let me know in the Comments, i will try to fix or add what you found/want :D
