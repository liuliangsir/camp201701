###github项目代码风格の比较###
<table  class="table table-bordered table-striped table-condensed">
<tr>
  <th rowspan="2" align="center">github项目名</center></th>
  <th colspan="3" align="center">广义的代码格式</center></th>
  <th colspan="10" align="center">狭义的代码格式</center></th>
  <th colspan="3" align="center">特殊的js风格</center></th>
</tr>
<tr>
  <th align="center">　　　　　　　　　　　　目录结构和文件名</th>
  <th align="center">　　　　　　　　　变量命名</center></th>
  <th align="center">　　　　　　　　　文档规范</center></th>
  <th align="center">　　　　　　　　　缩进方式</center></th>
  <th align="center">　　　　　　　　　使用字符串的方式</center></th>
  <th align="center">　　　　　　　　　　存在变量声明后未使用</center></th>
  <th align="center">　　　　　　　　　在语句，表达式结束处添加分号</center></th>
  <th align="center">　　　　　　　　　以<code>(</code>，<code>[</code>，<code>'</code>作为一行的开头</center></th>
  <th align="center">　　　　　　　　　关键词后有空格</center></th>
  <th align="center">　　　　　　　　　函数名后有空格</center></th>
  <th align="center">　　　　　　　　　使用严格模式进行值比较</center></th>
  <th align="center">　　　　　　　　　会进行错误处理</center></th>
  <th align="center">　　　　　　　　　使用全局变量，会添加<code>window</code></center></th>
  <th align="center">　　　　　　　　　IIFE</center></th>
  <th align="center">　　　　　　　　　严格模式</center></th>
  <th>模块</th>
</tr>
<tr>
    <th align="center">thinkjs</center></th>
    <td>
      <ul>
      <li>
        <code>doc</code>
        <ul>
          <li><code>README.md</code></li>
        </ul>
      </li>
      <li>
        <code>lib</code>
        <ul>
          <li><code>Common</code></li>
          <li><code>Conf</code></li>
          <li><code>Lib</code></li>
          <li><code>View</code></li>
          <li><code>think.js</code></li>
        </ul>
      </li>
      <li>
        <code>test</code>
        <ul>
          <li><code>Common</code></li>
          <li><code>Conf</code></li>
          <li><code>Lib</code></li>
          <li><code>View</code></li>
          <li><code>think.js</code></li>
        </ul>
      </li>
      </ul>
    </td>
    <td>
      <ol>
        <li>常量字母全部大写，多个单词之间使用下划线</li>
        <li>变量名为一个单词时，全部小写，多个单词驼峰写法</li>
        <li>第一层文件夹名字全部小写，第二层文件夹名字首字母大写</li>
      </ol>
    </td>
    <td>
      <ol>
        <li>文件头部进行文档注释，例如：
          <pre><code>
          /**
           *行为类
           *@return {[type]} [description]
          */
          </code></pre>
        </li>
        <li>文件关键部分进行文档注释，例如：
          <pre><code>
          /**
           * 生成cookie签名
           * @param  string val
           * @param  string secret
           * @return string
          */
          var cookieSign = function(val, secret){
            'use strict';
            secret = crypto.createHmac('sha256', secret).update(val).digest('base64');
            secret = secret.replace(/\=+$/, '');
            return val + '.' + secret;
          };
          </pre></code>
        </li>
      </ol>
    </td>
    <td align="center">2个空格</td>
    <td align="center">单引号</td>
    <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487714497_Close_Icon_Dark.png"/></td>
    <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
    <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487714497_Close_Icon_Dark.png"/></td>
    <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
    <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487714497_Close_Icon_Dark.png"/></td>
    <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
    <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
    <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
    <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487714497_Close_Icon_Dark.png"/></td>
    <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
    <td>ES6</td>
</tr>
<tr>
  <th align="center">avalon</center></th>
  <td>
    <ul>
      <li>
        <code>components</code>
        <ul>
          <li><code>button</code></li>
          <li><code>list</code></li>
          <li><code>loading</code></li>
          <li><code>pager</code></li>
          <li><code>panel</code></li>
          <li><code>router</code></li>
          <li><code>select</code></li>
          <li><code>logo.png</code></li>
        </ul>
      </li>
      <li>
        <code>dist</code>
        <ul>
          <li><code>arthur.js</code></li>
          <li><code>avalon.js</code></li>
          <li><code>avalon.modern.js</code></li>
        </ul>
      </li>
      <li>
        <code>test</code>
        <ul>
          <li><code>directives</code></li>
          <li><code>dom</code></li>
          <li><code>filters</code></li>
          <li><code>parser</code></li>
          <li><code>seed</code></li>
          <li><code>vdom</code></li>
          <li><code>vmodel</code></li>
          <li><code>vtree</code></li>
          <li><code>beforeIt.js</code></li>
          <li><code>jquery.js</code></li>
          <li><code>matchers.js</code></li>
          <li><code>promise.js</code></li>
          <li><code>spec.js</code></li>
          <li><code>spec.modern.js</code></li>
          <li><code>test.js</code></li>
        </ul>
      </li>
      <li>
        <code>src</code>
        <ul>
          <li><code>component</code></li>
          <li><code>directives</code></li>
          <li><code>dom</code></li>
          <li><code>effect</code></li>
          <li><code>filters</code></li>
          <li><code>gesture</code></li>
          <li><code>parser</code></li>
          <li><code>renders</code></li>
          <li><code>seed</code></li>
          <li><code>vdom</code></li>
          <li><code>vmodel</code></li>
          <li><code>vtree</code></li>
          <li><code>avalon.js</code></li>
          <li><code>avalon.modern.js</code></li>
          <li><code>avalon.tap.js</code></li>
          <li><code>pager.js</code></li>
          <li><code>routergrid.js</code></li>
        </ul>
      </li>
    </ul>
  </td>
  <td>
    <ol>
    <li>常量字母全部大写，多个单词之间使用下划线</li>
    <li>变量名为一个单词时，全部小写，多个单词驼峰写法</li>
    <li>文件夹名字均小写</li>
    </ol>
  </td>
  <td>
    <ol>
      <li>文件头部进行文档注释，例如：
        <pre><code>
        /*!
          built in 2017-2-17:17:59 version 2.2.4 by 司徒正美
          https://github.com/RubyLouvre/avalon/tree/2.2.4
          修正IE下 orderBy BUG
          更改下载Promise的提示
          修复avalon.modern 在Proxy 模式下使用ms-for 循环对象时出错的BUG
          修复effect内部传参 BUG
          重构ms-validate的绑定事件的机制
        */
        </code></pre>
      </li>
      <li>文件关键部分进行文档注释，例如：
        <pre><code>
        try {
          _slice.call(avalon.document.documentElement);
        } catch (e) {
        }
        </code></pre>
      </li>
    </ol>
  </td>
  <td align="center">四个空格</td>
  <td align="center">双引号</td>
  <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
  <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
  <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
  <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
  <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487714497_Close_Icon_Dark.png"/></td>
  <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
  <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
  <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
  <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
  <td align="center"><img src="http://ohupawle2.bkt.clouddn.com/1487713331_Tick_Mark_Dark.png"/></td>
  <td>ES6</td>
</tr>
</table>

---

综合比较，我还是喜欢avalon的文件命名方式，喜欢thinkjs的模块系统

