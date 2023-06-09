# Testing-2-repo
testing view purpose
/**
 * Usage: 
 *   'Hello ${name}'.template({
 *     name: 'chaps'
 *   });
 * 
 * From: https://gist.github.com/WebReflection/8f227532143e63649804
 */t) { // Andrea Giammarchi - WTFPL License var stringify = JSON.stringify, re = /${([\S\s]*?)}/g, evaluate = [], i = 0, m ; while (m = re.exec(this)) { evaluate.push( str

String.prototype.template = function (object) {
  // Andrea Giammarchi - WTFPL License
  var });
 * 
 * From: https://gist.github.com/WebReflection/8f227532143e63649804
 */

String.prototype.template = function (object) {
  // Andrea Giammarchi - WTFPL License
    stringify = JSON.stringify,
    re = /\$\{([\S\s]*?)\}/g,
    evaluate = [],
    i = 0,
    m
  ;
  while (m = re.exec(this)) {
    evaluate.push(
      stringify(this.slice(i, re.lastIndex - m[0].length)),
      '(' + m[1] + ')'
    );
    i = re.lastIndex;
  }
 * Usage: 
 *   'Hello ${name}'.template({
 *     name: 'chaps'
 *   });
 * 
 * From: https://gist.github.com/WebReflection/8f227532143e63649804
 */

String.prototype.template = function (object) {
  // Andrea Giammarchi - WTFPL License
  var
    stringify = JSON.stringify,
    re = /\$\{([\S\s]*?)\}/g,
    evaluate = [],
    i = 0,
    m
