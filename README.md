**Maintainer:** Gus Esquivel <br />
**Plugin Website:** https://github.com/gesquive/bootstrap-add-clear <br />
**Contributers:**
<a href="https://github.com/skorecky">Stephen Korecky</a>,
<a href="https://github.com/scoman81">scoman81</a>,
<a href="https://github.com/Steve887">Steve887</a>,
<a href="https://github.com/Deividy">Deividy</a>

<br />

## About
This project is a fork of Stephen Korecky's "[Add Clear](https://github.com/skorecky/Add-Clear)" project. It is meant to work as a drop-in replacement when using bootstrap.

## Getting Started
How you acquire bootstrap-add-clear is up to you.
#### Bower
Install with [Bower](http://bower.io/):
```bash
bower install bootstrap-add-clear
```

#### Github
Clone the [boostrap-add-clear repository](https://github.com/gesquive/bootstrap-add-clear/):
```bash
git clone git@github.com:gesquive/bootstrap-add-clear.git
```

#### Direct Download
 * [zip](https://github.com/gesquive/bootstrap-add-clear/archive/master.zip)
 * [tarbell](https://github.com/gesquive/bootstrap-add-clear/archive/master.tar.gz)
 * Individual Files
    * [bootstrap-add-clear.js](https://raw.githubusercontent.com/gesquive/bootstrap-add-clear/master/bootstrap-add-clear.js)
    * [bootstrap-add-clear.min.js](https://raw.githubusercontent.com/gesquive/bootstrap-add-clear/master/bootstrap-add-clear.min.js)

**Note**: bootstrap-add-clear has a dependency on jquery 1.8+ and Bootstrap 3

### Available Options

<table>
  <tr>
    <th>Option</th>
    <th>Type</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>closeSymbol</td>
    <td>string</td>
    <td></td>
  </tr>
  <tr>
    <td>symbolClass</td>
    <td>string</td>
    <td>glyphicon glyphicon-remove-circle</td>
  </tr>
  <tr>
    <td>wrapperClass</td>
    <td>string</td>
    <td></td>
  </tr>
  <tr>
    <td>top</td>
    <td>number</td>
    <td>0</td>
  </tr>
  <tr>
    <td>right</td>
    <td>number</td>
    <td>0</td>
  </tr>
  <tr>
    <td>returnFocus</td>
    <td>boolean</td>
    <td>true</td>
  </tr>
  <tr>
    <td>showOnLoad</td>
    <td>boolean</td>
    <td>false</td>
  </tr>
  <tr>
    <td>clearOnEscape</td>
    <td>boolean</td>
    <td>true</td>
  </tr>
  <tr>
    <td>hideOnBlur</td>
    <td>boolean</td>
    <td>false</td>
  </tr>
  <tr>
    <td>onClear</td>
    <td>function</td>
    <td>null</td>
  </tr>
</table>

#### Using Options
```javascript
$("input").addClear({top : -2, right : 6});

// Example onClear option usage
$(":input").addClear({
  onClear: function(){
    alert("call back!");
  }
});

// Example font awesome icon usage
$(":input").addClear({
    symbolClass: "fa fa-times-circle"
})
```
