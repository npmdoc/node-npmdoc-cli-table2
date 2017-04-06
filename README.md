# api documentation for  [cli-table2 (v0.2.0)](https://github.com/jamestalmage/cli-table2)  [![npm package](https://img.shields.io/npm/v/npmdoc-cli-table2.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cli-table2) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cli-table2.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cli-table2)
#### Pretty unicode tables for the command line. Based on the original cli-table.

[![NPM](https://nodei.co/npm/cli-table2.png?downloads=true)](https://www.npmjs.com/package/cli-table2)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cli-table2/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-cli-table2_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cli-table2/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cli-table2/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cli-table2/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Talmage"
    },
    "bugs": {
        "url": "https://github.com/jamestalmage/cli-table2/issues"
    },
    "dependencies": {
        "colors": "^1.1.2",
        "lodash": "^3.10.1",
        "string-width": "^1.0.1"
    },
    "description": "Pretty unicode tables for the command line. Based on the original cli-table.",
    "devDependencies": {
        "ansi-256-colors": "^1.1.0",
        "chai": "^3.4.1",
        "cli-table": "^0.3.1",
        "coveralls": "^2.11.4",
        "git-rev": "^0.2.1",
        "growl": "^1.8.1",
        "gulp": "^3.9.0",
        "gulp-istanbul": "^0.10.3",
        "gulp-mocha": "^2.2.0",
        "gulp-util": "^3.0.7",
        "sinon": "^1.17.2",
        "sinon-chai": "^2.8.0"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "2d1ef7f218a0e786e214540562d4bd177fe32d97",
        "tarball": "https://registry.npmjs.org/cli-table2/-/cli-table2-0.2.0.tgz"
    },
    "gitHead": "57111fff6349df8e47a3776ff9ea994ea8917e40",
    "homepage": "https://github.com/jamestalmage/cli-table2",
    "keywords": [
        "node",
        "command",
        "line",
        "cli",
        "table",
        "tables",
        "tabular",
        "unicode",
        "colors",
        "grid"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "jamestalmage",
            "email": "james@talmage.io"
        }
    ],
    "name": "cli-table2",
    "optionalDependencies": {
        "colors": "^1.1.2"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/jamestalmage/cli-table2.git"
    },
    "scripts": {
        "test": "gulp coverage"
    },
    "version": "0.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module cli-table2](#apidoc.module.cli-table2)
