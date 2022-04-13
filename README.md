### chrome devtools 所提供的的api
> 打开浏览器控制面板-查看记录的消息和运行的JavaScript日志
>> 一些快捷键-----开发人员常用
>>> 1. F12 / ctrl + shift + I 打开浏览器控制台
>>> 2.  ctrl + shift + J 打开控制台console面板
>>> 3.  ctrl + shift + C 打开控制台element面板
>>> 4.  F5 重新加载页面
>>> 5.  F8 断点调试向下执行一段代码块
>>> 6.  F10 跳过下一个函数调用-断点debbuger多
>>> 7.  F11 进入下一个函数调用-断点debbuger多
>>> 8.  ctrl + p 打开最近打开过的文件-用于搜索文件名
>>> 9.  ctrl + shift + F 在文件夹中搜索相关代码片段-搜索字符串
>>> 10.  ctrl + shift + + 在浏览器上缩放窗口的比例
>>> 11.  ctrl + - 在浏览器上缩小窗口的比例
>>> 12.  ctrl + z 撤销上一步操作
>>> 12.  alt  选中展区


### 在控制台console,输出日志
 > 1. $0, $1, $2, $3, $4,  选择dom节点
 ----
<script>
---
console.log("hello, console");
console.info("%c this is info")
console.warn("控制台发出警告");
console.error("控制台报错");
function sum(a, b) {
    return a + b
}
console.log(sum(1,2));
console.log(activeElement);
console.clear();
const x = 5;
const y = 3;
console.assert(x < y, {x, y, reason});
console.count();
console.count("coffee");
console.Reset();
console.Reset("coffee");
console.debug("debug");
console.dir(document.head);
console.dirxml(document);
const label = "控制台折叠组面板";
console.group(label);
console.info('leo');
console.info('mike');
console.info('Don');
console.info('Raph');
console.groupEnd(label);
console.table([
    {
        first: "Chaim",
        last: "Soutine",
        birthday: "121112"
    },
    {
        first: "aim",
        birthday: "143431112"
    }
]);
console.time();
  const arr = [5, 2, 7, 8, 34, 7, 39, 12, 56, 9, 1];
  function bubbleSort(arr) {
    const len = arr.length
    // 外层循环i控制比较的轮数
    for (let i = 0; i < len; i++) {
      // 里层循环控制每一轮比较的次数j，arr[i] 只用跟其余的len - i个元素比较
      for (let j = 1; j < len - i; j++) {
        // 若前一个元素"大于"后一个元素，则两者交换位置
        if (arr[j - 1] > arr[j]) {
          [arr[j - 1], arr[j]] = [arr[j], arr[j - 1]]
        }
      }
    }
    return arr
  };
  console.log(bubbleSort(arr));
  console.timeEnd();

console.time();
console.timeEnd();
const a = () => {b();}; const b = () => {c();}; const c = () => {d();};const d = () => {console.trace();};a();           console.log("输出栈内存的执行顺序");
console.trace();

$$;
document.querySelectorAll();
$X("?seach/path");
copy($0);
debug(getData)
---
</scipt>

## [参考文献](https://developer.chrome.com/docs/devtools/javascript/sources/#files)