1.  [function <span class="apidocSignatureSpan">cli-table2.</span>cell (options)](#apidoc.element.cli-table2.cell)
1.  object <span class="apidocSignatureSpan">cli-table2.</span>cell.prototype
1.  object <span class="apidocSignatureSpan">cli-table2.</span>layout_manager
1.  object <span class="apidocSignatureSpan">cli-table2.</span>utils

#### [module cli-table2.cell](#apidoc.module.cli-table2.cell)
1.  [function <span class="apidocSignatureSpan">cli-table2.</span>cell (options)](#apidoc.element.cli-table2.cell.cell)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.</span>ColSpanCell ()](#apidoc.element.cli-table2.cell.ColSpanCell)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.</span>RowSpanCell (originalCell)](#apidoc.element.cli-table2.cell.RowSpanCell)

#### [module cli-table2.cell.prototype](#apidoc.module.cli-table2.cell.prototype)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>_topLeftChar (offset)](#apidoc.element.cli-table2.cell.prototype._topLeftChar)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>draw (lineNum, spanningCell)](#apidoc.element.cli-table2.cell.prototype.draw)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>drawBottom (drawRight)](#apidoc.element.cli-table2.cell.prototype.drawBottom)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>drawEmpty (drawRight, spanningCell)](#apidoc.element.cli-table2.cell.prototype.drawEmpty)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>drawLine (lineNum, drawRight, forceTruncationSymbol, spanningCell)](#apidoc.element.cli-table2.cell.prototype.drawLine)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>drawTop (drawRight)](#apidoc.element.cli-table2.cell.prototype.drawTop)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>init (tableOptions)](#apidoc.element.cli-table2.cell.prototype.init)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>mergeTableOptions (tableOptions, cells)](#apidoc.element.cli-table2.cell.prototype.mergeTableOptions)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>setOptions (options)](#apidoc.element.cli-table2.cell.prototype.setOptions)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>stylizeLine (left, content, right)](#apidoc.element.cli-table2.cell.prototype.stylizeLine)
1.  [function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>wrapWithStyleColors (styleProperty, content)](#apidoc.element.cli-table2.cell.prototype.wrapWithStyleColors)
1.  object <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>x
1.  object <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>y

#### [module cli-table2.layout_manager](#apidoc.module.cli-table2.layout_manager)
1.  [function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>addRowSpanCells (table)](#apidoc.element.cli-table2.layout_manager.addRowSpanCells)
1.  [function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>computeHeights (vals, table)](#apidoc.element.cli-table2.layout_manager.computeHeights)
1.  [function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>computeWidths (vals, table)](#apidoc.element.cli-table2.layout_manager.computeWidths)
1.  [function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>fillInTable (table)](#apidoc.element.cli-table2.layout_manager.fillInTable)
1.  [function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>layoutTable (table)](#apidoc.element.cli-table2.layout_manager.layoutTable)
1.  [function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>makeTableLayout (rows)](#apidoc.element.cli-table2.layout_manager.makeTableLayout)
1.  [function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>maxWidth (table)](#apidoc.element.cli-table2.layout_manager.maxWidth)

#### [module cli-table2.utils](#apidoc.module.cli-table2.utils)
1.  [function <span class="apidocSignatureSpan">cli-table2.utils.</span>colorizeLines (input)](#apidoc.element.cli-table2.utils.colorizeLines)
1.  [function <span class="apidocSignatureSpan">cli-table2.utils.</span>mergeOptions (options, defaults)](#apidoc.element.cli-table2.utils.mergeOptions)
1.  [function <span class="apidocSignatureSpan">cli-table2.utils.</span>pad (str, len, pad, dir)](#apidoc.element.cli-table2.utils.pad)
1.  [function <span class="apidocSignatureSpan">cli-table2.utils.</span>repeat (str, times)](#apidoc.element.cli-table2.utils.repeat)
1.  [function <span class="apidocSignatureSpan">cli-table2.utils.</span>strlen (str)](#apidoc.element.cli-table2.utils.strlen)
1.  [function <span class="apidocSignatureSpan">cli-table2.utils.</span>truncate (str, desiredLength, truncateChar)](#apidoc.element.cli-table2.utils.truncate)
1.  [function <span class="apidocSignatureSpan">cli-table2.utils.</span>wordWrap (maxLength, input)](#apidoc.element.cli-table2.utils.wordWrap)



# <a name="apidoc.module.cli-table2"></a>[module cli-table2](#apidoc.module.cli-table2)

#### <a name="apidoc.element.cli-table2.cell"></a>[function <span class="apidocSignatureSpan">cli-table2.</span>cell (options)](#apidoc.element.cli-table2.cell)
- description and source-code
```javascript
function Cell(options){
  this.setOptions(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cli-table2.cell"></a>[module cli-table2.cell](#apidoc.module.cli-table2.cell)

#### <a name="apidoc.element.cli-table2.cell.cell"></a>[function <span class="apidocSignatureSpan">cli-table2.</span>cell (options)](#apidoc.element.cli-table2.cell.cell)
- description and source-code
```javascript
function Cell(options){
  this.setOptions(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.cell.ColSpanCell"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.</span>ColSpanCell ()](#apidoc.element.cli-table2.cell.ColSpanCell)
- description and source-code
```javascript
function ColSpanCell(){}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.cell.RowSpanCell"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.</span>RowSpanCell (originalCell)](#apidoc.element.cli-table2.cell.RowSpanCell)
- description and source-code
```javascript
function RowSpanCell(originalCell){
  this.originalCell = originalCell;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cli-table2.cell.prototype"></a>[module cli-table2.cell.prototype](#apidoc.module.cli-table2.cell.prototype)

#### <a name="apidoc.element.cli-table2.cell.prototype._topLeftChar"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>_topLeftChar (offset)](#apidoc.element.cli-table2.cell.prototype._topLeftChar)
- description and source-code
```javascript
_topLeftChar = function (offset){
  var x = this.x+offset;
  var leftChar;
  if(this.y == 0){
    leftChar = x == 0 ? 'topLeft' : (offset == 0 ? 'topMid' : 'top');
  } else  {
    if(x == 0){
      leftChar = 'leftMid';
    }
    else {
      leftChar = offset == 0 ? 'midMid' : 'bottomMid';
      if(this.cells){  //TODO: cells should always exist - some tests don't fill it in though
        var spanAbove = this.cells[this.y-1][x] instanceof Cell.ColSpanCell;
        if(spanAbove){
          leftChar = offset == 0 ? 'topMid' : 'mid';
        }
        if(offset == 0){
          var i = 1;
          while(this.cells[this.y][x-i] instanceof Cell.ColSpanCell){
            i++;
          }
          if(this.cells[this.y][x-i] instanceof Cell.RowSpanCell){
            leftChar = 'leftMid';
          }
        }
      }
    }
  }
  return this.chars[leftChar];
}
```
- example usage
```shell
...
 * @param drawRight - true if this method should render the right edge of the cell.
 * @returns {String}
 */
Cell.prototype.drawTop = function(drawRight){
var content = [];
if(this.cells){  //TODO: cells should always exist - some tests don't fill it in though
  _.forEach(this.widths,function(width,index){
    content.push(this._topLeftChar(index));
    content.push(
      utils.repeat(this.chars[this.y == 0 ? 'top' : 'mid'],width)
    );
  },this);
}
else {
  content.push(this._topLeftChar(0));
...
```

#### <a name="apidoc.element.cli-table2.cell.prototype.draw"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>draw (lineNum, spanningCell)](#apidoc.element.cli-table2.cell.prototype.draw)
- description and source-code
```javascript
draw = function (lineNum, spanningCell){
  if(lineNum == 'top') return this.drawTop(this.drawRight);
  if(lineNum == 'bottom') return this.drawBottom(this.drawRight);
  var padLen = Math.max(this.height - this.lines.length, 0);
  var padTop;
  switch (this.vAlign){
    case 'center':
      padTop = Math.ceil(padLen / 2);
      break;
    case 'bottom':
      padTop = padLen;
      break;
    default :
      padTop = 0;
  }
  if( (lineNum < padTop) || (lineNum >= (padTop + this.lines.length))){
    return this.drawEmpty(this.drawRight,spanningCell);
  }
  var forceTruncation = (this.lines.length > this.height) && (lineNum + 1 >= this.height);
  return this.drawLine(lineNum - padTop, this.drawRight, forceTruncation,spanningCell);
}
```
- example usage
```shell
...
  var originalY = this.originalCell.y;
  this.cellOffset = y - originalY;
  this.offset = findDimension(tableOptions.rowHeights,originalY,this.cellOffset);
};

RowSpanCell.prototype.draw = function(lineNum){
  if(lineNum == 'top'){
    return this.originalCell.draw(this.offset,this.cellOffset);
  }
  if(lineNum == 'bottom'){
    return this.originalCell.draw('bottom');
  }
  return this.originalCell.draw(this.offset + 1 + lineNum);
};
...
```

#### <a name="apidoc.element.cli-table2.cell.prototype.drawBottom"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>drawBottom (drawRight)](#apidoc.element.cli-table2.cell.prototype.drawBottom)
- description and source-code
```javascript
drawBottom = function (drawRight){
  var left = this.chars[this.x == 0 ? 'bottomLeft' : 'bottomMid'];
  var content = utils.repeat(this.chars.bottom,this.width);
  var right = drawRight ? this.chars['bottomRight'] : '';
  return this.wrapWithStyleColors('border',left + content + right);
}
```
- example usage
```shell
...
 * @param lineNum - can be 'top', 'bottom' or a numerical line number.
 * @param spanningCell - will be a number if being called from a RowSpanCell, and will represent how
 * many rows below it's being called from. Otherwise it's undefined.
 * @returns {String} The representation of this line.
 */
Cell.prototype.draw = function(lineNum,spanningCell){
if(lineNum == 'top') return this.drawTop(this.drawRight);
if(lineNum == 'bottom') return this.drawBottom(this.drawRight);
var padLen = Math.max(this.height - this.lines.length, 0);
var padTop;
switch (this.vAlign){
  case 'center':
    padTop = Math.ceil(padLen / 2);
    break;
  case 'bottom':
...
```

#### <a name="apidoc.element.cli-table2.cell.prototype.drawEmpty"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>drawEmpty (drawRight, spanningCell)](#apidoc.element.cli-table2.cell.prototype.drawEmpty)
- description and source-code
```javascript
drawEmpty = function (drawRight, spanningCell){
  var left = this.chars[this.x == 0 ? 'left' : 'middle'];
  if(this.x && spanningCell && this.cells){
    var cellLeft = this.cells[this.y+spanningCell][this.x-1];
    while(cellLeft instanceof ColSpanCell){
      cellLeft = this.cells[cellLeft.y][cellLeft.x-1];
    }
    if(!(cellLeft instanceof RowSpanCell)){
      left = this.chars['rightMid'];
    }
  }
  var right = (drawRight ? this.chars['right'] : '');
  var content = utils.repeat(' ',this.width);
  return this.stylizeLine(left , content , right);
}
```
- example usage
```shell
...
   case 'bottom':
     padTop = padLen;
     break;
   default :
     padTop = 0;
 }
 if( (lineNum < padTop) || (lineNum >= (padTop + this.lines.length))){
   return this.drawEmpty(this.drawRight,spanningCell);
 }
 var forceTruncation = (this.lines.length > this.height) && (lineNum + 1 >= this.height);
 return this.drawLine(lineNum - padTop, this.drawRight, forceTruncation,spanningCell);
};

/**
* Renders the top line of the cell.
...
```

#### <a name="apidoc.element.cli-table2.cell.prototype.drawLine"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>drawLine (lineNum, drawRight, forceTruncationSymbol, spanningCell)](#apidoc.element.cli-table2.cell.prototype.drawLine)
- description and source-code
```javascript
drawLine = function (lineNum, drawRight, forceTruncationSymbol, spanningCell){
  var left = this.chars[this.x == 0 ? 'left' : 'middle'];
  if(this.x && spanningCell && this.cells){
    var cellLeft = this.cells[this.y+spanningCell][this.x-1];
    while(cellLeft instanceof ColSpanCell){
      cellLeft = this.cells[cellLeft.y][cellLeft.x-1];
    }
    if(!(cellLeft instanceof RowSpanCell)){
      left = this.chars['rightMid'];
    }
  }
  var leftPadding = utils.repeat(' ', this.paddingLeft);
  var right = (drawRight ? this.chars['right'] : '');
  var rightPadding = utils.repeat(' ', this.paddingRight);
  var line = this.lines[lineNum];
  var len = this.width - (this.paddingLeft + this.paddingRight);
  if(forceTruncationSymbol) line += this.truncate || '…';
  var content = utils.truncate(line,len,this.truncate);
  content = utils.pad(content, len, ' ', this.hAlign);
  content = leftPadding + content + rightPadding;
  return this.stylizeLine(left,content,right);
}
```
- example usage
```shell
...
   default :
     padTop = 0;
 }
 if( (lineNum < padTop) || (lineNum >= (padTop + this.lines.length))){
   return this.drawEmpty(this.drawRight,spanningCell);
 }
 var forceTruncation = (this.lines.length > this.height) && (lineNum + 1 >= this.height);
 return this.drawLine(lineNum - padTop, this.drawRight, forceTruncation,spanningCell);
};

/**
* Renders the top line of the cell.
* @param drawRight - true if this method should render the right edge of the cell.
* @returns {String}
*/
...
```

#### <a name="apidoc.element.cli-table2.cell.prototype.drawTop"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>drawTop (drawRight)](#apidoc.element.cli-table2.cell.prototype.drawTop)
- description and source-code
```javascript
drawTop = function (drawRight){
  var content = [];
  if(this.cells){  //TODO: cells should always exist - some tests don't fill it in though
    _.forEach(this.widths,function(width,index){
      content.push(this._topLeftChar(index));
      content.push(
        utils.repeat(this.chars[this.y == 0 ? 'top' : 'mid'],width)
      );
    },this);
  }
  else {
    content.push(this._topLeftChar(0));
    content.push(utils.repeat(this.chars[this.y == 0 ? 'top' : 'mid'],this.width));
  }
  if(drawRight){
    content.push(this.chars[this.y == 0 ? 'topRight' : 'rightMid']);
  }
  return this.wrapWithStyleColors('border',content.join(''));
}
```
- example usage
```shell
...
 * This default implementation defers to methods 'drawTop', 'drawBottom', 'drawLine' and 'drawEmpty'.
 * @param lineNum - can be 'top', 'bottom' or a numerical line number.
 * @param spanningCell - will be a number if being called from a RowSpanCell, and will represent how
 * many rows below it's being called from. Otherwise it's undefined.
 * @returns {String} The representation of this line.
 */
Cell.prototype.draw = function(lineNum,spanningCell){
if(lineNum == 'top') return this.drawTop(this.drawRight);
if(lineNum == 'bottom') return this.drawBottom(this.drawRight);
var padLen = Math.max(this.height - this.lines.length, 0);
var padTop;
switch (this.vAlign){
  case 'center':
    padTop = Math.ceil(padLen / 2);
    break;
...
```

#### <a name="apidoc.element.cli-table2.cell.prototype.init"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>init (tableOptions)](#apidoc.element.cli-table2.cell.prototype.init)
- description and source-code
```javascript
init = function (tableOptions){
  var x = this.x;
  var y = this.y;
  this.widths = tableOptions.colWidths.slice(x, x + this.colSpan);
  this.heights = tableOptions.rowHeights.slice(y, y + this.rowSpan);
  this.width = _.reduce(this.widths,sumPlusOne);
  this.height = _.reduce(this.heights,sumPlusOne);

  this.hAlign = this.options.hAlign || tableOptions.colAligns[x];
  this.vAlign = this.options.vAlign || tableOptions.rowAligns[y];

  this.drawRight = x + this.colSpan == tableOptions.colWidths.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.cell.prototype.mergeTableOptions"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>mergeTableOptions (tableOptions, cells)](#apidoc.element.cli-table2.cell.prototype.mergeTableOptions)
- description and source-code
```javascript
mergeTableOptions = function (tableOptions, cells){
  this.cells = cells;

  var optionsChars = this.options.chars || {};
  var tableChars = tableOptions.chars;
  var chars = this.chars = {};
  _.forEach(CHAR_NAMES,function(name){
     setOption(optionsChars,tableChars,name,chars);
  });

  this.truncate = this.options.truncate || tableOptions.truncate;

  var style = this.options.style = this.options.style || {};
  var tableStyle = tableOptions.style;
  setOption(style, tableStyle, 'padding-left', this);
  setOption(style, tableStyle, 'padding-right', this);
  this.head = style.head || tableStyle.head;
  this.border = style.border || tableStyle.border;

  var fixedWidth = tableOptions.colWidths[this.x];
  if(tableOptions.wordWrap && fixedWidth){
    fixedWidth -= this.paddingLeft + this.paddingRight;
    this.lines = utils.colorizeLines(utils.wordWrap(fixedWidth,this.content));
  }
  else {
    this.lines = utils.colorizeLines(this.content.split('\n'));
  }

  this.desiredWidth = utils.strlen(this.content) + this.paddingLeft + this.paddingRight;
  this.desiredHeight = this.lines.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.cell.prototype.setOptions"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>setOptions (options)](#apidoc.element.cli-table2.cell.prototype.setOptions)
- description and source-code
```javascript
setOptions = function (options){
  if(_.isString(options) || _.isNumber(options) || _.isBoolean(options)){
    options = {content:''+options};
  }
  options = options || {};
  this.options = options;
  var content = options.content;
  if (_.isString(content) || _.isNumber(content) || _.isBoolean(content)) {
    this.content = String(content);
  } else if (!content) {
    this.content = '';
  } else {
    throw new Error('Content needs to be a primitive, got: ' + (typeof  content));
  }
  this.colSpan = options.colSpan || 1;
  this.rowSpan = options.rowSpan || 1;
}
```
- example usage
```shell
...
 * A representation of a cell within the table.
 * Implementations must have 'init' and 'draw' methods,
 * as well as 'colSpan', 'rowSpan', 'desiredHeight' and 'desiredWidth' properties.
 * @param options
 * @constructor
 */
function Cell(options){
this.setOptions(options);
}

Cell.prototype.setOptions = function(options){
if(_.isString(options) || _.isNumber(options) || _.isBoolean(options)){
  options = {content:''+options};
}
options = options || {};
...
```

#### <a name="apidoc.element.cli-table2.cell.prototype.stylizeLine"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>stylizeLine (left, content, right)](#apidoc.element.cli-table2.cell.prototype.stylizeLine)
- description and source-code
```javascript
stylizeLine = function (left, content, right){
  left = this.wrapWithStyleColors('border',left);
  right = this.wrapWithStyleColors('border',right);
  if(this.y === 0){
    content = this.wrapWithStyleColors('head',content);
  }
  return left + content + right;
}
```
- example usage
```shell
...
var rightPadding = utils.repeat(' ', this.paddingRight);
var line = this.lines[lineNum];
var len = this.width - (this.paddingLeft + this.paddingRight);
if(forceTruncationSymbol) line += this.truncate || '…';
var content = utils.truncate(line,len,this.truncate);
content = utils.pad(content, len, ' ', this.hAlign);
content = leftPadding + content + rightPadding;
return this.stylizeLine(left,content,right);
};

Cell.prototype.stylizeLine = function(left,content,right){
left = this.wrapWithStyleColors('border',left);
right = this.wrapWithStyleColors('border',right);
if(this.y === 0){
  content = this.wrapWithStyleColors('head',content);
...
```

#### <a name="apidoc.element.cli-table2.cell.prototype.wrapWithStyleColors"></a>[function <span class="apidocSignatureSpan">cli-table2.cell.prototype.</span>wrapWithStyleColors (styleProperty, content)](#apidoc.element.cli-table2.cell.prototype.wrapWithStyleColors)
- description and source-code
```javascript
wrapWithStyleColors = function (styleProperty, content){
  if(this[styleProperty] && this[styleProperty].length){
    try {
      var colors = require('colors/safe');
      for(var i = this[styleProperty].length - 1; i >= 0; i--){
        colors = colors[this[styleProperty][i]];
      }
      return colors(content);
    } catch (e) {
      return content;
    }
  }
  else {
    return content;
  }
}
```
- example usage
```shell
...
else {
  content.push(this._topLeftChar(0));
  content.push(utils.repeat(this.chars[this.y == 0 ? 'top' : 'mid'],this.width));
}
if(drawRight){
  content.push(this.chars[this.y == 0 ? 'topRight' : 'rightMid']);
}
return this.wrapWithStyleColors('border',content.join(''));
};

Cell.prototype._topLeftChar = function(offset){
var x = this.x+offset;
var leftChar;
if(this.y == 0){
  leftChar = x == 0 ? 'topLeft' : (offset == 0 ? 'topMid' : 'top');
...
```



# <a name="apidoc.module.cli-table2.layout_manager"></a>[module cli-table2.layout_manager](#apidoc.module.cli-table2.layout_manager)

#### <a name="apidoc.element.cli-table2.layout_manager.addRowSpanCells"></a>[function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>addRowSpanCells (table)](#apidoc.element.cli-table2.layout_manager.addRowSpanCells)
- description and source-code
```javascript
function addRowSpanCells(table){
  _.forEach(table,function(row,rowIndex){
    _.forEach(row,function(cell){
      for(var i = 1; i < cell.rowSpan; i++){
        var rowSpanCell = new RowSpanCell(cell);
        rowSpanCell.x = cell.x;
        rowSpanCell.y = cell.y + i;
        rowSpanCell.colSpan = cell.colSpan;
        insertCell(rowSpanCell,table[rowIndex+i]);
      }
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.layout_manager.computeHeights"></a>[function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>computeHeights (vals, table)](#apidoc.element.cli-table2.layout_manager.computeHeights)
- description and source-code
```javascript
computeHeights = function (vals, table){
  var result = [];
  var spanners = [];
  _.forEach(table,function(row){
    _.forEach(row,function(cell){
      if((cell[colSpan] || 1) > 1){
        spanners.push(cell);
      }
      else {
        result[cell[x]] = Math.max(result[cell[x]] || 0, cell[desiredWidth] || 0, forcedMin);
      }
    });
  });

  _.forEach(vals,function(val,index){
    if(_.isNumber(val)){
      result[index] = val;
    }
  });

  //_.forEach(spanners,function(cell){
  for(var k = spanners.length - 1; k >=0; k--){
    var cell = spanners[k];
    var span = cell[colSpan];
    var col = cell[x];
    var existingWidth = result[col];
    var editableCols = _.isNumber(vals[col]) ? 0 : 1;
    for(var i = 1; i < span; i ++){
      existingWidth += 1 + result[col + i];
      if(!_.isNumber(vals[col + i])){
        editableCols++;
      }
    }
    if(cell[desiredWidth] > existingWidth){
      i = 0;
      while(editableCols > 0 && cell[desiredWidth] > existingWidth){
        if(!_.isNumber(vals[col+i])){
          var dif = Math.round( (cell[desiredWidth] - existingWidth) / editableCols );
          existingWidth += dif;
          result[col + i] += dif;
          editableCols--;
        }
        i++;
      }
    }
  }

  _.extend(vals,result);
  for(var j = 0; j < vals.length; j++){
    vals[j] = Math.max(forcedMin, vals[j] || 0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.layout_manager.computeWidths"></a>[function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>computeWidths (vals, table)](#apidoc.element.cli-table2.layout_manager.computeWidths)
- description and source-code
```javascript
computeWidths = function (vals, table){
  var result = [];
  var spanners = [];
  _.forEach(table,function(row){
    _.forEach(row,function(cell){
      if((cell[colSpan] || 1) > 1){
        spanners.push(cell);
      }
      else {
        result[cell[x]] = Math.max(result[cell[x]] || 0, cell[desiredWidth] || 0, forcedMin);
      }
    });
  });

  _.forEach(vals,function(val,index){
    if(_.isNumber(val)){
      result[index] = val;
    }
  });

  //_.forEach(spanners,function(cell){
  for(var k = spanners.length - 1; k >=0; k--){
    var cell = spanners[k];
    var span = cell[colSpan];
    var col = cell[x];
    var existingWidth = result[col];
    var editableCols = _.isNumber(vals[col]) ? 0 : 1;
    for(var i = 1; i < span; i ++){
      existingWidth += 1 + result[col + i];
      if(!_.isNumber(vals[col + i])){
        editableCols++;
      }
    }
    if(cell[desiredWidth] > existingWidth){
      i = 0;
      while(editableCols > 0 && cell[desiredWidth] > existingWidth){
        if(!_.isNumber(vals[col+i])){
          var dif = Math.round( (cell[desiredWidth] - existingWidth) / editableCols );
          existingWidth += dif;
          result[col + i] += dif;
          editableCols--;
        }
        i++;
      }
    }
  }

  _.extend(vals,result);
  for(var j = 0; j < vals.length; j++){
    vals[j] = Math.max(forcedMin, vals[j] || 0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.layout_manager.fillInTable"></a>[function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>fillInTable (table)](#apidoc.element.cli-table2.layout_manager.fillInTable)
- description and source-code
```javascript
function fillInTable(table){
  var h_max = maxHeight(table);
  var w_max = maxWidth(table);
  for(var y = 0; y < h_max; y++){
    for(var x = 0; x < w_max; x++){
      if(!conflictExists(table,x,y)){
        var opts = {x:x,y:y,colSpan:1,rowSpan:1};
        x++;
        while(x < w_max && !conflictExists(table,x,y)){
          opts.colSpan++;
          x++;
        }
        var y2 = y + 1;
        while(y2 < h_max && allBlank(table,y2,opts.x,opts.x+opts.colSpan)){
          opts.rowSpan++;
          y2++;
        }

        var cell = new Cell(opts);
        cell.x = opts.x;
        cell.y = opts.y;
        insertCell(cell,table[y]);
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.layout_manager.layoutTable"></a>[function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>layoutTable (table)](#apidoc.element.cli-table2.layout_manager.layoutTable)
- description and source-code
```javascript
function layoutTable(table){
  _.forEach(table,function(row,rowIndex){
    _.forEach(row,function(cell,columnIndex){
      cell.y = rowIndex;
      cell.x = columnIndex;
      for(var y = rowIndex; y >= 0; y--){
        var row2 = table[y];
        var xMax = (y === rowIndex) ? columnIndex : row2.length;
        for(var x = 0; x < xMax; x++){
          var cell2 = row2[x];
          while(cellsConflict(cell,cell2)){
            cell.x++;
          }
        }
      }
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.layout_manager.makeTableLayout"></a>[function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>makeTableLayout (rows)](#apidoc.element.cli-table2.layout_manager.makeTableLayout)
- description and source-code
```javascript
function makeTableLayout(rows){
  var cellRows = generateCells(rows);
  layoutTable(cellRows);
  fillInTable(cellRows);
  addRowSpanCells(cellRows);
  addColSpanCells(cellRows);
  return cellRows;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.layout_manager.maxWidth"></a>[function <span class="apidocSignatureSpan">cli-table2.layout_manager.</span>maxWidth (table)](#apidoc.element.cli-table2.layout_manager.maxWidth)
- description and source-code
```javascript
function maxWidth(table) {
  var mw = 0;
  _.forEach(table, function (row) {
    _.forEach(row, function (cell) {
      mw = Math.max(mw,cell.x + (cell.colSpan || 1));
    });
  });
  return mw;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cli-table2.utils"></a>[module cli-table2.utils](#apidoc.module.cli-table2.utils)

#### <a name="apidoc.element.cli-table2.utils.colorizeLines"></a>[function <span class="apidocSignatureSpan">cli-table2.utils.</span>colorizeLines (input)](#apidoc.element.cli-table2.utils.colorizeLines)
- description and source-code
```javascript
function colorizeLines(input){
  var state = {};
  var output = [];
  for(var i = 0; i < input.length; i++){
    var line = rewindState(state,input[i]) ;
    state = readState(line);
    var temp = _.extend({},state);
    output.push(unwindState(temp,line));
  }
  return output;
}
```
- example usage
```shell
...
setOption(style, tableStyle, 'padding-right', this);
this.head = style.head || tableStyle.head;
this.border = style.border || tableStyle.border;

var fixedWidth = tableOptions.colWidths[this.x];
if(tableOptions.wordWrap && fixedWidth){
  fixedWidth -= this.paddingLeft + this.paddingRight;
  this.lines = utils.colorizeLines(utils.wordWrap(fixedWidth,this.content));
}
else {
  this.lines = utils.colorizeLines(this.content.split('\n'));
}

this.desiredWidth = utils.strlen(this.content) + this.paddingLeft + this.paddingRight;
this.desiredHeight = this.lines.length;
...
```

#### <a name="apidoc.element.cli-table2.utils.mergeOptions"></a>[function <span class="apidocSignatureSpan">cli-table2.utils.</span>mergeOptions (options, defaults)](#apidoc.element.cli-table2.utils.mergeOptions)
- description and source-code
```javascript
function mergeOptions(options, defaults){
  options = options || {};
  defaults = defaults || defaultOptions();
  var ret = _.extend({}, defaults, options);
  ret.chars = _.extend({}, defaults.chars, options.chars);
  ret.style = _.extend({}, defaults.style, options.style);
  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-table2.utils.pad"></a>[function <span class="apidocSignatureSpan">cli-table2.utils.</span>pad (str, len, pad, dir)](#apidoc.element.cli-table2.utils.pad)
- description and source-code
```javascript
function pad(str, len, pad, dir) {
  var length = strlen(str);
  if (len + 1 >= length) {
    var padlen = len - length;
    switch (dir) {
      case 'right':
        str = repeat(pad, padlen) + str;
        break;

      case 'center':
        var right = Math.ceil((padlen) / 2);
        var left = padlen - right;
        str = repeat(pad, left) + str + repeat(pad, right);
        break;

      default :
        str = str + repeat(pad,padlen);
        break;
    }
  }
  return str;
}
```
- example usage
```shell
...
var leftPadding = utils.repeat(' ', this.paddingLeft);
var right = (drawRight ? this.chars['right'] : '');
var rightPadding = utils.repeat(' ', this.paddingRight);
var line = this.lines[lineNum];
var len = this.width - (this.paddingLeft + this.paddingRight);
if(forceTruncationSymbol) line += this.truncate || '…';
var content = utils.truncate(line,len,this.truncate);
content = utils.pad(content, len, ' ', this.hAlign);
content = leftPadding + content + rightPadding;
return this.stylizeLine(left,content,right);
};

Cell.prototype.stylizeLine = function(left,content,right){
left = this.wrapWithStyleColors('border',left);
right = this.wrapWithStyleColors('border',right);
...
```

#### <a name="apidoc.element.cli-table2.utils.repeat"></a>[function <span class="apidocSignatureSpan">cli-table2.utils.</span>repeat (str, times)](#apidoc.element.cli-table2.utils.repeat)
- description and source-code
```javascript
function repeat(str, times){
  return Array(times + 1).join(str);
}
```
- example usage
```shell
...
 */
Cell.prototype.drawTop = function(drawRight){
var content = [];
if(this.cells){  //TODO: cells should always exist - some tests don't fill it in though
  _.forEach(this.widths,function(width,index){
    content.push(this._topLeftChar(index));
    content.push(
      utils.repeat(this.chars[this.y == 0 ? 'top' : 'mid'],width)
    );
  },this);
}
else {
  content.push(this._topLeftChar(0));
  content.push(utils.repeat(this.chars[this.y == 0 ? 'top' : 'mid'],this.width));
}
...
```

#### <a name="apidoc.element.cli-table2.utils.strlen"></a>[function <span class="apidocSignatureSpan">cli-table2.utils.</span>strlen (str)](#apidoc.element.cli-table2.utils.strlen)
- description and source-code
```javascript
function strlen(str){
  var code = codeRegex();
  var stripped = ("" + str).replace(code,'');
  var split = stripped.split("\n");
  return split.reduce(function (memo, s) { return (stringWidth(s) > memo) ? stringWidth(s) : memo }, 0);
}
```
- example usage
```shell
...
   fixedWidth -= this.paddingLeft + this.paddingRight;
   this.lines = utils.colorizeLines(utils.wordWrap(fixedWidth,this.content));
 }
 else {
   this.lines = utils.colorizeLines(this.content.split('\n'));
 }

 this.desiredWidth = utils.strlen(this.content) + this.paddingLeft + this.paddingRight;
 this.desiredHeight = this.lines.length;
};

/**
* Each cell will have it's 'x' and 'y' values set by the 'layout-manager' prior to
* 'init' being called;
* @type {Number}
...
```

#### <a name="apidoc.element.cli-table2.utils.truncate"></a>[function <span class="apidocSignatureSpan">cli-table2.utils.</span>truncate (str, desiredLength, truncateChar)](#apidoc.element.cli-table2.utils.truncate)
- description and source-code
```javascript
function truncate(str, desiredLength, truncateChar){
  truncateChar = truncateChar || '…';
  var lengthOfStr = strlen(str);
  if(lengthOfStr <= desiredLength){
    return str;
  }
  desiredLength -= strlen(truncateChar);

  ret = truncateWidthWithAnsi(str, desiredLength);

  return ret + truncateChar;
}
```
- example usage
```shell
...
}
var leftPadding = utils.repeat(' ', this.paddingLeft);
var right = (drawRight ? this.chars['right'] : '');
var rightPadding = utils.repeat(' ', this.paddingRight);
var line = this.lines[lineNum];
var len = this.width - (this.paddingLeft + this.paddingRight);
if(forceTruncationSymbol) line += this.truncate || '…';
var content = utils.truncate(line,len,this.truncate);
content = utils.pad(content, len, ' ', this.hAlign);
content = leftPadding + content + rightPadding;
return this.stylizeLine(left,content,right);
};

Cell.prototype.stylizeLine = function(left,content,right){
left = this.wrapWithStyleColors('border',left);
...
```

#### <a name="apidoc.element.cli-table2.utils.wordWrap"></a>[function <span class="apidocSignatureSpan">cli-table2.utils.</span>wordWrap (maxLength, input)](#apidoc.element.cli-table2.utils.wordWrap)
- description and source-code
```javascript
function multiLineWordWrap(maxLength, input){
  var output = [];
  input = input.split('\n');
  for(var i = 0; i < input.length; i++){
    output.push.apply(output,wordWrap(maxLength,input[i]));
  }
  return output;
}
```
- example usage
```shell
...
setOption(style, tableStyle, 'padding-right', this);
this.head = style.head || tableStyle.head;
this.border = style.border || tableStyle.border;

var fixedWidth = tableOptions.colWidths[this.x];
if(tableOptions.wordWrap && fixedWidth){
  fixedWidth -= this.paddingLeft + this.paddingRight;
  this.lines = utils.colorizeLines(utils.wordWrap(fixedWidth,this.content));
}
else {
  this.lines = utils.colorizeLines(this.content.split('\n'));
}

this.desiredWidth = utils.strlen(this.content) + this.paddingLeft + this.paddingRight;
this.desiredHeight = this.lines.length;
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
